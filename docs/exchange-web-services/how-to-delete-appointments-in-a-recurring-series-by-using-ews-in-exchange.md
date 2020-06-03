---
title: Exchange の EWS を使用して定期的なアイテム内の予定を削除する
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: a9d5244a-bc4a-4e9c-9c6c-ff361e04cbf8
description: EWS マネージ API または Exchange の EWS を使用して、定期的なアイテム内の予定を削除する方法について説明します。
ms.openlocfilehash: 5646a30d218ed4d795044aefe5efea1399d19a79
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528126"
---
# <a name="delete-appointments-in-a-recurring-series-by-using-ews-in-exchange"></a>Exchange の EWS を使用して定期的なアイテム内の予定を削除する

EWS マネージ API または Exchange の EWS を使用して、定期的なアイテム内の予定を削除する方法について説明します。
  
EWS マネージ API または EWS を使用すると、一連の予定や会議、またはその中の 1 つのインスタンスのみを削除できます。一連の予定を削除するために使用するプロセスは、単独の予定だけを削除するプロセスと本質的に同じです。[単独の予定または会議のインスタンスを削除する](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)場合と同じ EWS マネージ API メソッドまたは EWS 操作を使用します。違いは、メソッドまたは操作に含まれるアイテム ID です。最初に、両方のシナリオが同じであるという点を確認していきましょう。  
  
定期的なアイテムや、定期的なアイテム中の単独のアイテムのみを削除する場合、削除対象のアイテムまたは定期的なアイテムを見つけ、その後、適切なメソッドまたは操作を呼び出して削除します。あらゆる種類の予定を簡単に削除できますが、出席者や開催者については最新の情報を保持し、削除対象ユーザーが開催した会議はキャンセルし、対象ユーザーが開催しなかった会議は辞退することをお勧めします。
  
では、これらのシナリオにおける違いはどこにありますか? EWS マネージ API の場合にはメソッドを呼び出すために [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクトを使用し、EWS の場合には操作要求にアイテム ID を含めるという点のみです。 一連の予定全体を削除するには、定期的マスターの **Appointment** オブジェクトまたはアイテム ID が必要になります。 単独の予定を削除する場合には、その **Appointment** オブジェクトまたはアイテム ID が必要です。 
  
## <a name="delete-a-recurring-appointment-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して定期的な予定を削除する

この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。 _recurringItem_ パラメーターは、定期的マスターまたは単独の予定の **Appointment** オブジェクトです。 _deleteEntireSeries_ パラメーターは、_recurringItem_ が含まれる一連の予定全体を削除するかどうかを示します。 
  
```cs
public static bool DeleteRecurringItem(ExchangeService service, Appointment recurringItem, bool deleteEntireSeries)
{
    Appointment appointmentToDelete = null;
    // If the item is a single appointment, fail.
    if (recurringItem.AppointmentType == AppointmentType.Single)
    {
        Console.WriteLine("ERROR: The item to delete is not part of a recurring series.");
        return false;
    }
    // Check the Appointment that was passed. Is it
    // an occurrence or the recurring master?
    if (recurringItem.AppointmentType == AppointmentType.RecurringMaster)
    {
        if (!deleteEntireSeries)
        {
            // The item is the recurring master, so deleting it will delete
            // the entire series. The caller indicated that the entire series
            // should not be deleted, so fail.
            Console.WriteLine("ERROR: The item to delete is the recurring master of the series. Deleting it will delete the entire series.");
            return false;
        }
        else
        {
            appointmentToDelete = recurringItem;
        }
    }
    else
    {
        if (deleteEntireSeries)
        {
            // The item passed is not the recurring master, but the caller
            // wants to delete the entire series. Bind to the recurring
            // master to delete it.
            try
            {
                appointmentToDelete = Appointment.BindToRecurringMaster(service, recurringItem.Id);
            }
            catch (Exception ex)
            {
                Console.WriteLine("ERROR: {0}", ex.Message);
                return false;
            }
        }
        else
        {
            // The item passed is not the recurring master, but the caller
            // only wants to delete the occurrence, so just
            // delete the passed item.
            appointmentToDelete = recurringItem;
        }
    }
    if (appointmentToDelete != null)
    {
        // Remove the item, depending on the scenario. 
        if (appointmentToDelete.IsMeeting)
        {
            CalendarActionResults results;
            // If it's a meeting and the user is the organizer, cancel it.
            // Determine this by testing the AppointmentState bitmask for 
            // the presence of the second bit. This bit indicates that the appointment
            // was received, which means that someone sent it to the user. Therefore,
            // they're not the organizer.
            int isReceived = 2;
            if ((appointmentToDelete.AppointmentState &amp; isReceived) == 0)
            {
                results = appointmentToDelete.CancelMeeting("Cancelling this meeting.");
                return true;
            }
            // If it's a meeting and the user is not the organizer, decline it.
            else
            {
                results = appointmentToDelete.Decline(true);
                return true;
            }
        }
        else
        {
            // The item isn't a meeting, so just delete it.
            appointmentToDelete.Delete(DeleteMode.MoveToDeletedItems);
            return true;
        }
    }
    return false;
}
```

この例を使用するには、[1 つの予定または定期的マスターのいずれかにバインド](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)し、その結果の **Appointment** オブジェクトをメソッドに渡す必要があります。 [CalendarView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) クラスを使用して予定にアクセスする場合は、結果のアイテムはすべて単独のアイテムになることに留意してください。 対照的に、[ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) クラスを使用すると、結果のアイテムはすべて定期的マスターになります。 
  
## <a name="delete-a-recurring-appointment-by-using-ews"></a>EWS を使用して定期的な予定を削除する

EWS を使用して定期的なアイテムを削除する操作は、[単独の会議インスタンスを削除する](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)場合と同じです。実際、SOAP 要求の形式は同じです。既に述べた点ですが、要求で使用されるのはアイテム ID であるということが重要になります。アイテム ID が定期的マスターに対応する場合、一連の予定全体が削除されます。アイテム ID が単独の予定に対応する場合には、その予定のみが削除されます。
  
> [!NOTE]
> 次のコード例では、**ItemId**、**ChangeKey**、**RecurringMasterId** の各属性は読みやすくするために短縮されています。 
  
この例では、[CreateItem 操作](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)に、[CancelCalendarItem](https://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) 要素を設定して使用し、対象ユーザーが開催者となっている会議をキャンセルします。 [ReferenceItemId](https://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) 要素の値は、キャンセルするアイテムを示します。定期的マスターまたは単独の会議のどちらかのアイテム ID を指定できます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:CancelCalendarItem>
          <t:ReferenceItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
          <t:NewBodyContent BodyType="HTML">Cancelling this meeting.</t:NewBodyContent>
        </t:CancelCalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

この例では、**CreateItem 操作**に [DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) 要素を指定して使用し、対象ユーザーが開催者ではない会議を辞退します。 前の例でのように、**ReferenceItemId** 要素の値は辞退するアイテムを示します。定期的マスターまたは単独の会議のどちらかのアイテム ID を指定できます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:DeclineItem>
          <t:ReferenceItemId Id="AAMkADA6..." ChangeKey="DwAAABYA..." />
        </t:DeclineItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

この例では、[DeleteItem 操作](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)を使用して、出席者のいない単独の予定を削除します。 削除する対象は、[OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) 要素で指定します。この要素は、定期的マスターのアイテム ID と、予定のインデックスで構成されます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="MoveToDeletedItems" SendMeetingCancellations="SendToAllAndSaveCopy">
      <m:ItemIds>
        <t:OccurrenceItemId RecurringMasterId="AAMkADA8..." InstanceIndex="3" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

次に示されているように、**OccurrenceItemId** 要素を、予定のアイテム ID を含む [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) 要素と置き換えても同じ結果が得られることに注目してください。 
  
```XML
<m:ItemIds>
  <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
</m:ItemIds>

```

## <a name="see-also"></a>関連項目


- [定期的なパターンと EWS](recurrence-patterns-and-ews.md)
    
- [Exchange の EWS を使用して定期的なアイテムにアクセスする](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Exchange の EWS を使用して定期的なアイテムを作成する](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [EWS を使用して定期的なアイテムを更新する](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Exchange の EWS を使用して定期的なアイテムを更新する](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Exchange の予定表と EWS](calendars-and-ews-in-exchange.md)
    
- [Exchange 2013 で EWS を使用して予定と会議を作成する](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Exchange の EWS を使用して、予定を削除し、会議をキャンセルする](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    


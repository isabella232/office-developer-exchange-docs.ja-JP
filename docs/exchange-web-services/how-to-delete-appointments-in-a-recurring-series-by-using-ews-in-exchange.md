---
title: Exchange EWS を使用して一連の定期的な予定を削除します。
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: a9d5244a-bc4a-4e9c-9c6c-ff361e04cbf8
description: Exchange の EWS マネージ API または EWS を使用して、定期的なアイテム内の予定を削除する方法を説明します。
ms.openlocfilehash: 5e4d95058808adf8db159000bdf90c1f92945338
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758960"
---
# <a name="delete-appointments-in-a-recurring-series-by-using-ews-in-exchange"></a>Exchange EWS を使用して一連の定期的な予定を削除します。

Exchange の EWS マネージ API または EWS を使用して、定期的なアイテム内の予定を削除する方法を説明します。
  
予定または会議の系列または系列内の 1 つのインスタンスを削除するのには、EWS のマネージ API または EWS を使用できます。 シリーズ全体を削除するのにを使用するプロセスは、本質的には、1 つのアイテムのみを削除するのにを使用するプロセスと同じです。 EWS のマネージ API と同じ方法または[単独の予定または会議を削除](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)するために使用、EWS の操作を使用します。 違いは、メソッドまたは操作に含まれる項目 id です。 どのように両方のシナリオは、同じを見ていきましょう。 
  
定期的なアイテムや、定期的なアイテム中の単独のアイテムのみを削除する場合、削除対象のアイテムまたは定期的なアイテムを見つけ、その後、適切なメソッドまたは操作を呼び出して削除します。あらゆる種類の予定を簡単に削除できますが、出席者や開催者については最新の情報を保持し、削除対象ユーザーが開催した会議はキャンセルし、対象ユーザーが開催しなかった会議は辞退することをお勧めします。
  
その方法はシナリオ別でしょうか。 メソッド (EWS のマネージ API) またはアイテムの ID を呼び出すために使用する[予定](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)のオブジェクトの概要に記載 (EWS) の操作の要求。 シリーズ全体を削除するには、マスターの定期的な**予定**のオブジェクトまたは要素 ID が必要です。 1 つのオカレンスを削除するには、発生する**予定**のオブジェクトまたは要素 ID が必要です。 
  
## <a name="delete-a-recurring-appointment-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して定期的な予定を削除する

次の使用例は、認証済み Exchange サーバーおよび**サービス**をという名前の[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトを取得することを想定しています。 _RecurringItem_パラメーターは、1 回または定期的なマスターのいずれかの**予定**オブジェクトです。 _DeleteEntireSeries_パラメーターでは、 _recurringItem_の一部になっているデータ系列全体を削除するかどうかを示します。 
  
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

次の使用例を使用するには、[発生または定期的なマスターのいずれかにバインド](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)する必要があるし、**予定**オブジェクトをメソッドに渡します。 予定を[予定表ビュー](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx)クラスを使用してアクセスすると、結果として得られるアイテムが、1 つのすべての出現に留意してください。 逆に、 [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx)クラスを使用する場合、結果として得られる項目は、すべての定期的なマスターになります。 
  
## <a name="delete-a-recurring-appointment-by-using-ews"></a>EWS を使用して定期的な予定を削除する

[単独の会議を削除する](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)ことでは、EWS を使用して定期的な系列を削除します。 実際には、SOAP 要求は、同じ形式を実行します。 もう一度、キーは、要求で使用されている項目の ID です。 品目 ID は、定期的なマスターに対応して、データ系列全体が削除されます。 項目 ID は、1 回の発生に対応して、そのアイテムのみが削除されます。
  
> [!NOTE]
> 次のコードの例では**アイテム Id**、**変更キー**、および**RecurringMasterId**の属性は読みやすさの短縮します。 
  
この例では、 [CancelCalendarItem](http://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx)要素を使用して[CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)を使用して、ユーザーは開催者の会議をキャンセルします。 [ReferenceItemId](http://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx)要素の値は、取り消すには、アイテムを指定し、定期的なマスター、または 1 つの項目 ID を指定できます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

この例では、 [DeclineItem](http://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx)要素を使用して**CreateItem 操作**を使用して、対象のユーザーは開催者の会議を辞退します。 **ReferenceItemId**要素の値がこれを拒否すると、アイテムを指定する前の例のようにと、定期的なマスター、または 1 つの項目 ID を指定できます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

この例では、 [DeleteItem の操作](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)を使用していない参加者との予定の 1 つのアイテムを削除します。 発生を削除するのには、定期的なマスターの項目の ID と、出現する位置のインデックスが作成される[OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx)要素によって指定されます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

ように、出現する位置の項目の ID が含まれている[アイテム Id](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx)要素を使用して**OccurrenceItemId**要素を置き換えることによって同じ結果を得ることができることに注意してください。 
  
```XML
<m:ItemIds>
  <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
</m:ItemIds>

```

## <a name="see-also"></a>関連項目


- [定期的なパターンと EWS](recurrence-patterns-and-ews.md)
    
- [Exchange で EWS を使用して、定期的にアクセスします。](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用して定期的な系列を作成します。](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [EWS を使用して一連の定期的な更新プログラム](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Exchange EWS を使用して一連の定期的な更新プログラム](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Calendars and EWS in Exchange](calendars-and-ews-in-exchange.md)
    
- [Exchange 2013 の EWS を使用して予定および会議を作成します。](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [予定を削除して、Exchange で EWS を使用して会議をキャンセル](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    


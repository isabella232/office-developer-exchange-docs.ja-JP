---
title: Exchange で EWS を使用して定期的なアイテムを更新する
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: c922072f-ce33-4bff-97b0-1c1d0f9b880d
description: Exchange の EWS マネージ API または EWS を使用して、定期的なアイテム全体を一度に更新する方法を説明します。
ms.openlocfilehash: 03f414845674bfcacca62ef96fdb84f8b8823920
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759056"
---
# <a name="update-a-recurring-series-by-using-ews-in-exchange"></a>Exchange で EWS を使用して定期的なアイテムを更新する

Exchange の EWS マネージ API または EWS を使用して、定期的なアイテム全体を一度に更新する方法を説明します。
  
EWS マネージ API または EWS を使用して、定期的なアイテム全体を更新するか、[単一のアイテムを更新する](how-to-update-a-recurring-series-by-using-ews.md)ことによって、定期的なアイテムを更新します。 この記事では、定期的なアイテム全体を一度に更新する方法について説明します。
  
一般に、定期的なアイテムの更新は、[単一の予定の変更](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)に非常に似ています。 同じメソッドと操作を使用しますが、定期的なアイテムの定期的マスターのアイテム ID を使用します。 定期的マスターから始められないケースもあり、その場合は[定期的マスターのアイテム ID を見つける](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)必要が生じることがあります。
  
ただし、定期的なアイテムを更新する際に考慮すべき重要な違いが 1 つあります。定期的なパターンの更新です。 定期的なパターンの更新は定期的マスターでのみ可能であり、パターンの変更によってアイテムを追加したり削除したりできます。 たとえば、[Recurrence.EndDate](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.recurrence.enddate%28v=exchg.80%29.aspx) プロパティを現在の値より後の日付に変更すると、定期的なパターンが再評価され、追加のアイテムが追加される場合があります。 
  
## <a name="modify-all-occurrences-in-a-series-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して定期的なアイテム内のアイテムをすべて変更する

定期的なアイテム内のアイテムをすべて変更するには、次にようにします。
  
1. 定期的マスターの [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.appointment.bindtorecurringmaster%28v=exchg.80%29.aspx) または [Appointment.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) メソッドを使用して、定期的なアイテムの定期的マスターにバインドします。 
    
2. 定期的マスター [Appointment](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクトのプロパティを更新します。 
    
3. [Appointment.Save](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) メソッドを使用して、定期的マスターの変更を保存します。 
    
次の例では、定期的なアイテムを更新して、場所を変更し、出席者を追加し、定期的なパターンを変更します。 この例では、_service_ パラメーターで渡される [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトが、[Credentials](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) プロパティと [Url](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) プロパティの有効な値で初期化されているものとします。 _recurringAppointment_ パラメーターは、更新される定期的なアイテムのアイテムまたは定期的マスターのどちらかにバインドされる **Appointment** オブジェクトです。 
  
```cs
using Microsoft.Exchange.WebServices.Data;
public static bool UpdateRecurringSeries(ExchangeService service, Appointment recurringAppointment)
{
    Appointment recurringMaster = null;
    // If the item is a single appointment, fail.
    if (recurringAppointment.AppointmentType == AppointmentType.Single)
    {
        Console.WriteLine("ERROR: The item to delete is not part of a recurring series.");
        return false;
    }
    // Check the Appointment that was passed. Is it
    // an occurrence or the recurring master?
    if (recurringAppointment.AppointmentType != AppointmentType.RecurringMaster)
    {
        // If an occurrence was passed in, bind to the master.
        try
        {
            // This method results in a call to EWS.
            recurringMaster = Appointment.BindToRecurringMaster(service, recurringAppointment.Id);
        }
        catch (Exception ex)
        {
            Console.WriteLine("Couldn't bind to master: {0}", ex.Message);
            return false;
        }
    }
    else
    {
        // Bind to the appointment to load all properties.
        // This method results in a call to EWS.
        recurringMaster = Appointment.Bind(service, recurringAppointment.Id);
    }
    // Basic updates. These kinds of updates are the same
    // as if you were updating a single appointment.
    // Update the location. All occurrences will update to this new location.
    recurringMaster.Location = "Conference Room 2";
    // Add an attendee.
    Attendee newAttendee = new Attendee("sadie@contoso.com");
    recurringMaster.RequiredAttendees.Add(newAttendee);
    // Changes to the recurrence. This is only applicable to a recurring
    // master.
    // If the series has an end date, extend the series to add two more occurrences.
    if (recurringMaster.Recurrence.HasEnd)
    {
        // NumberOfOccurrences is only set if the user created the
        // appointment with a set number of occurrences.
        // Otherwise, there's a start and end date.
        if (recurringMaster.Recurrence.NumberOfOccurrences != null)
        {
            recurringMaster.Recurrence.NumberOfOccurrences += 2;
        }
        else
        {
            // This is a bit more complicated if you want to add two more
            // occurrences. You need to calculate a new end date.
            Type recurrenceType = recurringMaster.Recurrence.GetType();
            switch (recurrenceType.Name)
            {
                case "DailyPattern":
                    recurringMaster.Recurrence.EndDate =
                        recurringMaster.Recurrence.EndDate.Value.AddDays(2);
                    break;
                case "WeeklyPattern":
                    recurringMaster.Recurrence.EndDate =
                        recurringMaster.Recurrence.EndDate.Value.AddDays(14);
                    break;
                case "YearlyPattern":
                    recurringMaster.Recurrence.EndDate =
                        recurringMaster.Recurrence.EndDate.Value.AddYears(2);
                    break;
                default:
                    // Do nothing here. There are other recurrence
                    // types but for simplicity, these aren't covered.
                    break;
            }
        }
    }
    else
    {
        // If it has no end, set an end date to 2 weeks from today.
        recurringMaster.Recurrence.EndDate = DateTime.Now.AddDays(14);
    }
    // Update the series.
    try
    {
        // This method results in a call to EWS.
        recurringMaster.Update(ConflictResolutionMode.AutoResolve);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error updating series: {0}", ex.Message);
        return false;
    }
    return true;
}
```

## <a name="modify-all-occurrences-in-a-series-by-using-ews"></a>EWS を使用して定期的なアイテム内のアイテムをすべて変更する

定期的なアイテム内のアイテムをすべて変更するには、[UpdateItem 操作](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)を使用し、要求の [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) 要素に定期的マスターのアイテム ID を指定する必要があります。 要求の構造は、単一の予定を更新する要求と同じです。 
  
次の例では、定期的なアイテムが次のように更新されます。
  
- [Location](http://msdn.microsoft.com/library/3fcf7133-ae1c-47b4-a187-660045f71df0%28Office.15%29.aspx) 要素を設定することにより、定期的なアイテムの場所を更新します。 
    
- [RequiredAttendees](http://msdn.microsoft.com/library/422f8d44-b0eb-49ca-af0f-0e22b54c78d2%28Office.15%29.aspx) 要素を設定することにより、出席者を更新します。 
    
- [Recurrence (RecurrenceType)](http://msdn.microsoft.com/library/3d1c2c1c-4103-47ce-ad3c-ad16ec6e9b12%28Office.15%29.aspx) 要素を設定することにより、定期的なアイテムを更新します。 
    
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
    <m:UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" SendMeetingInvitationsOrCancellations="SendToAllAndSaveCopy">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Location" />
              <t:CalendarItem>
                <t:Location>Conference Room 2</t:Location>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:RequiredAttendees" />
              <t:CalendarItem>
                <t:RequiredAttendees>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Mack Chaves</t:Name>
                      <t:EmailAddress>mack@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Sadie Daniels</t:Name>
                      <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                </t:RequiredAttendees>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Recurrence" />
              <t:CalendarItem>
                <t:Recurrence>
                  <t:WeeklyRecurrence>
                    <t:Interval>1</t:Interval>
                    <t:DaysOfWeek>Tuesday</t:DaysOfWeek>
                  </t:WeeklyRecurrence>
                  <t:EndDateRecurrence>
                    <t:StartDate>2014-05-06</t:StartDate>
                    <t:EndDate>2014-06-22-04:00</t:EndDate>
                  </t:EndDateRecurrence>
                </t:Recurrence>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:MeetingTimeZone" />
              <t:CalendarItem>
                <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

サーバーは [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) 要素で応答します。この要素には、値が **NoError** (更新が正常に完了したことを示す) の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素が含まれます。
  
## <a name="see-also"></a>関連項目


- [Exchange の予定表と EWS](calendars-and-ews-in-exchange.md)
    
- [定期的なパターンと EWS](recurrence-patterns-and-ews.md)
    
- [Exchange で EWS を使用して予定と会議を更新する](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [EWS を使用して定期的なアイテムを更新する](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Exchange の EWS を使用して定期的なアイテムにアクセスする](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    


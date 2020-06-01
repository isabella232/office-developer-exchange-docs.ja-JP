---
title: EWS を使用して定期的なアイテムを更新する
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7e61bee9-4840-4773-a0a7-47b11e1fdf59
description: Exchange の EWS マネージ API または EWS を使用して、定期的なアイテムの予定を変更する方法を説明します。
ms.openlocfilehash: eb40dd60f28a6acf4395d3149744ce7321c34999
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455850"
---
# <a name="update-a-recurring-series-by-using-ews"></a>EWS を使用して定期的なアイテムを更新する

Exchange の EWS マネージ API または EWS を使用して、定期的なアイテムの予定を変更する方法を説明します。
  
EWS マネージ API または EWS を使用して、[定期的なアイテム全体を更新する](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)か、1 つのオカレンスを更新することによって定期的なアイテムを更新します。この記事では、1 つのオカレンスを更新する方法について説明します。
  
定期的なアイテムの単一の予定を変更するのは、[予定の単一のインスタンスを変更する](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)ことによく似ています。同じメソッドと操作を使用しますが、変更するオカレンスのアイテム ID を使用します。
  
定期的なアイテムの単一のオカレンスを変更する場合、そのオカレンスは、定期的なアイテムの定期的マスターに関連付けられている変更された予定の配列に追加されます。 [Appointment.ModifiedOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) EWS マネージ API プロパティまたは [ModifiedOccurrences](https://msdn.microsoft.com/library/552932fc-b3b4-486e-8d73-32c0bb10bd68%28Office.15%29.aspx) EWS 要素を使用して、変更された定期的なアイテムのすべての予定にアクセスできます。 
  
## <a name="modify-a-single-occurrence-in-a-series-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して定期的なアイテムの単一のオカレンスを変更する

定期的なアイテムの単一のインスタンスを変更するには、次の操作を実行します。
  
1. アイテムのインデックス値を指定した [Appointment.BindToOccurrence](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx) メソッドまたはオカレンスの ID を指定した [Appointment.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) メソッドを使用して、変更するオカレンスにバインドします。 この ID は、オカレンスに対応する [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクトの [Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) プロパティまたは、オカレンスに対応する [OccurrenceInfo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.occurrenceinfo%28v=exchg.80%29.aspx) オブジェクトの [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.occurrenceinfo.itemid%28v=exchg.80%29.aspx) プロパティから取得します。 
    
2. オカレンスの Appointment オブジェクトのプロパティを更新します。
    
3. [Appointment.Save](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) メソッドを使用して、オカレンスの予定オブジェクトへ変更を保存します。 
    
次の例では、定期的なアイテムでの予定を更新し、変更された予定が定期的マスター上で更新されたことを確認します。 この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。 `recurrenceMasterId` パラメーターは、変更するオカレンスの定期的マスターに関連付けられている識別子です。 
  
```cs
public static ItemId ModifyARecurringSeries(ExchangeService service, ItemId recurrenceMasterId)
{
    Appointment calendarItem = Appointment.Bind(service, recurrenceMasterId, new PropertySet(AppointmentSchema.AppointmentType));
    Appointment recurrMaster = new Appointment(service);
    if (calendarItem.AppointmentType == AppointmentType.RecurringMaster)
    {
        // Get the recurring master from an occurrence in a recurring series with the properties you need.
        recurrMaster = Appointment.Bind(service,
                                        recurrenceMasterId,
                                        new PropertySet(AppointmentSchema.AppointmentType,
                                                        AppointmentSchema.Subject,
                                                        AppointmentSchema.FirstOccurrence,
                                                        AppointmentSchema.LastOccurrence,
                                                        AppointmentSchema.ModifiedOccurrences,
                                                        AppointmentSchema.DeletedOccurrences));
    }
    else
    {
        Console.WriteLine("Item id was not for a recurring master.");
        return recurrenceMasterId;
    }
    // Bind to the second occurrence in the series with the properties to modify.
    Appointment occurrenceToModify = Appointment.BindToOccurrence(service,
                                                                    recurrMaster.Id,
                                                                    2,
                                                                    new PropertySet(AppointmentSchema.Location,
                                                                                    AppointmentSchema.Start,
                                                                                    AppointmentSchema.End,
                                                                                    AppointmentSchema.RequiredAttendees,
                                                                                    AppointmentSchema.Subject));
    // Update the properties you want to change.
    occurrenceToModify.Location = "Helipad of Contoso Bldg 1";
    occurrenceToModify.Start = occurrenceToModify.Start.AddDays(1);
    occurrenceToModify.End = occurrenceToModify.End.AddDays(1);
    occurrenceToModify.RequiredAttendees.Add("Contoso CEO", "sadie@contoso");
    occurrenceToModify.RequiredAttendees.Add("Contoso Head of Research", "ronnie@contoso.com");
    occurrenceToModify.RequiredAttendees.Add("Contoso Head of Security", "alfred@contoso.com");
    occurrenceToModify.Subject = occurrenceToModify.Subject.ToString() + ":Mandatory";
    // Update the occurrence in your calendar folder and send meeting update requests to attendees.
    // This method call results in an UpdateItem request to EWS.
    occurrenceToModify.Update(ConflictResolutionMode.AlwaysOverwrite, SendInvitationsOrCancellationsMode.SendToAllAndSaveCopy);
    // View updated and deleted occurrences on the recurring master prior to retrieving updated information.
    Console.WriteLine("Modified Occurrences prior to updating recurring master: {0}",
                    (recurrMaster.ModifiedOccurrences == null ? "None" : recurrMaster.ModifiedOccurrences.Count.ToString()));
    // Update the recurring master to view the modified and deleted occurrences.
    recurrMaster = Appointment.Bind(service, recurrenceMasterId, new PropertySet(AppointmentSchema.ModifiedOccurrences,
                                                                        AppointmentSchema.DeletedOccurrences));
    // View updated and deleted occurrences on the recurring master after retrieving updated information.
    Console.WriteLine("Modified Occurrences after updating recurring master:\t {0}",
                    (recurrMaster.ModifiedOccurrences == null ? "None" : recurrMaster.ModifiedOccurrences.Count.ToString()));
    return recurrMaster.Id;            
}

```

## <a name="modify-a-single-occurrence-in-a-series-by-using-ews"></a>EWS を使用して定期的なアイテムの単一のオカレンスを変更する

定期的なアイテムの単一のインスタンスを変更するのは、予定の単一のインスタンスを変更することと基本的に同じです。 [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) または [OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) 要素を使用して、変更するオカレンスを指定できます。 
  
次の例は、[UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) 操作を利用して、予定の定期的なアイテムでオカレンスを更新するときの、要求 XML を表しています。 **ItemId** と **ChangeKey** は読みやすいように短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:UpdateItem ConflictResolution="AlwaysOverwrite" SendMeetingInvitationsOrCancellations="SendToAllAndSaveCopy">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAAB" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Location" />
              <t:CalendarItem>
                <t:Location>Helipad of Contoso Bldg 1</t:Location>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Start" />
              <t:CalendarItem>
                <t:Start>2014-03-27T19:33:00.000-07:00</t:Start>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:End" />
              <t:CalendarItem>
                <t:End>2014-03-27T20:33:00.000-07:00</t:End>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:RequiredAttendees" />
              <t:CalendarItem>
                <t:RequiredAttendees>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Mack@contoso.com</t:Name>
                      <t:EmailAddress>Mack@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Sadie@contoso.com</t:Name>
                      <t:EmailAddress>Sadie@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Magdalena@contoso.com</t:Name>
                      <t:EmailAddress>Magdalena@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Contoso CEO</t:Name>
                      <t:EmailAddress>sadie@contoso</t:EmailAddress>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Contoso Head of Research</t:Name>
                      <t:EmailAddress>ronnie@contoso.com</t:EmailAddress>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Contoso Head of Security</t:Name>
                      <t:EmailAddress>alfred@contoso.com</t:EmailAddress>
                    </t:Mailbox>
                  </t:Attendee>
                </t:RequiredAttendees>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Weekly Update Meeting:Mandatory</t:Subject>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

サーバーは、[UpdateItemResponse](https://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) メッセージで **UpdateItem** 要求に応答します。このメッセージには、オカレンスが正常に更新されたことを示す **NoError** の [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値、および更新された予定の [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) が含まれます。 
  
## <a name="see-also"></a>関連項目


- [Exchange の予定表と EWS](calendars-and-ews-in-exchange.md)
    
- [Exchange の EWS を使用して予定と会議を更新する](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [定期的なパターンと EWS](recurrence-patterns-and-ews.md)
    
- [Exchange の EWS を使用して定期的なアイテムにアクセスする](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Exchange の EWS を使用して定期的なアイテムを作成する](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Exchange の EWS を使用して定期的なアイテムを削除する](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Exchange の EWS を使用して定期的なアイテムを更新する](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    


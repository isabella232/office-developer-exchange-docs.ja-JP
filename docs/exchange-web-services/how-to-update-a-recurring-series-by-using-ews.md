---
title: EWS を使用して定期的なアイテムを更新する
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7e61bee9-4840-4773-a0a7-47b11e1fdf59
description: Exchange の EWS マネージ API または EWS を使用して、定期的なアイテムの予定を変更する方法を説明します。
ms.openlocfilehash: ecee78457d2e6f91483cf897cfb4976fbd83400c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759071"
---
# <a name="update-a-recurring-series-by-using-ews"></a><span data-ttu-id="5d866-103">EWS を使用して定期的なアイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="5d866-103">How to: Update a recurring series by using EWS</span></span>

<span data-ttu-id="5d866-104">Exchange の EWS マネージ API または EWS を使用して、定期的なアイテムの予定を変更する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="5d866-104">Learn how to modify appointments in a recurring series by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="5d866-105">EWS マネージ API または EWS を使用して、[定期的なアイテム全体を更新する](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)か、単一のオカレンスを更新することによって定期的なアイテムを更新します。</span><span class="sxs-lookup"><span data-stu-id="5d866-105">You can use the EWS Managed API or EWS to update a recurring series by either [updating the entire series](how-to-update-a-recurring-series-by-using-ews-in-exchange.md), or by updating a single occurrence. In this article we'll discuss how to update a single occurrence.</span></span> <span data-ttu-id="5d866-106">この記事では、1 つのオカレンスを更新する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="5d866-106">In this article we'll discuss how to update a single occurrence.</span></span>
  
<span data-ttu-id="5d866-107">定期的なアイテムの単一の予定を変更するのは、[予定の単一のインスタンスを変更する](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)ことによく似ています。</span><span class="sxs-lookup"><span data-stu-id="5d866-107">Modifying a single appointment in a series is very similar to modifying a single instance appointment. You use the same methods and operations, but you use the item ID of the occurrence you want to change.</span></span> <span data-ttu-id="5d866-108">同じメソッドと操作を使用しますが、変更するオカレンスのアイテム ID を使用します。</span><span class="sxs-lookup"><span data-stu-id="5d866-108">Modifying a single appointment in a series is very similar to modifying a single instance appointment. You use the same methods and operations, but you use the item ID of the occurrence you want to change.</span></span>
  
<span data-ttu-id="5d866-109">定期的なアイテムの単一のオカレンスを変更する場合、そのオカレンスは、定期的なアイテムの定期的マスターに関連付けられている変更された予定の配列に追加されます。</span><span class="sxs-lookup"><span data-stu-id="5d866-109">When you change a single occurrence in a series, that occurrence is added to an array of modified appointments associated with the recurring master for the series. You can use the Appointment.ModifiedOccurrenceshttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences(v=exchg.80).aspx EWS Managed API property or the ModifiedOccurrences EWS element to access all the appointments in a series that have been modified.</span></span> <span data-ttu-id="5d866-110">[Appointment.ModifiedOccurrences](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) EWS マネージ API プロパティまたは [ModifiedOccurrences](http://msdn.microsoft.com/library/552932fc-b3b4-486e-8d73-32c0bb10bd68%28Office.15%29.aspx) EWS 要素を使用して、変更された定期的なアイテムのすべての予定にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="5d866-110">You can use the [Appointment.ModifiedOccurrences](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) EWS Managed API property or the [ModifiedOccurrences](http://msdn.microsoft.com/library/552932fc-b3b4-486e-8d73-32c0bb10bd68%28Office.15%29.aspx) EWS element to access all the appointments in a series that have been modified.</span></span> 
  
## <a name="modify-a-single-occurrence-in-a-series-by-using-the-ews-managed-api"></a><span data-ttu-id="5d866-111">EWS マネージ API を使用して定期的なアイテムの単一のオカレンスを変更する</span><span class="sxs-lookup"><span data-stu-id="5d866-111">Modify a single occurrence in a series by using the EWS Managed API</span></span>

<span data-ttu-id="5d866-112">定期的なアイテムの単一のインスタンスを変更するには、次の操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="5d866-112">To modify a single instance in a series, you:</span></span>
  
1. <span data-ttu-id="5d866-113">アイテムのインデックス値を指定した [Appointment.BindToOccurrence](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx) メソッドまたはオカレンスの ID を指定した [Appointment.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) メソッドを使用して、変更するオカレンスにバインドします。</span><span class="sxs-lookup"><span data-stu-id="5d866-113">Bind to the occurrence you want to modify by using either the [Appointment.BindToOccurrence](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx) method with the item's index value, or the [Appointment.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) method with the occurrence's ID.</span></span> <span data-ttu-id="5d866-114">この ID は、オカレンスに対応する [Appointment](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクトの [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) プロパティまたは、オカレンスに対応する [OccurrenceInfo](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.occurrenceinfo%28v=exchg.80%29.aspx) オブジェクトの [ItemId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.occurrenceinfo.itemid%28v=exchg.80%29.aspx) プロパティから取得します。</span><span class="sxs-lookup"><span data-stu-id="5d866-114">You obtain this ID from either the [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) property of an [Appointment](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object that corresponds to the occurrence, or from the [ItemId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.occurrenceinfo.itemid%28v=exchg.80%29.aspx) property of the [OccurrenceInfo](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.occurrenceinfo%28v=exchg.80%29.aspx) object that corresponds to the occurrence.</span></span> 
    
2. <span data-ttu-id="5d866-115">オカレンスの Appointment オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5d866-115">Update the properties on the occurrence's Appointment object.</span></span>
    
3. <span data-ttu-id="5d866-116">[Appointment.Save](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) メソッドを使用して、オカレンスの予定オブジェクトへ変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="5d866-116">Save the changes to the occurrence's appointment object by using the [Appointment.Savehttp://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.save(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="5d866-117">次の例では、定期的なアイテムでの予定を更新し、変更された予定が定期的マスター上で更新されたことを確認します。</span><span class="sxs-lookup"><span data-stu-id="5d866-117">The following example updates an appointment in a recurring series and verifies that the modified appointment is updated on the recurring master.</span></span> <span data-ttu-id="5d866-118">この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。</span><span class="sxs-lookup"><span data-stu-id="5d866-118">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeServicehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="5d866-119">`recurrenceMasterId` パラメーターは、変更するオカレンスの定期的マスターに関連付けられている識別子です。</span><span class="sxs-lookup"><span data-stu-id="5d866-119">The  `recurrenceMasterId` parameter is an identifier associated with the recurring master for the occurrence to modify.</span></span> 
  
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

## <a name="modify-a-single-occurrence-in-a-series-by-using-ews"></a><span data-ttu-id="5d866-120">EWS を使用して定期的なアイテムの単一のオカレンスを変更する</span><span class="sxs-lookup"><span data-stu-id="5d866-120">Modify a single occurrence in a series by using EWS</span></span>

<span data-ttu-id="5d866-121">定期的なアイテムの単一のインスタンスを変更するのは、予定の単一のインスタンスを変更することと基本的に同じです。</span><span class="sxs-lookup"><span data-stu-id="5d866-121">Modifying a single instance in a series is essentially the same as modifying a single instance appointment. You can specify the occurrence to change by using either an ItemId or an OccurrenceItemId element.</span></span> <span data-ttu-id="5d866-122">[ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) または [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) 要素を使用して、変更するオカレンスを指定できます。</span><span class="sxs-lookup"><span data-stu-id="5d866-122">Modifying a single instance in a series is essentially the same as modifying a single instance appointment. You can specify the occurrence to change by using either an [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) or an [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="5d866-123">次の例は、[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) 操作を利用して、予定の定期的なアイテムでオカレンスを更新するときの、要求 XML を表しています。</span><span class="sxs-lookup"><span data-stu-id="5d866-123">The following example shows the request XML when you use the [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) operation to update an occurrence in a recurring series of appointments. The ItemId and ChangeKey are shortened for readability.</span></span> <span data-ttu-id="5d866-124">**ItemId** と **ChangeKey** は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="5d866-124">The ItemId and ChangeKey attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="5d866-125">サーバーは、[UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) メッセージで **UpdateItem** 要求に応答します。このメッセージには、オカレンスが正常に更新されたことを示す **NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値、および更新された予定の [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5d866-125">The server responds to the **UpdateItem** request with an [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the occurrence was updated successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the updated appointment.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="5d866-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="5d866-126">See also</span></span>


- [<span data-ttu-id="5d866-127">Exchange の予定表と EWS</span><span class="sxs-lookup"><span data-stu-id="5d866-127">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="5d866-128">Exchange の EWS を使用して予定と会議を更新する</span><span class="sxs-lookup"><span data-stu-id="5d866-128">How to: Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="5d866-129">定期的なパターンと EWS</span><span class="sxs-lookup"><span data-stu-id="5d866-129">Recurrence patterns and EWS</span></span>](recurrence-patterns-and-ews.md)
    
- [<span data-ttu-id="5d866-130">Exchange の EWS を使用して定期的なアイテムにアクセスする</span><span class="sxs-lookup"><span data-stu-id="5d866-130">How to: Access a recurring series by using EWS in Exchange</span></span>](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="5d866-131">Exchange の EWS を使用して定期的なアイテムを作成する</span><span class="sxs-lookup"><span data-stu-id="5d866-131">How to: Create a recurring series by using EWS in Exchange</span></span>](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="5d866-132">Exchange の EWS を使用して定期的なアイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="5d866-132">How to: Delete appointments in a recurring series by using EWS in Exchange</span></span>](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="5d866-133">Exchange の EWS を使用して定期的なアイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="5d866-133">How to: Update a recurring series by using EWS in Exchange</span></span>](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    


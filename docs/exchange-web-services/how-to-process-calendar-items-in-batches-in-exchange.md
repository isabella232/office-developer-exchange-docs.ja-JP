---
title: Exchange においてバッチ処理で予定表アイテムを処理する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: fb2952e2-cbfe-43ac-b746-f071faa7665c
description: Exchange で EWS マネージ API または EWS を使用して、1 回の呼び出しで予定表アイテムの作成、取得、更新、または削除をバッチ処理する方法について説明します。
ms.openlocfilehash: 1c4431ab86088d4a8a5d8e2e8378e392786fa8b5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513109"
---
# <a name="process-calendar-items-in-batches-in-exchange"></a>Exchange においてバッチ処理で予定表アイテムを処理する

Exchange で EWS マネージ API または EWS を使用して、1 回の呼び出しで予定表アイテムの作成、取得、更新、または削除をバッチ処理する方法について説明します。

EWS マネージ API または EWS を使用すると、予定と会議のバッチ処理を行うことができ、Exchange サーバーに対するクライアントの呼び出し回数が減少します。 EWS マネージ API を使用して予定表アイテムのバッチ処理を作成、取得、更新、削除する場合は、[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクト メソッドを使用します。1 つの予定表アイテムが処理対象の場合には [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクト メソッドを使用します。 EWS を使用している場合は、単一の呼び出しと同じバッチ呼び出しの操作を使用します。

**表 1. 予定表アイテムをバッチ処理するための EWS マネージ API メソッドと EWS 操作**

|**目的**|**使用する EWS マネージ API メソッド**|**使用する EWS 操作**|
|:-----|:-----|:-----|
|バッチ処理で予定表アイテムを作成する  <br/> |[CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|バッチ処理で予定表アイテムを取得する  <br/> |[BindToItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|バッチ処理で予定表アイテムを更新する  <br/> |[UpdateItems](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) <br/> |[UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|バッチ処理で予定表アイテムを削除する  <br/> |[DeleteItems](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) <br/> |[DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |

この記事では、EWS マネージ API または EWS を使用して予定表アイテムのバッチ処理を行うための基本的なタスクの実行方法について説明します。

この記事の EWS マネージ API の例では、メソッドが連続して呼び出される場合に予定表アイテムのバッチを作成、取得、更新、および削除できます。

```cs
Collection<ItemId> itemIds = BatchCreateCalendarItems(service);
Collection<Appointment> myAppointments = BatchGetCalendarItems(service, itemIds);
itemIds = BatchUpdateCalendarItems(service, myAppointments);
BatchDeleteCalendarItemsTwice(service, itemIds);

```

## <a name="create-calendar-items-in-batches-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してバッチ処理で予定表アイテムを作成する
<a name="bk_createewsma"> </a>

次の例に示されているように、EWS マネージ API の [CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) メソッドを使用すると、バッチ処理で予定表アイテムを作成できます。 この例では 3 つの [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクト (単一インスタンスの予定、定期的な予定、および会議) を作成して、これらをコレクションに追加します。

この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。

```cs
public static Collection<ItemId> BatchCreateCalendarItems(ExchangeService service)
{
    // These are unsaved local instances of an Appointment object.
    // Despite the required parameter of an ExchangeService object (service), no call
    // to an Exchange server is made when the objects are instantiated.
    // A call to the Exchange server is made when the service.CreateItems() method is called.
    Appointment appt1 = new Appointment(service);
    Appointment recurrAppt2 = new Appointment(service);
    Appointment meeting3 = new Appointment(service);
    // Set the properties for a single instance appointment.
    appt1.Subject = "Review current quarterly deliverables";
    appt1.Body = "Wrap up all outstanding deliverables for this quarter and prepare for Q2.";
    appt1.Start = DateTime.Now.AddDays(2);
    appt1.End = appt1.Start.AddHours(3);
    appt1.Location = "My office";
    appt1.ReminderMinutesBeforeStart = 30;
    // Set the properties for a recurring appointment.
    recurrAppt2.Subject = "Food bank delivery";
    recurrAppt2.Body = "Deliver the team's weekly food drive collection to the food bank.";
    recurrAppt2.Start = DateTime.Now.AddDays(1);
    recurrAppt2.End = recurrAppt2.Start.AddHours(1);
    recurrAppt2.Location = "Local food bank";
    arecurrAppt2.ReminderMinutesBeforeStart = 30;
    DayOfTheWeek[] dow = new DayOfTheWeek[] {(DayOfTheWeek)recurrAppt2.Start.DayOfWeek};
    recurrAppt2.Recurrence = new Recurrence.WeeklyPattern(recurrAppt2.Start.Date, 1, dow);
    recurrAppt2.Recurrence.StartDate = recurrAppt2.Start.Date;
    recurrAppt2.Recurrence.NumberOfOccurrences = 10;
    // Set the properties for a single instance meeting.
    meeting3.Subject = "Code Blast";
    meeting3.Body = "Let's get together to finish all the methods and unit tests for the ContosoLive project.";
    meeting3.Start = DateTime.Now.AddDays(3);
    meeting3.End = meeting3.Start.AddHours(6);
    meeting3.Location = "The lounge";
    meeting3.RequiredAttendees.Add("Mack@contoso.com");
    meeting3.RequiredAttendees.Add("Sadie@contoso.com");
    meeting3.RequiredAttendees.Add("Magdalena@contoso.com");
    meeting3.ReminderMinutesBeforeStart = 30;
    // Add the appointment objects to a collection.
    Collection<Appointment> calendarItems = new Collection<Appointment>() { appt1, recurrAppt2, meeting3 };
    // Instantiate a collection of item IDs to populate from the values that are returned by the Exchange server.
    Collection<ItemId> itemIds = new Collection<ItemId>();

    // Send the batch of Appointment objects.
    // Note that multiple calls to the Exchange server might be made when Appointment objects have attachments.
    // Note also that the the ID of the item collection passed as the first parameter to CreateItems is set on return.
    ServiceResponseCollection<ServiceResponse> response = service.CreateItems(calendarItems,
                                                                              WellKnownFolderName.Calendar,
                                                                              MessageDisposition.SendAndSaveCopy,
                                                                              SendInvitationsMode.SendToAllAndSaveCopy);
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("All appointments and meetings sucessfully created.");
    }
    // Collect the item IDs from the created calendar items.
    foreach (Appointment appt in calendarItems)
    {
        itemIds.Add(appt.Id);
    }
    int counter = 1;
    // Show the IDs and errors for each message.
    foreach (ServiceResponse resp in response)
    {
        // Because item IDs are long, show only five characters.
        Console.WriteLine("Result (message {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(0, 5), resp.Result);
        Console.WriteLine("Error Code: {0}", resp.ErrorCode);
        Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
        counter++;
    }
// Return the collection of item IDs.
return itemIds;
}

```

コレクション内の [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクトは、予定または会議、および単一のインスタンスか定期的なアイテムのいずれかとして使用できます。

## <a name="create-calendar-items-in-batches-by-using-ews"></a>EWS を使用してバッチ処理で予定表アイテムを作成する
<a name="bk_createews"> </a>

次のコード例に示すように、EWS の [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) 操作を使用して、バッチ処理で予定表アイテムを作成できます。これは、EWS マネージ API を使用して[バッチ処理で予定表アイテムを作成](#bk_createewsma)するときに EWS マネージ API が送信する XML 要求でもあります。

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy" SendMeetingInvitations="SendToAllAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Review current quarterly deliverables</t:Subject>
          <t:Body BodyType="HTML">Wrap up all outstanding deliverables for this quarter and prepare for Q2.</t:Body>
          <t:ReminderDueBy>2014-01-07T12:13:40.333-08:00</t:ReminderDueBy>
          <t:Start>2014-01-08T13:13:37.717-08:00</t:Start>
          <t:End>2014-01-08T16:13:37.717-08:00</t:End>
          <t:Location>Local food bank</t:Location>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
        <t:CalendarItem>
          <t:Subject>Food bank delivery</t:Subject>
          <t:Body BodyType="HTML">Deliver the team's weekly food drive collection to the food bank.</t:Body>
          <t:Start>2014-01-07T13:13:40.333-08:00</t:Start>
          <t:End>2014-01-07T14:13:40.333-08:00</t:End>
          <t:Recurrence>
            <t:WeeklyRecurrence>
              <t:Interval>1</t:Interval>
              <t:DaysOfWeek>Tuesday</t:DaysOfWeek>
            </t:WeeklyRecurrence>
            <t:NumberedRecurrence>
              <t:StartDate>2014-01-07-08:00</t:StartDate>
              <t:NumberOfOccurrences>10</t:NumberOfOccurrences>
            </t:NumberedRecurrence>
          </t:Recurrence>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
        <t:CalendarItem>
          <t:Subject>Code Blast</t:Subject>
          <t:Body BodyType="HTML">Let's get together to finish all the methods and unit tests for the ContosoLive project.</t:Body>
          <t:ReminderMinutesBeforeStart>30</t:ReminderMinutesBeforeStart>
          <t:Start>2014-01-09T13:13:44.998-08:00</t:Start>
          <t:End>2014-01-09T19:13:44.998-08:00</t:End>
          <t:Location>The lounge</t:Location>
          <t:RequiredAttendees>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Mack@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Sadie@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Magdalena@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
          </t:RequiredAttendees>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

サーバーは、**CreateItem** 要求に [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージで応答します。このメッセージには、それぞれの新しい予定表アイテムが正常に作成および保存されたことを示す、**NoError** の [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれます。 

予定表アイテムは Exchange Server に渡された各予定表アイテムの要素の値にしたがって、会議か予定、または単一のインスタンスか定期的なアイテムのいずれかになります。

次の XML はサーバーからの応答です。**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="847" MinorBuildNumber="12" Version="V2_8"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="get-calendar-items-in-batches-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してバッチ処理で予定表アイテムを取得する
<a name="bk_getewsma"> </a>

次の例に示されているように、EWS マネージ API の [BindToItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) メソッドを使用すると、バッチ処理で予定表アイテムを取得できます。

この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。

```cs
public static Collection<Appointment> BatchGetCalendarItems(ExchangeService service, Collection<ItemId> itemIds)
{
    // As a best practice, create a property set that limits the properties returned by the Bind method to only those that are required.
    PropertySet appointmentProps = new PropertySet(BasePropertySet.IdOnly,
                                                   AppointmentSchema.Subject,
                                                   AppointmentSchema.Body,
                                                   AppointmentSchema.ReminderMinutesBeforeStart,
                                                   AppointmentSchema.Start,
                                                   AppointmentSchema.End,
                                                   AppointmentSchema.AppointmentType,
                                                   AppointmentSchema.Location,
                                                   AppointmentSchema.RequiredAttendees);

    ServiceResponseCollection<GetItemResponse> response = service.BindToItems(itemIds, appointmentProps);
    Collection<Appointment> calendarItems = new Collection<Appointment>();
    foreach (GetItemResponse items in response)
    {
        Item item = items.Item;
        Appointment appointmentItem = (Appointment)item;
        calendarItems.Add(appointmentItem);
        Console.WriteLine("Found item {0}.", appointmentItem.Id.ToString().Substring(144));
    }
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("All calendar items retrieved successfully.");
        Console.WriteLine("\r\n");
    }
    else
    {
        int counter = 1;
        // List the status of each message.
        foreach (ServiceResponse resp in response)
        {
            // Because item IDs are long, show only last 8 characters.
            Console.WriteLine("Result (message {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(144), resp.Result);
            Console.WriteLine("Error Code: {0}", resp.ErrorCode);
            Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
            Console.WriteLine("\r\n");
            counter++;
        }
    }
    return calendarItems;
}

```

## <a name="get-calendar-items-in-batches-by-using-ews"></a>EWS を使用してバッチ処理で予定表アイテムを取得する
<a name="bk_getews"> </a>

次の例に示すように、EWS の [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) 操作を使用して、バッチ処理で予定表アイテムを取得できます。これは、EWS マネージ API を使用して[バッチ処理で予定表アイテムを取得](#bk_getewsma)するときに EWS マネージ API が送信する XML 要求でもあります。

**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:Body" />
          <t:FieldURI FieldURI="item:ReminderMinutesBeforeStart" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:RequiredAttendees" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>

```

サーバーは **GetItem** 要求に [GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) メッセージで応答します。このメッセージには、次の例に示すように、各アイテムの要求されたプロパティが含まれます。

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="847" MinorBuildNumber="16" Version="V2_8"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
              <t:Subject>Review current quarterly deliverables</t:Subject>
              <t:Body BodyType="HTML">
                &amp;lt;html&amp;gt;
                &amp;lt;head&amp;gt;
                &amp;lt;meta http-equiv="Content-Type" content="text/html; charset=utf-8"&amp;gt;
                &amp;lt;/head&amp;gt;
                &amp;lt;body&amp;gt;
                Wrap up all outstanding deliverables for this quarter and prepare for Q2.
                &amp;lt;/body&amp;gt;
                &amp;lt;/html&amp;gt;
              </t:Body>
              <t:ReminderMinutesBeforeStart>30</t:ReminderMinutesBeforeStart>
              <t:Start>2014-01-19T18:59:07Z</t:Start>
              <t:End>2014-01-19T21:59:07Z</t:End>
              <t:Location>Local food bank</t:Location>
              <t:CalendarItemType>Single</t:CalendarItemType>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
              <t:Subject>Food bank delivery</t:Subject>
              <t:Body BodyType="HTML">
                &amp;lt;html&amp;gt;
                &amp;lt;head&amp;gt;
                &amp;lt;meta http-equiv="Content-Type" content="text/html; charset=utf-8"&amp;gt;
                &amp;lt;/head&amp;gt;
                &amp;lt;body&amp;gt;
                Deliver the team's weekly food drive collection to the food bank.
                &amp;lt;/body&amp;gt;
                &amp;lt;/html&amp;gt;
              </t:Body>
              <t:ReminderMinutesBeforeStart>15</t:ReminderMinutesBeforeStart>
              <t:Start>2014-01-18T18:59:07Z</t:Start>
              <t:End>2014-01-18T19:59:07Z</t:End>
              <t:CalendarItemType>RecurringMaster</t:CalendarItemType>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
              <t:Subject>Code Blast</t:Subject>
              <t:Body BodyType="HTML">
                &amp;lt;html&amp;gt;
                &amp;lt;head&amp;gt;
                &amp;lt;meta http-equiv="Content-Type" content="text/html; charset=utf-8"&amp;gt;
                &amp;lt;/head&amp;gt;
                &amp;lt;body&amp;gt;
                Let's get together to finish all the methods and unit tests for the ContosoLive project.
                &amp;lt;/body&amp;gt;
                &amp;lt;/html&amp;gt;
              </t:Body>
              <t:ReminderMinutesBeforeStart>30</t:ReminderMinutesBeforeStart>
              <t:Start>2014-01-20T18:59:08Z</t:Start>
              <t:End>2014-01-21T00:59:08Z</t:End>
              <t:Location>The lounge</t:Location>
              <t:CalendarItemType>Single</t:CalendarItemType>
              <t:RequiredAttendees>
                <t:Attendee>
                  <t:Mailbox>
                    <t:Name>Mack@contoso.com</t:Name>
                    <t:EmailAddress>Mack@contoso.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                  </t:Mailbox>
                  <t:ResponseType>Unknown</t:ResponseType>
                </t:Attendee>
                <t:Attendee>
                  <t:Mailbox>
                    <t:Name>Sadie@contoso.com</t:Name>
                    <t:EmailAddress>Sadie@contoso.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                  </t:Mailbox>
                  <t:ResponseType>Unknown</t:ResponseType>
                </t:Attendee>
                <t:Attendee>
                  <t:Mailbox>
                    <t:Name>Magdalena@contoso.com</t:Name>
                    <t:EmailAddress>Magdalena@contoso.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                  </t:Mailbox>
                  <t:ResponseType>Unknown</t:ResponseType>
                </t:Attendee>
              </t:RequiredAttendees>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="update-calendar-items-in-batches-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してバッチ処理で予定表アイテムを更新する
<a name="bk_updateewsma"> </a>

次の例に示されているように、EWS マネージ API の [UpdateItems](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) メソッドを使用すると、バッチ処理で予定表アイテムのプロパティを更新できます。

この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。

```cs
public static Collection<ItemId> BatchUpdateCalendarItems(ExchangeService service, Collection<Appointment> calendarItems)
{
    int i = 1;
    // Appointment item IDs to return.
    Collection<ItemId> itemIds = new Collection<ItemId>();

    // Update the subject of each calendar item locally.
    foreach (Appointment appointment in calendarItems)
    {
        // Update the subject of each calendar item in the collection
        appointment.Subject = "Company headquarters are moving down the street to 1234 Contoso Drive!: " + appointment.Subject.ToString();
        Console.WriteLine("Updated the subject property for calendar item {0} of {1}, item id {2}.", i, calendarItems.Count, appointment.Id.ToString().Substring(0, 5));
        i++;
        // Collect item IDs to return instead of appointment objects.
        itemIds.Add(appointment.Id);
    }
    // Send the updated items to the server.
    // This method call results in an UpdateItem call to EWS.
    ServiceResponseCollection<UpdateItemResponse> response = service.UpdateItems(calendarItems,
                                                                                 WellKnownFolderName.Calendar,
                                                                                 ConflictResolutionMode.AutoResolve,
                                                                                 MessageDisposition.SendAndSaveCopy,
                                                                                    SendInvitationsOrCancellationsMode.SendToChangedAndSaveCopy);
    // Display the result of the UpdateItems method call.
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("Calendar items successfully updated.\r\n");
    }
    else
    {
        Console.WriteLine("Not all items were successfully updated on the server.\r\n");
        i = 1;
        foreach (ServiceResponse srvResponse in response)
        {
            Console.WriteLine("Result for message {0}: {1}", i, srvResponse.Result);
            Console.WriteLine("Error code: {0}", srvResponse.ErrorCode);
            Console.WriteLine("ErrorMessage: {0}\r\n", srvResponse.ErrorMessage);
            i++;
        }
    }
    return itemIds;
}

```

## <a name="update-calendar-items-in-batches-by-using-ews"></a>EWS を使用してバッチ処理で予定表アイテムを更新する
<a name="bk_updateews"> </a>

次のコード例に示されているように、EWS の [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) 操作を使用して、複数の予定表アイテムを更新できます。これは、EWS マネージ API を使用して[バッチ処理で予定表アイテムを更新](#bk_updateewsma)するときに EWS マネージ API が送信する XML 要求でもあります。

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:UpdateItem MessageDisposition="SendAndSaveCopy" ConflictResolution="AutoResolve"
                  SendMeetingInvitationsOrCancellations="SendToChangedAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar" />
      </m:SavedItemFolderId>
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Company headquarters are moving down the street to 1234 Contoso Drive!: Review current quarterly deliverables
                </t:Subject>
                </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Company headquarters are moving down the street to 1234 Contoso Drive!: Food bank delivery</t:Subject>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Company headquarters are moving down the street to 1234 Contoso Drive!: Code Blast</t:Subject>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>

```

サーバーは、**UpdateItem** 要求に [UpdateItemResponse](https://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) メッセージで応答します。このメッセージには、それぞれの更新がサーバーで正常に行われたことを示す、**NoError** の [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれます。競合は、[ConflictResult](https://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) 要素で報告されます。

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="859" MinorBuildNumber="13"
                         Version="V2_8" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UpdateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
          <m:ConflictResults>
            <t:Count>1</t:Count>
          </m:ConflictResults>
        </m:UpdateItemResponseMessage>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
          <m:ConflictResults>
            <t:Count>1</t:Count>
          </m:ConflictResults>
        </m:UpdateItemResponseMessage>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
          <m:ConflictResults>
            <t:Count>1</t:Count>
          </m:ConflictResults>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </m:UpdateItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="delete-calendar-items-in-batches-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してバッチ処理で予定表アイテムを削除する
<a name="bk_deleteewsma"> </a>

次の例に示されているように、EWS マネージ API [DeleteItems](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) メソッドを使用すると、バッチ処理で予定表アイテムを削除できます。 この例では 2 回削除要求を行い、例外がスローされないこと、ただしサーバーが **ErrorItemNotFound** エラーを返して、呼び出しが行われたときに削除対象のアイテムがストアになかったことを示しています。 アイテムが既に削除されていたり、無効なアイテム ID がサーバーに渡されると、このエラーが返されます。

この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。

```cs
public static void BatchDeleteCalendarItemsTwice(ExchangeService service, Collection<ItemId> itemIds)
{
    // Delete the batch of appointment objects
    // This method call results in a DeleteItem call to EWS.
    ServiceResponseCollection<ServiceResponse> response = service.DeleteItems(itemIds,
                                                                                DeleteMode.MoveToDeletedItems,
                                                                                SendCancellationsMode.SendToAllAndSaveCopy,
                                                                                AffectedTaskOccurrence.AllOccurrences);
    int counter = 1;
    // Show the IDs and errors for each message.
    foreach (ServiceResponse resp in response)
    {
        // Because item IDs are long, show only five characters.
        Console.WriteLine("Result (message {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(0, 5), resp.Result);
        Console.WriteLine("Error Code: {0}", resp.ErrorCode);
        Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
        counter++;
    }

    // Now attempt to delete the same items again.
    response = service.DeleteItems(itemIds,
                                    DeleteMode.MoveToDeletedItems,
                                    SendCancellationsMode.SendToAllAndSaveCopy,
                                    AffectedTaskOccurrence.AllOccurrences);
    counter = 1;
    // Show the IDs and errors for each message.
    foreach (ServiceResponse resp in response)
    {
        // Because item IDs are long, show only five characters.
        Console.WriteLine("Result (message {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(0, 5), resp.Result);
        Console.WriteLine("Error Code: {0}", resp.ErrorCode);
        Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
        counter++;
    }
}

```

2 回目に **DeleteItems** メソッドが呼び出されると、例外はスローされませんが、結果にサーバーが **ErrorItemNotFound** エラーを返します。

## <a name="delete-calendar-items-in-batches-by-using-ews"></a>EWS を使用してバッチ処理で予定表アイテムを削除する
<a name="bk_deleteews"> </a>

次のコード例に示されているように、[DeleteItem](../web-service-reference/deleteitem-operation.md) EWS 操作を使用して、バッチ処理で予定表アイテムを削除できます。これは、EWS マネージ API を使用して[バッチ処理で予定表アイテムを削除](#bk_deleteewsma)するときに EWS マネージ API が送信する XML 要求でもあります。 

**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="MoveToDeletedItems"
                  AffectedTaskOccurrences="AllOccurrences"
                  SendMeetingCancellations="SendToAllAndSaveCopy">
      <m:ItemIds>
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>

```

サーバーは、**DeleteItem** 要求に [DeleteItemResponse](https://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) メッセージで応答します。このメッセージには、削除された各アイテムの **NoError** の [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれます。 

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="859" MinorBuildNumber="13" Version="V2_8"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:DeleteItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </m:DeleteItemResponse>
  </s:Body>
</s:Envelope>

```

関連付けられたアイテムが既に削除されているときに **DeleteItem** 要求が行われると、例外はスローされませんが、結果としてサーバーが **ErrorItemNotFound** エラーを返します。次の例では、関連付けられたアイテムが既に削除されているときに、サーバーが **DeleteItem** 要求に応答します。

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="859" MinorBuildNumber="13" Version="V2_8"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:DeleteItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteItemResponseMessage>
        <m:DeleteItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteItemResponseMessage>
        <m:DeleteItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </m:DeleteItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="verifying-that-a-batch-process-completed-successfully"></a>バッチ処理が正常に完了したことを確認する
<a name="bk_successful"> </a>

バッチ要求の 1 つ以上の予定表アイテムを要求どおりに処理できないと、失敗した予定表アイテムごとにエラーが返されます。バッチ処理のそれ以外の予定表アイテムは想定どおりに処理されます。対象アイテムが削除されたために送信、取得、更新できなかったり、対象アイテムが別のフォルダーに移動したためにアイテム ID が新しくなり、送信されたアイテム ID で変更できない場合は、バッチ処理でエラーが生じます。このセクションの情報には、予定表アイテムのバッチ処理で生じたエラーの詳細を取得する方法が示されています。

EWS マネージ API を使用してバッチ処理が成功したかどうかは、[ServiceResponseCollection](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) の [OverallResult](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) プロパティが [ServiceResult.Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx) と等しいかどうかを調べることで確認できます。 等しい場合は、すべての予定表アイテムが正常に処理されています。 **OverallResult** が **ServiceResult.Success** と等しくない場合は、1 つ以上の予定表アイテムが正常に処理されませんでした。 **ServiceResponseCollection** で返される各オブジェクトには、次のプロパティが含まれます。

- [ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)

- [ErrorDetails](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)

- [ErrorMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)

- [ErrorProperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)

- [Result](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)

これらのプロパティには、予定表アイテムを要求どおりに処理できなかった原因についての情報が含まれます。この記事の例では、エラーが生じた各アイテムの **Result**、**ErrorCode**、**ErrorMessage** が出力されます。これらの結果を使用して問題を調査できます。

EWS でバッチ処理が成功したことを確認するには、各処理対象アイテムの [ResponseClass](https://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) 属性を調べます。すべての応答メッセージの派生元となる基本タイプの **ResponseMessageType** の基本構造を次に示します。 

```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

**ResponseClass** 属性は、予定表アイテムが正常に処理された場合には **Success** に設定され、正常に処理されなかった場合には **Error** に設定されます。予定表アイテムの場合、バッチ処理中に **Warning** が示されることはありません。**ResponseClass** が **Success** の場合、それに続く [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素は必ず **NoError** に設定されます。**ResponseClass** が **Error** の場合、[MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx)、**ResponseCode**、[MessageXml](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) の各要素の値を確認し、問題の原因を特定する必要があります。[DescriptiveLinkKey](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) は現在使用されていません。

## <a name="see-also"></a>関連項目


- [Exchange の予定表と EWS](calendars-and-ews-in-exchange.md)

- [Exchange の EWS を使用して予定と会議を取得する](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)

- [Exchange で EWS を使用して予定と会議を更新する](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)

- [Exchange の EWS を使用して、予定を削除し、会議をキャンセルする](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)

- [Exchange においてバッチ処理で予定表アイテムを処理する](how-to-process-calendar-items-in-batches-in-exchange.md)

- [EWS のバッチ要求の調整の影響](ews-throttling-in-exchange.md#throttling-implications-for-ews-batch-requests)

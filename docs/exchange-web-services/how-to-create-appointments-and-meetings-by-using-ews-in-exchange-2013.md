---
title: Exchange 2013 の EWS を使用して予定と会議を作成する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fdea70a4-9267-4e5d-9152-b749e2acc3b0
description: Exchange で EWS マネージ API または EWS を使用して、予定と会議を作成する方法について説明します。
ms.openlocfilehash: 1c840fac2ecca9fb51a28044dfac6299cb4fc038
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758940"
---
# <a name="create-appointments-and-meetings-by-using-ews-in-exchange-2013"></a><span data-ttu-id="2da56-103">Exchange 2013 の EWS を使用して予定と会議を作成する</span><span class="sxs-lookup"><span data-stu-id="2da56-103">How to: Create appointments and meetings by using EWS in Exchange 2013</span></span>

<span data-ttu-id="2da56-104">Exchange で EWS マネージ API または EWS を使用して、予定と会議を作成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="2da56-104">Learn how to create appointments and meetings by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="2da56-105">会議と予定の根本的な違いは、会議には出席者がいますが、予定にはいない点です。</span><span class="sxs-lookup"><span data-stu-id="2da56-105">The essential difference between meetings and appointments is that meetings have attendees, and appointments don't.</span></span> <span data-ttu-id="2da56-106">予定も会議も、単一のインスタンスまたは定期的に連続で発生するアイテムの一部ですが、予定は出席者、会議室、またはリソースを含まないため、メッセージの送信を必要としません。</span><span class="sxs-lookup"><span data-stu-id="2da56-106">Both appointments and meetings can be single instances or part of a recurring series, but because appointments don't include attendees, rooms, or resources, they do not require a message to be sent.</span></span> <span data-ttu-id="2da56-107">内部的には、Exchange は会議と予定の両方に同じオブジェクトを使用します。</span><span class="sxs-lookup"><span data-stu-id="2da56-107">Internally, Exchange uses the same object for both meetings and appointments.</span></span> <span data-ttu-id="2da56-108">EWS マネージ API [Appointment クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)または EWS [CalendarItem](http://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) 要素を使用して、会議や予定を操作します。</span><span class="sxs-lookup"><span data-stu-id="2da56-108">You use the EWS Managed API [Appointment class](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) or the EWS [CalendarItem](http://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) element to work with meetings and appointments.</span></span> 
  
<span data-ttu-id="2da56-109">**表 1. 予定や会議を処理するための EWS マネージ API メソッドおよび EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="2da56-109">**Table 1.  EWS Managed API methods and EWS operations for working with appointments and meetings**</span></span>

|<span data-ttu-id="2da56-110">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="2da56-110">**EWS Managed API method**</span></span>|<span data-ttu-id="2da56-111">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="2da56-111">**EWS operation**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2da56-112">Appointment.Save</span><span class="sxs-lookup"><span data-stu-id="2da56-112">Appointment.Save</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="2da56-113">CreateItem 操作 (予定表アイテム)</span><span class="sxs-lookup"><span data-stu-id="2da56-113">CreateItem operation (calendar item)</span></span>](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="2da56-114">Item.Bind</span><span class="sxs-lookup"><span data-stu-id="2da56-114">Item.Bind</span></span>](http://msdn.microsoft.com/ja-JP/library/dd634410%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="2da56-115">GetItem 操作 (予定表アイテム)</span><span class="sxs-lookup"><span data-stu-id="2da56-115">GetItem operation (calendar item)</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
   
## <a name="create-an-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="2da56-116">EWS マネージ API を使用して予定を作成する</span><span class="sxs-lookup"><span data-stu-id="2da56-116">Create an appointment by using the EWS Managed API</span></span>
<span data-ttu-id="2da56-117"><a name="bk_CreateApptEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="2da56-117"></span></span>

<span data-ttu-id="2da56-118">次のコード例では、[Appointment オブジェクト](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)を使用して予定を作成する方法、その予定を [Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) メソッドを使用して予定表フォルダーに保存する方法、および [Item.Bind](http://msdn.microsoft.com/ja-JP/library/dd634410%28v=exchg.80%29.aspx) メソッドを使用して予定が作成されたかどうかを確認する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="2da56-118">The following code example shows how to use the [Appointment objecthttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) to create an appointment, the [Savehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to save it to your calendar folder, and the [Item.Bindhttp://msdn.microsoft.com/en-us/library/dd634410(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/dd634410%28v=exchg.80%29.aspx) method to verify that the appointment was created.</span></span> 
  
<span data-ttu-id="2da56-119">この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。</span><span class="sxs-lookup"><span data-stu-id="2da56-119">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeServicehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
```cs
Appointment appointment = new Appointment(service);
// Set the properties on the appointment object to create the appointment.
appointment.Subject = "Tennis lesson";
appointment.Body = "Focus on backhand this week.";
appointment.Start = DateTime.Now.AddDays(2);
appointment.End = appointment.Start.AddHours(1);
appointment.Location = "Tennis club";
appointment.ReminderDueBy = DateTime.Now;
// Save the appointment to your calendar.
appointment.Save(SendInvitationsMode.SendToNone);
// Verify that the appointment was created by using the appointment's item ID.
Item item = Item.Bind(service, appointment.Id, new PropertySet(ItemSchema.Subject));
Console.WriteLine("\nAppointment created: " + item.Subject + "\n");

```

<span data-ttu-id="2da56-120">Appointment オブジェクトのプロパティを設定したら、Appointment オブジェクトの [Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) メソッドを使用して、予定を予定表フォルダーに保存します。</span><span class="sxs-lookup"><span data-stu-id="2da56-120">After setting the properties on the appointment object, you save the appointment to the calendar folder by using the appointment object's [Savehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx)  method.</span></span> 
  
<span data-ttu-id="2da56-121">確認手順において、予定に関連付けられているアイテムの [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) を使用して、予定が予定表フォルダーにあることを確認します。</span><span class="sxs-lookup"><span data-stu-id="2da56-121">Note that in the verification step, you use the item [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) associated with the appointment to verify that the appointment is in the calendar folder.</span></span> <span data-ttu-id="2da56-122">ベスト プラクティスとして、サーバーによって返されるプロパティを、必要なもの (この場合は予定の件名) だけに制限します。</span><span class="sxs-lookup"><span data-stu-id="2da56-122">As a best practice, limit the properties returned by the server to only what you need — in this case, the appointment's subject.</span></span> 
  
## <a name="create-an-appointment-by-using-ews"></a><span data-ttu-id="2da56-123">EWS を使用して予定を作成する</span><span class="sxs-lookup"><span data-stu-id="2da56-123">Create an appointment by using EWS</span></span>
<span data-ttu-id="2da56-124"><a name="bk_CreateApptEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="2da56-124"></span></span>

<span data-ttu-id="2da56-125">次の例の要求と応答の XML は、「[EWS マネージ API を使用して予定を作成する](#bk_CreateApptEWSMA)」の EWS マネージ API コードの呼び出しに対応します。</span><span class="sxs-lookup"><span data-stu-id="2da56-125">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Update an appointment by using the EWS Managed API](#bk_CreateApptEWSMA).</span></span> <span data-ttu-id="2da56-126">予定アイテムが予定表フォルダー内にあることを確認する要求と応答の XML も同様に示されています。</span><span class="sxs-lookup"><span data-stu-id="2da56-126">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in Create an appointment using the EWS Managed API. The request and response XML that verifies that the appointment items are in the calendar folder are shown as well.</span></span>
  
<span data-ttu-id="2da56-127">次の例は、[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) 操作を使用して、予定を作成する場合の要求 XML を表しています。</span><span class="sxs-lookup"><span data-stu-id="2da56-127">The following example shows the request XML when you use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create an appointment.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Tennis lesson</t:Subject>
          <t:Body BodyType="HTML">Focus on backhand this week.</t:Body>
          <t:ReminderDueBy>2013-09-19T14:37:10.732-07:00</t:ReminderDueBy>
          <t:Start>2013-09-21T19:00:00.000Z</t:Start>
          <t:End>2013-09-21T20:00:00.000Z</t:End>
          <t:Location>Tennis club</t:Location>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

 <span data-ttu-id="2da56-128">次の例は、**CreateItem** 操作で返される応答 XML を表しています。</span><span class="sxs-lookup"><span data-stu-id="2da56-128">The following example shows the response XML that is returned by the **CreateItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2da56-129">**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="2da56-129">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
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

<span data-ttu-id="2da56-130">次の例は、[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) 操作を使用して予定が作成されたかどうかを確認するときに生成される要求の XML を示しています。</span><span class="sxs-lookup"><span data-stu-id="2da56-130">The following example shows the request XML that is generated when you use the [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) operation to verify that the appointment was created.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2da56-131">**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="2da56-131">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>

```

 <span data-ttu-id="2da56-132">次の例は、**GetItem** 操作で返される応答 XML を表しています。</span><span class="sxs-lookup"><span data-stu-id="2da56-132">The following example shows the response XML that is returned by the **GetItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2da56-133">**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="2da56-133">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
              <t:Subject>Tennis lesson</t:Subject>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="create-a-meeting-by-using-the-ews-managed-api"></a><span data-ttu-id="2da56-134">EWS マネージ API を使用して会議を作成する</span><span class="sxs-lookup"><span data-stu-id="2da56-134">Create a meeting by using the EWS Managed API</span></span>
<span data-ttu-id="2da56-135"><a name="bk_CreateMtgEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="2da56-135"></span></span>

<span data-ttu-id="2da56-p104">予定表フォルダーにアイテムを保存して、さらに会議の作成を行う場合は、通常、出席者に会議出席依頼を送信することも必要になります。次のコード例は、会議を作成して出席依頼を送信する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2da56-p104">When you create a meeting, in addition to saving an item to the calendar folder, you also typically want to send meeting requests to attendees. The following code example shows how to create a meeting and send meeting requests.</span></span>
  
<span data-ttu-id="2da56-138">この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。</span><span class="sxs-lookup"><span data-stu-id="2da56-138">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeServicehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
```cs
Appointment meeting = new Appointment(service);
// Set the properties on the meeting object to create the meeting.
meeting.Subject = "Team building exercise";
meeting.Body = "Let's learn to really work as a team and then have lunch!";
meeting.Start = DateTime.Now.AddDays(2);            
meeting.End = meeting.Start.AddHours(4);
meeting.Location = "Conference Room 12";
meeting.RequiredAttendees.Add("Mack@contoso.com");
meeting.RequiredAttendees.Add("Sadie@contoso.com");
meeting.OptionalAttendees.Add("Magdalena@contoso.com");
meeting.ReminderMinutesBeforeStart = 60;
// Save the meeting to the Calendar folder and send the meeting request.
meeting.Save(SendInvitationsMode.SendToAllAndSaveCopy);
// Verify that the meeting was created.
Item item = Item.Bind(service, meeting.Id, new PropertySet(ItemSchema.Subject));
Console.WriteLine("\nMeeting created: " + item.Subject + "\n");

```

<span data-ttu-id="2da56-139">[Appointment](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクトのプロパティを設定したら、[Save](http://msdn.microsoft.com/ja-JP/library/dd635394%28v=exchg.80%29.aspx) メソッドを使用して、予定表フォルダーに会議を保存します。</span><span class="sxs-lookup"><span data-stu-id="2da56-139">After setting the properties on the [Appointment](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object, save the meeting to your calendar folder by using the [Save](http://msdn.microsoft.com/ja-JP/library/dd635394%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="2da56-140">[SendInvitationsMode](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.sendinvitationsmode%28v=exchg.80%29.aspx) 列挙の値を **SendOnlyToAll** または **SendToAllAndSaveCopy** に設定すると、出席者に招待状が送信されます。</span><span class="sxs-lookup"><span data-stu-id="2da56-140">When you set the [SendInvitationsMode](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.sendinvitationsmode%28v=exchg.80%29.aspx) enumeration value to **SendOnlyToAll** or **SendToAllAndSaveCopy**, invitations are sent to attendees.</span></span>
  
<span data-ttu-id="2da56-141">会議に関連付けられたアイテムの [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) を使用して、会議が予定表フォルダーに保存されたことを確認します。</span><span class="sxs-lookup"><span data-stu-id="2da56-141">Use the item [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) associated with the meeting to verify that it was saved in the calendar folder.</span></span> <span data-ttu-id="2da56-142">ベスト プラクティスとして、サーバーによって返されるプロパティを、必要なもの (この場合は会議の件名) だけに制限します。</span><span class="sxs-lookup"><span data-stu-id="2da56-142">As a best practice, limit the properties returned by the server to only what you need - in this case, the meeting's subject.</span></span> 
  
## <a name="create-a-meeting-by-using-ews"></a><span data-ttu-id="2da56-143">EWS を使用して会議を作成する</span><span class="sxs-lookup"><span data-stu-id="2da56-143">Create a meeting by using EWS</span></span>
<span data-ttu-id="2da56-144"><a name="bk_CreateMtgEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="2da56-144"></span></span>

<span data-ttu-id="2da56-145">次の例の要求と応答の XML は、「[EWS マネージ API を使用して会議を作成する](#bk_CreateMtgEWSMA)」の EWS マネージ API コードの呼び出しに対応します。</span><span class="sxs-lookup"><span data-stu-id="2da56-145">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Update a meeting using the EWS Managed API](#bk_CreateMtgEWSMA).</span></span> <span data-ttu-id="2da56-146">会議アイテムが予定表フォルダー内にあることを確認する要求と応答の XML も同様に示されています。</span><span class="sxs-lookup"><span data-stu-id="2da56-146">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in Create a meeting using the EWS Managed API. The request and response XML that verifies that the meeting items are in the calendar folder are shown as well.</span></span>
  
<span data-ttu-id="2da56-147">次の例は、[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) 操作を使用して、会議を更新する場合の要求 XML を表しています。</span><span class="sxs-lookup"><span data-stu-id="2da56-147">The following example shows the request XML when you use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a meeting.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToAllAndSaveCopy">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Team building exercise</t:Subject>
          <t:Body BodyType="HTML">Let's learn to really work as a team and then have lunch!</t:Body>
          <t:ReminderMinutesBeforeStart>60</t:ReminderMinutesBeforeStart>
          <t:Start>2013-09-21T16:00:00.000Z</t:Start>
          <t:End>2013-09-21T20:00:00.000Z</t:End>
          <t:Location>Conference Room 12</t:Location>
          <t:RequiredAttendees>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Mack.Chaves@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Sadie.Daniels@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
          </t:RequiredAttendees>
          <t:OptionalAttendees>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Magdalena.Kemp@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
          </t:OptionalAttendees>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2da56-148">次の例は、**CreateItem** 操作で返される応答 XML を表しています。</span><span class="sxs-lookup"><span data-stu-id="2da56-148">The following example shows the response XML that is returned by the **CreateItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2da56-149">**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="2da56-149">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
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

<span data-ttu-id="2da56-150">次の例は、予定が作成されたかどうかを確認するときに、[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) 操作によって生成される要求の XML を示しています。</span><span class="sxs-lookup"><span data-stu-id="2da56-150">The following example shows the request XML that is generated by the [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) operation when you verify that the meeting was created.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2da56-151">**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="2da56-151">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2da56-152">次の例は、**GetItem** 操作で返される応答 XML を表しています。</span><span class="sxs-lookup"><span data-stu-id="2da56-152">The following example shows the response XML that is returned by the **GetItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2da56-153">**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="2da56-153">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
              <t:Subject>Team building exercise</t:Subject>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="2da56-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="2da56-154">See also</span></span>

- [<span data-ttu-id="2da56-155">Exchange の予定表と EWS</span><span class="sxs-lookup"><span data-stu-id="2da56-155">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)  
- [<span data-ttu-id="2da56-156">Exchange の EWS を使用して予定と会議を取得する</span><span class="sxs-lookup"><span data-stu-id="2da56-156">How to: Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)  
- [<span data-ttu-id="2da56-157">Exchange で EWS を使用して予定と会議を更新する</span><span class="sxs-lookup"><span data-stu-id="2da56-157">How to: Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="2da56-158">Exchange の EWS を使用して、予定を削除し、会議をキャンセルする</span><span class="sxs-lookup"><span data-stu-id="2da56-158">How to: Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="2da56-159">Exchange で EWS を使用して会議の新しい日時を提案する</span><span class="sxs-lookup"><span data-stu-id="2da56-159">How to: Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    


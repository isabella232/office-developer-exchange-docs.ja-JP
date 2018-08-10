---
title: Exchange で EWS を使用して予定と会議を更新する
manager: sethgros
ms.date: 12/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 13256625-083e-4a17-8fd1-2bed1f7cc14e
description: EWS マネージ API または Exchange で EWS を使用して、予定と会議を更新する方法を説明します。
ms.openlocfilehash: a4265a14a46c146c584a3daa61cef5486958e14e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759061"
---
# <a name="update-appointments-and-meetings-by-using-ews-in-exchange"></a><span data-ttu-id="9e563-103">Exchange で EWS を使用して予定と会議を更新する</span><span class="sxs-lookup"><span data-stu-id="9e563-103">How to: Update appointments and meetings by using EWS in Exchange</span></span>

<span data-ttu-id="9e563-104">EWS マネージ API または Exchange で EWS を使用して、予定と会議を更新する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="9e563-104">Learn how to update appointments and meetings by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="9e563-105">会議と予定の根本的な違いは、会議には出席者がいますが、予定にはいません。</span><span class="sxs-lookup"><span data-stu-id="9e563-105">The essential difference between meetings and appointments is that meetings have attendees, and appointments don't.</span></span> <span data-ttu-id="9e563-106">予定も会議も、単一のインスタンスまたは定期的に連続で発生するアイテムの一部ですが、予定は出席者、会議室、またはリソースを含まないため、メッセージの送信を必要としません。</span><span class="sxs-lookup"><span data-stu-id="9e563-106">Both appointments and meetings can be single instances or part of a recurring series, but because appointments don't include attendees, rooms, or resources, they do not require a message to be sent.</span></span> <span data-ttu-id="9e563-107">内部的には、Exchange は会議と予定の両方に同じオブジェクトを使用します。</span><span class="sxs-lookup"><span data-stu-id="9e563-107">Internally, Exchange uses the same object for both meetings and appointments.</span></span> <span data-ttu-id="9e563-108">EWS マネージ API [Appointment クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)または EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) 要素を使用して、会議や予定を操作します。</span><span class="sxs-lookup"><span data-stu-id="9e563-108">You use the EWS Managed API [Appointment class](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) or the EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) element to work with meetings and appointments.</span></span> 
  
<span data-ttu-id="9e563-109">**表 1. 予定や会議を更新するための EWS マネージ API メソッドおよび EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="9e563-109">**Table 1.  EWS Managed API method and EWS operations for updating appointments and meetings**</span></span>

|<span data-ttu-id="9e563-110">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="9e563-110">**EWS Managed API method**</span></span>|<span data-ttu-id="9e563-111">**EWS 操作に対応**</span><span class="sxs-lookup"><span data-stu-id="9e563-111">**Corresponding EWS operations**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e563-112">Appointment.Update</span><span class="sxs-lookup"><span data-stu-id="9e563-112">Appointment.Update</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="9e563-113">UpdateItem </span><span class="sxs-lookup"><span data-stu-id="9e563-113">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)<br/><br/>          [<span data-ttu-id="9e563-114">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="9e563-114">UpdateItemResponse</span></span>](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) <br/> |
   
## <a name="update-an-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="9e563-115">EWS マネージ API を使用して予定を更新する</span><span class="sxs-lookup"><span data-stu-id="9e563-115">Update an appointment by using the EWS Managed API</span></span>
<span data-ttu-id="9e563-116"><a name="bk_UpdateApptEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="9e563-116"></span></span>

<span data-ttu-id="9e563-117">次のコード例は、[Appointment オブジェクト](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)を使用して、予定に関連付けられているプロパティを更新する方法、および [Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) メソッドを使用して予定を予定表フォルダーに保存する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="9e563-117">The following code example shows how to use the [Appointment objecthttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) to update properties associated with an appointment and the [Updatehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) method to save the appointment to your calendar folder.</span></span> 
  
<span data-ttu-id="9e563-118">この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。</span><span class="sxs-lookup"><span data-stu-id="9e563-118">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeServicehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="9e563-119">ローカル変数 `appointmentId` は、既存の予定に関連付けられた識別子です。</span><span class="sxs-lookup"><span data-stu-id="9e563-119">The local variable  `appointmentId` is an identifier associated with an existing appointment.</span></span> 
  
```cs
// Instantiate an appointment object by binding to it by using the ItemId.
// As a best practice, limit the properties returned to only the ones you need.
Appointment appointment = Appointment.Bind(service, appointmentId, new PropertySet(AppointmentSchema.Subject, AppointmentSchema.Start, AppointmentSchema.End));
string oldSubject = appointment.Subject;
// Update properties on the appointment with a new subject, start time, and end time.
appointment.Subject = appointment.Subject + " moved one hour later and to the day after " + appointment.Start.DayOfWeek + "!";
appointment.Start.AddHours(25);
appointment.End.AddHours(25);
// Unless explicitly specified, the default is to use SendToAllAndSaveCopy.
// This can convert an appointment into a meeting. To avoid this,
// explicitly set SendToNone on non-meetings.
SendInvitationsOrCancellationsMode mode = appointment.IsMeeting ? 
    SendInvitationsOrCancellationsMode.SendToAllAndSaveCopy : SendInvitationsOrCancellationsMode.SendToNone;
// Send the update request to the Exchange server.
appointment.Update(ConflictResolutionMode.AlwaysOverwrite, mode);
// Verify the update.
Console.WriteLine("Subject for the appointment was \"" + oldSubject + "\". The new subject is \"" + appointment.Subject + "\"");

```

## <a name="update-an-appointment-by-using-ews"></a><span data-ttu-id="9e563-120">EWS を使用して予定を更新する</span><span class="sxs-lookup"><span data-stu-id="9e563-120">Update an appointment by using EWS</span></span>
<span data-ttu-id="9e563-121"><a name="bk_UpdateApptEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="9e563-121"></span></span>

<span data-ttu-id="9e563-122">次の例の要求と応答 XML は、「[EWS マネージ API を使用して予定を更新する](#bk_UpdateApptEWSMA)」の EWS マネージ API コードの呼び出しに対応します。</span><span class="sxs-lookup"><span data-stu-id="9e563-122">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Update an appointment by using the EWS Managed API](#bk_UpdateApptEWSMA).</span></span>
  
<span data-ttu-id="9e563-123">次の例は、[UpdateItem](http://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) 操作を利用して、予定を更新するときの、要求 XML を示しています。</span><span class="sxs-lookup"><span data-stu-id="9e563-123">The following example shows the request XML when you use the [UpdateItem](http://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) operation to update an appointment.</span></span> 
  
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
    <m:UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AlwaysOverwrite" SendMeetingInvitationsOrCancellations="SendToNone">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAAB" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Tennis Lesson moved one hour later and to the day after Wednesday!</t:Subject>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="9e563-124">次の例は、[UpdateItem](http://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) 要求への応答として返された XML を示しています。</span><span class="sxs-lookup"><span data-stu-id="9e563-124">The following example shows the XML that is returned in response to an [UpdateItem](http://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) request. The ChangeKey and ItemId attributes have been shortened for readability.</span></span> <span data-ttu-id="9e563-125">**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="9e563-125">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="815" MinorBuildNumber="6" Version="V2_7" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UpdateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exc
hange/services/2006/types">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAAB" />
            </t:CalendarItem>
          </m:Items>
          <m:ConflictResults>
            <t:Count>0</t:Count>
          </m:ConflictResults>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </m:UpdateItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="update-a-meeting-by-using-the-ews-managed-api"></a><span data-ttu-id="9e563-126">EWS マネージ API を使用して会議を更新する</span><span class="sxs-lookup"><span data-stu-id="9e563-126">Update a meeting by using the EWS Managed API</span></span>
<span data-ttu-id="9e563-127"><a name="bk_UpdateMtgEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="9e563-127"></span></span>

<span data-ttu-id="9e563-p104">予定表フォルダーに変更した予定アイテムを保存することに加えて、さらに会議を更新する場合、出席者に更新した会議への出席依頼を送信することもできます。次のコード例は、会議を更新して出席依頼を送信する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="9e563-p104">When you update a meeting, in addition to saving the modified appointment item to the calendar folder, you also typically want to send updated meeting requests to attendees. The following code example shows how to update a meeting and send meeting requests.</span></span>
  
<span data-ttu-id="9e563-130">この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。</span><span class="sxs-lookup"><span data-stu-id="9e563-130">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeServicehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="9e563-131">ローカル変数 `meetingId` は、既存の予定に関連付けられた識別子です。</span><span class="sxs-lookup"><span data-stu-id="9e563-131">The local variable  `meetingId` is an identifier that is associated with an existing appointment.</span></span> 
  
```cs
// Instantiate an appointment object by binding to it using the ItemId.
// As a best practice, limit the properties returned to only the Appointment ID.
Appointment meeting = Appointment.Bind(service, meetingId, new PropertySet(AppointmentSchema.Subject, 
                                                                           AppointmentSchema.Location, 
                                                                           AppointmentSchema.RequiredAttendees, 
                                                                           AppointmentSchema.Resources));
string oldSubject = meeting.Subject;
// Update properties on the appointment with a new subject, location, an additional required attendee, and a resource.
meeting.Subject = "Team building exercise has moved!";
meeting.Location = "4567 Contoso Way, Redmond, OH 33333, USA";
meeting.RequiredAttendees.Add("alisa@contoso.com");
meeting.Resources.Add("dlpprojector@contoso.com");
// Send the update request to the Exchange server.
meeting.Update(ConflictResolutionMode.AlwaysOverwrite, SendInvitationsOrCancellationsMode.SendToAllAndSaveCopy);
// Verify the update.
Console.WriteLine("Subject for the meeting was \"" + oldSubject + "\". The new subject is \"" + meeting.Subject + "\"");

```

<span data-ttu-id="9e563-132">[Appointment](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクトのプロパティを設定した後、[Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) メソッドを使用して、会議を予定表フォルダーに保存し、更新された会議への出席依頼を送信します。</span><span class="sxs-lookup"><span data-stu-id="9e563-132">After setting the properties on the [Appointmenthttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)  object, save the meeting to your calendar folder and send updated meeting requests by using the [Updatehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="9e563-133">[Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) メソッドを呼び出すときに、2 つの列挙値のいずれかをパラメーターとして渡すことができます。</span><span class="sxs-lookup"><span data-stu-id="9e563-133">You can pass in one of two enumeration values as parameters when you call the [Updatehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) method:</span></span> 
  
- <span data-ttu-id="9e563-134">[ConflictResolutionMode 列挙体 ](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.conflictresolutionmode%28v=exchg.80%29.aspx) — クライアントとサーバーとの間の競合状態を処理する方法を決定します。</span><span class="sxs-lookup"><span data-stu-id="9e563-134">[ConflictResolutionMode enumerationhttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.conflictresolutionmode(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.conflictresolutionmode%28v=exchg.80%29.aspx) — Determines how conflicting states between client and server are handled.</span></span> 
    
- <span data-ttu-id="9e563-135">[SendInvitationsOrCancellationsMode 列挙体 ](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.sendinvitationsorcancellationsmode%28v=exchg.80%29.aspx) — 会議更新依頼の送信および保存に影響を及ぼします。</span><span class="sxs-lookup"><span data-stu-id="9e563-135">[SendInvitationsOrCancellationsMode enumerationhttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.sendinvitationsorcancellationsmode(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.sendinvitationsorcancellationsmode%28v=exchg.80%29.aspx) — Affects the sending and saving of meeting update requests.</span></span> 
    
<span data-ttu-id="9e563-136">[ConflictResolutionMode](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.conflictresolutionmode%28v=exchg.80%29.aspx) 列挙値を **AlwaysOverwrite** に設定すると、お使いのバージョンの会議は常に予定表フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="9e563-136">When you set the [ConflictResolutionModehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.conflictresolutionmode(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.conflictresolutionmode%28v=exchg.80%29.aspx) enumeration value to **AlwaysOverwrite**, your version of the meeting will always be saved to the calendar folder.</span></span>
  
## <a name="update-a-meeting-by-using-ews"></a><span data-ttu-id="9e563-137">EWS を使用して会議を更新する</span><span class="sxs-lookup"><span data-stu-id="9e563-137">Update a meeting by using EWS</span></span>
<span data-ttu-id="9e563-138"><a name="bk_UpdateMtgEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="9e563-138"></span></span>

<span data-ttu-id="9e563-139">次の例の要求と応答 XML は、「[EWS マネージ API を使用して会議を更新する](#bk_UpdateMtgEWSMA)」の EWS マネージ API コードの呼び出しに対応します。</span><span class="sxs-lookup"><span data-stu-id="9e563-139">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Update a meeting using the EWS Managed API](#bk_UpdateMtgEWSMA).</span></span> 
  
<span data-ttu-id="9e563-140">次の例は、[UpdateItem](http://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) 操作を利用して、会議を更新するときの、要求 XML を示しています。</span><span class="sxs-lookup"><span data-stu-id="9e563-140">The following example shows the request XML when you use the [UpdateItem](http://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) operation to update a meeting.</span></span> 
  
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
    <m:UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AlwaysOverwrite" SendMeetingInvitationsOrCancellations="SendToAllAndSaveCopy">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Team building exercise has moved!</t:Subject>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Location" />
              <t:CalendarItem>
                <t:Location>4567 Contoso Way, Redmond, OH 33333, USA</t:Location>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:RequiredAttendees" />
              <t:CalendarItem>
                <t:RequiredAttendees>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Mack.Chaves@contoso.com</t:Name>
                      <t:EmailAddress>Mack.Chaves@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Sadie.Daniels@contoso.com</t:Name>
                      <t:EmailAddress>Sadie.Daniels@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:EmailAddress>alisa@contoso.com</t:EmailAddress>
                    </t:Mailbox>
                  </t:Attendee>
                </t:RequiredAttendees>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Resources" />
              <t:CalendarItem>
                <t:Resources>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:EmailAddress>dlpprojector@contoso.com</t:EmailAddress>
                    </t:Mailbox>
                  </t:Attendee>
                </t:Resources>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

 <span data-ttu-id="9e563-141">次の例は、[UpdateItem](http://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) 要求への応答として返された XML を示しています。</span><span class="sxs-lookup"><span data-stu-id="9e563-141">The following example shows the XML that is returned in response to an [UpdateItem](http://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) request. The ChangeKey and ItemId attributes have been shortened for readability.</span></span> <span data-ttu-id="9e563-142">**ChangeKey** 属性と **ItemId** 属性は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="9e563-142">The **ItemId** and ChangeKey attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="815" MinorBuildNumber="6" Version="V2_7" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UpdateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
          <m:ConflictResults>
            <t:Count>0</t:Count>
          </m:ConflictResults>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </m:UpdateItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="9e563-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="9e563-143">See also</span></span>

- [<span data-ttu-id="9e563-144">Exchange の予定表と EWS</span><span class="sxs-lookup"><span data-stu-id="9e563-144">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)   
- [<span data-ttu-id="9e563-145">Exchange 2013 の EWS を使用して予定と会議を作成する</span><span class="sxs-lookup"><span data-stu-id="9e563-145">How to: Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)   
- [<span data-ttu-id="9e563-146">Exchange の EWS を使用して予定と会議を取得する</span><span class="sxs-lookup"><span data-stu-id="9e563-146">How to: Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)  
- [<span data-ttu-id="9e563-147">Exchange の EWS を使用して、予定を削除し、会議をキャンセルする</span><span class="sxs-lookup"><span data-stu-id="9e563-147">How to: Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)  
- [<span data-ttu-id="9e563-148">Exchange で EWS を使用して会議の新しい日時を提案する</span><span class="sxs-lookup"><span data-stu-id="9e563-148">How to: Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    


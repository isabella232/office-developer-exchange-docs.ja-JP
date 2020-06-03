---
title: Exchange で EWS を使用して終日イベントを作成する
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 0fcb484b-4ffc-41a5-aeed-8c797766b70c
description: Exchange で EWS マネージ API または EWS を使用して、終日イベントを作成する方法について説明します。
ms.openlocfilehash: 6be638c17cc0e0c86fa6b4217169aa7259dfd4aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456865"
---
# <a name="create-all-day-events-by-using-ews-in-exchange"></a><span data-ttu-id="bf46a-103">Exchange で EWS を使用して終日イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="bf46a-103">Create all-day events by using EWS in Exchange</span></span>

<span data-ttu-id="bf46a-104">Exchange で EWS マネージ API または EWS を使用して、終日イベントを作成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="bf46a-104">Learn how to create all-day events by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="bf46a-p101">終日イベントは、休日や休暇など、1 日または複数の日で発生する事項を表す方法を提供します。EWS マネージ API または EWS を使用した終日イベントの作成は、簡単な作業です。[予定の作成](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)と似ていますが、少しだけ違いがあります。</span><span class="sxs-lookup"><span data-stu-id="bf46a-p101">All-day events provide a way to represent something that happens for an entire day or multiple days—for example, a holiday, or vacation days. Creating all-day events with the EWS Managed API or EWS is a snap. It's just like [creating appointments](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), but with a few small changes.</span></span>
  
## <a name="setting-start-and-end-times"></a><span data-ttu-id="bf46a-108">開始時間と終了時間の設定</span><span class="sxs-lookup"><span data-stu-id="bf46a-108">Setting start and end times</span></span>

<span data-ttu-id="bf46a-p102">定義では、終日イベントは特定の午前 0 時に開始され、24 時間 (または24 時間の倍数) 後に終了します。ただし、EWS マネージ APIと EWS では、終日イベントを作成するときに、午前 0 時以外の時刻を指定できます。これにより、サーバーでのこれらの時間変換の方法を認識していないと、予期しない動作が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="bf46a-p102">By definition, all-day events start at midnight on a specific day, and end 24 hours (or a multiple of 24 hours) later. However, the EWS Managed API and EWS allow you to specify times other than midnight when creating all day events. This can lead to unintended behavior if you're not aware of how these times get translated on the server.</span></span>
  
<span data-ttu-id="bf46a-112">([要求または予定のタイム ゾーン](time-zones-and-ews-in-exchange.md)の) 午前 0 時以外の開始時間または終了時間を持つ終日イベントを新しく作成する通知を受信すると、これらの時間は次の規則に従い、適切なタイム ゾーンの午前 0 時に調整されます。</span><span class="sxs-lookup"><span data-stu-id="bf46a-112">When a request is received to create a new all-day event with non-midnight (in the [time zone of the request or appointment](time-zones-and-ews-in-exchange.md)) start and/or end times, those times get adjusted to midnight in the appropriate time zone according to the following rules:</span></span>
  
- <span data-ttu-id="bf46a-p103">午前 0 時以外の開始時間は、指定した時刻より前の午前 0 時に調整されます。たとえば、6 月 6 日の午後 1 時は、6 月 6 日の午前 0 時に調整されます。</span><span class="sxs-lookup"><span data-stu-id="bf46a-p103">Non-midnight start times are adjusted to the midnight prior to the time specified. For example, 1:00 PM on June 6 gets adjusted to 12:00 AM on June 6.</span></span>
    
- <span data-ttu-id="bf46a-p104">午前 0 時以外の終了時間は、指定した時刻より後の午前 0 時に調整されます。たとえば、6 月 6 日の午後 1 時は、6 月 7 日の午前 0 時に調整されます。</span><span class="sxs-lookup"><span data-stu-id="bf46a-p104">Non-midnight end times are adjusted to the midnight after the time specified. For example, 1:00 PM on June 6 gets adjusted to 12:00 AM on June 7.</span></span>
    
<span data-ttu-id="bf46a-p105">このため、作成する終日イベントは、常に指定した開始時刻と終了時刻を含みますが、午前 0 時への移動により、ユーザーの予定表に追加の時間を要求することがあります。サーバーは、開始時刻と終了時刻を午前 0 時に調整するため、意図しない時間の変更を避けるために、開始時刻と終了時刻を午前 0 時に指定することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="bf46a-p105">So the all-day event that you create is always inclusive of the start and end time that you specify, but might claim additional time on the user's calendar due to the shift to midnight. Because the server will adjust the start and end time to midnight, we recommend that you specify your start and end time at midnight to avoid any unintended changes to the times.</span></span>
  
<span data-ttu-id="bf46a-p106">終日イベントを作成するときのタイム ゾーンを考慮することも重要です。Exchange サーバーにより、要求または予約のタイム ゾーンで午前 0 時の開始時刻と終了時刻が適用されるため、別のタイム ゾーンに構成されたクライアントで終日イベントを表示すると、予期しない結果になる可能性があります。クライアントによっては、終日イベントの一部として意図していない余分な日が終日イベントとして表示されたり、終日イベントとして表示されないことがあります。このため、終日イベントを作成するとき、可能な場合は常にユーザーが優先するタイム ゾーンを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="bf46a-p106">It's also important to consider time zones when creating all-day events. Because the Exchange server enforces a midnight start and end time in the time zone of the request or appointment, viewing that all-day event in a client configured for a different time zone can yield unexpected results. Depending on the client, it might appear as an all-day event with extra days that you did not intend to include, or it might not appear as an all-day event altogether. Because of this, we recommend that you use the user's preferred time zone whenever possible when you create all-day events.</span></span>
  
## <a name="create-an-all-day-event-by-using-the-ews-managed-api"></a><span data-ttu-id="bf46a-123">EWS マネージ API を使用して終日イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="bf46a-123">Create an all-day event by using the EWS Managed API</span></span>

<span data-ttu-id="bf46a-124">次の例は、EWS マネージ API を使用して、_startDate_ パラメーターによって指定される日付から始まり、_numDays_ パラメーターによって指定される日数続く終日イベントを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="bf46a-124">The following example shows how to use the EWS Managed API to create an all-day event, starting on the date specified by the  _startDate_ parameter and lasting for the number of days specified by the  _numDays_ parameter.</span></span> <span data-ttu-id="bf46a-125">予定は [ExchangeService.TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) プロパティによって指定されるタイム ゾーンで作成されます。</span><span class="sxs-lookup"><span data-stu-id="bf46a-125">Note that the appointment will be created in the time zone specified by the [ExchangeService.TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) property.</span></span> <span data-ttu-id="bf46a-126">この例では、_service_ パラメーターで渡される [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトが、[Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) プロパティと [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) プロパティの有効な値で初期化されているものとします。</span><span class="sxs-lookup"><span data-stu-id="bf46a-126">This example assumes that the [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object passed in the  _service_ parameter has been initialized with valid values for the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
static void CreateAllDayAppointment(ExchangeService service, DateTime startDate, int numDays)
{
    // Best practice is to set the start date to midnight
    // on the first day of the all-day event.
    DateTime startDateMidnight = startDate.Date;
    // The end date should be midnight on the first day
    // after the event.
    DateTime endDateMidnight = startDateMidnight.AddDays(numDays);
    Appointment allDayEvent = new Appointment(service);
    // Set IsAllDayEvent to true.
    allDayEvent.IsAllDayEvent = true;
    // Set other properties.
    allDayEvent.Subject = "Vacation";
    allDayEvent.LegacyFreeBusyStatus = LegacyFreeBusyStatus.OOF;
    allDayEvent.Start = startDateMidnight;
    allDayEvent.End = endDateMidnight;
    // Save the appointment.
    try
    {
        allDayEvent.Save(WellKnownFolderName.Calendar, SendInvitationsMode.SendToNone);
        Console.WriteLine("All day event created.");
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error saving all day event: {0}", ex.Message);
    }
}
```

## <a name="create-an-all-day-event-by-using-ews"></a><span data-ttu-id="bf46a-127">EWS を使用して終日イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="bf46a-127">Create an all-day event by using EWS</span></span>

<span data-ttu-id="bf46a-128">次の例では、終日イベントを作成する EWS [CreateItem 操作](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)要求を示します。</span><span class="sxs-lookup"><span data-stu-id="bf46a-128">The following example shows an EWS [CreateItem operation](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request to create an all-day event.</span></span> <span data-ttu-id="bf46a-129">予定は、[TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) 要素で示すように、米国東部標準時ゾーンで作成されます。</span><span class="sxs-lookup"><span data-stu-id="bf46a-129">The appointment is created in the Eastern time zone, as indicated by the [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="bf46a-130">なお、[Start](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) 要素と [End](https://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) 要素の値の時間部分は両方とも 04:00Z であり、これは夏時間中の米国東部標準時ゾーンの午前 0 時に変換されます。</span><span class="sxs-lookup"><span data-stu-id="bf46a-130">Notice that the time portion of the values of the [Start](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) and [End](https://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) elements are both 04:00Z, which converts to midnight in the Eastern time zone during daylight saving time.</span></span> 
  
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
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Vacation</t:Subject>
          <t:Start>2014-06-09T04:00:00.000Z</t:Start>
          <t:End>2014-06-10T04:00:00.000Z</t:End>
          <t:IsAllDayEvent>true</t:IsAllDayEvent>
          <t:LegacyFreeBusyStatus>OOF</t:LegacyFreeBusyStatus>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="bf46a-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="bf46a-131">See also</span></span>


- [<span data-ttu-id="bf46a-132">Exchange の予定表と EWS</span><span class="sxs-lookup"><span data-stu-id="bf46a-132">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="bf46a-133">Exchange 2013 の EWS を使用して予定と会議を作成する</span><span class="sxs-lookup"><span data-stu-id="bf46a-133">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="bf46a-134">Exchange のタイム ゾーンと EWS</span><span class="sxs-lookup"><span data-stu-id="bf46a-134">Time zones and EWS in Exchange</span></span>](time-zones-and-ews-in-exchange.md)
    


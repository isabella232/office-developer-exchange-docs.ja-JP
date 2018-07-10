---
title: EWS を使用して Exchange、終日のイベントを作成します。
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 0fcb484b-4ffc-41a5-aeed-8c797766b70c
description: Exchange で EWS マネージ API または EWS を使用して、終日イベントを作成する方法について説明します。
ms.openlocfilehash: 0547fdf0ca92ba0648caeb5de6940d90d2a8ff46
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758931"
---
# <a name="create-all-day-events-by-using-ews-in-exchange"></a><span data-ttu-id="4206b-103">EWS を使用して Exchange、終日のイベントを作成します。</span><span class="sxs-lookup"><span data-stu-id="4206b-103">Create all-day events by using EWS in Exchange</span></span>

<span data-ttu-id="4206b-104">Exchange で EWS マネージ API または EWS を使用して、終日イベントを作成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="4206b-104">Learn how to create all-day events by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="4206b-105">終日のイベントが 1 日または複数の日で発生した何かを表す方法を提供するなど、休日や休暇などのです。</span><span class="sxs-lookup"><span data-stu-id="4206b-105">All-day events provide a way to represent something that happens for an entire day or multiple days—for example, a holiday, or vacation days.</span></span> <span data-ttu-id="4206b-106">スナップは、EWS のマネージ API または EWS に終日のイベントを作成します。</span><span class="sxs-lookup"><span data-stu-id="4206b-106">Creating all-day events with the EWS Managed API or EWS is a snap.</span></span> <span data-ttu-id="4206b-107">[予定を作成する](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)と同じようには、いくつかの小さな変更をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="4206b-107">It's just like [creating appointments](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), but with a few small changes.</span></span>
  
## <a name="setting-start-and-end-times"></a><span data-ttu-id="4206b-108">開始時間と終了時間の設定</span><span class="sxs-lookup"><span data-stu-id="4206b-108">Setting start and end times</span></span>

<span data-ttu-id="4206b-p102">定義では、終日イベントは特定の午前 0 時に開始され、24 時間 (または24 時間の倍数) 後に終了します。ただし、EWS マネージ APIと EWS では、終日イベントを作成するときに、午前 0 時以外の時刻を指定できます。これにより、サーバーでのこれらの時間変換の方法を認識していないと、予期しない動作が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="4206b-p102">By definition, all-day events start at midnight on a specific day, and end 24 hours (or a multiple of 24 hours) later. However, the EWS Managed API and EWS allow you to specify times other than midnight when creating all day events. This can lead to unintended behavior if you're not aware of how these times get translated on the server.</span></span>
  
<span data-ttu-id="4206b-112">以外の午前 0 時 ([依頼または予定のタイム ゾーン](time-zones-and-ews-in-exchange.md)) で開始または終了時刻と新しい終日イベントを作成する要求が受信されると、これらの時間を取得、次の規則に従って、適切なタイム ゾーンの午前 0 時に調整します。</span><span class="sxs-lookup"><span data-stu-id="4206b-112">When a request is received to create a new all-day event with non-midnight (in the [time zone of the request or appointment](time-zones-and-ews-in-exchange.md)) start and/or end times, those times get adjusted to midnight in the appropriate time zone according to the following rules:</span></span>
  
- <span data-ttu-id="4206b-p103">午前 0 時以外の開始時間は、指定した時刻より前の午前 0 時に調整されます。たとえば、6 月 6 日の午後 1 時は、6 月 6 日の午前 0 時に調整されます。</span><span class="sxs-lookup"><span data-stu-id="4206b-p103">Non-midnight start times are adjusted to the midnight prior to the time specified. For example, 1:00 PM on June 6 gets adjusted to 12:00 AM on June 6.</span></span>
    
- <span data-ttu-id="4206b-p104">午前 0 時以外の終了時間は、指定した時刻より後の午前 0 時に調整されます。たとえば、6 月 6 日の午後 1 時は、6 月 7 日の午前 0 時に調整されます。</span><span class="sxs-lookup"><span data-stu-id="4206b-p104">Non-midnight end times are adjusted to the midnight after the time specified. For example, 1:00 PM on June 6 gets adjusted to 12:00 AM on June 7.</span></span>
    
<span data-ttu-id="4206b-p105">このため、作成する終日イベントは、常に指定した開始時刻と終了時刻を含みますが、午前 0 時への移動により、ユーザーの予定表に追加の時間を要求することがあります。サーバーは、開始時刻と終了時刻を午前 0 時に調整するため、意図しない時間の変更を避けるために、開始時刻と終了時刻を午前 0 時に指定することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="4206b-p105">So the all-day event that you create is always inclusive of the start and end time that you specify, but might claim additional time on the user's calendar due to the shift to midnight. Because the server will adjust the start and end time to midnight, we recommend that you specify your start and end time at midnight to avoid any unintended changes to the times.</span></span>
  
<span data-ttu-id="4206b-p106">終日イベントを作成するときのタイム ゾーンを考慮することも重要です。Exchange サーバーにより、要求または予約のタイム ゾーンで午前 0 時の開始時刻と終了時刻が適用されるため、別のタイム ゾーンに構成されたクライアントで終日イベントを表示すると、予期しない結果になる可能性があります。クライアントによっては、終日イベントの一部として意図していない余分な日が終日イベントとして表示されたり、終日イベントとして表示されないことがあります。このため、終日イベントを作成するとき、可能な場合は常にユーザーが優先するタイム ゾーンを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="4206b-p106">It's also important to consider time zones when creating all-day events. Because the Exchange server enforces a midnight start and end time in the time zone of the request or appointment, viewing that all-day event in a client configured for a different time zone can yield unexpected results. Depending on the client, it might appear as an all-day event with extra days that you did not intend to include, or it might not appear as an all-day event altogether. Because of this, we recommend that you use the user's preferred time zone whenever possible when you create all-day events.</span></span>
  
## <a name="create-an-all-day-event-by-using-the-ews-managed-api"></a><span data-ttu-id="4206b-123">EWS マネージ API を使用して終日イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="4206b-123">Create an all-day event by using the EWS Managed API</span></span>

<span data-ttu-id="4206b-124">次の例では、EWS のマネージ API を使用して、_開始日_のパラメーターで指定され、 _numDays_パラメーターで指定された日数の継続期間が日付に開始、終日イベントを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="4206b-124">The following example shows how to use the EWS Managed API to create an all-day event, starting on the date specified by the  _startDate_ parameter and lasting for the number of days specified by the  _numDays_ parameter.</span></span> <span data-ttu-id="4206b-125">[ExchangeService.TimeZone](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx)プロパティで指定されたタイム ゾーンで予定を作成することに注意してください。</span><span class="sxs-lookup"><span data-stu-id="4206b-125">Note that the appointment will be created in the time zone specified by the [ExchangeService.TimeZone](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) property.</span></span> <span data-ttu-id="4206b-126">次の使用例では、[資格情報](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx)および[Url](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx)プロパティの有効な値を持つ_サービス_のパラメーターに渡された[ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトが初期化されたことを前提としています。</span><span class="sxs-lookup"><span data-stu-id="4206b-126">This example assumes that the [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object passed in the  _service_ parameter has been initialized with valid values for the [Credentials](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
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

## <a name="create-an-all-day-event-by-using-ews"></a><span data-ttu-id="4206b-127">EWS を使用して終日イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="4206b-127">Create an all-day event by using EWS</span></span>

<span data-ttu-id="4206b-128">終日イベントを作成するのには、EWS [CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)の要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4206b-128">The following example shows an EWS [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request to create an all-day event.</span></span> <span data-ttu-id="4206b-129">[TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx)要素で示されるように、東部タイム ゾーンで、予定が作成されます。</span><span class="sxs-lookup"><span data-stu-id="4206b-129">The appointment is created in the Eastern time zone, as indicated by the [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="4206b-130">[開始](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx)および[終了](http://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx)要素の値の時刻部分に変換する午前 0 時、東部標準時ゾーンの夏時間の期間中に両方の 04:00Z であることに注目してください。</span><span class="sxs-lookup"><span data-stu-id="4206b-130">Notice that the time portion of the values of the [Start](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) and [End](http://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) elements are both 04:00Z, which converts to midnight in the Eastern time zone during daylight saving time.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="4206b-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="4206b-131">See also</span></span>


- [<span data-ttu-id="4206b-132">Calendars and EWS in Exchange</span><span class="sxs-lookup"><span data-stu-id="4206b-132">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="4206b-133">Exchange 2013 の EWS を使用して予定および会議を作成します。</span><span class="sxs-lookup"><span data-stu-id="4206b-133">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="4206b-134">Exchange のタイム ゾーンと EWS</span><span class="sxs-lookup"><span data-stu-id="4206b-134">Time zones and EWS in Exchange</span></span>](time-zones-and-ews-in-exchange.md)
    


---
title: Exchange EWS を使用して予定のタイム ゾーンを更新します。
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: dc2240c1-5500-4d5c-97d5-09d63ffd30d5
description: Exchange の EWS マネージ API または EWS を使用して、既存の予定または会議のタイム ゾーンを更新する方法について説明します。
ms.openlocfilehash: 535eb9f546d9a4353408579f3a24750f32237699
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759068"
---
# <a name="update-the-time-zone-for-an-appointment-by-using-ews-in-exchange"></a><span data-ttu-id="602c1-103">Exchange EWS を使用して予定のタイム ゾーンを更新します。</span><span class="sxs-lookup"><span data-stu-id="602c1-103">Update the time zone for an appointment by using EWS in Exchange</span></span>

<span data-ttu-id="602c1-104">Exchange の EWS マネージ API または EWS を使用して、既存の予定または会議のタイム ゾーンを更新する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="602c1-104">Learn how to update the time zone for an existing appointment or meeting by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="602c1-p101">Exchange の予定表に予定または会議を作成するときに、開始時刻と終了時刻の指定に使用したタイム ゾーンは、予定の作成タイム ゾーンとして保存されます。このタイム ゾーンは、EWS マネージ API または EWS を使用することで変更できます。ただし、予定のタイム ゾーンの変更は、予定の開始時刻と終了時刻にも作用します。</span><span class="sxs-lookup"><span data-stu-id="602c1-p101">When an appointment or meeting is created on an Exchange calendar, the time zone used to specify the start and end times is saved as the creation time zone for the appointment. You can change that time zone by using the EWS Managed API or EWS. However, changing the time zone on an appointment has other effects on the start and end time of the appointment.</span></span>
  
<span data-ttu-id="602c1-108">時刻の値は、世界協定時刻 (UTC) で Exchange サーバーに格納されます。</span><span class="sxs-lookup"><span data-stu-id="602c1-108">Time values are stored on the Exchange server in Coordinate Universal Time (UTC).</span></span> <span data-ttu-id="602c1-109">1時 00分 PM (13:00) 東部標準時ゾーンで開始する予定が設定されている場合は (UTC 05:00)、値はサーバーでタイム ゾーンが (標準時) の段階にあると仮定した場合、6時 00分 PM (18:00) で保存することです。</span><span class="sxs-lookup"><span data-stu-id="602c1-109">So if an appointment is set to start at 1:00 PM (13:00) in the Eastern time zone (UTC-05:00), that value is stored as 6:00 PM (18:00) on the server, assuming that the time zone is in its standard time phase.</span></span> <span data-ttu-id="602c1-110">他のタイム ゾーンでその予定を表示すると、適切な時間数が追加または、特定のタイム ゾーンの時刻を確認するのには UTC 値から減算します。</span><span class="sxs-lookup"><span data-stu-id="602c1-110">When that appointment is viewed in other time zones, the appropriate number of hours is added or subtracted from the UTC value to determine the time zone-specific time.</span></span> <span data-ttu-id="602c1-111">午後 1時 00分に開始時刻を予定がある場合など東部 (午後 6時 00分 UTC) 太平洋標準時ゾーンのクライアントから表示し、(UTC 08:00)、特定のタイム ゾーンのクライアントは午前 10時 00分 (18時 00分-08:00) の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="602c1-111">For example, if an appointment has a start time at 1:00 PM Eastern (6:00 PM UTC), and is viewed from a client in the Pacific time zone (UTC-08:00), the time-zone specific start time for that client would be 10:00 AM (18:00 - 08:00).</span></span>
  
<span data-ttu-id="602c1-p103">開始時刻と終了時刻の更新なしに予定のタイム ゾーンを更新すると、サーバーに保存されている UTC の値は、開始時刻と終了時刻がタイム ゾーン固有の時刻と同じになるようにサーバーによって更新されます。たとえば、1:00 PM 東部標準時の予定について考えてみます。この時刻は、18:00 UTC としてサーバーに保存されます。予定のタイム ゾーンが太平洋標準時に変更されると、サーバーによって開始時刻が 1:00 PM 太平洋標準時 (21:00 UTC) にシフトされます。</span><span class="sxs-lookup"><span data-stu-id="602c1-p103">When you update the time zone of the appointment without updating the start and end time, the server updates the UTC values stored on the server to keep the start and end time as the same time zone-specific times. For example, consider the 1:00 PM Eastern appointment. The time is stored as 18:00 UTC on the server. If the time zone of the appointment is changed to the Pacific time zone, the server shifts the start time to 1:00 PM Pacific (21:00 UTC).</span></span>
  
<span data-ttu-id="602c1-116">この動作は、開始時刻と終了時刻を明示的に設定することで変更できます。</span><span class="sxs-lookup"><span data-stu-id="602c1-116">You can change this behavior by explicitly setting the start and end times.</span></span>
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="602c1-117">既存の予定のタイム ゾーンを更新する (EWS マネージ API を使用する場合)</span><span class="sxs-lookup"><span data-stu-id="602c1-117">Updating the time zone on an existing appointment by using the EWS Managed API</span></span>

<span data-ttu-id="602c1-118">次の例では、サーバーのタイム ゾーンに、 **Appointment.StartTimeZone**と**Appointment.EndTimeZone**のプロパティを更新することによって既存の予定のタイム ゾーンを更新するのには、EWS のマネージ API が使用されます。</span><span class="sxs-lookup"><span data-stu-id="602c1-118">In the following example, the EWS Managed API is used to update the time zone on an existing appointment to the Central time zone by updating the **Appointment.StartTimeZone** and **Appointment.EndTimeZone** properties.</span></span> <span data-ttu-id="602c1-119">_ShiftAppointnment_パラメーターは、 **true**に設定されている場合、コードでは予定の開始時刻と終了時刻は明示的に設定しません。</span><span class="sxs-lookup"><span data-stu-id="602c1-119">If the  _shiftAppointnment_ parameter is set to **true**, the code does not explicitly set the start and end times on the appointment.</span></span> <span data-ttu-id="602c1-120">この場合、サーバーは削除しないときは、同じタイム ゾーンの相対の時点で新しいタイム ゾーンの開始と終了時間に変更されます。</span><span class="sxs-lookup"><span data-stu-id="602c1-120">In this case, the server will shift the start and end times to keep them at the same time zone-relative times in the new time zone.</span></span> <span data-ttu-id="602c1-121">場合を**false**に設定、コードでは、UTC で同時に予定を維持するには、明示的に開始および終了時刻に変換します。</span><span class="sxs-lookup"><span data-stu-id="602c1-121">If set to **false**, the code converts the start and end times explicitly to keep the appointment at the same time in UTC.</span></span> 

<span data-ttu-id="602c1-122">次の使用例では、[資格情報](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx)と[Url](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx)のプロパティで有効な値を持つ**ExchangeService**オブジェクトが初期化されたことを前提としています。</span><span class="sxs-lookup"><span data-stu-id="602c1-122">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
static void UpdateAppointmentTimeZone(ExchangeService service, ItemId apptId, bool shiftAppointment)
{
    PropertySet includeTimeZones = new PropertySet(AppointmentSchema.Subject,
                                                   AppointmentSchema.Start,
                                                   AppointmentSchema.ReminderDueBy,
                                                   AppointmentSchema.End,
                                                   AppointmentSchema.StartTimeZone,
                                                   AppointmentSchema.EndTimeZone);
    Appointment apptToUpdate;
    // Load the existing appointment.
    // This will result in a call to EWS.
    try
    {
        apptToUpdate = Appointment.Bind(service, apptId, includeTimeZones);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error retrieving existing appointment: {0}", ex.Message);
        return;
    }
    Console.WriteLine("Before update:");
    // Output the current start, reminder, end, and time zones.
    Console.WriteLine("  Start: {0}", apptToUpdate.Start);
    Console.WriteLine("  Start time zone: {0}", apptToUpdate.StartTimeZone.DisplayName);
    Console.WriteLine("  Reminder: {0}", apptToUpdate.ReminderDueBy);
    Console.WriteLine("  End: {0}", apptToUpdate.End);
    Console.WriteLine("  End time zone: {0}", apptToUpdate.EndTimeZone.DisplayName);
    // Retrieve the Central time zone.
    TimeZoneInfo centralTZ = TimeZoneInfo.FindSystemTimeZoneById("Central Standard Time");
    // Update the time zones on the appointment.
    apptToUpdate.StartTimeZone = centralTZ;
    apptToUpdate.EndTimeZone = centralTZ;
    if (!shiftAppointment)
    {
        // Set the start and end times explicitly so that the appointment
        // will start and end at the same UTC time.
        // Convert the times to then Central time zone. This
        // will keep them at the same time in UTC.
        // For example, 1:00 PM Eastern becomes 12:00 PM Central.
        DateTime newStartTime = TimeZoneInfo.ConvertTime(
            apptToUpdate.Start, centralTZ);
        DateTime newEndTime = TimeZoneInfo.ConvertTime(
            apptToUpdate.End, centralTZ);
        apptToUpdate.Start = newStartTime;
        apptToUpdate.End = newEndTime;
    }
    try
    {
        // Save the changes. This will result in a call to EWS.
        apptToUpdate.Update(ConflictResolutionMode.AlwaysOverwrite, 
            SendInvitationsOrCancellationsMode.SendToNone);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error updating appointment: {0}", ex.Message);
        return;
    }
    // Now rebind to the appointment to get the new values.
    Appointment apptAfterUpdate;
    
    try
    {
        // This will result in a call to EWS.
        apptAfterUpdate = Appointment.Bind(service, apptId, includeTimeZones);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error retrieving existing appointment: {0}", ex.Message);
        return;
    }
    Console.WriteLine("After update:");
    // Output the current start, reminder, end, and time zones.
    Console.WriteLine("  Start: {0}", apptAfterUpdate.Start);
    Console.WriteLine("  Start time zone: {0}", apptAfterUpdate.StartTimeZone.DisplayName);
    Console.WriteLine("  Reminder: {0}", apptAfterUpdate.ReminderDueBy);
    Console.WriteLine("  End: {0}", apptAfterUpdate.End);
    Console.WriteLine("  End time zone: {0}", apptAfterUpdate.EndTimeZone.DisplayName);
}
```

<span data-ttu-id="602c1-123">午後 1時 00分に開始する予定を更新する例を使用すると東部と、午後 2時 00分で終了し東部、 _shiftAppointment_パラメーターを使用して true の場合、および[ExchangeService.TimeZone](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx)は米国東部標準時ゾーンには、出力は次の次のように。</span><span class="sxs-lookup"><span data-stu-id="602c1-123">When the example is used to update an appointment that starts at 1:00 PM Eastern and ends at 2:00 PM Eastern, with the  _shiftAppointment_ parameter set to true, and the [ExchangeService.TimeZone](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) property set to the Eastern time zone, the output looks like the following.</span></span> 
  
```MS-DOS
Before update:
  Start: 6/20/2014 1:00:00 PM
  Start time zone: (UTC-05:00) Eastern Time (US &amp; Canada)
  Reminder: 6/20/2014 1:00:00 PM
  End: 6/20/2014 2:00:00 PM
  End time zone: (UTC-05:00) Eastern Time (US &amp; Canada)
After update:
  Start: 6/20/2014 2:00:00 PM
  Start time zone: (UTC-06:00) Central Time (US &amp; Canada)
  Reminder: 6/20/2014 2:00:00 PM
  End: 6/20/2014 3:00:00 PM
  End time zone: (UTC-06:00) Central Time (US &amp; Canada)
```

<span data-ttu-id="602c1-124">_ShiftAppointment_パラメーターが false に設定と**タイム ゾーン**プロパティが東部標準時ゾーンに設定してもう一度同じ予定を更新する例を使用する場合、出力が少し異なるになります。</span><span class="sxs-lookup"><span data-stu-id="602c1-124">When the example is used to update the same appointment with the  _shiftAppointment_ parameter set to false, and with the **TimeZone** property again set to the Eastern time zone, the output looks a little different.</span></span> 
  
```MS-DOS
Before update:
  Start: 6/20/2014 1:00:00 PM
  Start time zone: (UTC-05:00) Eastern Time (US &amp; Canada)
  Reminder: 6/20/2014 1:00:00 PM
  End: 6/20/2014 2:00:00 PM
  End time zone: (UTC-05:00) Eastern Time (US &amp; Canada)
After update:
  Start: 6/20/2014 1:00:00 PM
  Start time zone: (UTC-06:00) Central Time (US &amp; Canada)
  Reminder: 6/20/2014 1:00:00 PM
  End: 6/20/2014 2:00:00 PM
  End time zone: (UTC-06:00) Central Time (US &amp; Canada)
```

<span data-ttu-id="602c1-125">開始時刻と終了時刻が変更されていないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="602c1-125">Notice that the start and end times did not change.</span></span> <span data-ttu-id="602c1-126">時間東部標準時で解釈されるためにはこのゾーンのため、**タイム ゾーン**プロパティは、東部標準時に設定されます)、シフトから予定を防ぐために、時間の値が更新されたとします。</span><span class="sxs-lookup"><span data-stu-id="602c1-126">This is because the times are being interpreted in the Eastern time zone (because the **TimeZone** property is set to the Eastern time zone), and the time values were updated to prevent the appointment from shifting.</span></span> 
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-ews"></a><span data-ttu-id="602c1-127">既存の予定のタイム ゾーンを更新する (EWS を使用する場合)</span><span class="sxs-lookup"><span data-stu-id="602c1-127">Updating the time zone on an existing appointment by using EWS</span></span>

<span data-ttu-id="602c1-128">次の例の EWS [UpdateItem 操作](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)要求は、予定のタイム ゾーンを更新します。</span><span class="sxs-lookup"><span data-stu-id="602c1-128">The following example EWS [UpdateItem operation](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) request updates the time zone on an appointment.</span></span> <span data-ttu-id="602c1-129">相対タイム ゾーンの新しいタイム ゾーンで同時に保持する予定の開始および終了時刻をサーバーが変更されますので、次の使用例はのみ[StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx)と[EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx)の要素を更新します。</span><span class="sxs-lookup"><span data-stu-id="602c1-129">This example only updates the [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) and [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) elements, so the server will shift the start and end times of the appointment to keep it at the same time-zone-relative time in the new time zone.</span></span> <span data-ttu-id="602c1-130">**アイテム Id**要素の値は、読みやすくするために短縮されます。</span><span class="sxs-lookup"><span data-stu-id="602c1-130">The value of the **ItemId** element is shortened for readability.</span></span> 
  
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
    <m:UpdateItem ConflictResolution="AlwaysOverwrite" SendMeetingInvitationsOrCancellations="SendToNone">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:StartTimeZone" />
              <t:CalendarItem>
                <t:StartTimeZone Id="Central Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:EndTimeZone" />
              <t:CalendarItem>
                <t:EndTimeZone Id="Central Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="602c1-131">次の例の要求は、予定のタイム ゾーンを更新しも明示的に**開始**および**終了**要素を設定することにより、開始時刻と終了時刻を更新します。</span><span class="sxs-lookup"><span data-stu-id="602c1-131">The following example request updates the time zone of the appointment, and also updates the start and end times by explicitly setting the **Start** and **End** elements.</span></span> <span data-ttu-id="602c1-132">**アイテム Id**要素の値は、読みやすくするために短縮されます。</span><span class="sxs-lookup"><span data-stu-id="602c1-132">The value of the **ItemId** element is shortened for readability.</span></span> 
  
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
    <m:UpdateItem ConflictResolution="AlwaysOverwrite" SendMeetingInvitationsOrCancellations="SendToNone">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:StartTimeZone" />
              <t:CalendarItem>
                <t:StartTimeZone Id="Central Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:EndTimeZone" />
              <t:CalendarItem>
                <t:EndTimeZone Id="Central Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Start" />
              <t:CalendarItem>
                <t:Start>2014-06-20T17:00:00.000Z</t:Start>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:End" />
              <t:CalendarItem>
                <t:End>2014-06-20T18:00:00.000Z</t:End>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="602c1-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="602c1-133">See also</span></span>

- [<span data-ttu-id="602c1-134">Exchange のタイム ゾーンと EWS</span><span class="sxs-lookup"><span data-stu-id="602c1-134">Time zones and EWS in Exchange</span></span>](time-zones-and-ews-in-exchange.md)   
- [<span data-ttu-id="602c1-135">Exchange EWS を使用して、特定のタイム ゾーンで予定を作成します。</span><span class="sxs-lookup"><span data-stu-id="602c1-135">Create appointments in a specific time zone by using EWS in Exchange</span></span>](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="602c1-136">Exchange EWS を使用して予定および会議を更新します。</span><span class="sxs-lookup"><span data-stu-id="602c1-136">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    


---
title: Exchange の EWS を使用して予定のタイム ゾーンを更新する
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: dc2240c1-5500-4d5c-97d5-09d63ffd30d5
description: Exchange の EWS マネージ API または EWS を使用して、既存の予定または会議のタイム ゾーンを更新する方法について説明します。
ms.openlocfilehash: 064f99997b7c3d1197cb8d1ee6a24f8fb874f706
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455843"
---
# <a name="update-the-time-zone-for-an-appointment-by-using-ews-in-exchange"></a>Exchange の EWS を使用して予定のタイム ゾーンを更新する

Exchange の EWS マネージ API または EWS を使用して、既存の予定または会議のタイム ゾーンを更新する方法について説明します。
  
Exchange の予定表に予定または会議を作成するときに、開始時刻と終了時刻の指定に使用したタイム ゾーンは、予定の作成タイム ゾーンとして保存されます。このタイム ゾーンは、EWS マネージ API または EWS を使用することで変更できます。ただし、予定のタイム ゾーンの変更は、予定の開始時刻と終了時刻にも作用します。
  
時刻の値は、協定世界時 (UTC) で Exchange サーバーに保存されます。 そのため、予定の開始が東部標準時 (UTC-05:00) で 1:00 PM (13:00) に設定されている場合、その値は 6:00 PM (18:00) としてサーバーに保存されます (タイム ゾーンが標準時のフェーズ内にあると想定しています)。 その予定が別のタイム ゾーンで表示されるときには、UTC 値に適切な時間数が加減算されて、タイム ゾーン固有の時刻が決定されます。 たとえば、予定の開始時刻が 1:00 PM 東部標準時 (6:00 PM UTC) のときに、その予定が太平洋標準時 (UTC - 08:00) のクライアントで表示されると、そのクライアントのタイム ゾーン固有の開始時刻は 10:00 AM (18:00 - 08:00) になります。
  
開始時刻と終了時刻の更新なしに予定のタイム ゾーンを更新すると、サーバーに保存されている UTC の値は、開始時刻と終了時刻がタイム ゾーン固有の時刻と同じになるようにサーバーによって更新されます。たとえば、1:00 PM 東部標準時の予定について考えてみます。この時刻は、18:00 UTC としてサーバーに保存されます。予定のタイム ゾーンが太平洋標準時に変更されると、サーバーによって開始時刻が 1:00 PM 太平洋標準時 (21:00 UTC) にシフトされます。
  
この動作は、開始時刻と終了時刻を明示的に設定することで変更できます。
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-the-ews-managed-api"></a>既存の予定のタイム ゾーンを更新する (EWS マネージ API を使用する場合)

次の例では、EWS マネージ API を使用して、**Appointment.StartTimeZone** プロパティと **Appointment.EndTimeZone** プロパティを更新することで、既存の予定のタイム ゾーンを中部標準時に更新しています。 _shiftAppointment_ パラメーターが **true** に設定されている場合は、コードでは予定の開始時刻と終了時刻を明示的に設定しません。 この場合、開始時刻と終了時刻は新しいタイム ゾーンで同じタイム ゾーン相対時刻になるようにサーバーによってシフトされます。 **false** に設定されている場合は、予定が UTC で同じ時刻になるように、開始時刻と終了時刻を明示的にコードで変換します。 

この例では、**ExchangeService** オブジェクトは [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) プロパティと [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) プロパティの有効な値で初期化されているものとします。 
  
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

この例を使用して、開始が 1:00 PM 東部標準時で終了が 2:00 PM 東部標準時の予定を更新する場合、_shiftAppointment_ パラメーターが true に設定されていて、[ExchangeService.TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) プロパティが東部標準時に設定されていると、出力は次のようになります。 
  
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

この例を使用して同じ予定を更新するときに、_shiftAppointment_ パラメーターが false に設定されていて、**TimeZone** プロパティが東部標準時に設定されていると、出力はわずかに異なります。 
  
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

開始時刻と終了時刻が変更されていない点に注目してください。 これは、時刻が東部標準時で解釈されていて (**TimeZone** プロパティが東部標準時に設定されているため)、予定がずれないように時刻の値が更新されたためです。 
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-ews"></a>既存の予定のタイム ゾーンを更新する (EWS を使用する場合)

次に示す EWS の [UpdateItem 操作](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)要求の例では、予定のタイム ゾーンを更新します。 この例では、[StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) 要素と [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) 要素のみを更新しています。そのため、開始時刻と終了時刻は新しいタイム ゾーンで同じタイム ゾーン相対時刻になるようにサーバーによってシフトされます。 **ItemId** 要素の値は、読みやすいよう短縮してあります。 
  
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

次に示す要求例では、予定のタイム ゾーンを更新します。さらに、**Start** 要素と **End** 要素を明示的に設定することで開始時刻と終了時刻も更新します。 **ItemId** 要素の値は、読みやすいよう短縮してあります。 
  
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

## <a name="see-also"></a>関連項目

- [Exchange のタイム ゾーンと EWS](time-zones-and-ews-in-exchange.md)   
- [Exchange の EWS を使用して、特定のタイム ゾーンで予定を作成する](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)   
- [Exchange で EWS を使用して予定と会議を更新する](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    


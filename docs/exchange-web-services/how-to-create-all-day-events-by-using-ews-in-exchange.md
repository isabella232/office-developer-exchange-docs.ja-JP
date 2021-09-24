---
title: Exchange で EWS を使用して終日イベントを作成する
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 0fcb484b-4ffc-41a5-aeed-8c797766b70c
description: Exchange で EWS マネージ API または EWS を使用して、終日イベントを作成する方法について説明します。
ms.openlocfilehash: 8769999907df46f519355a36fdf409f9ad347330
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521222"
---
# <a name="create-all-day-events-by-using-ews-in-exchange"></a>Exchange で EWS を使用して終日イベントを作成する

Exchange で EWS マネージ API または EWS を使用して、終日イベントを作成する方法について説明します。
  
終日イベントは、休日や休暇など、1 日または複数の日で発生する事項を表す方法を提供します。EWS マネージ API または EWS を使用した終日イベントの作成は、簡単な作業です。[予定の作成](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)と似ていますが、少しだけ違いがあります。
  
## <a name="setting-start-and-end-times"></a>開始時間と終了時間の設定

定義では、終日イベントは特定の午前 0 時に開始され、24 時間 (または24 時間の倍数) 後に終了します。ただし、EWS マネージ APIと EWS では、終日イベントを作成するときに、午前 0 時以外の時刻を指定できます。これにより、サーバーでのこれらの時間変換の方法を認識していないと、予期しない動作が発生する可能性があります。
  
([要求または予定のタイム ゾーン](time-zones-and-ews-in-exchange.md)の) 午前 0 時以外の開始時間または終了時間を持つ終日イベントを新しく作成する通知を受信すると、これらの時間は次の規則に従い、適切なタイム ゾーンの午前 0 時に調整されます。
  
- 午前 0 時以外の開始時間は、指定した時刻より前の午前 0 時に調整されます。たとえば、6 月 6 日の午後 1 時は、6 月 6 日の午前 0 時に調整されます。
    
- 午前 0 時以外の終了時間は、指定した時刻より後の午前 0 時に調整されます。たとえば、6 月 6 日の午後 1 時は、6 月 7 日の午前 0 時に調整されます。
    
このため、作成する終日イベントは、常に指定した開始時刻と終了時刻を含みますが、午前 0 時への移動により、ユーザーの予定表に追加の時間を要求することがあります。サーバーは、開始時刻と終了時刻を午前 0 時に調整するため、意図しない時間の変更を避けるために、開始時刻と終了時刻を午前 0 時に指定することをお勧めします。
  
終日イベントを作成するときのタイム ゾーンを考慮することも重要です。Exchange サーバーにより、要求または予約のタイム ゾーンで午前 0 時の開始時刻と終了時刻が適用されるため、別のタイム ゾーンに構成されたクライアントで終日イベントを表示すると、予期しない結果になる可能性があります。クライアントによっては、終日イベントの一部として意図していない余分な日が終日イベントとして表示されたり、終日イベントとして表示されないことがあります。このため、終日イベントを作成するとき、可能な場合は常にユーザーが優先するタイム ゾーンを使用することをお勧めします。
  
## <a name="create-an-all-day-event-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して終日イベントを作成する

次の例は、EWS マネージ API を使用して、_startDate_ パラメーターによって指定される日付から始まり、_numDays_ パラメーターによって指定される日数続く終日イベントを作成する方法を示します。 予定は [ExchangeService.TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) プロパティによって指定されるタイム ゾーンで作成されます。 この例では、_service_ パラメーターで渡される [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトが、[Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) プロパティと [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) プロパティの有効な値で初期化されているものとします。 
  
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

## <a name="create-an-all-day-event-by-using-ews"></a>EWS を使用して終日イベントを作成する

次の例では、終日イベントを作成する EWS [CreateItem 操作](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)要求を示します。予定は、[TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) 要素で示すように、米国東部標準時ゾーンで作成されます。なお、[Start](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) 要素と [End](https://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) 要素の値の時間部分は両方とも 04:00Z であり、これは夏時間中の米国東部標準時ゾーンの午前 0 時に変換します。 
  
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

## <a name="see-also"></a>関連項目


- [Exchange の予定表と EWS](calendars-and-ews-in-exchange.md)
    
- [Exchange 2013 の EWS を使用して予定と会議を作成する](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Exchange のタイム ゾーンと EWS](time-zones-and-ews-in-exchange.md)
    


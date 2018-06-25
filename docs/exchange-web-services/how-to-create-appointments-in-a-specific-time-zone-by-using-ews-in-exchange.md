---
title: Exchange EWS を使用して、特定のタイム ゾーンで予定を作成します。
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e68aaa27-250e-4170-b099-077a979c127c
description: Exchange の EWS マネージ API または EWS を使用して、特定のタイム ゾーンで予定を作成する方法について説明します。
ms.openlocfilehash: 1725498847f89a417b62a06fb8a3109af5c4deb0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758941"
---
# <a name="create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange"></a>Exchange EWS を使用して、特定のタイム ゾーンで予定を作成します。

Exchange の EWS マネージ API または EWS を使用して、特定のタイム ゾーンで予定を作成する方法について説明します。
  
Exchange の予定表の予定または会議が作成されると、予定の作成のタイム ゾーンとして、開始時刻と終了時刻を指定するために使用するタイム ゾーンが保存されます。 そのタイム ゾーンにも使用[、明示的なタイム ゾーンが指定されていない日付と時刻の値の意味](time-zones-and-ews-in-exchange.md)を、タイム ゾーンを指定してオプションについて理解することが重要であるようにします。
  
## <a name="creating-appointments-in-different-time-zones-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して異なるタイムゾーンで予定を作成する

EWS マネージ API を使用して予定または会議を作成するときには、タイム ゾーンを指定するための 3 オプションがあります。
  
- EWS のマネージ API が実行されているコンピューターのタイム ゾーンを使用するに指定しないタイム ゾーン、 [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトを作成するときです。 
    
- すべての日付と時刻のプロパティの特定のタイム ゾーンを使用するには、プロパティを含む新しい予定を作成するときや、会議は、 **ExchangeService**オブジェクトのコンス トラクターでタイム ゾーンを指定します。 
    
- [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx)プロパティで指定されたよりも、別のタイム ゾーンを使用するには、 [Appointment.StartTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx)と[Appointment.EndTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx)のプロパティを使用します。 
    
    > [!NOTE]
    > **EndTimeZone**プロパティをできるは、 **Exchange2010**またはそれ以降、 [ExchangeService.RequestedServerVersion](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx)プロパティが設定されている場合だけです。 使用できない場合は**StartTimeZone**を設定する予定の時間の開始と終了の両方に適用されます。 
  
次の例では、EWS のマネージ API を使用して、次の 3 つの予定を作成できます。 未指定のタイム ゾーンと最後に 1 時間後からここでは、2 日の午後 1時 00分に開始する予定が設定されています。 最初の予定は、EWS のマネージ API の既定の動作を使用して、クライアント コンピューターのタイム ゾーンで作成されます。 **Appointment.StartTimeZone**および**Appointment.EndTimeZone**プロパティを使用してサーバーの全体のタイム ゾーンで 2 番目が作成されます。 山地標準時ゾーンで、 **ExchangeService.TimeZone**プロパティを使用して 3 番目が作成されます。 
  
```cs
using Microsoft.Exchange.WebServices.Data;
using System.Security;
static void CreateAppointments(string userEmail, SecureString userPass)
{
    // *****************************************************
    // Create an appointment using the client computer's time zone.
    // *****************************************************
    // Do not specify a time zone when creating the ExchangeService.
    ExchangeService clientTZService = new ExchangeService(ExchangeVersion.Exchange2010);
    clientTZService.Credentials = new NetworkCredential(userEmail, userPass);
    clientTZService.AutodiscoverUrl(userEmail, redirectionCallback);
    // Create the appointment.
    Appointment clientTZAppt = new Appointment(clientTZService);
    clientTZAppt.Subject = "Appointment created using client time zone";
    clientTZAppt.Body = new MessageBody(string.Format("Time zone: {0}", clientTZService.TimeZone.DisplayName));
    // Set the start time to 1:00 PM two days from today.
    DateTime startTime = new DateTime(DateTime.Now.Year, DateTime.Now.Month, DateTime.Now.Day + 2);
    startTime = startTime.AddHours(13);
    clientTZAppt.Start = startTime;
    // Set the end time to 2:00 PM on that same day.
    DateTime endTime = startTime.AddHours(1);
    clientTZAppt.End = endTime;
    // Save the appointment to the default calendar.
    try
    {
        // This method results in a call to EWS.
        clientTZAppt.Save(SendInvitationsMode.SendToNone);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error saving appointment: {0}", ex.Message);
    }
    // *****************************************************
    // Create an appointment in the Central time zone by
    // using the StartTimeZone property.
    // *****************************************************
    // Retrieve the Central time zone.
    TimeZoneInfo centralTZ = TimeZoneInfo.FindSystemTimeZoneById("Central Standard Time");
    // Create the appointment.
    Appointment centralTZAppt = new Appointment(clientTZService);
    centralTZAppt.Subject = "Appointment created using Central time zone";
    centralTZAppt.Body = new MessageBody(string.Format("Time zone: {0}", centralTZ.DisplayName));
    // Set the time zone on the appointment.
    centralTZAppt.StartTimeZone = centralTZ;
    centralTZAppt.EndTimeZone = centralTZ;
    // Set the start time to 1:00 PM two days from today.
    centralTZAppt.Start = startTime;
    // Set the end time to 2:00 PM on that same day.
    centralTZAppt.End = endTime;
    // Save the appointment to the default calendar.
    try
    {
        // This method results in a call to EWS.
        centralTZAppt.Save(SendInvitationsMode.SendToNone);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error saving appointment: {0}", ex.Message);
    }
    // *****************************************************
    // Create an appointment in the Mountain time zone by
    // using the ExchangeService.TimeZone property.
    // *****************************************************
    // Specify the Mountain time zone when creating the ExchangeService.
    TimeZoneInfo mountainTZ = TimeZoneInfo.FindSystemTimeZoneById("Mountain Standard Time");
    ExchangeService mountainTZService = new ExchangeService(ExchangeVersion.Exchange2010, mountainTZ);
    mountainTZService.Credentials = new NetworkCredential(userEmail, userPass);
    mountainTZService.AutodiscoverUrl(userEmail, redirectionCallback);
    // Create the appointment.
    Appointment mountainTZAppt = new Appointment(mountainTZService);
    mountainTZAppt.Subject = "Appointment created using Mountain time zone";
    mountainTZAppt.Body = new MessageBody(string.Format("Time zone: {0}", mountainTZService.TimeZone.DisplayName));
    // Set the start time to 1:00 PM two days from today.
    mountainTZAppt.Start = startTime;
    // Set the end time to 2:00 PM on that same day.
    mountainTZAppt.End = endTime;
    // Save the appointment to the default calendar.
    try
    {
        // This method results in a call to EWS.
        mountainTZAppt.Save(SendInvitationsMode.SendToNone);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error saving appointment: {0}", ex.Message);
    }
}
```

この例を東部標準時で構成されているクライアント コンピューターで実行して、それによって作成された予定を東部標準時で構成されているクライアントで表示すると、それぞれの予定が 1:00 PM、2:00 PM、および 3:00 PM に始まるように示されます。
  
## <a name="creating-appointments-in-different-time-zones-by-using-ews"></a>EWS を使用して異なるタイムゾーンで予定を作成する

EWS を使用して予定または会議を作成するときには、タイム ゾーンを指定するための 3 オプションがあります。
  
- 使用するには世界協定時刻 (UTC) に含まれない[TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx)要素、 [MeetingTimeZone](http://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx)の要素 (Exchange 2007 のみ) または[StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx)および[EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx)要素 (Exchange 2010 およびそれ以降)、 [CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)要求します。 
    
- すべての日付と時刻のプロパティの特定のタイム ゾーンを使用するには、プロパティを含む新しい予定を作成するときや、会議は[CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)要求内の[TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx)要素でタイム ゾーンを指定します。 
    
- [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx)要素で指定されたよりも、別のタイム ゾーンを使用するには、要素の[TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) 、 [MeetingTimeZone](http://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx)要素 (Exchange 2007 のみ) または[StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx)と[EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx)の要素 (Exchange 2010 以降) [CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)の要求にします。 
    
次の使用例[CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)の要求では、UTC を使用して予定を作成します。 **TimeZoneContext**要素、 **StartTimeZone**要素、および**EndTimeZone**の要素が存在しないことに注意してください。 要素の**開始**と**終了**の値は UTC で表されます。 
  
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
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Appointment created using UTC</t:Subject>
          <t:Body BodyType="HTML">Time zone: UTC</t:Body>
          <t:Start>2014-06-07T17:00:00.000Z</t:Start>
          <t:End>2014-06-07T18:00:00.000Z</t:End>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

次の使用例[CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)要求は、予定のサーバーの全体のタイム ゾーンを指定するのには、 **StartTimeZone**と**EndTimeZone**の要素を使用します。 **TimeZoneContext**要素が存在しないことに注意してください。 ただし、存在する場合は、 **StartTimeZone**と**EndTimeZone**の要素の値はその値をオーバーライドします。 もう一度、**開始**および**終了**要素の値は UTC で表されます。 
  
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
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Appointment created using Central time zone</t:Subject>
          <t:Body BodyType="HTML">Time zone: (UTC-06:00) Central Time (US &amp;amp; Canada)</t:Body>
          <t:Start>2014-06-07T18:00:00.000Z</t:Start>
          <t:End>2014-06-07T19:00:00.000Z</t:End>
          <t:StartTimeZone Id="Central Standard Time" />
          <t:EndTimeZone Id="Central Standard Time" />
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

次の使用例[CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)の要求は、 **TimeZoneContext**要素を山地標準時に設定します。 **StartTimeZone**と**EndTimeZone**の要素が存在しないことに注意してください。 もう一度、**開始**および**終了**要素の値は UTC で表されます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Mountain Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Appointment created using Mountain time zone</t:Subject>
          <t:Body BodyType="HTML">Time zone: (UTC-07:00) Mountain Time (US &amp;amp; Canada)</t:Body>
          <t:Start>2014-06-07T19:00:00.000Z</t:Start>
          <t:End>2014-06-07T20:00:00.000Z</t:End>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

前述の EWS 要求の例で作成された 3 つの予定を東部標準時で構成されているクライアントで表示すると、それぞれの予定が 1:00 PM、2:00 PM、および 3:00 PM に始まるように示されます。
  
## 

特定のタイム ゾーンで予定を作成する方法を理解する別[の既存の予定のタイム ゾーンを更新](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)する場合があります。 
  
## <a name="see-also"></a>関連項目


- [Exchange のタイム ゾーンと EWS](time-zones-and-ews-in-exchange.md)
    
- [Exchange EWS を使用して予定のタイム ゾーンを更新します。](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
- [Exchange 2013 の EWS を使用して予定および会議を作成します。](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    


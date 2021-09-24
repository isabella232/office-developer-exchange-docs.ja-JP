---
title: Exchange の EWS を使用して、特定のタイム ゾーンで予定を作成する
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: e68aaa27-250e-4170-b099-077a979c127c
description: Exchange の EWS マネージ API または EWS を使用して、特定のタイム ゾーンで予定を作成する方法について説明します。
ms.openlocfilehash: 589c72982fdda568170468c376b8a6d9f598aa36
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521145"
---
# <a name="create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange"></a>Exchange の EWS を使用して、特定のタイム ゾーンで予定を作成する

Exchange の EWS マネージ API または EWS を使用して、特定のタイム ゾーンで予定を作成する方法について説明します。
  
Exchange の予定表に予定または会議を作成するときに、開始時刻と終了時刻の指定に使用したタイム ゾーンは、予定の作成タイム ゾーンとして保存されます。そのタイム ゾーンは、[明示的にタイム ゾーンが指定されていない日付および時刻の値の解釈](time-zones-and-ews-in-exchange.md)にも使用されるため、タイム ゾーンを指定するオプションについて理解することが重要になります。
  
## <a name="creating-appointments-in-different-time-zones-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して異なるタイムゾーンで予定を作成する

EWS マネージ API を使用して予定または会議を作成するときには、タイム ゾーンを指定するための 3 つのオプションがあります。
  
- EWS マネージ API を実行しているコンピューターのタイム ゾーン使用する。この場合は、[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトの作成時にタイム ゾーンを指定しません。 
    
- すべての日付/時刻のプロパティ (新しい予定や会議の作成時のプロパティも含む) に特定のタイム ゾーンを指定する。この場合は、**ExchangeService** オブジェクトのコンストラクターでタイム ゾーンを指定します。 
    
- [ExchangeService.TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) プロパティで指定したものとは別のタイム ゾーンを使用する。この場合は、[Appointment.StartTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) プロパティと [Appointment.EndTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) プロパティを使用します。 
    
    > [!NOTE]
    > **EndTimeZone** プロパティは、[ExchangeService.RequestedServerVersion](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) プロパティが **Exchange2010** 以降に設定されている場合にのみ使用できます。 使用できない場合は、**StartTimeZone** を設定して、予定の開始時刻と終了時刻の両方に適用します。 
  
次の例では、3 つの予定の作成に EWS マネージ API が使用されています。それぞれの予定は、未指定のタイム ゾーンで現在から 2 日後の 1:00 PM に始まり、その 1 時間後に終わります。最初の予定は、既定の EWS マネージ API の動作を使用することで、クライアント コンピューターのタイム ゾーンで作成されます。2 番目は、**Appointment.StartTimeZone** プロパティと **Appointment.EndTimeZone** プロパティを使用することで、中部標準時で作成されます。3 番目は、**ExchangeService.TimeZone** プロパティを使用することで、山地標準時で作成されます。 
  
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
  
- 協定世界時 (UTC) を使用する。この場合は、[TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) 要素、[MeetingTimeZone](https://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) 要素 (Exchange 2007 のみ)、または [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) 要素と [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) 要素 (Exchange 2010 以降) を [CreateItem 操作](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)要求に含めません。 
    
- すべての日付/時刻のプロパティ (新しい予定や会議の作成時のプロパティも含む) に特定のタイム ゾーンを指定する。この場合は、[CreateItem 操作](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)要求の [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) 要素でタイム ゾーンを指定します。 
    
- [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) 要素で指定したものとは別のタイム ゾーンを使用する。この場合は、[TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) 要素、[MeetingTimeZone](https://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) 要素 (Exchange 2007 のみ)、または [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) 要素と [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) 要素 (Exchange 2010 以降) を [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 操作要求に含めません。 
    
次の [CreateItem 操作](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)要求の例では、UTC を使用して予定を作成します。**TimeZoneContext** 要素、**StartTimeZone** 要素、および **EndTimeZone** 要素が存在していないことに注目してください。**Start** 要素と **End** 要素の値は UTC で表されます。  
  
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

次の [CreateItem 操作](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)要求の例では、**StartTimeZone** 要素と **EndTimeZone** 要素を使用して、予定に中部標準時を指定します。**TimeZoneContext** 要素が存在していないことに注目してください。ただし、その要素が存在していたとしても、その値は **StartTimeZone** 要素と **EndTimeZone** 要素の値で上書きされます。この場合も、**Start** 要素と **End** 要素の値は UTC で表されます。 
  
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

次の [CreateItem 操作](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)要求の例では、**TimeZoneContext** 要素を山地標準時に設定します。**StartTimeZone** 要素と **EndTimeZone** 要素が存在していないことに注目してください。この場合も、**Start** 要素と **End** 要素の値は UTC で表されます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

特定のタイム ゾーンで予定を作成する方法について理解できました。次は、[既存の予定のタイム ゾーンを更新](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)して別のタイム ゾーンにしてみてください。 
  
## <a name="see-also"></a>関連項目


- [Exchange のタイム ゾーンと EWS](time-zones-and-ews-in-exchange.md)
    
- [Exchange の EWS を使用して予定のタイム ゾーンを更新する](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
- [Exchange 2013 の EWS を使用して予定と会議を作成する](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    


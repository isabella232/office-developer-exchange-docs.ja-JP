---
title: Exchange の EWS を使用して、特定のタイム ゾーンで予定を作成する
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e68aaa27-250e-4170-b099-077a979c127c
description: Exchange の EWS マネージ API または EWS を使用して、特定のタイム ゾーンで予定を作成する方法について説明します。
ms.openlocfilehash: 1725498847f89a417b62a06fb8a3109af5c4deb0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758941"
---
# <a name="create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange"></a><span data-ttu-id="462ea-103">Exchange の EWS を使用して、特定のタイム ゾーンで予定を作成する</span><span class="sxs-lookup"><span data-stu-id="462ea-103">How to: Create appointments in a specific time zone by using EWS in Exchange</span></span>

<span data-ttu-id="462ea-104">Exchange の EWS マネージ API または EWS を使用して、特定のタイム ゾーンで予定を作成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="462ea-104">Learn how to create appointments in specific time zones by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="462ea-105">Exchange の予定表に予定または会議を作成するときに、開始時刻と終了時刻の指定に使用したタイム ゾーンは、予定の作成タイム ゾーンとして保存されます。</span><span class="sxs-lookup"><span data-stu-id="462ea-105">When an appointment or meeting is created on an Exchange calendar, the time zone used to specify the start and end times is saved as the creation time zone for the appointment. That time zone is also used to interpret date and time values that do not have an explicit time zone specified, so it is important to understand your options to specify the time zone.</span></span> <span data-ttu-id="462ea-106">そのタイム ゾーンは、[明示的にタイム ゾーンが指定されていない日付および時刻の値の解釈](time-zones-and-ews-in-exchange.md)にも使用されるため、タイム ゾーンを指定するオプションについて理解することが重要になります。</span><span class="sxs-lookup"><span data-stu-id="462ea-106">When an appointment or meeting is created on an Exchange calendar, the time zone used to specify the start and end times is saved as the creation time zone for the appointment. That time zone is also used to [interpret date and time values that do not have an explicit time zone specified](time-zones-and-ews-in-exchange.md), so it is important to understand your options to specify the time zone.</span></span>
  
## <a name="creating-appointments-in-different-time-zones-by-using-the-ews-managed-api"></a><span data-ttu-id="462ea-107">EWS マネージ API を使用して異なるタイムゾーンで予定を作成する</span><span class="sxs-lookup"><span data-stu-id="462ea-107">Creating appointments in different time zones by using the EWS Managed API</span></span>

<span data-ttu-id="462ea-108">EWS マネージ API を使用して予定または会議を作成するときには、タイム ゾーンを指定するための 3 つのオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="462ea-108">When creating appointments or meetings using the EWS Managed API, you have three options for specifying the time zone:</span></span>
  
- <span data-ttu-id="462ea-109">EWS マネージ API を実行しているコンピューターのタイム ゾーン使用する。この場合は、[ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトの作成時にタイム ゾーンを指定しません。</span><span class="sxs-lookup"><span data-stu-id="462ea-109">To use the time zone of the computer where your EWS Managed API is executing, do not specify a time zone when creating the [ExchangeServicehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object.</span></span> 
    
- <span data-ttu-id="462ea-110">すべての日付/時刻のプロパティ (新しい予定や会議の作成時のプロパティも含む) に特定のタイム ゾーンを指定する。この場合は、**ExchangeService** オブジェクトのコンストラクターでタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="462ea-110">To use a specific time zone for all date/time properties, including properties when creating a new appointment or meeting, specify a time zone in the constructor for the **ExchangeService** object.</span></span> 
    
- <span data-ttu-id="462ea-111">[ExchangeService.TimeZone](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) プロパティで指定したものとは別のタイム ゾーンを使用する。この場合は、[Appointment.StartTimeZone](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) プロパティと [Appointment.EndTimeZone](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="462ea-111">To use a different time zone than the one specified in the [ExchangeService.TimeZone](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) property, use the [Appointment.StartTimeZone](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) and [Appointment.EndTimeZone](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) properties.</span></span> 
    
    > [!NOTE]
    > <span data-ttu-id="462ea-112">**EndTimeZone** プロパティは、[ExchangeService.RequestedServerVersion](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) プロパティが **Exchange2010** 以降に設定されている場合にのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="462ea-112">The **EndTimeZone** property is only available when the [ExchangeService.RequestedServerVersion](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) property is set to **Exchange2010** or later.</span></span> <span data-ttu-id="462ea-113">使用できない場合は、**StartTimeZone** を設定して、予定の開始時刻と終了時刻の両方に適用します。</span><span class="sxs-lookup"><span data-stu-id="462ea-113">If it is not available, setting the **StartTimeZone** applies to both the start and end times of the appointment.</span></span> 
  
<span data-ttu-id="462ea-114">次の例では、3 つの予定の作成に EWS マネージ API が使用されています。</span><span class="sxs-lookup"><span data-stu-id="462ea-114">In the following example, the EWS Managed API is used to create three appointments.</span></span> <span data-ttu-id="462ea-115">それぞれの予定は、未指定のタイム ゾーンで現在から 2 日後の 1:00 PM に始まり、その 1 時間後に終わります。</span><span class="sxs-lookup"><span data-stu-id="462ea-115">Each appointment is set to start at 1:00 PM two days from now, in an unspecified time zone, and end one hour later.</span></span> <span data-ttu-id="462ea-116">最初の予定は、既定の EWS マネージ API の動作を使用することで、クライアント コンピューターのタイム ゾーンで作成されます。</span><span class="sxs-lookup"><span data-stu-id="462ea-116">The first appointment is created in the client computer's time zone by using default EWS Managed API behavior.</span></span> <span data-ttu-id="462ea-117">2 番目は、**Appointment.StartTimeZone** と **Appointment.EndTimeZone** プロパティを使用することで、中部標準時で作成されます。</span><span class="sxs-lookup"><span data-stu-id="462ea-117">The second is created in the Central time zone by using the **Appointment.StartTimeZone** and **Appointment.EndTimeZone** properties.</span></span> <span data-ttu-id="462ea-118">3 番目は、**ExchangeService.TimeZone** プロパティを使用することで、山地標準時で作成されます。</span><span class="sxs-lookup"><span data-stu-id="462ea-118">The third is created in the Mountain time zone by using the **ExchangeService.TimeZone** property.</span></span> 
  
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

<span data-ttu-id="462ea-119">この例を東部標準時で構成されているクライアント コンピューターで実行して、それによって作成された予定を東部標準時で構成されているクライアントで表示すると、それぞれの予定が 1:00 PM、2:00 PM、および 3:00 PM に始まるように示されます。</span><span class="sxs-lookup"><span data-stu-id="462ea-119">When this example is executed on a client computer configured in the Eastern time zone, and the three appointments it creates are viewed from a client configured in the Eastern time zone, they appear at 1:00 PM, 2:00 PM, and 3:00 PM, respectively.</span></span>
  
## <a name="creating-appointments-in-different-time-zones-by-using-ews"></a><span data-ttu-id="462ea-120">EWS を使用して異なるタイムゾーンで予定を作成する</span><span class="sxs-lookup"><span data-stu-id="462ea-120">Creating appointments in different time zones by using EWS</span></span>

<span data-ttu-id="462ea-121">EWS を使用して予定または会議を作成するときには、タイム ゾーンを指定するための 3 オプションがあります。</span><span class="sxs-lookup"><span data-stu-id="462ea-121">When creating appointments or meetings using EWS, you have three options for specifying the time zone:</span></span>
  
- <span data-ttu-id="462ea-122">協定世界時 (UTC) を使用する。この場合は、[TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) 要素、[MeetingTimeZone](http://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) 要素 (Exchange 2007 のみ)、または [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) 要素と [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) 要素 (Exchange 2010 以降) を [CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)要求に含めません。</span><span class="sxs-lookup"><span data-stu-id="462ea-122">To use Coordinated Universal Time (UTC), do not include a [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element, [MeetingTimeZone](http://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) element (Exchange 2007 only), or [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) and [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) elements (Exchange 2010 and later) in the [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request.</span></span> 
    
- <span data-ttu-id="462ea-123">すべての日付/時刻のプロパティ (新しい予定や会議の作成時のプロパティも含む) に特定のタイム ゾーンを指定する。この場合は、[CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)要求の [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) 要素でタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="462ea-123">To use a specific time zone for all date/time properties, including properties when creating a new appointment or meeting, specify a time zone in the [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element in the [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request.</span></span> 
    
- <span data-ttu-id="462ea-124">[TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) 要素で指定したものとは別のタイム ゾーンを使用する。この場合は、[TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) 要素、[MeetingTimeZone](http://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) 要素 (Exchange 2007 のみ)、または [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) 要素と [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) 要素 (Exchange 2010 以降) を [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 操作要求に含めません。</span><span class="sxs-lookup"><span data-stu-id="462ea-124">To use a different time zone than the one specified in the [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element, include a [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element, [MeetingTimeZone](http://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) element (Exchange 2007 only), or [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) and [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) elements (Exchange 2010 and later) in the [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request.</span></span> 
    
<span data-ttu-id="462ea-125">次の [CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)要求の例では、UTC を使用して予定を作成します。</span><span class="sxs-lookup"><span data-stu-id="462ea-125">The following example [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request creates an appointment using UTC.</span></span> <span data-ttu-id="462ea-126">**TimeZoneContext** 要素、**StartTimeZone** 要素、**EndTimeZone** 要素が存在しないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="462ea-126">Notice that the **TimeZoneContext** element, the **StartTimeZone** element, and the **EndTimeZone** element are absent.</span></span> <span data-ttu-id="462ea-127">**Start** 要素と **End** 要素の値は UTC で表されます。</span><span class="sxs-lookup"><span data-stu-id="462ea-127">The **Start** and **End** element values are expressed in UTC.</span></span> 
  
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

<span data-ttu-id="462ea-128">次の [CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)要求の例では、**StartTimeZone** 要素と **EndTimeZone** 要素を使用して、予定に中部標準時を指定します。</span><span class="sxs-lookup"><span data-stu-id="462ea-128">The following example [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request uses the **StartTimeZone** and **EndTimeZone** elements to specify the Central time zone for the appointment.</span></span> <span data-ttu-id="462ea-129">**TimeZoneContext** 要素が存在しないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="462ea-129">Notice that the **TimeZoneContext** element is absent.</span></span> <span data-ttu-id="462ea-130">ただし、その要素が存在していたとしても、その値は **StartTimeZone** 要素と **EndTimeZone** 要素の値で上書きされます。</span><span class="sxs-lookup"><span data-stu-id="462ea-130">However, if it were present, the values of the **StartTimeZone** and **EndTimeZone** elements would override its value.</span></span> <span data-ttu-id="462ea-131">この場合も、**Start** 要素と **End** 要素の値は UTC で表されます。</span><span class="sxs-lookup"><span data-stu-id="462ea-131">Again, the **Start** and **End** element values are expressed in UTC.</span></span> 
  
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

<span data-ttu-id="462ea-132">次の [CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)要求の例では、**TimeZoneContext** 要素を山地標準時に設定します。</span><span class="sxs-lookup"><span data-stu-id="462ea-132">The following example [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request sets the **TimeZoneContext** element to the Mountain time zone. Notice that the StartTimeZone and EndTimeZone elements are absent. Again, the Start and End element values are expressed in UTC.</span></span> <span data-ttu-id="462ea-133">**StartTimeZone** 要素と **EndTimeZone**要素が存在しないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="462ea-133">Notice that the **StartTimeZone** and **EndTimeZone** elements are absent.</span></span> <span data-ttu-id="462ea-134">この場合も、**Start** 要素と **End** 要素の値は UTC で表されます。</span><span class="sxs-lookup"><span data-stu-id="462ea-134">Again, the **Start** and **End** element values are expressed in UTC.</span></span> 
  
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

<span data-ttu-id="462ea-135">前述の EWS 要求の例で作成された 3 つの予定を東部標準時で構成されているクライアントで表示すると、それぞれの予定が 1:00 PM、2:00 PM、および 3:00 PM に始まるように示されます。</span><span class="sxs-lookup"><span data-stu-id="462ea-135">When the three appointments created by the previous EWS example requests are viewed from a client configured in the Eastern time zone, they appear at 1:00 PM, 2:00 PM, and 3:00 PM, respectively.</span></span>
  
## 

<span data-ttu-id="462ea-136">特定のタイム ゾーンで予定を作成する方法について理解できました。次は、[既存の予定のタイム ゾーンを更新](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)して別のタイム ゾーンにしてみてください。</span><span class="sxs-lookup"><span data-stu-id="462ea-136">Now that you know how to create appointments in specific time zones, you might want to [update the time zones on existing appointments](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md) to a different one.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="462ea-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="462ea-137">See also</span></span>


- [<span data-ttu-id="462ea-138">Exchange のタイム ゾーンと EWS</span><span class="sxs-lookup"><span data-stu-id="462ea-138">Time zones and EWS in Exchange</span></span>](time-zones-and-ews-in-exchange.md)
    
- [<span data-ttu-id="462ea-139">Exchange の EWS を使用して予定のタイム ゾーンを更新する</span><span class="sxs-lookup"><span data-stu-id="462ea-139">How to: Update the time zone for an appointment by using EWS in Exchange</span></span>](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="462ea-140">Exchange 2013 の EWS を使用して予定と会議を作成する</span><span class="sxs-lookup"><span data-stu-id="462ea-140">How to: Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    


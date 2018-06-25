---
title: Exchange の偽装を使用して予定を追加します。
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78d5e51b-900f-4302-b9a8-fdc9aa4b65a5
description: 偽装を使用して、EWS のマネージ API または EWS を Exchange ユーザーの予定表に予定を追加する方法について説明します。
ms.openlocfilehash: fe737658b88aca66d8b4c2860245db000888ba17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758939"
---
# <a name="add-appointments-by-using-exchange-impersonation"></a><span data-ttu-id="381f8-103">Exchange の偽装を使用して予定を追加します。</span><span class="sxs-lookup"><span data-stu-id="381f8-103">Add appointments by using Exchange impersonation</span></span>

<span data-ttu-id="381f8-104">偽装を使用して、EWS のマネージ API または EWS を Exchange ユーザーの予定表に予定を追加する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="381f8-104">Learn how to use impersonation with the EWS Managed API or EWS in Exchange to add appointments to users' calendars.</span></span>
  
<span data-ttu-id="381f8-105">[ロールが有効な](how-to-configure-impersonation.md) **AppplicationImpersonation**を持つサービス アカウントを使用して Exchange の予定表に予定を挿入するサービス アプリケーションを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="381f8-105">You can create a service application that inserts appointments directly into an Exchange calendar by using a service account that has the **AppplicationImpersonation**[role enabled](how-to-configure-impersonation.md).</span></span> <span data-ttu-id="381f8-106">ユーザーとしてアプリケーションが動作している偽装を使用する場合ユーザーが、Outlook などのクライアントを使用して予定表に予定を追加をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="381f8-106">When you use impersonation, the application is acting as the user; it's as if the user added the appointment to the calendar by using a client such as Outlook.</span></span> 
  
<span data-ttu-id="381f8-107">偽装を使用する場合は、次のことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="381f8-107">When you are using impersonation, keep in mind the following:</span></span>
  
- <span data-ttu-id="381f8-108">[ExchangeService](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx)オブジェクトは、サービス アカウントにバインドしてください。</span><span class="sxs-lookup"><span data-stu-id="381f8-108">Your [ExchangeService](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) object must be bound to the service account.</span></span> <span data-ttu-id="381f8-109">偽装するアカウントごとに[ImpersonatedUserId](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx)プロパティを変更することで複数のアカウントを偽装するように、同一の**ExchangeService**オブジェクトを使用できます。</span><span class="sxs-lookup"><span data-stu-id="381f8-109">You can use the same **ExchangeService** object to impersonate multiple accounts by changing the [ImpersonatedUserId](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) property for each account that you want to impersonate.</span></span> 
    
- <span data-ttu-id="381f8-110">偽装されたアカウントを保存する任意の項目は、1 回のみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="381f8-110">Any item that you save to an impersonated account can only be used once.</span></span> <span data-ttu-id="381f8-111">複数のアカウントで同じ予定を保存する場合は、たとえば、あるアカウントごとの[予定](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="381f8-111">If you want to save the same appointment in multiple accounts, for example, you have to create an [Appointment](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) object for each account.</span></span> 
    
## <a name="prerequisites"></a><span data-ttu-id="381f8-112">前提条件</span><span class="sxs-lookup"><span data-stu-id="381f8-112">Prerequisites</span></span>

<span data-ttu-id="381f8-113">アプリケーションでは、偽装を使用する前に、Exchange サーバーへの接続に使用するアカウントが必要です。</span><span class="sxs-lookup"><span data-stu-id="381f8-113">Your application needs an account to use to connect to the Exchange server before it can use impersonation.</span></span> <span data-ttu-id="381f8-114">アカウントにアクセスすることをアプリケーションの偽装の役割を与えられているアプリケーションのサービス アカウントを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="381f8-114">We suggest that you use a service account for the application that has been granted the Application Impersonation role for the accounts that it will be accessing.</span></span> <span data-ttu-id="381f8-115">詳細については、[偽装を構成する](how-to-configure-impersonation.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="381f8-115">For more information, see [Configure impersonation](how-to-configure-impersonation.md)</span></span>
  
## <a name="add-appointments-by-using-impersonation-with-the-ews-managed-api"></a><span data-ttu-id="381f8-116">EWS マネージ API で偽装を使用して予定を追加する</span><span class="sxs-lookup"><span data-stu-id="381f8-116">Add appointments by using impersonation with the EWS Managed API</span></span>

<span data-ttu-id="381f8-p105">次の例では、1 つ以上の Exchange アカウントの予定表に予定または会議を追加します。メソッドは、次の 3 つのパラメーターを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="381f8-p105">The following example adds an appointment or meeting to the calendar of one or more Exchange accounts. The method takes three parameters.</span></span>
  
-  <span data-ttu-id="381f8-119">_サービス_: サービス アプリケーションのアカウントに Exchange サーバー上の**ExchangeService**オブジェクトにバインドされています。</span><span class="sxs-lookup"><span data-stu-id="381f8-119">_service_ — An **ExchangeService** object bound to the service application's account on the Exchange server.</span></span> 
    
-  <span data-ttu-id="381f8-120">_emailAddresses_ - [System.List](http://msdn.microsoft.com/library/6sh2ey19.aspx)オブジェクトが SMTP 電子メール アドレスの文字列のリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="381f8-120">_emailAddresses_ — A [System.List](http://msdn.microsoft.com/library/6sh2ey19.aspx) object containing a list of SMTP email address strings.</span></span> 
    
-  <span data-ttu-id="381f8-121">_工場出荷時_: **IAppointmentFactory**インターフェイスを実装するオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="381f8-121">_factory_ — An object that implements the **IAppointmentFactory** interface.</span></span> <span data-ttu-id="381f8-122">このインターフェイスは、1 つのメソッドでは、 **GetAppointment**をパラメーターとして**ExchangeService**オブジェクトを受け取り**予定**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="381f8-122">This interface has one method, **GetAppointment** that takes an **ExchangeService** object as a parameter and returns an **Appointment** object.</span></span> <span data-ttu-id="381f8-123">**IAppointmentFactory**インタ フェースが定義されている[IAppointmentFactory インターフェイス](#bk_IAppointmentFactory)です。</span><span class="sxs-lookup"><span data-stu-id="381f8-123">The **IAppointmentFactory** interface is defined [IAppointmentFactory interface](#bk_IAppointmentFactory).</span></span>
    
```cs
private static void CreateAppointments(ExchangeService service, List<string> emailAddresses, IAppointmentFactory factory)
{
  // Loop through the list of email addresses to add the appointment.
  foreach (var emailAddress in emailAddresses)
  {
    Console.WriteLine(string.Format("  Placing appointment in calendar for {0}.", emailAddress));
    // Set the email address of the account to get the appointment.
    service.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, emailAddress);
    // Get the appointment to add.
    Appointment appointment = factory.GetAppointment(service);
    // Save the appointment.
    try
    {
      if (appointment.RequiredAttendees.Count > 0)
      {
        // The appointment has attendees so send them the meeting request.
        appointment.Save(SendInvitationsMode.SendToAllAndSaveCopy);
      }
      else
      {
        // The appointment does not have attendees, so just save to calendar.
        appointment.Save(SendInvitationsMode.SendToNone);
      }
    }
    catch (ServiceResponseException ex)
    {
      Console.WriteLine(string.Format("Could not create appointment for {0}", emailAddress));
      Console.WriteLine(ex.Message);
    }
  }
}
```

<span data-ttu-id="381f8-124">予定を保存するには、出席者が、 [RequiredAttendees](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx)プロパティに追加されているかどうかを決定するコードをチェックします。</span><span class="sxs-lookup"><span data-stu-id="381f8-124">When saving the appointment, the code checks to determine whether any attendees have been added to the [RequiredAttendees](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) property.</span></span> <span data-ttu-id="381f8-125">場合は、 [Appointment.Save](http://msdn.microsoft.com/library/dd635394.aspx)メソッドが[SendToAllAndSaveCopy](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx)の列挙値を持つ、出席者が会議出席依頼の場合は; を受信できるようにそれ以外の場合、 **Appointment.Save**メソッドが[SendToNone](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx)の列挙値の[Appointment.IsMeeting](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx)プロパティを**false**に設定を使用して偽装されたユーザーの予定表に予定が保存されるようです。</span><span class="sxs-lookup"><span data-stu-id="381f8-125">If they have, the [Appointment.Save](http://msdn.microsoft.com/library/dd635394.aspx) method is called with the [SendToAllAndSaveCopy](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) enumeration value so that the attendees receive meeting requests; otherwise, the **Appointment.Save** method is called with the [SendToNone](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) enumeration value so that the appointment is saved into the impersonated user's calendar with the [Appointment.IsMeeting](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) property set to **false**.</span></span>
  
### <a name="iappointmentfactory-interface"></a><span data-ttu-id="381f8-126">IAppointmentFactory インターフェイス</span><span class="sxs-lookup"><span data-stu-id="381f8-126">IAppointmentFactory interface</span></span>
<span data-ttu-id="381f8-127"><a name="bk_IAppointmentFactory"> </a></span><span class="sxs-lookup"><span data-stu-id="381f8-127"></span></span>

<span data-ttu-id="381f8-128">必要なため、新しい**予定**のオブジェクト、偽装されたユーザーの予定表に予定を保存するたびに、 **IAppointmentFactory**インタ フェースは**予定**の各オブジェクトの作成に使用するオブジェクトを抽出します。</span><span class="sxs-lookup"><span data-stu-id="381f8-128">Because you need a new **Appointment** object each time that you want to save an appointment on an impersonated user's calendar, the **IAppointmentFactory** interface abstracts the object used to populate each **Appointment** object.</span></span> <span data-ttu-id="381f8-129">このバージョンは、 **GetAppointment**、 **ExchangeService**オブジェクトをパラメーターとしては、その**ExchangeService**オブジェクトにバインドされている新しい**予定**オブジェクトを取得する 1 つのメソッドを含む単純なインターフェイスです。</span><span class="sxs-lookup"><span data-stu-id="381f8-129">This version is a simple interface that contains only one method, **GetAppointment**, that takes an **ExchangeService** object as a parameter and returns a new **Appointment** object bound to that **ExchangeService** object.</span></span> 
  
```cs
interface IAppointmentFactory
{
  Appointment GetAppointment(ExchangeService service);
}
```

<span data-ttu-id="381f8-130">**AppointmentFactory**クラスの次の例では、簡単な予定を取得する**IAppointmentFactory**インターフェイスの実装では、今から 3 日間が発生したを示します。</span><span class="sxs-lookup"><span data-stu-id="381f8-130">The following **AppointmentFactory** class example shows an implementation of the **IAppointmentFactory** interface that returns a simple appointment that occurs three days from now.</span></span> <span data-ttu-id="381f8-131">コメントを解除する場合、`appointment.RequiredAttendees.Add`ライン、 **GetAppointment**メソッドを返します会議とその行では、開催者として表示されている偽装されたユーザーを含む会議出席依頼が届きますが指定されている電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="381f8-131">If you uncomment the  `appointment.RequiredAttendees.Add` line, the **GetAppointment** method will return a meeting and the email address specified in that line will receive a meeting request with the impersonated user listed as the organizer.</span></span> 
  
```cs
class AppointmentFactory : IAppointmentFactory
{
  public Appointment GetAppointment(ExchangeService service)
  {
    // First create the appointment to add.
    Appointment appointment = new Appointment(service);
    // Set the properties on the appointment.
    appointment.Subject = "Tennis lesson";
    appointment.Body = "Focus on backhand this week.";
    appointment.Start = DateTime.Now.AddDays(3);
    appointment.End = appointment.Start.AddHours(1);
    appointment.Location = "Tennis club";
    // appointment.RequiredAttendees.Add(new Attendee("sonyaf@contoso1000.onmicrosoft.com"));
    return appointment;
  }
}

```

## <a name="add-appointments-by-using-impersonation-with-ews"></a><span data-ttu-id="381f8-132">EWS で偽装を使用して予定を追加する</span><span class="sxs-lookup"><span data-stu-id="381f8-132">Add appointments by using impersonation with EWS</span></span>

<span data-ttu-id="381f8-133">EWS では、予定表の所有者の代わりにカレンダーに項目を追加するのには、偽装を使用するアプリケーションを使用できます。</span><span class="sxs-lookup"><span data-stu-id="381f8-133">EWS enables you application to use impersonation to add items to a calendar on behalf the calendar's owner.</span></span> <span data-ttu-id="381f8-134">次の使用例は、 [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx)操作を使用して、偽装されたアカウントの予定表に予定を追加する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="381f8-134">This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to add an appointment to the calendar of an impersonated account.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>alfred@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
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

<span data-ttu-id="381f8-135">**ExchangeImpersonation**の私たちを偽装しているアカウントを指定するのには SOAP ヘッダー内の追加以外に注意してください、これは、同じ XML 要求が偽装を使用せずに予定を作成するために使用します。</span><span class="sxs-lookup"><span data-stu-id="381f8-135">Note that other than the addition of the **ExchangeImpersonation** element in the SOAP header to specify the account that we are impersonating, this is the same XML request used to create an appointment without using impersonation.</span></span> 
  
<span data-ttu-id="381f8-136">**CreateItem**操作から返される XML 応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="381f8-136">The following example shows the response XML that is returned by the **CreateItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="381f8-137">**アイテム Id**と**変更キー**の属性は、読みやすくするために短縮されます。</span><span class="sxs-lookup"><span data-stu-id="381f8-137">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
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

<span data-ttu-id="381f8-138">繰り返しますが、これは、偽装を使用せず、 **CreateItem**操作を使用するときに返されるのと同じ XML です。</span><span class="sxs-lookup"><span data-stu-id="381f8-138">Again, this is the same XML that is returned when you use the **CreateItem** operation without using impersonation.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="381f8-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="381f8-139">See also</span></span>


- [<span data-ttu-id="381f8-140">Exchange の偽装と EWS</span><span class="sxs-lookup"><span data-stu-id="381f8-140">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
    
- [<span data-ttu-id="381f8-141">ApplicationImpersonation 役割</span><span class="sxs-lookup"><span data-stu-id="381f8-141">ApplicationImpersonation role</span></span>](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)
    
- [<span data-ttu-id="381f8-142">偽装を構成します。</span><span class="sxs-lookup"><span data-stu-id="381f8-142">Configure impersonation</span></span>](how-to-configure-impersonation.md)
    
- [<span data-ttu-id="381f8-143">偽装するアカウントを識別します。</span><span class="sxs-lookup"><span data-stu-id="381f8-143">Identify the account to impersonate</span></span>](how-to-identify-the-account-to-impersonate.md)
    
- [<span data-ttu-id="381f8-144">Exchange 2013 の EWS を使用して予定および会議を作成します。</span><span class="sxs-lookup"><span data-stu-id="381f8-144">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="381f8-145">CreateItem 操作 (予定表アイテム)</span><span class="sxs-lookup"><span data-stu-id="381f8-145">CreateItem operation (calendar item)</span></span>](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx)
    
- [<span data-ttu-id="381f8-146">ExchangeService.ImpersonatedUserId プロパティ</span><span class="sxs-lookup"><span data-stu-id="381f8-146">ExchangeService.ImpersonatedUserId property</span></span>](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx.aspx)
    


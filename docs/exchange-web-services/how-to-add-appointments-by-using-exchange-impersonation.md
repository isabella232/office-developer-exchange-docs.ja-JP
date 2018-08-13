---
title: Exchange の偽装を使用して予定を追加する
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78d5e51b-900f-4302-b9a8-fdc9aa4b65a5
description: Exchange の EWS マネージ API または EWS で偽造を使用し、ユーザーの予定表に予定を追加する方法について説明します。
ms.openlocfilehash: ab10a7d65a5603a84e12d918dd54198927d88b8a
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353456"
---
# <a name="add-appointments-by-using-exchange-impersonation"></a><span data-ttu-id="def28-103">Exchange の偽装を使用して予定を追加する</span><span class="sxs-lookup"><span data-stu-id="def28-103">Add appointments by using Exchange impersonation</span></span>

<span data-ttu-id="def28-104">Exchange の EWS マネージ API または EWS で偽造を使用し、ユーザーの予定表に予定を追加する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="def28-104">Learn how to use impersonation with the EWS Managed API or EWS in Exchange to add appointments to users’ calendars.</span></span>
  
<span data-ttu-id="def28-105">**AppplicationImpersonation** の[役割が有効になっている](how-to-configure-impersonation.md)サービス アカウントを使用して、Exchange の予定表に予定を直接挿入するサービス アプリケーションを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="def28-105">You can create a service application that inserts appointments directly into an Exchange calendar by using a service account that has the AppplicationImpersonation role enabled. When you use impersonation, the application is acting as the user; it’s as if the user added the appointment to the calendar by using a client such as Outlook.</span></span> <span data-ttu-id="def28-106">偽装を使用すると、アプリケーションがユーザーとして動作し、ユーザーが Outlook などのクライアントを使用して予定表に予定を追加するかのように動作します。</span><span class="sxs-lookup"><span data-stu-id="def28-106">You can create a service application that inserts appointments directly into an Exchange calendar by using a service account that has the AppplicationImpersonationrole enabled. When you use impersonation, the application is acting as the user; it’s as if the user added the appointment to the calendar by using a client such as Outlook.</span></span> 
  
<span data-ttu-id="def28-107">偽装を使用する場合は、次のことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="def28-107">When you are using impersonation, keep in mind the following:</span></span>
  
- <span data-ttu-id="def28-108">[ExchangeService](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) オブジェクトは、サービス アカウントにバインドする必要があります。</span><span class="sxs-lookup"><span data-stu-id="def28-108">Your [ExchangeService](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) object must be bound to the service account.</span></span> <span data-ttu-id="def28-109">同じ **ExchangeService** オブジェクトを使用して、複数のアカウントを偽装できます。その場合、偽装する各アカウント用に [ImpersonatedUserId](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) プロパティを変更します。</span><span class="sxs-lookup"><span data-stu-id="def28-109">Your   ExchangeService http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx  object must be bound to the service account. You can use the same ExchangeService object to impersonate multiple accounts by changing the  ImpersonatedUserId http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx  property for each account that you want to impersonate.</span></span> 
    
- <span data-ttu-id="def28-110">偽装されたアカウントに保存するアイテムは、1 回のみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="def28-110">Any item that you save to an impersonated account can only be used once.</span></span> <span data-ttu-id="def28-111">たとえば、複数のアカウントで同じ予定を保存する場合は、アカウントごとに[予定](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx)オブジェクトを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="def28-111">Any item that you save to an impersonated account can only be used once. If you want to save the same appointment in multiple accounts, for example, you have to create an [Appointmenthttp://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) object for each account.</span></span> 
    
## <a name="prerequisites"></a><span data-ttu-id="def28-112">前提条件</span><span class="sxs-lookup"><span data-stu-id="def28-112">Prerequisites</span></span>

<span data-ttu-id="def28-113">アプリケーションでは、偽装を使用する前に、Exchange サーバーへの接続に使用するアカウントが必要です。</span><span class="sxs-lookup"><span data-stu-id="def28-113">Your application needs an account to use to connect to the Exchange server before it can use impersonation.</span></span> <span data-ttu-id="def28-114">アクセスするアカウントのアプリケーション偽装の役割が付与されているアプリケーションのサービス アカウントを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="def28-114">Your application needs an account to use to connect to the Exchange server before it can use impersonation. We suggest that you use a service account for the application that has been granted the Application Impersonation role for the accounts that it will be accessing. For more information, see How to: Configure impersonation.</span></span> <span data-ttu-id="def28-115">詳細については、「[偽装を構成する](how-to-configure-impersonation.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="def28-115">For more information, see [Configure impersonation](how-to-configure-impersonation.md)</span></span>
  
## <a name="add-appointments-by-using-impersonation-with-the-ews-managed-api"></a><span data-ttu-id="def28-116">EWS マネージ API で偽装を使用して予定を追加する</span><span class="sxs-lookup"><span data-stu-id="def28-116">Add appointments by using impersonation with the EWS Managed API</span></span>

<span data-ttu-id="def28-p105">次の例では、1 つ以上の Exchange アカウントの予定表に予定または会議を追加します。この方法では、 3 つのパラメーターが必要です。</span><span class="sxs-lookup"><span data-stu-id="def28-p105">The following example adds an appointment or meeting to the calendar of one or more Exchange accounts. The method takes three parameters.</span></span>
  
-  <span data-ttu-id="def28-119">_service_ — Exchange Server のサービス アプリケーションのアカウントにバインドされる **ExchangeService** オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="def28-119">_service_ — An **ExchangeService** object bound to the service application’s account on the Exchange server.</span></span> 
    
-  <span data-ttu-id="def28-120">_emailAddresses_ — SMTP メール アドレスの文字列のリストを含む [System.List](http://msdn.microsoft.com/library/6sh2ey19.aspx) オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="def28-120">_emailAddresses_ — A [System.Listhttp://msdn.microsoft.com/library/6sh2ey19.aspx](http://msdn.microsoft.com/library/6sh2ey19.aspx) object containing a list of SMTP email address strings.</span></span> 
    
-  <span data-ttu-id="def28-121">_factory_ — **IAppointmentFactory** インターフェイスを実装するオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="def28-121">_factory_ — An object that implements the **IAppointmentFactory** interface.</span></span> <span data-ttu-id="def28-122">このインターフェイスには、**ExchangeService** オブジェクトをパラメータとして使用する **GetAppointment** という方法があり、**予定**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="def28-122">factory — An object that implements the **IAppointmentFactory** interface. This interface has one method, **GetAppointment** that takes an **ExchangeService** object as a parameter and returns an Appointment object. The IAppointmentFactory interface is defined below.</span></span> <span data-ttu-id="def28-123">**IAppointmentFactory** のインターフェイスは、[IAppointmentFactory インターフェイス](#bk_IAppointmentFactory)と定義されます。</span><span class="sxs-lookup"><span data-stu-id="def28-123">The **IAppointmentFactory** interface is defined [IAppointmentFactory interface](#bk_IAppointmentFactory).</span></span>
    
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

<span data-ttu-id="def28-124">予定を保存するときに、コードは、出席者が [RequiredAttendees](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) プロパティに追加されているかどうかを判断するための確認を行います。</span><span class="sxs-lookup"><span data-stu-id="def28-124">When saving the appointment, the code checks to determine whether any attendees have been added to the [RequiredAttendees](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) property.</span></span> <span data-ttu-id="def28-125">追加されている場合は、[SendToAllAndSaveCopy](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) 列挙値を指定して [Appointment.Save](http://msdn.microsoft.com/library/dd635394.aspx) メソッドが呼び出され、出席者は会議出席依頼を受信します。それ以外の場合、[SendToNone](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) 列挙値を指定して **Appointment.Save** メソッドが呼び出され、[Appointment.IsMeeting](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) プロパティが **false** に設定されて偽装されたユーザーの予定表に予定が保存されます。</span><span class="sxs-lookup"><span data-stu-id="def28-125">If they have, the [Appointment.Save](http://msdn.microsoft.com/library/dd635394.aspx) method is called with the [SendToAllAndSaveCopy](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) enumeration value so that the attendees receive meeting requests; otherwise, the **Appointment.Save** method is called with the [SendToNone](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) enumeration value so that the appointment is saved into the impersonated user's calendar with the [Appointment.IsMeeting](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) property set to **false**.</span></span>
  
### <a name="iappointmentfactory-interface"></a><span data-ttu-id="def28-126">IAppointmentFactory インターフェイス</span><span class="sxs-lookup"><span data-stu-id="def28-126">IAppointmentFactory interface</span></span>
<span data-ttu-id="def28-127"><a name="bk_IAppointmentFactory"> </a></span><span class="sxs-lookup"><span data-stu-id="def28-127"></span></span>

<span data-ttu-id="def28-128">偽装されたユーザーの予定表に予定を保存する場合は毎回新しい**予定**オブジェクトが必要なため、 **IAppointmentFactory** インターフェイスはそれぞれの**予定**オブジェクトの設定に使用されるオブジェクトを抽象化します。</span><span class="sxs-lookup"><span data-stu-id="def28-128">Because you need a new **Appointment** object each time that you want to save an appointment on an impersonated user’s calendar, the **IAppointmentFactory** interface abstracts the object used to populate each **Appointment** object. This version is a simple interface that contains only one method, GetAppointment, that takes an ExchangeService object as a parameter and returns a new Appointment object bound to that ExchangeService object.</span></span> <span data-ttu-id="def28-129">このバージョンは、**ExchangeService** オブジェクトをパラメータに使い、その **ExchangeService** オブジェクトにバインドされている新しい**予定**オブジェクトを返す、**GetAppointment** メソッド のみを含む単純なインターフェイスです。</span><span class="sxs-lookup"><span data-stu-id="def28-129">Because you need a new **Appointment** object each time that you want to save an appointment on an impersonated user’s calendar, the **IAppointmentFactory** interface abstracts the object used to populate each **Appointment** object. This version is a simple interface that contains only one method, **GetAppointment**, that takes an ExchangeService object as a parameter and returns a new Appointment object bound to that ExchangeService object.</span></span> 
  
```cs
interface IAppointmentFactory
{
  Appointment GetAppointment(ExchangeService service);
}
```

<span data-ttu-id="def28-130">次の **AppointmentFactory** クラスの例は、今から 3 日の間に発生する単純な予定を返す **IAppointmentFactory** インターフェイスの実装を示しています。</span><span class="sxs-lookup"><span data-stu-id="def28-130">The following **AppointmentFactory** class example shows an implementation of the **IAppointmentFactory** interface that returns a simple appointment that occurs three days from now.</span></span> <span data-ttu-id="def28-131">`appointment.RequiredAttendees.Add` 行のコメントを解除すると、**GetAppointment** メソッドは会議を返し、その行に指定されたメール アドレスに、偽装されたユーザーを開催者とする会議出席依頼が届きます。</span><span class="sxs-lookup"><span data-stu-id="def28-131">The following **AppointmentFactory** class example shows an implementation of the IAppointmentFactory interface that returns a simple appointment that occurs three days from now. If you uncomment the appointment.RequiredAttendees.Add`appointment.RequiredAttendees.Add` line, the GetAppointment method will return a meeting and the email address specified in that line will receive a meeting request with the impersonated user listed as the organizer.</span></span> 
  
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

## <a name="add-appointments-by-using-impersonation-with-ews"></a><span data-ttu-id="def28-132">EWS で偽装を使用して予定を追加する</span><span class="sxs-lookup"><span data-stu-id="def28-132">Add appointments by using impersonation with EWS</span></span>

<span data-ttu-id="def28-133">EWS では、予定表の所有者の代わりにアプリケーションでカレンダーにアイテムを追加するために偽装を使用できます。</span><span class="sxs-lookup"><span data-stu-id="def28-133">EWS enables you application to use impersonation to add items to a calendar on behalf the calendar's owner.</span></span> <span data-ttu-id="def28-134">次の例は、[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) 操作を使用して、偽装されたアカウントの予定表に予定を追加する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="def28-134">EWS enables you application to use impersonation to add items to a calendar on behalf the calendar’s owner. This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to add an appointment to the calendar of an impersonated account.</span></span> 
  
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

<span data-ttu-id="def28-135">偽装しているアカウントを指定するための SOAP ヘッダーの **ExchangeImpersonation** 要素の追加以外は、偽装を使用しないで予定を作成するための XML 要求と同じものを使用します。</span><span class="sxs-lookup"><span data-stu-id="def28-135">Note that other than the addition of the **ExchangeImpersonation** element in the SOAP header to specify the account that we are impersonating, this is the same XML request used to create an appointment without using impersonation.</span></span> 
  
<span data-ttu-id="def28-136">次の例は、**CreateItem** 操作で返される応答 XML を表しています。</span><span class="sxs-lookup"><span data-stu-id="def28-136">The following example shows the response XML that is returned by the **CreateItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="def28-137">**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="def28-137">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
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

<span data-ttu-id="def28-138">この場合も、偽装を使用せずに **CreateItem** 操作をするときに戻される XML と同じものが使用されます。</span><span class="sxs-lookup"><span data-stu-id="def28-138">Again, this is the same XML that is returned when you use the **CreateItem** operation without using impersonation.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="def28-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="def28-139">See also</span></span>


- [<span data-ttu-id="def28-140">Exchange の偽装と EWS</span><span class="sxs-lookup"><span data-stu-id="def28-140">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
    
- [<span data-ttu-id="def28-141">ApplicationImpersonation 役割</span><span class="sxs-lookup"><span data-stu-id="def28-141">ApplicationImpersonation role</span></span>](http://technet.microsoft.com/ja-JP/library/dd776119%28v=exchg.150%29.aspx)
    
- [<span data-ttu-id="def28-142">偽装を構成する</span><span class="sxs-lookup"><span data-stu-id="def28-142">Configure impersonation</span></span>](how-to-configure-impersonation.md)
    
- [<span data-ttu-id="def28-143">偽装するアカウントを識別する</span><span class="sxs-lookup"><span data-stu-id="def28-143">Identify the account to impersonate</span></span>](how-to-identify-the-account-to-impersonate.md)
    
- [<span data-ttu-id="def28-144">Exchange 2013 の EWS を使用して予定と会議を作成する</span><span class="sxs-lookup"><span data-stu-id="def28-144">How to: Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="def28-145">CreateItem 操作 (予定表アイテム)</span><span class="sxs-lookup"><span data-stu-id="def28-145">CreateItem operation (calendar item)</span></span>](../web-service-reference/createitem-operation-calendar-item.md)
    
- <span data-ttu-id="def28-146">
  [ExchangeService.ImpersonatedUserId プロパティ](https://docs.microsoft.com/en-us/dotnet/api/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid?view=exchange-ews-api)</span><span class="sxs-lookup"><span data-stu-id="def28-146">[ExchangeService.ImpersonatedUserId property](https://docs.microsoft.com/en-us/dotnet/api/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid?view=exchange-ews-api)</span></span>
    


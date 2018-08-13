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
# <a name="add-appointments-by-using-exchange-impersonation"></a>Exchange の偽装を使用して予定を追加する

Exchange の EWS マネージ API または EWS で偽造を使用し、ユーザーの予定表に予定を追加する方法について説明します。
  
**AppplicationImpersonation** の[役割が有効になっている](how-to-configure-impersonation.md)サービス アカウントを使用して、Exchange の予定表に予定を直接挿入するサービス アプリケーションを作成することができます。 偽装を使用すると、アプリケーションがユーザーとして動作し、ユーザーが Outlook などのクライアントを使用して予定表に予定を追加するかのように動作します。 
  
偽装を使用する場合は、次のことに注意してください。
  
- [ExchangeService](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) オブジェクトは、サービス アカウントにバインドする必要があります。 同じ **ExchangeService** オブジェクトを使用して、複数のアカウントを偽装できます。その場合、偽装する各アカウント用に [ImpersonatedUserId](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) プロパティを変更します。 
    
- 偽装されたアカウントに保存するアイテムは、1 回のみ使用できます。 たとえば、複数のアカウントで同じ予定を保存する場合は、アカウントごとに[予定](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx)オブジェクトを作成する必要があります。 
    
## <a name="prerequisites"></a>前提条件

アプリケーションでは、偽装を使用する前に、Exchange サーバーへの接続に使用するアカウントが必要です。 アクセスするアカウントのアプリケーション偽装の役割が付与されているアプリケーションのサービス アカウントを使用することをお勧めします。 詳細については、「[偽装を構成する](how-to-configure-impersonation.md)」を参照してください。
  
## <a name="add-appointments-by-using-impersonation-with-the-ews-managed-api"></a>EWS マネージ API で偽装を使用して予定を追加する

次の例では、1 つ以上の Exchange アカウントの予定表に予定または会議を追加します。この方法では、 3 つのパラメーターが必要です。
  
-  _service_ — Exchange Server のサービス アプリケーションのアカウントにバインドされる **ExchangeService** オブジェクト。 
    
-  _emailAddresses_ — SMTP メール アドレスの文字列のリストを含む [System.List](http://msdn.microsoft.com/library/6sh2ey19.aspx) オブジェクト。 
    
-  _factory_ — **IAppointmentFactory** インターフェイスを実装するオブジェクト。 このインターフェイスには、**ExchangeService** オブジェクトをパラメータとして使用する **GetAppointment** という方法があり、**予定**オブジェクトを返します。 **IAppointmentFactory** のインターフェイスは、[IAppointmentFactory インターフェイス](#bk_IAppointmentFactory)と定義されます。
    
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

予定を保存するときに、コードは、出席者が [RequiredAttendees](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) プロパティに追加されているかどうかを判断するための確認を行います。 追加されている場合は、[SendToAllAndSaveCopy](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) 列挙値を指定して [Appointment.Save](http://msdn.microsoft.com/library/dd635394.aspx) メソッドが呼び出され、出席者は会議出席依頼を受信します。それ以外の場合、[SendToNone](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) 列挙値を指定して **Appointment.Save** メソッドが呼び出され、[Appointment.IsMeeting](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) プロパティが **false** に設定されて偽装されたユーザーの予定表に予定が保存されます。
  
### <a name="iappointmentfactory-interface"></a>IAppointmentFactory インターフェイス
<a name="bk_IAppointmentFactory"> </a>

偽装されたユーザーの予定表に予定を保存する場合は毎回新しい**予定**オブジェクトが必要なため、 **IAppointmentFactory** インターフェイスはそれぞれの**予定**オブジェクトの設定に使用されるオブジェクトを抽象化します。 このバージョンは、**ExchangeService** オブジェクトをパラメータに使い、その **ExchangeService** オブジェクトにバインドされている新しい**予定**オブジェクトを返す、**GetAppointment** メソッド のみを含む単純なインターフェイスです。 
  
```cs
interface IAppointmentFactory
{
  Appointment GetAppointment(ExchangeService service);
}
```

次の **AppointmentFactory** クラスの例は、今から 3 日の間に発生する単純な予定を返す **IAppointmentFactory** インターフェイスの実装を示しています。 `appointment.RequiredAttendees.Add` 行のコメントを解除すると、**GetAppointment** メソッドは会議を返し、その行に指定されたメール アドレスに、偽装されたユーザーを開催者とする会議出席依頼が届きます。 
  
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

## <a name="add-appointments-by-using-impersonation-with-ews"></a>EWS で偽装を使用して予定を追加する

EWS では、予定表の所有者の代わりにアプリケーションでカレンダーにアイテムを追加するために偽装を使用できます。 次の例は、[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) 操作を使用して、偽装されたアカウントの予定表に予定を追加する方法を示します。 
  
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

偽装しているアカウントを指定するための SOAP ヘッダーの **ExchangeImpersonation** 要素の追加以外は、偽装を使用しないで予定を作成するための XML 要求と同じものを使用します。 
  
次の例は、**CreateItem** 操作で返される応答 XML を表しています。 
  
> [!NOTE]
> **ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。 
  
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

この場合も、偽装を使用せずに **CreateItem** 操作をするときに戻される XML と同じものが使用されます。 
  
## <a name="see-also"></a>関連項目


- [Exchange の偽装と EWS](impersonation-and-ews-in-exchange.md)
    
- [ApplicationImpersonation 役割](http://technet.microsoft.com/ja-JP/library/dd776119%28v=exchg.150%29.aspx)
    
- [偽装を構成する](how-to-configure-impersonation.md)
    
- [偽装するアカウントを識別する](how-to-identify-the-account-to-impersonate.md)
    
- [Exchange 2013 の EWS を使用して予定と会議を作成する](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [CreateItem 操作 (予定表アイテム)](../web-service-reference/createitem-operation-calendar-item.md)
    
- 
  [ExchangeService.ImpersonatedUserId プロパティ](https://docs.microsoft.com/en-us/dotnet/api/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid?view=exchange-ews-api)
    


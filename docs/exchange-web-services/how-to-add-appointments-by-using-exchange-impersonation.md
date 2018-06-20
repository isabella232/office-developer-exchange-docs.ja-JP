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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758939"
---
# <a name="add-appointments-by-using-exchange-impersonation"></a>Exchange の偽装を使用して予定を追加します。

偽装を使用して、EWS のマネージ API または EWS を Exchange ユーザーの予定表に予定を追加する方法について説明します。
  
[ロールが有効な](how-to-configure-impersonation.md) **AppplicationImpersonation**を持つサービス アカウントを使用して Exchange の予定表に予定を挿入するサービス アプリケーションを作成することができます。 ユーザーとしてアプリケーションが動作している偽装を使用する場合ユーザーが、Outlook などのクライアントを使用して予定表に予定を追加をお勧めします。 
  
偽装を使用する場合は、次のことに注意してください。
  
- [ExchangeService](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx)オブジェクトは、サービス アカウントにバインドしてください。 偽装するアカウントごとに[ImpersonatedUserId](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx)プロパティを変更することで複数のアカウントを偽装するように、同一の**ExchangeService**オブジェクトを使用できます。 
    
- 偽装されたアカウントを保存する任意の項目は、1 回のみ使用できます。 複数のアカウントで同じ予定を保存する場合は、たとえば、あるアカウントごとの[予定](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx)オブジェクトを作成します。 
    
## <a name="prerequisites"></a>前提条件

アプリケーションでは、偽装を使用する前に、Exchange サーバーへの接続に使用するアカウントが必要です。 アカウントにアクセスすることをアプリケーションの偽装の役割を与えられているアプリケーションのサービス アカウントを使用することをお勧めします。 詳細については、[偽装を構成する](how-to-configure-impersonation.md)を参照してください。
  
## <a name="add-appointments-by-using-impersonation-with-the-ews-managed-api"></a>EWS マネージ API で偽装を使用して予定を追加する

次の例では、1 つ以上の Exchange アカウントの予定表に予定または会議を追加します。メソッドは、次の 3 つのパラメーターを受け取ります。
  
-  _サービス_: サービス アプリケーションのアカウントに Exchange サーバー上の**ExchangeService**オブジェクトにバインドされています。 
    
-  _emailAddresses_ - [System.List](http://msdn.microsoft.com/library/6sh2ey19.aspx)オブジェクトが SMTP 電子メール アドレスの文字列のリストが含まれています。 
    
-  _工場出荷時_: **IAppointmentFactory**インターフェイスを実装するオブジェクトです。 このインターフェイスは、1 つのメソッドでは、 **GetAppointment**をパラメーターとして**ExchangeService**オブジェクトを受け取り**予定**オブジェクトを返します。 **IAppointmentFactory**インタ フェースが定義されている[IAppointmentFactory インターフェイス](#bk_IAppointmentFactory)です。
    
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

予定を保存するには、出席者が、 [RequiredAttendees](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx)プロパティに追加されているかどうかを決定するコードをチェックします。 場合は、 [Appointment.Save](http://msdn.microsoft.com/library/dd635394.aspx)メソッドが[SendToAllAndSaveCopy](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx)の列挙値を持つ、出席者が会議出席依頼の場合は; を受信できるようにそれ以外の場合、 **Appointment.Save**メソッドが[SendToNone](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx)の列挙値の[Appointment.IsMeeting](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx)プロパティを**false**に設定を使用して偽装されたユーザーの予定表に予定が保存されるようです。
  
### <a name="iappointmentfactory-interface"></a>IAppointmentFactory インターフェイス
<a name="bk_IAppointmentFactory"> </a>

必要なため、新しい**予定**のオブジェクト、偽装されたユーザーの予定表に予定を保存するたびに、 **IAppointmentFactory**インタ フェースは**予定**の各オブジェクトの作成に使用するオブジェクトを抽出します。 このバージョンは、 **GetAppointment**、 **ExchangeService**オブジェクトをパラメーターとしては、その**ExchangeService**オブジェクトにバインドされている新しい**予定**オブジェクトを取得する 1 つのメソッドを含む単純なインターフェイスです。 
  
```cs
interface IAppointmentFactory
{
  Appointment GetAppointment(ExchangeService service);
}
```

**AppointmentFactory**クラスの次の例では、簡単な予定を取得する**IAppointmentFactory**インターフェイスの実装では、今から 3 日間が発生したを示します。 コメントを解除する場合、`appointment.RequiredAttendees.Add`ライン、 **GetAppointment**メソッドを返します会議とその行では、開催者として表示されている偽装されたユーザーを含む会議出席依頼が届きますが指定されている電子メール アドレスです。 
  
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

EWS では、予定表の所有者の代わりにカレンダーに項目を追加するのには、偽装を使用するアプリケーションを使用できます。 次の使用例は、 [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx)操作を使用して、偽装されたアカウントの予定表に予定を追加する方法を示しています。 
  
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

**ExchangeImpersonation**の私たちを偽装しているアカウントを指定するのには SOAP ヘッダー内の追加以外に注意してください、これは、同じ XML 要求が偽装を使用せずに予定を作成するために使用します。 
  
**CreateItem**操作から返される XML 応答の例を次に示します。 
  
> [!NOTE]
> **アイテム Id**と**変更キー**の属性は、読みやすくするために短縮されます。 
  
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

繰り返しますが、これは、偽装を使用せず、 **CreateItem**操作を使用するときに返されるのと同じ XML です。 
  
## <a name="see-also"></a>関連項目


- [Exchange の偽装と EWS](impersonation-and-ews-in-exchange.md)
    
- [ApplicationImpersonation 役割](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)
    
- [偽装を構成します。](how-to-configure-impersonation.md)
    
- [偽装するアカウントを識別します。](how-to-identify-the-account-to-impersonate.md)
    
- [Exchange 2013 の EWS を使用して予定および会議を作成します。](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [CreateItem 操作 (予定表アイテム)](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx)
    
- [ExchangeService.ImpersonatedUserId プロパティ](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx.aspx)
    


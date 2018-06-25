---
title: Exchange から自動検出を使用してユーザー設定を取得します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 6d90c305-4802-4e18-8d52-f60349feaa8d
description: 自動検出を使用して Exchange サーバーからユーザー構成設定を取得する方法について説明します。
ms.openlocfilehash: f37de55d6681bcdef381561b166adf209d3919a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758956"
---
# <a name="get-user-settings-from-exchange-by-using-autodiscover"></a>Exchange から自動検出を使用してユーザー設定を取得します。

自動検出を使用して Exchange サーバーからユーザー構成設定を取得する方法について説明します。
  
自動検出では、ユーザーの電子メール アドレスとパスワードだけを使用してユーザーの構成情報に簡単にアクセスを提供することによってアプリケーションの構成が簡略化されます。 [ユーザーの構成設定の数](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx)は、自動検出では、ユーザーの表示名または外部の web サービスの URL などです。 
  
自動検出サービスからユーザーの設定を取得するために、次の開発テクノロジのうちのいずれかを使用できます。
  
- [EWS のマネージ API のクライアント アプリケーションを開始](get-started-with-ews-managed-api-client-applications.md)する
    
- [Web サービスの SOAP の自動検出](http://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx)
    
- [POX の自動検出 web サービス](http://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx)
    
EWS のマネージ API は、ユーザー設定を取得するためのオブジェクト ベースのインタ フェースを提供します。 クライアント アプリケーションは、マネージ コードを使用する場合は、EWS のマネージ API を使用することをお勧めします。 EWS のマネージ API を使用する場合は、必要な設定は[Microsoft.Exchange.WebServices.Autodiscover.UserSettingName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=EXCHG.80%29.aspx)列挙体で使用できるかどうかを決定します。 、されていない場合は、SOAP または POX の自動検出サービスを使用します。 
  
Web サービスを使用する場合お勧め、SOAP の自動検出サービスを使用すること POX の自動検出サービスよりも豊富な機能をサポートしているためです。 SOAP の自動検出サービスを使用できない場合の代替として最適では POX の自動検出サービスです。
  
## <a name="set-up-to-get-user-settings"></a>ユーザー設定を取得するように設定する
<a name="bk_Prereq"> </a>

自動検出サービスを使用してユーザー設定を取得する前に、次のものを使用しているか確認してください。
  
- EWS マネージ API または POX ベースの自動検出サービス、Exchange Online 、Office 365 の一部としての Exchange Online、または Exchange 2007 SP1 以降のバージョンの Exchange を実行しているサーバーを使用しているか。  
    
- SOAP ベースの自動検出サービス、Exchange Online、または Exchange 2010 以降のバージョンの Exchange を使用しているか。
    
> [!NOTE]
> EWS のマネージ API を使用する場合は、いくつかの状況での[証明書検証のコールバック メソッドを提供](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)する必要があります。 証明書検証コールバック メソッドによって生成されたプロキシのライブラリ、Visual Studio によって作成されたものなどをする必要もあります。 
  
## <a name="get-user-settings-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してユーザー設定を取得する
<a name="bk_Managed"> </a>

次の例のように、ユーザーの構成情報を取得するために[GetUserSettings](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx)メソッドを使用できます。 この例では、(から[UserSettingName](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.autodiscover.usersettingname%28v=exchg.80%29.aspx)列挙に含まれる) を取得するユーザー設定の配列を指定することができ、メソッドは、Exchange サーバーからリダイレクト応答に従います。 
  
```cs
using System;
using System.Net;
using Microsoft.Exchange.WebServices.Autodiscover;
public static GetUserSettingsResponse GetUserSettings(
    AutodiscoverService service,
    string emailAddress,
    int maxHops,
    params UserSettingName[] settings)
{
    Uri url = null;
    GetUserSettingsResponse response = null;
    for (int attempt = 0; attempt < maxHops; attempt++)
    {
        service.Url = url;
        service.EnableScpLookup = (attempt < 2);
        response = service.GetUserSettings(emailAddress, settings);
        if (response.ErrorCode == AutodiscoverErrorCode.RedirectAddress)
        {
            url = new Uri(response.RedirectTarget);
        }
        else if (response.ErrorCode == AutodiscoverErrorCode.RedirectUrl)
        {
            url = new Uri(response.RedirectTarget);
        }
        else
        {
            return response;
        }
    }
    throw new Exception("No suitable Autodiscover endpoint was found.");
}
```

ユーザー設定の配列の各キー/値ペアにアクセスするために返されるコレクションを解析することができます。次の使用例は、返された各要素を解析し、各キー/値ペアの名前と値を表示する方法を示しています。
  
```cs
// Display each retrieved value. The settings are part of a key/value pair.
// userresponse is a GetUserSettingsResonse object.
foreach (KeyValuePair<UserSettingName, Object> usersetting in userresponse.Settings)
{
    Console.WriteLine(usersetting.Key.ToString() + ": " + usersetting.Value);
}
```

または、特定の設定の値を取得できます。 次の例では、 **UserDisplayName**の設定、表示されます。 
  
```cs
// Display a specific setting, such as UserDisplayName.
Console.WriteLine(userresponse.Settings[UserSettingName.UserDisplayName]);
```

## <a name="get-user-settings-by-using-soap-autodiscover"></a>SOAP 自動検出を使用してユーザー設定を取得する
<a name="bk_SOAP"> </a>

EWS マネージ API を使用していない場合は、SOAP の自動検出 Web サービスを使用することをお勧めします。SOAP の自動検出 Web サービスが失敗した、または利用できない場合にのみ、POX 自動検出 Web サービスを使用します。  
  
ユーザー設定を取得するには、 [GetUserSettings 操作 (SOAP)](http://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx)を使用します。 要求された設定は、 [UserSetting の要素](http://msdn.microsoft.com/library/aac6dc31-edd2-49d7-b845-1df4d77da58c%28Office.15%29.aspx)として返されます。
  
次の例では、サーバーからユーザー設定を取得する SOAP 自動検出要求を示しています。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>mara@contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>UserDisplayName</a:Setting>
          <a:Setting>UserDN</a:Setting>
          <a:Setting>UserDeploymentId</a:Setting>
          <a:Setting>InternalMailboxServer</a:Setting>
          <a:Setting>MailboxDN</a:Setting>
          <a:Setting>PublicFolderServer</a:Setting>
          <a:Setting>ActiveDirectoryServer</a:Setting>
          <a:Setting>ExternalMailboxServer</a:Setting>
          <a:Setting>EcpDeliveryReportUrlFragment</a:Setting>
          <a:Setting>EcpPublishingUrlFragment</a:Setting>
          <a:Setting>EcpTextMessagingUrlFragment</a:Setting>
          <a:Setting>ExternalEwsUrl</a:Setting>
          <a:Setting>CasVersion</a:Setting>
          <a:Setting>EwsSupportedSchemas</a:Setting>
          <a:Setting>GroupingInformation</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>
```

次の例では、クライアントからの要求を解析した後に、サーバーによって返される SOAP 応答を示します。応答には、要求される設定のみが含まれます (存在する場合)。
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>160</h:MajorBuildNumber>
      <h:MinorBuildNumber>4</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>NoError</ErrorCode>
            <ErrorMessage>No error.</ErrorMessage>
            <RedirectTarget i:nil="true" />
            <UserSettingErrors />
            <UserSettings>
              <UserSetting i:type="StringSetting">
                <Name>UserDisplayName</Name>
                <Value>Mara Whitley</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>UserDN</Name>
                <Value>/o=microsoft/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=mara</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>UserDeploymentId</Name>
                <Value>649d50b8-a1ce-4bac-8ace-2321   e463f701</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>CasVersion</Name>
                <Value>15.01.0160.004</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>EwsSupportedSchemas</Name>
                <Value>Exchange2007, Exchange2007_SP1, Exchange2010, Exchange2010_SP1, Exchange2010_SP2, Exchange2013</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>InternalMailboxServer</Name>
                <Value>mail.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ActiveDirectoryServer</Name>
                <Value>dc.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>MailboxDN</Name>
                <Value>/o=microsoft/ou=Exchange Administrative Group 
                  (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=mail.contoso.com/cn=Contoso Private MDB</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>PublicFolderServer</Name>
                <Value>public.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>EcpDeliveryReportUrlFragment</Name>
                <Value>PersonalSettings/DeliveryReport.aspx?exsvurl=1&amp;amp;IsOWA=&amp;lt;IsOWA&amp;gt;&amp;amp;MsgID=&amp;lt;MsgID&amp;gt;&amp;amp;Mbx=&amp;lt;Mbx&amp;gt;</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>EcpTextMessagingUrlFragment</Name>
                <Value>?p=sms/textmessaging.slab&amp;amp;exsvurl=1</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>EcpPublishingUrlFragment</Name>
                <Value>customize/calendarpublishing.slab?exsvurl=1&amp;amp;FldID=&amp;lt;FldID&amp;gt;</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ExternalEwsUrl</Name>
                <Value>https://mail.contoso.com/EWS/Exchange.asmx</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ExternalMailboxServer</Name>
                <Value>mail.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>GroupingInformation</Name>
                <Value>CONTOSO-1</Value>
              </UserSetting>
            </UserSettings>
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope
```

## <a name="get-user-settings-by-using-pox-autodiscover"></a>POX 自動検出を使用してユーザー設定を取得する
<a name="bk_POX"> </a>

SOAP の自動検出 web サービスを使用することをお勧めします、POX の自動検出 web サービスは SOAP が使用できない場合のための適切なバックアップ オプション。 POX の自動検出 web サービスを使用する Exchange 2007 を対象とする場合があるので、2007 は、SOAP の自動検出 web サービスをサポートしていないを交換します。 SOAP の自動検出 web サービスとは異なり POX の自動検出サービスはできません固有の設定を要求します。 代わりに、サーバーは、すべての[プロトコル要素](http://msdn.microsoft.com/library/f77e4d66-6fdd-4999-9339-f7d7f9c86f44%28Office.15%29.aspx)の子要素として使用可能な設定の一覧を返します。
  
次の例では、サーバーからユーザー設定を取得する SOAP の自動検出要求を示しています。次の XML は、HTTP POST 経由でサーバーに送信されます。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>mara@contoso.com</EMailAddress>
    <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

次の例は、サーバーに返される POX の応答を示しています。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <User>
      <DisplayName>Mara Whitley</DisplayName>
      <LegacyDN>/o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=f5eeabead90d4b6fb51d6379474692cd-Mara</LegacyDN>
      <AutoDiscoverSMTPAddress>mara@contoso.com</AutoDiscoverSMTPAddress>
      <DeploymentId>50817eff-b925-4578-a0db-13bfc635e7a5</DeploymentId>
    </User>
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <MicrosoftOnline>False</MicrosoftOnline>
      <Protocol>
        <Type>EXCH</Type>
        <Server>5f76be3c-9138-4f66-85e0-21bc23ca35f0@contoso.com</Server>
        <ServerDN>/o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=5f76be3c-9138-4f66-85e0-21bc23ca35f0@contoso.com</ServerDN>
        <ServerVersion>73C08204</ServerVersion>
        <MdbDN>/o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=5f76be3c-9138-4f66-85e0-21bc23ca35f0@contoso.com/cn=Microsoft Private MDB</MdbDN>
        <PublicFolderServer>public.contoso.com</PublicFolderServer>
        <AD>dc.contoso.com</AD>
        <ASUrl>https://mail.contoso.com/EWS/Exchange.asmx</ASUrl>
        <EwsUrl>https://mail.contoso.com/EWS/Exchange.asmx</EwsUrl>
        <EmwsUrl>https://mail.contoso.com/EWS/Exchange.asmx</EmwsUrl>
        <EcpUrl>https://mail.contoso.com/ecp/</EcpUrl>
        <EcpUrl-um>?rfr=olk&amp;amp;p=customize/voicemail.aspx&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-um>
        <EcpUrl-aggr>?rfr=olk&amp;amp;p=personalsettings/EmailSubscriptions.slab&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-aggr>
        <EcpUrl-mt>PersonalSettings/DeliveryReport.aspx?rfr=olk&amp;amp;exsvurl=1&amp;amp;IsOWA=&amp;lt;IsOWA&amp;gt;&amp;amp;MsgID=&amp;lt;MsgID&amp;gt;&amp;amp;Mbx=&amp;lt;Mbx&amp;gt;&amp;amp;realm=contoso.com</EcpUrl-mt>
        <EcpUrl-ret>?rfr=olk&amp;amp;p=organize/retentionpolicytags.slab&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-ret>
        <EcpUrl-sms>?rfr=olk&amp;amp;p=sms/textmessaging.slab&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-sms>
        <EcpUrl-publish>customize/calendarpublishing.slab?rfr=olk&amp;amp;exsvurl=1&amp;amp;FldID=&amp;lt;FldID&amp;gt;&amp;amp;realm=contoso.com</EcpUrl-publish>
        <EcpUrl-photo>PersonalSettings/EditAccount.aspx?rfr=olk&amp;amp;chgPhoto=1&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-photo>
        <EcpUrl-tm>?rfr=olk&amp;amp;ftr=TeamMailbox&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-tm>
        <EcpUrl-tmCreating>?rfr=olk&amp;amp;ftr=TeamMailboxCreating&amp;amp;SPUrl=&amp;lt;SPUrl&amp;gt;&amp;amp;Title=&amp;lt;Title&amp;gt;&amp;amp;SPTMAppUrl=&amp;lt;SPTMAppUrl&amp;gt;&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-tmCreating>
        <EcpUrl-tmEditing>?rfr=olk&amp;amp;ftr=TeamMailboxEditing&amp;amp;Id=&amp;lt;Id&amp;gt;&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-tmEditing>
        <EcpUrl-extinstall>Extension/InstalledExtensions.slab?rfr=olk&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-extinstall>
        <OOFUrl>https://mail.contoso.com/EWS/Exchange.asmx</OOFUrl>
        <UMUrl>https://mail.contoso.com/EWS/UM2007Legacy.asmx</UMUrl>
        <OABUrl>https://mail.contoso.com/OAB/c21c7bc2-53b3-4ddc-ad89-1219b486c37c/</OABUrl>
        <ServerExclusiveConnect>off</ServerExclusiveConnect>
      </Protocol>
      <Protocol>
        <Type>EXPR</Type>
        <Server>mail.contoso.com</Server>
        <SSL>Off</SSL>
        <AuthPackage>Ntlm</AuthPackage>
        <ServerExclusiveConnect>on</ServerExclusiveConnect>
        <CertPrincipalName>None</CertPrincipalName>
      </Protocol>
      <Protocol>
        <Type>WEB</Type>
        <Internal>
          <OWAUrl AuthenticationMethod="Basic, Fba">https://mail.contoso.com/owa/</OWAUrl>
          <Protocol>
            <Type>EXCH</Type>
            <ASUrl>https://mail.contoso.com/EWS/Exchange.asmx</ASUrl>
          </Protocol>
        </Internal>
      </Protocol>
    </Account>
  </Response>
</Autodiscover>
```

## <a name="next-steps"></a>次の手順
<a name="bk_Next"> </a>

サーバーからユーザーのために必要な構成の詳細を取得した後は、アプリケーションが必要な処理を実行する Exchange との通信ができています。 次のステップは、Exchange と通信する方法と、実行する内容によって異なります。 によって、インスピレーションを提供する必要があり、EWS を使用している場合は、いくつかのアイデアの[交換 101 のコード サンプル](http://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c)を表示する可能性があります。 
  
## <a name="see-also"></a>関連項目


- [Exchange の自動検出](autodiscover-for-exchange.md)
    
- [Exchange Web サービス (EWS) の管理の API](http://msdn.microsoft.com/en-us/library/exchange/jj220535%28v=exchg.80%29.aspx)
    
- [Exchange の自動検出 web サービスの参照が SOAP します。](http://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx)
    
- [Exchange の POX の自動検出 web サービスの参照](http://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx)
    


---
title: GetUserSettings 操作 (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 758d965c-ef63-4de4-9120-e293abf14ff8
description: GetUserSettings 操作には、ユーザーのクライアント アクセスの構成のクエリが含まれています。
ms.openlocfilehash: 8bb8f766da3419ea33f89716e588a22d3924e1a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831704"
---
# <a name="getusersettings-operation-soap"></a>GetUserSettings 操作 (SOAP)

**GetUserSettings**操作には、ユーザーのクライアント アクセスの構成のクエリが含まれています。 
  
## <a name="getusersettings-request-example"></a>GetUserSettings 要求の例

### <a name="description"></a>説明

次の XML の例は、ユーザーの表示名、識別名、展開の ID、メールボックス サーバー、メールボックスの識別名、Active Directory サーバー、クライアント アクセス サーバーのバージョン、およびサポートされている Exchange Web を要求する自動検出要求の本文を示しています。サービスのスキーマです。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover"      
               xmlns:wsa="http://www.w3.org/2005/08/addressing" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"      
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2010</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://myserver.contoso.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>UserName@domain.contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>UserDisplayName</a:Setting>
          <a:Setting>UserDN</a:Setting>
          <a:Setting>UserDeploymentId</a:Setting>
          <a:Setting>InternalMailboxServer</a:Setting>
          <a:Setting>MailboxDN</a:Setting>
          <a:Setting>ActiveDirectoryServer</a:Setting>
          <a:Setting>CasVersion</a:Setting>
          <a:Setting>EwsSupportedSchemas</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a>要素を要求します。

次の要素は、要求の本体で使用されます。
  
- [GetUserSettingsRequestMessage (SOAP)](getusersettingsrequestmessage-soap.md)
    
- [メールボックス (SOAP)](mailbox-soap.md)
    
- [要求 (SOAP)](request-soap.md)
    
- [RequestedServerVersion (SOAP)](requestedserverversion-soap.md)
    
- [RequestedSettings (SOAP)](requestedsettings-soap.md)
    
- [(SOAP) の設定](setting-soap.md)
    
- [ユーザー (SOAP)](user-soap.md)
    
- [ユーザー (SOAP)](users-soap.md)
    
## <a name="getusersettings-response-example"></a>GetUserSettings の応答の例

### <a name="description"></a>説明

次の例では、正常な**GetUserSettings**応答を示します。 
  
### <a name="code"></a>コード

```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
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
                <Value>UserDisplayName</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>UserDN</Name>
                <Value>/o=First Organization/ou=Exchange Administrative Group (SDASDASDJ)/cn=Recipients/cn=UserDisplayName</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>UserDeploymentId</Name>
                <Value>a40E2742-21c6-4050-8Ed2-d41f100c22b8</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>CasVersion</Name>
                <Value>14.00.0478.000</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>EwsSupportedSchemas</Name>
                <Value>Exchange2007,  Exchange2010</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>InternalMailboxServer</Name>
                <Value>machinename.domain.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ActiveDirectoryServer</Name>
                <Value>machinename.domain.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>MailboxDN</Name>
                <Value>/o=First Organization/ou=Exchange Administrative Group (SDASDASDJ)/cn=Configuration/cn=Servers/cn=server/cn=Contoso Pri MDB</Value>
              </UserSetting>
            </UserSettings>
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

### <a name="response-elements"></a>応答の要素

応答の本体では、次の要素が使用されます。
  
- [エラー コード (SOAP)](errorcode-soap.md)
    
- [エラー メッセージ (SOAP)](errormessage-soap.md)
    
- [GetUserSettingsResponseMessage (SOAP)](getusersettingsresponsemessage-soap.md)
    
- [名 (SOAP)](name-soap.md)
    
- [RedirectTarget (SOAP)](redirecttarget-soap.md)
    
- [応答 (SOAP)](response-soap.md)
    
- [UserResponse (SOAP)](userresponse-soap.md)
    
- [UserResponses (SOAP)](userresponses-soap.md)
    
- [UserSetting (SOAP)](usersetting-soap.md)
    
- [UserSettingErrors (SOAP)](usersettingerrors-soap.md)
    
- [ユーザー (SOAP)](usersettings-soap.md)
    
- [値 (SOAP)](value-soap.md)
    
## <a name="see-also"></a>関連項目



[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)
  
[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)


[Exchange 2013 の自動検出の XML 要素を SOAP](soap-autodiscover-xml-elements-for-exchange-2013.md)


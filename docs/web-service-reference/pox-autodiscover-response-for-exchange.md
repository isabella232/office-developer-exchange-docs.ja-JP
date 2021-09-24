---
title: POX 自動検出応答のExchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 08c6c5a2-a67a-4141-a8bd-1b5d560b90a7
description: 自動検出応答には、Exchange Web Services (EWS) とのバインドを確立するために使用される URL の一覧を含む自動検出要求に対する応答が含まれます。
ms.openlocfilehash: 42705856a28a1b5e595e55ab3f77f78089a1ee21
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527901"
---
# <a name="pox-autodiscover-response-for-exchange"></a>POX 自動検出応答のExchange

自動検出応答には、Exchange Web Services (EWS) とのバインドを確立するために使用される URL の一覧を含む自動検出要求に対する応答が含まれます。
  
## <a name="autodiscover-response-example"></a>自動検出応答の例

### <a name="description"></a>説明

次の例は、自動検出応答の成功を示しています。
  
### <a name="code"></a>コード

```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <User>
      <DisplayName>First Last</DisplayName>
      <LegacyDN>/o=contoso/ou=First Administrative Group/cn=Recipients/cn=iuser885646</LegacyDN>
      <DeploymentId>644560b8-a1ce-429c-8ace-23395843f701</DeploymentId>
    </User>
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <Protocol>
        <Type>EXCH</Type>
        <Server>MBX-SERVER.mail.internal.contoso.com</Server>
        <ServerDN>/o=contoso/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=MBX-SERVER</ServerDN>
        <ServerVersion>72008287</ServerVersion>
        <MdbDN>/o=contoso/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=MBX-SERVER/cn=Microsoft Private MDB</MdbDN>
        <ASUrl>https://mail.contoso.com/ews/exchange.asmx</ASUrl>
        <OOFUrl>https://mail.contoso.com/ews/exchange.asmx</OOFUrl>
        <UMUrl>https://mail.contoso.com/unifiedmessaging/service.asmx</UMUrl>
        <OABUrl>https://mail.contoso.com/OAB/d29844a9-724e-468c-8820-0f7b345b767b/</OABUrl>
      </Protocol>
      <Protocol>
        <Type>EXPR</Type>
        <Server>Exchange.contoso.com</Server>
        <ASUrl>https://mail.contoso.com/ews/exchange.asmx</ASUrl>
        <OOFUrl>https://mail.contoso.com/ews/exchange.asmx</OOFUrl>
        <UMUrl>https://mail.contoso.com/unifiedmessaging/service.asmx</UMUrl>
        <OABUrl>https://mail.contoso.com/OAB/d29844a9-724e-468c-8820-0f7b345b767b/</OABUrl>
      </Protocol>
      <Protocol>
        <Type>WEB</Type>
        <Internal>
          <OWAUrl AuthenticationMethod="Ntlm, WindowsIntegrated">https://cas-01-server.mail.internal.contoso.com/owa</OWAUrl>
          <OWAUrl AuthenticationMethod="Ntlm, WindowsIntegrated">https://cas-02-server.mail.internal.contoso.com/owa</OWAUrl>
          <OWAUrl AuthenticationMethod="Basic">https://cas-04-server.mail.internal.contoso.com/owa</OWAUrl>
          <OWAUrl AuthenticationMethod="Ntlm, WindowsIntegrated">https://cas-05-server.mail.internal.contoso.com/owa</OWAUrl>
        </Internal>
      </Protocol>
    </Account>
  </Response>
</Autodiscover>
```

### <a name="comments"></a>コメント

Web サービスにバインド[Exchange、ASUrl (POX)](asurl-pox.md)要素で識別される URL を使用します。 
  
### <a name="response-element"></a>Response 要素

応答本文では、次の要素が使用されます。
  
- [AutoDiscover (POX)](autodiscover-pox.md)
    
- [Response (POX)](response-pox.md)
    
- [User (POX)](user-pox.md)
    
- [DisplayName (POX)](displayname-pox.md)
    
- [LegacyDN (POX)](legacydn-pox.md)
    
- [DeploymentId (POX)](deploymentid-pox.md)
    
- [Account (POX)](account-pox.md)
    
- [AccountType (POX)](accounttype-pox.md)
    
- [Action (POX)](action-pox.md)
    
- [Protocol (POX)](protocol-pox.md)
    
- [Type (POX)](type-pox.md)
    
- [Server (POX)](server-pox.md)
    
- [ServerDN (POX)](serverdn-pox.md)
    
- [ServerVersion (POX)](serverversion-pox.md)
    
- [MdbDN (POX)](mdbdn-pox.md)
    
- [ASUrl (POX)](asurl-pox.md)
    
- [OOFUrl (POX)](oofurl-pox.md)
    
- [UMUrl (POX)](umurl-pox.md)
    
- [OABUrl (POX)](oaburl-pox.md)
    
- [内部 (POX)](internal-pox.md)
    
- [OWAUrl (POX)](owaurl-pox.md)
    
## <a name="autodiscover-error-response-example"></a>自動検出エラー応答の例

### <a name="description"></a>説明

次の例は、自動検出エラー応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
    <Error Time="21:25:04.8897083" Id="4130155072">
      <ErrorCode>600</ErrorCode>
      <Message>Invalid Request</Message>
      <DebugData />
    </Error>
  </Response>
</Autodiscover>
```

### <a name="error-response-element"></a>エラー応答要素

応答本文では、次の要素が使用されます。
  
- [AutoDiscover (POX)](autodiscover-pox.md)
    
- [Response (POX)](response-pox.md)
    
- [Error (POX)](error-pox.md)
    
- [ErrorCode (POX)](errorcode-pox.md)
    
- [Message (POX)](message-pox.md)
    
- [DebugData (POX)](debugdata-pox.md)
    
## <a name="see-also"></a>関連項目

- [POX 自動検出要求のExchange](pox-autodiscover-request-for-exchange.md)
- [Exchange 用 POX 自動検出 Web サービス リファレンス](pox-autodiscover-web-service-reference-for-exchange.md) 
- [POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)


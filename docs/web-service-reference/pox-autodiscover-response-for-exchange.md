---
title: POX Exchange の自動検出の応答
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 08c6c5a2-a67a-4141-a8bd-1b5d560b90a7
description: 自動検出の応答には、Exchange Web サービス (EWS) でのバインドを確立するために使用する Url の一覧を含む自動検出の要求に対する応答が含まれています。
ms.openlocfilehash: d9f8a5cc86efaa4dceda7385164872ecc5409252
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832863"
---
# <a name="pox-autodiscover-response-for-exchange"></a>POX Exchange の自動検出の応答

自動検出の応答には、Exchange Web サービス (EWS) でのバインドを確立するために使用する Url の一覧を含む自動検出の要求に対する応答が含まれています。
  
## <a name="autodiscover-response-example"></a>自動検出応答の例

### <a name="description"></a>説明

正常な自動検出応答の例を次に示します。
  
### <a name="code"></a>コード

```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
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

Exchange Web サービスにバインドするには、 [ASUrl (POX)](asurl-pox.md)要素で指定された URL を使用します。 
  
### <a name="response-element"></a>Response 要素

応答の本体では、次の要素が使用されます。
  
- [(POX) を自動検出](autodiscover-pox.md)
    
- [応答 (POX)](response-pox.md)
    
- [ユーザー (POX)](user-pox.md)
    
- [DisplayName (POX)](displayname-pox.md)
    
- [LegacyDN (POX)](legacydn-pox.md)
    
- [DeploymentId (POX)](deploymentid-pox.md)
    
- [アカウント (POX)](account-pox.md)
    
- [AccountType (POX)](accounttype-pox.md)
    
- [アクション (POX)](action-pox.md)
    
- [プロトコル (POX)](protocol-pox.md)
    
- [(POX) の種類](type-pox.md)
    
- [サーバー (POX)](server-pox.md)
    
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

自動検出エラー応答の例を次に示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
    <Error Time="21:25:04.8897083" Id="4130155072">
      <ErrorCode>600</ErrorCode>
      <Message>Invalid Request</Message>
      <DebugData />
    </Error>
  </Response>
</Autodiscover>
```

### <a name="error-response-element"></a>エラー応答の要素

応答の本体では、次の要素が使用されます。
  
- [(POX) を自動検出](autodiscover-pox.md)
    
- [応答 (POX)](response-pox.md)
    
- [エラー (POX)](error-pox.md)
    
- [エラー コード (POX)](errorcode-pox.md)
    
- [メッセージ (POX)](message-pox.md)
    
- [DebugData (POX)](debugdata-pox.md)
    
## <a name="see-also"></a>関連項目

- [POX の自動検出要求の交換](pox-autodiscover-request-for-exchange.md)
- [Exchange の POX の自動検出 web サービスの参照](pox-autodiscover-web-service-reference-for-exchange.md) 
- [交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)


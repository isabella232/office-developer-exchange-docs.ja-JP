---
title: GetMailTips 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTips
api_type:
- schema
ms.assetid: 025483ec-a9f3-4735-8a95-d26e30ea7974
description: GetMailTips 操作は、指定したメールボックスのメール ヒントの情報を取得します。
ms.openlocfilehash: 15c21bef90fdc4cbc6cd65512cdc078fcdf31e60
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760786"
---
# <a name="getmailtips-operation"></a>GetMailTips 操作

**GetMailTips**操作は、指定したメールボックスのメール ヒントの情報を取得します。 
  
## <a name="getmailtips-request-example"></a>GetMailTips 要求の例

### <a name="description"></a>説明

クライアントは、要求の XML を構築し、サーバーに送信します。 要求のクライアントがメールボックスと、メールのヒントを取得するために送信し、どのようなメール ヒントは、要求されたユーザーを指定します。 この例では、クライアントは、選択したメールボックスのすべてのメール ヒントが返されることを要求します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"> 
  <soap:Header> 
    <t:RequestServerVersion Version="Exchange2010" /> 
  </soap:Header> 
  <soap:Body> 
    <GetMailTips xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"> 
      <SendingAs> 
        <t:EmailAddress> user1@contoso.com </t:EmailAddress> 
        <t:RoutingType>SMTP</t:RoutingType> 
      </SendingAs> 
      <Recipients> 
        <t:Mailbox> 
          <t:EmailAddress> user2@contoso.com </t:EmailAddress> 
          <t:RoutingType>SMTP</t:RoutingType> 
        </t:Mailbox> 
      </Recipients> 
      <MailTipsRequested>All</MailTipsRequested> 
    </GetMailTips> 
  </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a>要素を要求します。

要求では、次の要素が含まれています。
  
- [GetMailTips](getmailtips.md)
    
- [SendingAs](sendingas.md)
    
- [受信者 (ArrayOfRecipientsType)](recipients-arrayofrecipientstype.md)
    
- [MailTipsRequested](mailtipsrequested.md)
    
## <a name="successful-getmailtips-response-example"></a>成功した GetMailTips の応答の例

### <a name="description"></a>説明

Simple Object Access Protocol (SOAP) 本文の次の使用例は、 **GetMailTips**要求に正常な応答を示しています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?> 
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"> 
  <s:Header> 
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="0" MajorBuildNumber="536" MinorBuildNumber="0" Version="Exchange2010" 
xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:xsd="http://www.w3.org/2001/XMLSchema"/> 
  </s:Header> 
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <GetMailTipsResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"> 
      <ResponseCode>NoError</ResponseCode> 
      <ResponseMessages> 
        <MailTipsResponseMessageType ResponseClass="Success"> 
        <ResponseCode>NoError</ResponseCode> 
        <m:MailTips xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"> 20 / 29 [MS-OXWMT] — v20100517 Mail Tips Web Service Extensions Copyright © 2010 Microsoft Corporation. Release: Monday, May 17, 2010 
          <t:RecipientAddress xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"> 
          <t:Name/> 
          <t:EmailAddress>user2@contoso.com</t:EmailAddress> 
          <t:RoutingType>SMTP</t:RoutingType> 
          </t:RecipientAddress> 
          <t:PendingMailTips xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/> 
          <t:OutOfOffice xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"> 
            <t:ReplyBody> 
              <t:Message/> 
            </t:ReplyBody> 
          </t:OutOfOffice> 
          <t:MailboxFull xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">false</t:MailboxFull> 
          <t:CustomMailTip xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">Hello World Mailtips</t:CustomMailTip> 
          <t:TotalMemberCount xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">1</t:TotalMemberCount> 
          <t:ExternalMemberCount xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">0</t:ExternalMemberCount> 
          <t:MaxMessageSize xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">10485760</t:MaxMessageSize> 
          <t:DeliveryRestricted xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">false</t:DeliveryRestricted> 
          <t:IsModerated xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">false</t:IsModerated> 
          <t:InvalidRecipient xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">false</t:InvalidRecipient> 
        </m:MailTips> 
        </MailTipsResponseMessageType> 
      </ResponseMessages> 
    </GetMailTipsResponse> 
  </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a>応答の要素

応答では、次の要素が含まれています。
  
- [ResponseCode](responsecode.md)
    
- [メール ヒント](mailtips.md)
    
## <a name="see-also"></a>関連項目



[Exchange での EWS の操作](ews-operations-in-exchange.md)
  
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


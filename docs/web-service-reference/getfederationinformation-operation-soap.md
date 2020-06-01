---
title: GetFederationInformation 操作 (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c6666a42-a18f-4e4b-beb6-b25ff62cfcc5
description: GetFederationInformation 操作は、組織のフェデレーションの状態 (この組織を対象としたトークンを要求するときに使用されるターゲット URI、および組織がフェデレーションを行うその他のドメイン) についての情報を提供します。
ms.openlocfilehash: 533b2f6d282e3287f4945df56b169f5bc93ff445
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455626"
---
# <a name="getfederationinformation-operation-soap"></a>GetFederationInformation 操作 (SOAP)

**GetFederationInformation**操作は、組織のフェデレーションの状態 (この組織を対象としたトークンを要求するときに使用されるターゲット URI、および組織がフェデレーションを行うその他のドメイン) についての情報を提供します。 
  
外部ユーザーに予定表、連絡先、メッセージを共有できるのは、フェデレーション組織のみです。
  
## <a name="getfederationinformation-request-example"></a>GetFederationInformation 要求の例

### <a name="description"></a>説明

**GetFederationInformation**要求の次の例は、ユーザーのフェデレーション情報の要求を示しています。 クライアントは、この要求をサーバーに送信します。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?> 
<soap:Envelope xmlns:exm="https://schemas.microsoft.com/exchange/services/2006/messages"
           xmlns:ext="https://schemas.microsoft.com/exchange/services/2006/types"
           xmlns:a="http://www.w3.org/2005/08/addressing"
           xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <soap:Header> 
        <a:MessageID>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:MessageID> 
        <a:Action soap:mustUnderstand="1">https://schemas.microsoft.com/
            exchange/2010/Autodiscover/Autodiscover/GetFederationInformation
        </a:Action> 
        <a:To soap:mustUnderstand="1">https://autodiscover.byfcxu-
            dom.extest.microsoft.com/autodiscover/autodiscover.svc</a:To> 
        <a:ReplyTo>
            <a:Address>http://www.w3.org/2005/08/addressing/anonymous</a:Address> 
        </a:ReplyTo> 
    </soap:Header> 
    <soap:Body> 
        <GetFederationInformationRequestMessage 
            xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Request> 
                <Domain>contoso.com</Domain> 
            </Request> 
        </GetFederationInformationRequestMessage>
    </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a>Request 要素

要求では、次の要素が使用されます。
  
- [GetFederationInformationRequestMessage (SOAP)](getfederationinformationrequestmessage-soap.md)
    
- [要求 (SOAP)](request-soap.md)
    
- [ドメイン (SOAP)](domain-soap.md)
    
## <a name="getfederationinformation-response-example"></a>GetFederationInformation response の例

### <a name="description"></a>説明

次の例は、サーバーがクライアントに送信する**GetFederationInformation**要求に対する正常な応答を示しています。 
  
### <a name="code"></a>コード

```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
xmlns:a="http://www.w3.org/2005/08/addressing"> 
    <s:Header> 
        <a:Action s:mustUnderstand="1">
            https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetFederationInformationResponse
        </a:Action> 
        <a:RelatesTo>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:RelatesTo> 
    </s:Header> 
    <s:Body> 
        <GetFederationInformationResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
                <ErrorCode>NoError</ErrorCode> 
                <ErrorMessage/> 
                <ApplicationUri>BYFCXU-DOM.EXTEST.MICROSOFT.COM</ApplicationUri> 
                <Domains> 
                    <Domain>contoso.com</Domain> 
                    <Domain>europe.contoso.com</Domain> 
                    <Domain>americas.contoso.com</Domain> 
                    <Domain>contosolive.com</Domain> 
                </Domains> 
            </Response> 
        </GetFederationInformationResponseMessage> 
    </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a>Response 要素

応答では、次の要素が使用されます。
  
- [GetFederationInformationResponseMessage (SOAP)](getfederationinformationresponsemessage-soap.md)
    
- [応答 (SOAP)](response-soap.md)
    
- [ErrorCode (SOAP)](errorcode-soap.md)
    
- [ErrorMessage (SOAP)](errormessage-soap.md)
    
- [ApplicationUri (SOAP)](applicationuri-soap.md)
    
- [Domains (SOAP)](domains-soap.md)
    
- [ドメイン (SOAP)](domain-soap.md)
    
## <a name="see-also"></a>関連項目

- [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
- [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)


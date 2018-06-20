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
description: GetFederationInformation 操作には、対象の URI は、この組織と組織には、また他のドメインを対象とするトークンを要求するときに使用するなど、組織のフェデレーションの状態に関する情報が用意されています。連合。
ms.openlocfilehash: bf38b2f2b3db3e38b9b0157d1677efe4fc274e1b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760734"
---
# <a name="getfederationinformation-operation-soap"></a>GetFederationInformation 操作 (SOAP)

**GetFederationInformation**操作には、組織のフェデレーションの状態に関する情報が用意されています、この組織では、およびその他のドメインをターゲットなどトークンを要求するときに使用する URI が対象としている組織フェデレーションがも。 
  
フェデレーションの組織には、予定表、連絡先、および外部ユーザーにメッセージを共有できます。
  
## <a name="getfederationinformation-request-example"></a>GetFederationInformation 要求の例

### <a name="description"></a>説明

**GetFederationInformation**要求の次の使用例は、フェデレーションのユーザーの設定情報の要求を示しています。 クライアントは、この要求をサーバーに送信します。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?> 
<soap:Envelope xmlns:exm="http://schemas.microsoft.com/exchange/services/2006/messages"
           xmlns:ext="http://schemas.microsoft.com/exchange/services/2006/types"
           xmlns:a="http://www.w3.org/2005/08/addressing"
           xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <soap:Header> 
        <a:MessageID>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:MessageID> 
        <a:Action soap:mustUnderstand="1">http://schemas.microsoft.com/
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
            xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Request> 
                <Domain>contoso.com</Domain> 
            </Request> 
        </GetFederationInformationRequestMessage>
    </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a>要素を要求します。

次の要素は、要求で使用されます。
  
- [GetFederationInformationRequestMessage (SOAP)](getfederationinformationrequestmessage-soap.md)
    
- [要求 (SOAP)](request-soap.md)
    
- [ドメイン (SOAP)](domain-soap.md)
    
## <a name="getfederationinformation-response-example"></a>GetFederationInformation の応答の例

### <a name="description"></a>説明

次の例では、サーバーがクライアントに送信する**GetFederationInformation**要求に正常な応答を示します。 
  
### <a name="code"></a>コード

```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
xmlns:a="http://www.w3.org/2005/08/addressing"> 
    <s:Header> 
        <a:Action s:mustUnderstand="1">
            http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetFederationInformationResponse
        </a:Action> 
        <a:RelatesTo>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:RelatesTo> 
    </s:Header> 
    <s:Body> 
        <GetFederationInformationResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover"> 
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

### <a name="response-elements"></a>応答の要素

次の要素は、応答で使用されます。
  
- [GetFederationInformationResponseMessage (SOAP)](getfederationinformationresponsemessage-soap.md)
    
- [応答 (SOAP)](response-soap.md)
    
- [エラー コード (SOAP)](errorcode-soap.md)
    
- [エラー メッセージ (SOAP)](errormessage-soap.md)
    
- [ApplicationUri (SOAP)](applicationuri-soap.md)
    
- [ドメイン (SOAP)](domains-soap.md)
    
- [ドメイン (SOAP)](domain-soap.md)
    
## <a name="see-also"></a>関連項目

- [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
- [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)


---
title: GetClientAccessToken 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 086876cc-e22c-4e89-89f9-19e78af51217
description: 操作 GetClientAccessToken EWS についての情報を検索します。
ms.openlocfilehash: afa9a315a8421f31c345c9547a5d80bed41e9fbc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760655"
---
# <a name="getclientaccesstoken-operation"></a>GetClientAccessToken 操作

**GetClientAccessToken** EWS の操作に関する情報を検索します。 
  
**GetClientAccessToken**操作では、Outlook のメール アプリケーションにクライアントのアクセスを取得します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-getclientaccesstoken-operation"></a>GetClientAccessToken 操作を使用します。

**GetClientAccessToken**操作の要求は、2 つの必要な引数: アプリケーション、およびトークンの種類の識別子です。 [GetAppManifests 操作](getappmanifests-operation.md)を使用するアプリケーション id を要求します。 
  
### <a name="getclientaccesstoken-operation-soap-headers"></a>GetClientAccessToken 操作の SOAP ヘッダー

**GetClientAccessToken**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="getclientaccesstoken-operation-request-example-get-a-caller-identity-token"></a>GetClientAccessToken 操作の要求の例: 呼び出し元 id のトークンを取得します。

**GetClientAccessToken**操作要求の次の例では、アプリケーションの呼び出し元 id のトークンを取得する方法を示します。 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetClientAccessToken>
         <m:TokenRequests>
            <t:TokenRequest>
               <t:Id>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</t:Id>
               <t:TokenType>CallerIdentity</t:TokenType>
            </t:TokenRequest>
         </m:TokenRequests>
      </m:GetClientAccessToken>
   </soap:Body>
</soap:Envelope>

```

要求 SOAP 本体にはには、次の要素が含まれています。
  
- [GetClientAccessToken](getclientaccesstoken.md)
    
- [TokenRequests](tokenrequests.md)
    
- [TokenRequest](tokenrequest.md)
    
- [ID (文字列)](id-string.md)
    
- [TokenType](tokentype.md)
    
## <a name="successful-getclientaccesstoken-operation-response"></a>GetClientAccessToken 操作の成功の応答

次の例では、アプリケーションの呼び出し元 id のトークンを取得するのには、 **GetClientAccessToken**操作の要求に正常な応答を示します。 
  
> [!NOTE]
> この資料では、トークンの値は、読みやすさを保持するために短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetClientAccessTokenResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetClientAccessTokenResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Token>
                  <t:Id>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</t:Id>
                  <t:TokenType>CallerIdentity</t:TokenType>
                  <t:TokenValue>eyJ0eXAmv0QitaJg</t:TokenValue>
                  <t:TTL>479</t:TTL>
               </m:Token>
            </m:GetClientAccessTokenResponseMessage>
         </m:ResponseMessages>
      </m:GetClientAccessTokenResponse>
   </s:Body>
</s:Envelope>

```

応答 SOAP 本文には、次の要素が含まれています。
  
- [GetClientAccessTokenResponse](getclientaccesstokenresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetClientAccessTokenResponseMessage](getclientaccesstokenresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [トークン (ClientAccessTokenType)](token-clientaccesstokentype.md)
    
- [ID (文字列)](id-string.md)
    
- [TokenType (ClientAccessTokenType)](tokentype-clientaccesstokentype.md)
    
- [TokenValue](tokenvalue.md)
    
- [TTL (ClientAccessTokenTypeType)](ttl-clientaccesstokentypetype.md)
    
## <a name="getclientaccesstoken-operation-error-response"></a>GetClientAccessToken 操作のエラー応答

**GetClientAccessToken**操作の要求に対してエラー応答の例を次に示します。 これは、適切なアクセス許可のないトークン、拡張子コールバックを取得する要求に応答します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetClientAccessTokenResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetClientAccessTokenResponseMessage ResponseClass="Error">
               <m:MessageText>The caller does not have enough permission for this token request.</m:MessageText>
               <m:ResponseCode>ErrorInvalidClientAccessTokenRequest</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
            </m:GetClientAccessTokenResponseMessage>
         </m:ResponseMessages>
      </m:GetClientAccessTokenResponse>
   </s:Body>
</s:Envelope>
```

エラー応答 SOAP 本体にはには、次の要素が含まれています。
  
- [GetClientAccessTokenResponse](getclientaccesstokenresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetClientAccessTokenResponseMessage](getclientaccesstokenresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。
  
## <a name="see-also"></a>関連項目

- [Exchange での EWS の操作](ews-operations-in-exchange.md)
    
- [GetAppManifests 操作](getappmanifests-operation.md)
    
- [Outlook アドイン](http://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    


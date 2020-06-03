---
title: GetClientAccessToken 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 086876cc-e22c-4e89-89f9-19e78af51217
description: GetClientAccessToken EWS 操作についての情報を検索します。
ms.openlocfilehash: 2d49d675fcedb0e7e8312a9715f095c47fcf3d77
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462039"
---
# <a name="getclientaccesstoken-operation"></a>GetClientAccessToken 操作

**GetClientAccessToken** EWS 操作についての情報を検索します。 
  
**GetClientAccessToken**操作は、Outlook 用メールアプリのクライアントアクセストークンを取得します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-getclientaccesstoken-operation"></a>GetClientAccessToken 操作の使用

**GetClientAccessToken**操作要求は、次の2つの必要な引数を受け取ります。アプリの識別子とトークンの種類。 [Getappmanifests 操作](getappmanifests-operation.md)を使用して、アプリ識別子を要求できます。 
  
### <a name="getclientaccesstoken-operation-soap-headers"></a>GetClientAccessToken 操作の SOAP ヘッダー

**GetClientAccessToken**操作では、次の表に示す SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは応答に適用されます。  <br/> |
   
## <a name="getclientaccesstoken-operation-request-example-get-a-caller-identity-token"></a>GetClientAccessToken 操作要求の例: 発信者 id トークンを取得します。

次の**GetClientAccessToken**操作要求の例は、アプリの発信者番号トークンを取得する方法を示しています。 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

要求 SOAP 本文には、次の要素が含まれています。
  
- [GetClientAccessToken](getclientaccesstoken.md)
    
- [TokenRequests](tokenrequests.md)
    
- [TokenRequest](tokenrequest.md)
    
- [ID (文字列)](id-string.md)
    
- [TokenType](tokentype.md)
    
## <a name="successful-getclientaccesstoken-operation-response"></a>成功した GetClientAccessToken 操作の応答

次の例は、 **GetClientAccessToken**操作要求に対する正常な応答を示しています。アプリの発信者番号トークンを取得します。 
  
> [!NOTE]
> この記事のトークンの値は、読みやすくするために短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetClientAccessTokenResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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
    
## <a name="getclientaccesstoken-operation-error-response"></a>GetClientAccessToken 操作エラー応答

次の例は、 **GetClientAccessToken**操作要求へのエラー応答を示しています。 これは、適切なアクセス許可を持たない拡張コールバックトークンを取得する要求に対する応答です。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetClientAccessTokenResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

エラー応答 SOAP 本文には、次の要素が含まれています。
  
- [GetClientAccessTokenResponse](getclientaccesstokenresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetClientAccessTokenResponseMessage](getclientaccesstokenresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)
  
## <a name="see-also"></a>関連項目

- [Exchange での EWS 操作](ews-operations-in-exchange.md)
    
- [GetAppManifests 操作](getappmanifests-operation.md)
    
- [Outlook アドイン](https://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    


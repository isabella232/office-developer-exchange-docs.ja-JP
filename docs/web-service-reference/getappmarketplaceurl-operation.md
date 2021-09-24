---
title: GetAppMarketplaceUrl 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 2c016fc3-0e13-4624-9a5b-d3e84577a860
description: GetAppMarketplaceUrl EWS 操作に関する情報を検索します。
ms.openlocfilehash: f9dd41a43b92910ec596b95a0ce1e99a239ba01e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530091"
---
# <a name="getappmarketplaceurl-operation"></a>GetAppMarketplaceUrl 操作

**GetAppMarketplaceUrl** EWS 操作に関する情報を検索します。 
  
**GetAppMarketplaceUrl 操作** は、クライアントがアクセスしてメールボックスにインストールするアプリを取得できるアプリマーケットプレースの URL を取得します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-getappmarketplaceurl-operation"></a>GetAppMarketplaceUrl 操作の使用

**GetAppMarketplaceUrl** 操作は、クライアントがアプリをインストールできるマーケットプレースの URL を要求する引数を取らない。 応答には、アプリマーケットプレースへの URL が含まれる。 
  
### <a name="getappmarketplaceurl-operation-soap-headers"></a>GetAppMarketplaceUrl 操作 SOAP ヘッダー

**GetAppMarketplaceUrl 操作** では、次の表に示す SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**Element**|**説明**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマ バージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="getappmarketplaceurl-operation-request-example-get-the-app-marketplace-url-for-a-mailbox"></a>GetAppMarketplaceUrl 操作要求の例: メールボックスのアプリマーケットプレース URL を取得する

**GetAppMarketplaceUrl 操作要求の次** の例は、メールボックスのアプリマーケットプレース URL を取得する方法を示しています。 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013_SP1" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:GetAppMarketplaceUrl>
        <m:ApiVersionSupported>1.0</m:ApiVersionSupported>
        <m:SchemaVersionSupported>1.0</m:SchemaVersionSupported>
      </m:GetAppMarketplaceUrl>
   </soap:Body>
</soap:Envelope>

```

要求 SOAP 本文には、次の要素が含まれています。
  
- [GetAppMarketplaceUrl](getappmarketplaceurl.md)
    
- [ApiVersionSupported](apiversionsupported.md)
    
- [SchemaVersionSupported](schemaversionsupported.md)
    
## <a name="successful-getappmarketplaceurl-operation-response"></a>GetAppMarketplaceUrl 操作応答の成功

次の例は **、GetAppMarketplaceUrl** 操作要求に対して、メールボックスのアプリ マーケットプレース URL を取得する正常な応答を示しています。 
  
> [!NOTE]
> 読みやすさを維持するためにアプリマーケットプレースの URL が変更されました。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="7" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppMarketplaceUrlResponse ResponseClass="Success" 
                                    xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <AppMarketplaceUrl>http://marketplace.contoso.com</AppMarketplaceUrl>
      </GetAppMarketplaceUrlResponse>
   </s:Body>
</s:Envelope>

```

応答 SOAP 本文には、次の要素が含まれています。
  
- [GetAppMarketplaceUrlResponse](getappmarketplaceurlresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [AppMarketplaceUrl](appmarketplaceurl.md)
    
## <a name="getappmarketplaceurl-operation-error-response"></a>GetAppMarketPlaceUrl 操作エラー応答

この操作で返されるエラーは、正しくないサービス構成に関連するか、汎用的な EWS エラーです。 EWS に汎用的で、この操作に固有のエラー コードについては [、「ResponseCode」を参照してください](responsecode.md)。 
  
次の例は、外部コントロール パネル (ECP) が構成Exchange返されるエラー応答を示しています。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="7" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppMarketplaceUrlResponse ResponseClass="Error" 
                                    xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot get external ECP URL. This might happen if external ECP URL isn't configured.</MessageText>
         <ResponseCode>ErrorCannotGetExternalEcpUrl</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetAppMarketplaceUrlResponse>
   </s:Body>
</s:Envelope>
```

エラー応答 SOAP 本文には、次の要素が含まれています。
  
- [GetAppMarketplaceUrlResponse](getappmarketplaceurlresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>関連項目

- [EWS 操作 (Exchange](ews-operations-in-exchange.md)
    
- [DisableApp 操作](disableapp-operation.md)
    
- [InstallApp 操作](installapp-operation.md)
    
- [UninstallApp 操作](uninstallapp-operation.md)
    
- [GetAppManifests 操作](getappmanifests-operation.md)
    


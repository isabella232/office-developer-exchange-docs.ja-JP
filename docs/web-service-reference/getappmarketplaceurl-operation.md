---
title: GetAppMarketplaceUrl 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2c016fc3-0e13-4624-9a5b-d3e84577a860
description: GetAppMarketplaceUrl EWS 操作についての情報を検索します。
ms.openlocfilehash: 6797af44c3aaa6653c440b3d53a282d8c90a4381
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459526"
---
# <a name="getappmarketplaceurl-operation"></a>GetAppMarketplaceUrl 操作

**GetAppMarketplaceUrl** EWS 操作についての情報を検索します。 
  
**GetAppMarketplaceUrl**操作は、メールボックスにインストールするアプリを取得するためにクライアントがアクセスできるアプリケーションマーケットプレースの URL を取得します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-getappmarketplaceurl-operation"></a>GetAppMarketplaceUrl 操作の使用

**GetAppMarketplaceUrl**操作では、クライアントがアプリをインストールできる MARKETPLACE の URL を要求する引数はありません。 応答には、アプリマーケットプレースへの URL が含まれます。 
  
### <a name="getappmarketplaceurl-operation-soap-headers"></a>GetAppMarketplaceUrl 操作の SOAP ヘッダー

**GetAppMarketplaceUrl**操作では、次の表に示す SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは応答に適用されます。  <br/> |
   
## <a name="getappmarketplaceurl-operation-request-example-get-the-app-marketplace-url-for-a-mailbox"></a>GetAppMarketplaceUrl 操作要求の例: メールボックスのアプリマーケットプレース URL を取得します。

次の**GetAppMarketplaceUrl**操作要求の例は、メールボックスのアプリマーケットプレース URL を取得する方法を示しています。 
  
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
    
- [サポートされている apiversion](apiversionsupported.md)
    
- [SchemaVersionSupported](schemaversionsupported.md)
    
## <a name="successful-getappmarketplaceurl-operation-response"></a>成功した GetAppMarketplaceUrl 操作の応答

次の例は、 **GetAppMarketplaceUrl**操作要求に対する正常な応答を示しています。メールボックスのアプリマーケットプレース URL を取得します。 
  
> [!NOTE]
> アプリケーションマーケットプレース URL は、読みやすくするために変更されています。 
  
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

この操作に対して返されたエラーは、正しくないサービス構成に関連付けられているか、または一般的な EWS エラーであることを示します。 EWS で汎用的で、この操作に固有のエラーコードについては、「応答」を[参照して](responsecode.md)ください。 
  
次の例は、外部の Exchange コントロールパネル (ECP) が構成されていない場合に返されるエラー応答を示しています。
  
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

- [Exchange での EWS 操作](ews-operations-in-exchange.md)
    
- [DisableApp 操作](disableapp-operation.md)
    
- [InstallApp 操作](installapp-operation.md)
    
- [アン Installapp 操作](uninstallapp-operation.md)
    
- [GetAppManifests 操作](getappmanifests-operation.md)
    


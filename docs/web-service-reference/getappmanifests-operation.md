---
title: GetAppManifests 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 21a4987c-c24d-4a6e-ace4-e81edcda6303
description: GetAppManifests EWS 操作に関する情報を検索します。
ms.openlocfilehash: 979a09d24d0c9365a92e589aa169bebf2340411b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509918"
---
# <a name="getappmanifests-operation"></a>GetAppManifests 操作

**GetAppManifests** EWS 操作に関する情報を検索します。 
  
**GetAppManifests 操作は**、アプリ マニフェストを取得します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-getappmanifests-operation"></a>GetAppManifests 操作の使用

**GetAppManifests** 操作は、メールボックスのアプリ マニフェストを要求する引数を取らない。 応答には、メールボックスにインストールされているアプリごとに base64 エンコードされた XML マニフェスト ファイルが含まれます。 
  
### <a name="getappmanifests-operation-soap-headers"></a>GetAppManifests 操作 SOAP ヘッダー

**GetAppManifests 操作** では、次の表に示す SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**Element**|**説明**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマ バージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="getappmanifests-operation-request-example-get-the-app-manifests-for-a-mailbox"></a>GetAppManifests 操作要求の例: メールボックスのアプリ マニフェストを取得する

**GetAppManifests** 操作要求の次の例は、メールボックスのアプリ マニフェストを取得する方法を示しています。 [ApiVersionSupported 要素](apiversionsupported.md)と[SchemaVersionSupported 要素は](schemaversionsupported.md)オプションです。 
  
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
      <m:GetAppManifests>
        <m:ApiVersionSupported>1.1</m:ApiVersionSupported>
        <m:SchemaVersionSupported>1.1</m:SchemaVersionSupported>
      </m:GetAppManifests>
   </soap:Body>
</soap:Envelope>

```

要求 SOAP 本文には、次の要素が含まれます。
  
- [GetAppManifests](getappmanifests.md)
    
- [ApiVersionSupported](apiversionsupported.md)
    
- [SchemaVersionSupported](schemaversionsupported.md)
    
## <a name="successful-getappmanifests-operation-response"></a>GetAppManifests 操作応答の成功

次の例は、メールボックスのアプリ マニフェストを取得する **GetAppManifests** 操作要求に対する正常な応答を示しています。 
  
> [!NOTE]
> すべての base64 アプリ マニフェストは、読みやすさを維持するために任意に切り捨てられていました。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="07" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppManifestsResponse ResponseClass="Success" 
                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <m:Apps xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
          <t:App xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
            <t:Manifest>WNlQXBwPg==</t:Manifest>
          </t:App>
         </m:Apps>
      </GetAppManifestsResponse>
   </s:Body>
</s:Envelope>
```

応答 SOAP 本文には、次の要素が含まれています。
  
- [GetAppManifestsResponse](getappmanifestsresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [アプリ](apps.md)
    
- [アプリ](app.md)
    
- [マニフェスト](manifest.md)
    
応答 SOAP 本文には、次の要素も含まれます。
  
- [マニフェスト](manifests.md)
    
## <a name="getappmanifests-operation-error-response"></a>GetAppManifests 操作エラー応答

この操作で返されるエラーは、入力パラメーターの形式が無効であるか、汎用的な EWS エラーです。 EWS に汎用的で、この操作に固有のエラー コードについては [、「ResponseCode」を参照してください](responsecode.md)。
  
```
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="07"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetAppManifestsResponse ResponseClass="Error"
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>The apiVersionSupported parameter is invalid. 
                   It should be in the form of major version, minor 
                   version, separated by '.', for example '2.34'.</MessageText>
      <ResponseCode>ErrorInvalidRequest</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetAppManifestsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a>関連項目

- [EWS 操作 (Exchange](ews-operations-in-exchange.md)
    
- [DisableApp 操作](disableapp-operation.md)
    
- [InstallApp 操作](installapp-operation.md)
    
- [UninstallApp 操作](uninstallapp-operation.md)
    
- [GetAppMarketplaceUrl 操作](getappmarketplaceurl-operation.md)
    


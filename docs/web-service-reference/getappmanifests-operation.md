---
title: GetAppManifests 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 21a4987c-c24d-4a6e-ace4-e81edcda6303
description: 操作 GetAppManifests EWS についての情報を検索します。
ms.openlocfilehash: 9c919bac9ac0042890d1c439454b37e6b7c60876
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760625"
---
# <a name="getappmanifests-operation"></a>GetAppManifests 操作

**GetAppManifests** EWS の操作に関する情報を検索します。 
  
**GetAppManifests**操作は、アプリケーション マニフェストを取得します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-getappmanifests-operation"></a>GetAppManifests 操作を使用します。

**GetAppManifests**操作には、メールボックスのアプリケーション マニフェストを要求するすべての引数になりません。 Base64 でエンコードされた XML マニフェスト ファイル、メールボックスにインストールされている各アプリケーションの応答が含まれます。 
  
### <a name="getappmanifests-operation-soap-headers"></a>GetAppManifests 操作の SOAP ヘッダー

**GetAppManifests**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="getappmanifests-operation-request-example-get-the-app-manifests-for-a-mailbox"></a>GetAppManifests 操作の要求の例: メールボックスのアプリケーション マニフェストを取得します。

**GetAppManifests**操作要求の次の使用例では、メールボックスのアプリケーション マニフェストを取得する方法を示します。 [ApiVersionSupported](apiversionsupported.md)要素と、 [SchemaVersionSupported](schemaversionsupported.md)はオプションです。 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

要求 SOAP 本体にはには、次の要素が含まれています。
  
- [GetAppManifests](getappmanifests.md)
    
- [ApiVersionSupported](apiversionsupported.md)
    
- [SchemaVersionSupported](schemaversionsupported.md)
    
## <a name="successful-getappmanifests-operation-response"></a>GetAppManifests 操作の成功の応答

メールボックスのアプリケーション マニフェストを取得する**GetAppManifests**操作要求に正常な応答の例を次に示します。 
  
> [!NOTE]
> すべて base64 形式のアプリケーション マニフェストは、読みやすさを保持するために任意に切り捨てられました。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="07" 
                           Version="V2_10" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppManifestsResponse ResponseClass="Success" 
                               xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <m:Apps xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
          <t:App xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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
    
- [App](app.md)
    
- [Manifest](manifest.md)
    
応答 SOAP 本文には、次の要素を含めることも。
  
- [マニフェスト](manifests.md)
    
## <a name="getappmanifests-operation-error-response"></a>GetAppManifests 操作のエラー応答

この操作で返されるエラーは無効な形式の入力パラメーターに関連付けられているまたは EWS の一般的なエラーです。 EWS にジェネリックとこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。
  
```
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="07"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetAppManifestsResponse ResponseClass="Error"
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

- [Exchange での EWS の操作](ews-operations-in-exchange.md)
    
- [DisableApp 操作](disableapp-operation.md)
    
- [InstallApp 操作](installapp-operation.md)
    
- [UninstallApp 操作](uninstallapp-operation.md)
    
- [GetAppMarketplaceUrl 操作](getappmarketplaceurl-operation.md)
    


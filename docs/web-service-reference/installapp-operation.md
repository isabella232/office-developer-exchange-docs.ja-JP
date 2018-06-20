---
title: InstallApp 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 596eae95-3e78-489a-8bb2-d2dd4a026405
description: 操作 InstallApp EWS についての情報を検索します。
ms.openlocfilehash: ccc5d2dde949070bae905ff1ebb182c892f07fcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831951"
---
# <a name="installapp-operation"></a>InstallApp 操作

**InstallApp** EWS の操作に関する情報を検索します。 
  
**InstallApp**操作は、Outlook のメールボックスでのメール アプリケーションをインストールします。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-installapp-operation"></a>InstallApp 操作を使用します。

**InstallApp**操作では、インストールするのには、メール アプリケーションを識別する 1 つの引数を受け取ります。 引数には、base64 でエンコードされたメール アプリケーションのマニフェストが含まれています。 
  
### <a name="installapp-operation-soap-headers"></a>InstallApp 操作の SOAP ヘッダー

**InstallApp**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="installapp-operation-request-example-install-a-mail-app-in-a-mailbox"></a>InstallApp 操作の要求の例: メールボックスにメール アプリケーションをインストールします。

**InstallApp**操作要求の次の例では、Outlook のメール アプリケーションをインストールする方法を示します。 [GetAppManifests 操作](getappmanifests-operation.md)を使用してアプリケーション マニフェストをご覧ください。
  
> [!NOTE]
> Base64 でエンコードされたアプリケーション マニフェストは、読みやすさを保持するために任意には切り捨てられましたし、有効なマニフェストではありません。 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:InstallApp>
         <m:Manifest>TUwiIC8+CiAgPC9SdWxlPgo8L09mZmljZUFwcD4=</m:Manifest>
      </m:InstallApp>
   </soap:Body>
</soap:Envelope>

```

要求 SOAP 本体にはには、次の要素が含まれています。
  
- [InstallApp](installapp.md)
    
- [Manifest](manifest.md)
    
## <a name="successful-installapp-operation-response"></a>InstallApp 操作の成功の応答

次の例では、メール アプリケーションをインストールするのには、 **InstallApp**操作の要求に正常な応答を示します。 
  
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
      <InstallAppResponse ResponseClass="Success" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>
```

応答 SOAP 本文には、次の要素が含まれています。
  
- [InstallAppResponse](installappresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="installapp-operation-error-response"></a>InstallApp 操作のエラー応答

**InstallApp**操作要求に対するエラー応答の例を次に示します。 これは、無効なマニフェストが含まれている要求への応答です。 
  
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
      <InstallAppResponse ResponseClass="Error" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>This app can't be installed. Missing OfficeApp element.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>

```

エラー応答 SOAP 本体にはには、次の要素が含まれています。
  
- [InstallAppResponse](installappresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>関連項目

- [Exchange での EWS の操作](ews-operations-in-exchange.md)
    
- [DisableApp 操作](disableapp-operation.md)
    
- [UninstallApp 操作](uninstallapp-operation.md)
    
- [GetAppManifests](getappmanifests.md)
    
- [GetAppMarketplaceUrl 操作](getappmarketplaceurl-operation.md)
    


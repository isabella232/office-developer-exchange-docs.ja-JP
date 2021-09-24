---
title: UninstallApp 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7707aa6a-381d-43f7-a454-54f6343ed127
description: UninstallApp EWS 操作に関する情報を検索します。
ms.openlocfilehash: 8a301360b2b4c38d85e8c5be2e80c79378d0fd97
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527147"
---
# <a name="uninstallapp-operation"></a>UninstallApp 操作

**UninstallApp** EWS 操作に関する情報を検索します。 
  
**UninstallApp 操作では**、メール アプリがアンインストールOutlook。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-uninstallapp-operation"></a>UninstallApp 操作の使用

**UninstallApp 操作は**、アンインストールするメール アプリを識別する 1 つの引数を要求で受け取ります。 
  
### <a name="uninstallapp-operation-soap-headers"></a>UninstallApp 操作 SOAP ヘッダー

**UninstallApp 操作では**、次の表に示す SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**Element**|**説明**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマ バージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="uninstallapp-operation-request-example-uninstall-a-mail-app-in-a-mailbox"></a>UninstallApp 操作要求の例: メールボックス内のメール アプリをアンインストールする

**UninstallApp** 操作要求の次の例は、アプリ識別子を使用してメール アプリをアンインストールする方法を示しています。 アプリ識別子は [、GetAppManifests](getappmanifests-operation.md)操作によって返されるアプリ マニフェストで確認できます。
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:UninstallApp>
         <m:ID>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</m:ID>
      </m:UninstallApp>
   </soap:Body>
</soap:Envelope>
```

要求 SOAP 本文には、次の要素が含まれています。
  
- [UninstallApp](uninstallapp.md)
    
- [ID (String)](id-string.md)
    
## <a name="successful-uninstallapp-operation-response"></a>UninstallApp 操作の正常な応答

次の例は、メール アプリをアンインストールする **UninstallApp** 操作要求に対する正常な応答を示しています。 
  
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
      <UninstallAppResponse ResponseClass="Success" 
                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

応答 SOAP 本文には、次の要素が含まれています。
  
- [UninstallAppResponse](uninstallappresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="uninstallapp-operation-error-response"></a>UninstallApp 操作エラー応答

次の例は、UninstallApp 操作要求に対する **エラー応答を** 示しています。 これは、既にアンインストールされているメール アプリをアンインストールする要求に対する応答です。 
  
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
      <UninstallAppResponse ResponseClass="Error" 
                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1c50226d-04b5-4ab2-9fcd-42e236b59e4b can't be found.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

エラー応答 SOAP 本文には、次の要素が含まれています。
  
- [UninstallAppResponse](uninstallappresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
EWS に汎用的で、この操作に固有の追加のエラー コードについては [、「ResponseCode」を参照してください](responsecode.md)。
  
## <a name="see-also"></a>関連項目

- [EWS 操作 (Exchange](ews-operations-in-exchange.md)
    
- [InstallApp 操作](installapp-operation.md)
    
- [DisableApp 操作](disableapp-operation.md)
    
- [GetAppManifests](getappmanifests.md)
    
- [GetAppMarketplaceUrl 操作](getappmarketplaceurl-operation.md)
    


---
title: アン Installapp 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7707aa6a-381d-43f7-a454-54f6343ed127
description: アン Installapp EWS 操作に関する情報を検索します。
ms.openlocfilehash: 27931636ee13a251fb03fe804987d7b01a325230
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467152"
---
# <a name="uninstallapp-operation"></a>アン Installapp 操作

**アン Installapp** EWS 操作に関する情報を検索します。 
  
**アン installapp**操作は、Outlook 用のメールアプリをアンインストールします。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-uninstallapp-operation"></a>アン Installapp 操作の使用

**アン Installapp**操作は、アンインストールするメールアプリを識別する要求で1つの引数を取ります。 
  
### <a name="uninstallapp-operation-soap-headers"></a>アン Installapp operation SOAP ヘッダー

**アン Installapp**操作では、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは応答に適用されます。  <br/> |
   
## <a name="uninstallapp-operation-request-example-uninstall-a-mail-app-in-a-mailbox"></a>アン Installapp 操作要求の例: メールボックス内のメールアプリをアンインストールする

次の例の例では **、アプリ識別子**を使用してメールアプリをアンインストールする方法について説明します。 アプリ識別子は、 [Getappmanifests 操作](getappmanifests-operation.md)によって返されるアプリマニフェストに含まれています。
  
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
    
- [ID (文字列)](id-string.md)
    
## <a name="successful-uninstallapp-operation-response"></a>成功した Installapp 操作の応答

次の例は、メールアプリをアンインストールするための、**アン Installapp**操作要求に対する正常な応答を示しています。 
  
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
    
## <a name="uninstallapp-operation-error-response"></a>アン Installapp 操作エラー応答

次の例は、**アン Installapp**操作要求へのエラー応答を示しています。 これは、既にアンインストールされているメールアプリをアンインストールする要求に対する応答です。 
  
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
    
EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)
  
## <a name="see-also"></a>関連項目

- [Exchange での EWS 操作](ews-operations-in-exchange.md)
    
- [InstallApp 操作](installapp-operation.md)
    
- [DisableApp 操作](disableapp-operation.md)
    
- [Getappmanifests が](getappmanifests.md)
    
- [GetAppMarketplaceUrl 操作](getappmarketplaceurl-operation.md)
    


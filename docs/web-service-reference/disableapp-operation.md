---
title: DisableApp 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 211731a3-2470-49af-bda3-1ddfc15a8e46
description: DisableApp EWS 操作に関する情報を検索します。
ms.openlocfilehash: 7a4d3a13351042cc1a192388416381ebe28206bd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510156"
---
# <a name="disableapp-operation"></a>DisableApp 操作

**DisableApp** EWS 操作に関する情報を検索します。 
  
**DisableApp 操作は**、ユーザーのメール アプリを無効Outlook。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-disableapp-operation"></a>DisableApp 操作の使用

**DisableApp 操作は**、無効にするメール アプリと無効にされた理由を識別する 2 つの引数を要求で受け取ります。 
  
### <a name="disableapp-operation-soap-headers"></a>DisableApp 操作 SOAP ヘッダー

**DisableApp 操作では**、次の表に示す SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**Element**|**説明**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマ バージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="disableapp-operation-request-example-disable-a-mail-app-installed-in-a-mailbox"></a>DisableApp 操作要求の例: メールボックスにインストールされているメール アプリを無効にする

DisableApp 操作要求の次 **の例** は、メール アプリを無効にする方法を示しています。 アプリ識別子は [、GetAppManifests](getappmanifests-operation.md) 操作応答で返されるアプリ マニフェストで確認できます。 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:DisableApp>
         <m:ID>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</m:ID>
         <m:DisableReason>NoReason</m:DisableReason>
      </m:DisableApp>
   </soap:Body>
</soap:Envelope>
```

要求 SOAP 本文には、次の要素が含まれています。
  
- [DisableApp](disableapp.md)
    
- [ID (String)](id-string.md)
    
- [DisableReason](disablereason.md)
    
## <a name="successful-disableapp-operation-response"></a>DisableApp 操作の応答の成功

次の例は、メール アプリを無効にする **DisableApp** 操作要求に対する正常な応答を示しています。 
  
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
      <DisableAppResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </DisableAppResponse>
   </s:Body>
</s:Envelope>
```

応答 SOAP 本文には、次の要素が含まれています。
  
- [DisableAppResponse](disableappresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="disableapp-operation-error-response"></a>DisableApp 操作エラー応答

次の例は、DisableApp 操作要求に対する **エラー応答を** 示しています。 これは、メールボックスにインストールされていないメール アプリを無効にする要求に対する応答です。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="556" MinorBuildNumber="14" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <DisableAppResponse ResponseClass="Error" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1C50226D-04B5-4AB2-9FCD-42E236B59E4A can't be found.</MessageText>
         <ResponseCode>ErrorExtensionNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </DisableAppResponse>
   </s:Body>
</s:Envelope>
```

エラー応答 SOAP 本文には、次の要素が含まれています。
  
- [DisableAppResponse](disableappresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
EWS に汎用的で、この操作に固有の追加のエラー コードについては [、「ResponseCode」を参照してください](responsecode.md)。
  
## <a name="see-also"></a>関連項目

- [EWS 操作 (Exchange](ews-operations-in-exchange.md)   
- [InstallApp 操作](installapp-operation.md)   
- [UninstallApp 操作](uninstallapp-operation.md)   
- [GetAppManifests](getappmanifests.md)   
- [GetAppMarketplaceUrl 操作](getappmarketplaceurl-operation.md)   
- [Outlook アドイン](https://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    


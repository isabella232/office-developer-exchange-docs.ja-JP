---
title: アーカイブアイテムの操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1af216b3-13ea-498e-b4fc-23513755d731
description: アーカイブアイテム EWS 操作に関する情報を検索します。
ms.openlocfilehash: d1e18122e67c36babbc8bf01d305309e2b17b568
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463434"
---
# <a name="archiveitem-operation"></a>アーカイブアイテムの操作

**アーカイブアイテム**EWS 操作に関する情報を検索します。 
  
**アーカイブアイテム**の操作によって、アイテムがメールボックスユーザーのアーカイブメールボックスに移動されます。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-archiveitem-operation"></a>アーカイブアイテム操作の使用

アーカイブ**アイテム**操作は、アーカイブメールボックスに移動するアイテムとそれらのアイテムの宛先フォルダーに移動するアイテムを識別する2つの引数を要求で受け取ります。 この操作を動作させるには、アーカイブメールボックスを有効にする必要があります。 アーカイブメールボックスを有効にする方法については、「[インプレースアーカイブを管理](https://technet.microsoft.com/library/jj651146.aspx)する」を参照してください。
  
### <a name="archiveitem-operation-soap-headers"></a>アーカイブアイテム操作 SOAP ヘッダー

**アーカイブアイテム**操作では、次の表に示す SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアントアプリケーションが偽装しているユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066 で定義されているように、メールボックスへのアクセスに使用される**言語の識別用のタグ**を識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは応答に適用されます。  <br/> |
   
## <a name="archiveitem-operation-request-example-move-an-item-to-the-archive-inbox-folder"></a>アーカイブアイテム操作の要求例: アイテムをアーカイブ受信トレイフォルダーに移動します。

次のアーカイブ**アイテム**操作要求の例は、アイテムをアーカイブ受信トレイフォルダーに移動する方法を示しています。 
  
> [!NOTE]
> この記事のすべてのアイテム識別子と変更キーは、読みやすくするために短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body>
      <m:ArchiveItem>
         <m:ArchiveSourceFolderId>
            <t:DistinguishedFolderId Id="inbox"/>
         </m:ArchiveSourceFolderId>
         <m:ItemIds>
            <t:ItemId Id="AQMkG5BBwrQAAAxoAAAA=" ChangeKey="CQAAAHCtAAAAAAB7"/>
         </m:ItemIds>
      </m:ArchiveItem>
   </soap:Body>
</soap:Envelope>
```

要求 SOAP 本文には、次の要素が含まれています。
  
- [ArchiveItem](archiveitem.md)    
- [ArchiveSourceFolderId](archivesourcefolderid.md)    
- [DistinguishedFolderId](distinguishedfolderid.md)    
- [ItemIds](itemids.md)   
- [ItemId](itemid.md)
    
## <a name="successful-archiveitem-operation-response"></a>アーカイブアイテム操作の応答が正常に行われる

次の例は、アーカイブメールボックスにアイテムを移動するための、アーカイブ**アイテム**操作要求に対する正常な応答を示しています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:ArchiveItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:ArchiveItemResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Items/>
            </m:ArchiveItemResponseMessage>
         </m:ResponseMessages>
      </m:ArchiveItemResponse>
   </s:Body>
</s:Envelope>
```

応答 SOAP 本文には、次の要素が含まれています。
  
- [アーカイブ Itemresponse](archiveitemresponse.md)    
- [ResponseMessages](responsemessages.md)   
- [ArchiveItemResponseMessage](archiveitemresponsemessage.md)    
- [ResponseCode](responsecode.md)    
- [Items](items.md)
    
## <a name="archiveitem-operation-error-response"></a>アーカイブアイテムの操作エラー応答

次の例は、**アーカイブアイテム**操作要求へのエラー応答を示しています。 これは、アーカイブメールボックスがユーザーに対して有効になっていない場合にアイテムをアーカイブするための有効な要求に対する応答です。 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:ArchiveItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:ArchiveItemResponseMessage ResponseClass="Error">
               <m:MessageText>Archive mailbox is not enabled for this user.</m:MessageText>
               <m:ResponseCode>ErrorInvalidOperation</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:Items/>
            </m:ArchiveItemResponseMessage>
         </m:ResponseMessages>
      </m:ArchiveItemResponse>
   </s:Body>
</s:Envelope>
```

エラー応答 SOAP 本文には、次の要素が含まれています。
  
- [アーカイブ Itemresponse](archiveitemresponse.md)    
- [ResponseMessages](responsemessages.md)    
- [ArchiveItemResponseMessage](archiveitemresponsemessage.md)    
- [MessageText](messagetext.md)    
- [ResponseCode](responsecode.md)    
- [DescriptiveLinkKey](descriptivelinkkey.md)    
- [Items](items.md)
    
EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)
  
## <a name="see-also"></a>関連項目

- [Exchange での EWS 操作](ews-operations-in-exchange.md) 
- [Exchange での EWS のアーカイブ](https://msdn.microsoft.com/library/78ae179b-ae4f-4f64-911a-e0c70e0fa314%28Office.15%29.aspx)
    


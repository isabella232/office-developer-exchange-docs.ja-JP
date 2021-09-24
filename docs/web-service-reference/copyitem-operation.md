---
title: CopyItem の操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CopyItem
api_type:
- schema
ms.assetid: bcc68f9e-d511-4c29-bba6-ed535524624a
description: CopyItem 操作では、アイテムがコピーされ、アイテムが別のフォルダーに格納されます。
ms.openlocfilehash: 62785d9acb784bcffe7d3279de8a80abc803adf4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518646"
---
# <a name="copyitem-operation"></a>CopyItem の操作

**CopyItem 操作では**、アイテムがコピーされ、アイテムが別のフォルダーに格納されます。 
  
## <a name="copyitem-request-example"></a>CopyItem 要求の例

### <a name="description"></a>説明

CopyItem 要求の次 **の例** は、アイテムを受信トレイにコピーする要求を形成する方法を示しています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <ItemIds>
        <t:ItemId Id="AS4AUnV="/>
      </ItemIds>
    </CopyItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

> [!NOTE]
> フォルダー ID と変更キーは、読みやすさを維持するために短縮されました。 
  
### <a name="request-elements"></a>要求要素

要求では、次の要素が使用されます。
  
- [CopyItem](copyitem.md)
    
- [ToFolderId](tofolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
> [!NOTE]
> この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。 
  
**CopyItem** 操作の要求メッセージの他のオプションを見つけるには、スキーマ階層を確認します。 [CopyItem 要素から開始](copyitem.md)します。 
  
## <a name="successful-copyitem-response"></a>CopyItem 応答の成功

### <a name="description"></a>説明

次の例は **、CopyItem** 要求に対する正常な応答を示しています。 
  
新しいアイテムのアイテム識別子が応答メッセージに返されます。 アイテム識別子は、パブリック フォルダーの CopyItem 操作に対するクロスメールボックスまたはメールボックスに対する応答 **では返** されません。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemID Id="AAMkAd" ChangeKey="FwAAABY" />
            </t:Message>
          </m:Items>
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CopyItemResponse](copyitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CopyItemResponseMessage](copyitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items](items.md)
    
**CopyItem** 操作の応答メッセージの他のオプションを見つけるには、スキーマ階層を確認します。 [CopyItemResponse 要素から開始](copyitemresponse.md)します。 
  
## <a name="copyitem-error-response"></a>CopyItem エラー応答

### <a name="description"></a>説明

次の例は、CopyItem 要求に対するエラー **応答を示** しています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>エラー応答要素

エラー応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CopyItemResponse](copyitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CopyItemResponseMessage](copyitemresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Items](items.md)
    
**CopyItem** 操作のエラー応答メッセージの他のオプションを見つけるには、スキーマ階層を確認します。 [CopyItemResponse 要素から開始](copyitemresponse.md)します。 
  
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


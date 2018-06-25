---
title: MoveItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveItem
api_type:
- schema
ms.assetid: dcf40fa7-7796-4a5c-bf5b-7a509a18d208
description: MoveItem 操作を使用して、1 つまたは複数の項目を単一の宛先フォルダーに移動します。
ms.openlocfilehash: c5619befb02ec20ef0911992484dcc00cc2c5e92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832492"
---
# <a name="moveitem-operation"></a>MoveItem 操作

**MoveItem**操作を使用して、1 つまたは複数の項目を単一の宛先フォルダーに移動します。 
  
## <a name="moveitem-request-example"></a>MoveItem 要求の例

### <a name="description"></a>説明

**MoveItem**要求の次の例では、[下書き] フォルダーにアイテムを移動する方法を示します。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <ToFolderId>
        <t:DistinguishedFolderId Id="drafts"/>
      </ToFolderId>
      <ItemIds>
        <t:ItemId Id="AAAtAEF/swbAAA=" ChangeKey="EwAAABYA/s4b"/>
      </ItemIds>
    </MoveItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

[ToFolderId](tofolderid.md)要素は、項目の移動先フォルダーを指定します。 [Itemid](itemids.md)コレクション内のすべてのアイテムがコピー先のフォルダー終了することに注意してください。 別のインストール先のフォルダーにアイテムを配置するのには別の**MoveItem**呼び出しを行う必要があります。 
  
> [!NOTE]
> 項目の識別子と変更キーは、読みやすさを保持するために短縮されています。 
  
### <a name="request-elements"></a>要素を要求します。

次の要素は、要求で使用されます。
  
- [MoveItem](moveitem.md)
    
- [ToFolderId](tofolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [Itemid](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="moveitem-response-example"></a>MoveItem 応答の例

### <a name="description"></a>説明

**MoveItem**要求に正常な応答の例を次に示します。 
  
応答メッセージでは、新しい項目の項目の識別子が返されます。 **MoveItem**操作のパブリック フォルダーには、応答間のメールボックスまたはメールボックスのアイテム識別子は返されません。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <MoveItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemID Id="AAMkAd" ChangeKey="FwAAABY" />
            </t:Message>
          </m:Items>
        </m:MoveItemResponseMessage>
      </m:ResponseMessages>
    </MoveItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

移動が成功した場合、 **MoveItem**操作は成功を示します。 
  
### <a name="successful-response-elements"></a>正常な応答の要素

次の要素は、応答で使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [MoveItemResponse](moveitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MoveItemResponseMessage](moveitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items](items.md)
    
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


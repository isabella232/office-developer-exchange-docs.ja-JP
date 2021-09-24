---
title: CopyItem
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
ms.assetid: ffb4c13e-e7ea-4e6b-87a0-509ce5371100
description: CopyItem 要素は、アイテム ストア内のメールボックス内のアイテムをコピーする要求をExchangeします。
ms.openlocfilehash: 7f083f09a587b4788180711039e1cfdbbe6a10cd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529177"
---
# <a name="copyitem"></a>CopyItem

**CopyItem 要素は**、アイテム ストア内のメールボックス内のアイテムをコピーする要求Exchangeします。 
  
```XML
<CopyItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</CopyItem>
```

 **CopyItemType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ToFolderId](tofolderid.md) <br/> |コピーされたアイテムの移動先フォルダーを表します。  <br/> |
|[ItemIds](itemids.md) <br/> |[ToFolderId](tofolderid.md)要素で表されるフォルダーにコピーする、識別されたアイテムの配列を格納します。  <br/> |
|[ReturnNewItemIds](returnnewitemids.md) <br/> |新しいアイテムのアイテム識別子が応答で返されるかどうかを示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[CopyItem 操作](copyitem-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


---
title: CopyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItem
api_type:
- schema
ms.assetid: ffb4c13e-e7ea-4e6b-87a0-509ce5371100
description: CopyItem 要素は、Exchange ストア内のメールボックス内のアイテムをコピーする要求を定義します。
ms.openlocfilehash: b9af1670fd580107de08ad3b950191399436388d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458503"
---
# <a name="copyitem"></a>CopyItem

**Copyitem**要素は、Exchange ストア内のメールボックス内のアイテムをコピーする要求を定義します。 
  
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
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目




  [CopyItem 操作](copyitem-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


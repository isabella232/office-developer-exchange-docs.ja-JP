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
description: CopyItem 要素は、Exchange ストア内のメールボックスにアイテムをコピーするための要求を定義します。
ms.openlocfilehash: 08cc1b67f7c7d369263acfc4b3d13e8aa70d2d5f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759784"
---
# <a name="copyitem"></a>CopyItem

**CopyItem**要素は、Exchange ストア内のメールボックスにアイテムをコピーするための要求を定義します。 
  
```XML
<CopyItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</CopyItem>
```

 **CopyItemType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ToFolderId](tofolderid.md) <br/> |コピーされたアイテムのコピー先フォルダーを表します。  <br/> |
|[Itemid](itemids.md) <br/> |[ToFolderId](tofolderid.md)要素によって表されるフォルダーにコピーするのには特定の項目の配列が含まれています。  <br/> |
|[ReturnNewItemIds](returnnewitemids.md) <br/> |新しい項目の項目の識別子が応答で返されるかどうかを示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [CopyItem 操作](copyitem-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


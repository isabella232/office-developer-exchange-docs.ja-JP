---
title: MoveItem
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
ms.assetid: a4593377-22dd-415f-b01d-387389ef650f
description: MoveItem 要素は、Exchange ストア内のアイテムを移動する要求を定義します。
ms.openlocfilehash: cd7f35bdabe8a596f4c186df1c8cd54e0ea1c540
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832486"
---
# <a name="moveitem"></a>MoveItem

**MoveItem**要素は、Exchange ストア内のアイテムを移動する要求を定義します。 
  
```XML
<MoveItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</MoveItem>
```

 **MoveItemType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ToFolderId](tofolderid.md) <br/> |移動された項目のコピー先フォルダーを表します。  <br/> |
|[Itemid](itemids.md) <br/> |[ToFolderId](tofolderid.md)要素によって表されるフォルダーに移動する特定の項目の配列が含まれています。  <br/> |
|[ReturnNewItemIds](returnnewitemids.md) <br/> |新しい項目の項目の識別子が応答で返されるかどうかを示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

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




  [MoveItem 操作](moveitem-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


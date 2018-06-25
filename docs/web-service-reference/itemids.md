---
title: ItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemIds
api_type:
- schema
ms.assetid: 6b82122b-5544-4adf-91b7-ef2db7d5046f
description: Itemid の要素には、アイテム、出現アイテム、および削除、送信、取得、移動、または Exchange ストア内のアイテムのコピーに使用される、マスターの定期的なアイテムの一意の id が含まれています。
ms.openlocfilehash: 1bd4d6f4593a7c3b418561269d8b29707cc6030c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832155"
---
# <a name="itemids"></a>ItemIds
  
**Itemid**の要素には、アイテム、出現アイテム、および削除、送信、取得、移動、または Exchange ストア内のアイテムのコピーに使用される、マスターの定期的なアイテムの一意の id が含まれています。
  
```xml
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

**NonEmptyArrayOfBaseItemIdsType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。 
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |定期的なアイテムの 1 回の発生を識別します。  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |関連の出現アイテムの id のいずれかを識別することによって、定期的な予定のマスター アイテムを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[会話 (ConversationType)](conversation-conversationtype.md) <br/> |1 つのテーマを表します。  <br/> |
|[DeleteItem](deleteitem.md) <br/> |Exchange ストア内の項目を削除する要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/DeleteItem` <br/> |
|[SendItem](senditem.md) <br/> |Exchange ストア内のアイテムを送信する要求を定義するルート要素です。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/SendItem` <br/> |
|[GetItem](getitem.md) <br/> |Exchange ストアから項目を取得する要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/GetItem` <br/> |
|[MoveItem](moveitem.md) <br/> |Exchange ストア内のアイテムを移動するための要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Exchange ストア内のアイテムをコピーするための要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/CopyItem` <br/> |
   
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

- [DeleteItem の操作](deleteitem-operation.md)
- 
  [SendItem 操作](senditem-operation.md) 
- 
  [GetItem 操作](getitem-operation.md)
- 
  [MoveItem 操作](moveitem-operation.md)
- 
  [CopyItem 操作](copyitem-operation.md)
- 
  [FindConversation 操作](findconversation-operation.md)


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
description: ItemIds 要素には、アイテム、発生アイテム、および定期的なマスターアイテムの一意の id が含まれており、Exchange ストア内のアイテムの削除、送信、取得、移動、またはコピーに使用できます。
ms.openlocfilehash: bbd594ce2610bd625b0e16a0383fda552ee9eb19
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460604"
---
# <a name="itemids"></a>ItemIds
  
**Itemids**要素には、アイテム、発生アイテム、および定期的なマスターアイテムの一意の id が含まれており、Exchange ストア内のアイテムの削除、送信、取得、移動、またはコピーに使用できます。
  
```xml
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

**非 Emptyarrayofbaseitemidstype**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。 
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |定期的なアイテムの1回の出現を識別します。  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |関連するオカレンスアイテムの識別子の1つを識別することによって、定期的なアイテムのマスターアイテムを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[会話 (ConversationType)](conversation-conversationtype.md) <br/> |単一の会話を表します。  <br/> |
|[DeleteItem](deleteitem.md) <br/> |Exchange ストア内のアイテムを削除するための要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/DeleteItem` <br/> |
|[SendItem](senditem.md) <br/> |Exchange ストア内のアイテムを送信するための要求を定義するルート要素です。  <br/> この要素の XPath 式を次に示します。  <br/>  `/SendItem` <br/> |
|[GetItem](getitem.md) <br/> |Exchange ストアからアイテムを取得するための要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/GetItem` <br/> |
|[MoveItem](moveitem.md) <br/> |Exchange ストア内のアイテムを移動する要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Exchange ストア内のアイテムをコピーするための要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/CopyItem` <br/> |
   
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

- [DeleteItem 操作](deleteitem-operation.md)
- [SendItem 操作](senditem-operation.md) 
- [GetItem 操作](getitem-operation.md)
- [MoveItem 操作](moveitem-operation.md)
- [CopyItem 操作](copyitem-operation.md)
- [FindConversation 操作](findconversation-operation.md)


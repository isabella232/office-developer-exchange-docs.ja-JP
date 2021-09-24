---
title: ItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ItemIds
api_type:
- schema
ms.assetid: 6b82122b-5544-4adf-91b7-ef2db7d5046f
description: ItemIds 要素には、Exchange ストア内のアイテムの削除、送信、取得、移動、またはコピーに使用されるアイテム、オカレンス アイテム、および定期的なマスター アイテムの一意の ID が含まれます。
ms.openlocfilehash: 7341b8214b4d61564bd87707a9d8c76fbca07628
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522888"
---
# <a name="itemids"></a>ItemIds
  
**ItemIds** 要素には、Exchange ストア内のアイテムの削除、送信、取得、移動、またはコピーに使用されるアイテム、オカレンス アイテム、および定期的なマスター アイテムの一意の ID が含まれます。
  
```xml
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

**NonEmptyArrayOfBaseItemIdsType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。 
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |ストア内のアイテムの一意の識別子と変更キー Exchangeします。  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |定期的なアイテムの 1 回の出現を識別します。  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |関連するアイテムの識別子の 1 つを識別して、定期的なマスター アイテムを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |1 つの会話を表します。  <br/> |
|[DeleteItem](deleteitem.md) <br/> |ストア内のアイテムを削除する要求をExchangeします。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/DeleteItem` <br/> |
|[SendItem](senditem.md) <br/> |ストア内のアイテムを送信する要求を定義するルートExchangeです。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/SendItem` <br/> |
|[GetItem](getitem.md) <br/> |ストアからアイテムを取得する要求をExchangeします。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/GetItem` <br/> |
|[MoveItem](moveitem.md) <br/> |ストア内のアイテムを移動する要求をExchangeします。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |ストア内のアイテムをコピーする要求をExchangeします。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/CopyItem` <br/> |
   
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

- [DeleteItem 操作](deleteitem-operation.md)
- [SendItem 操作](senditem-operation.md) 
- [GetItem 操作](getitem-operation.md)
- [MoveItem 操作](moveitem-operation.md)
- [CopyItem 操作](copyitem-operation.md)
- [FindConversation 操作](findconversation-operation.md)


---
title: OccurrenceItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- OccurrenceItemId
api_type:
- schema
ms.assetid: 4a15bbc3-5b93-4193-b9ec-da32f0a9a552
description: OccurrenceItemId 要素は、定期的なアイテムの 1 回の出現を識別します。
ms.openlocfilehash: ac6fc081e67f3897880ad30fcc1b62fe2e844459
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515419"
---
# <a name="occurrenceitemid"></a>OccurrenceItemId

**OccurrenceItemId 要素** は、定期的なアイテムの 1 回の出現を識別します。 
  
```XML
<OccurrenceItemId RecurringMasterId="" ChangeKey="" InstanceIndex=""/>
```

**OccurrenceItemIdType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**RecurringMasterId** <br/> |定期的なアイテムの定期的なマスターを識別します。 この属性は必須です。  <br/> |
|**ChangeKey** <br/> |定期的なマスターまたはアイテムの出現の特定のバージョンを識別します。 定期的なマスターまたは発生するマスターが変更された場合は **、ChangeKey が変更** されます。 **ChangeKey は**、定期的なマスターとすべてのオカレンスで同じです。  <br/> |
|**InstanceIndex** <br/> |アイテムの出現のインデックスを識別します。 この属性は必須です。 この値は整数を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |メールボックス内のすべての会話アイテムのアイテム識別子のコレクションを格納します。  <br/> |
|[ItemIds](itemids.md) <br/> | Exchange ストア内のアイテムの削除、送信、取得、移動、またはコピーに使用されるアイテム、オカレンス アイテム、および定期的なマスター アイテムの一意の ID をExchangeします。 <br/><br/>この要素の XPath 式を次に示します。 <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/>**メモ**: [MoveItem 操作と](moveitem-operation.md) [CopyItem 操作は、](copyitem-operation.md) 単一の予定表アイテムと定期的なマスター アイテムでのみ機能します。 アイテムの出現は、これらの操作では無効です。           |
|[ItemChange](itemchange.md) <br/> |アイテム識別子とアイテムに適用する更新プログラムが含まれています。<br/><br/> 次に、この要素の XPath 式を示します。  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

次の例は、ID 34vswe4 を持つ定期的なアイテムの 4 番目の出現を識別します。
  
```XML
<OccurrenceItemId RecurringMasterId="34vswe4" InstanceIndex="4" />
```

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [RecurringMasterItemId](recurringmasteritemid.md)
- [FindConversation 操作](findconversation-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


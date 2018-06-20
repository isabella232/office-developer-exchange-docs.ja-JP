---
title: OccurrenceItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OccurrenceItemId
api_type:
- schema
ms.assetid: 4a15bbc3-5b93-4193-b9ec-da32f0a9a552
description: OccurrenceItemId 要素は、定期的なアイテムの 1 回の発生を識別します。
ms.openlocfilehash: e3d7b6efc49775f54219ce0dc0ec39a34a95f8fd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832639"
---
# <a name="occurrenceitemid"></a>OccurrenceItemId

**OccurrenceItemId**要素は、定期的なアイテムの 1 回の発生を識別します。 
  
```XML
<OccurrenceItemId RecurringMasterId="" ChangeKey="" InstanceIndex=""/>
```

**OccurrenceItemIdType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**RecurringMasterId** <br/> |定期的なアイテムの定期的なマスターを識別します。 この属性は、必要があります。  <br/> |
|**変更キー** <br/> |定期的なマスターか、アイテムの特定のバージョンを識別します。 定期的なマスターまたはその項目のいずれかのいずれかを変更する場合は、**変更キー**が変更されます。 **変更キー**は、定期的なマスターとすべて同じです。  <br/> |
|**InstanceIndex** <br/> |アイテムの出現するインデックス位置を識別します。 この属性は、必要があります。 この値は、整数を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |メールボックス内のすべての会話項目の項目の識別子のコレクションが含まれています。  <br/> |
|[Itemid](itemids.md) <br/> | アイテム、出現アイテム、および削除、送信、取得、移動、または Exchange ストア内のアイテムのコピーに使用される、マスターの定期的なアイテムの一意の id が含まれています。 <br/><br/>この要素への XPath 式は、次のように。 <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/>**注**: [MoveItem 操作](moveitem-operation.md)および[CopyItem の操作](copyitem-operation.md)が 1 つの予定表アイテムと定期的なアイテムをマスターでのみ動作します。 アイテムの出現回数は、これらの操作では無効です。           |
|[ItemChange](itemchange.md) <br/> |アイテム識別子と、アイテムに適用する更新プログラムが含まれています。<br/><br/> この要素への XPath 式は、次のようにします。  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

次の例では、4 番目の id 34vswe4 を持つ定期的なアイテムの発生を識別します。
  
```XML
<OccurrenceItemId RecurringMasterId="34vswe4" InstanceIndex="4" />
```

## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [RecurringMasterItemId](recurringmasteritemid.md)
- 
  [FindConversation 操作](findconversation-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


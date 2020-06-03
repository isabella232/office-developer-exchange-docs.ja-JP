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
description: OccurrenceItemId 要素は、定期的なアイテムの単一のオカレンスを識別します。
ms.openlocfilehash: 37c3a2442afb3302bca88ef0301e98013ff0319b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468377"
---
# <a name="occurrenceitemid"></a>OccurrenceItemId

**OccurrenceItemId**要素は、定期的なアイテムの単一のオカレンスを識別します。 
  
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
|**ChangeKey** <br/> |特定のバージョンの定期的なマスターまたはアイテムの発生を識別します。 定期的マスターまたはそのいずれかのオカレンスが変更された場合は、 **Changekey**が変更されます。 **Changekey**は、定期的なマスターとすべてのオカレンスで同じです。  <br/> |
|**InstanceIndex** <br/> |アイテムのオカレンスのインデックスを識別します。 この属性は必須です。 この値は、整数を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |メールボックス内のすべての会話アイテムのアイテム識別子のコレクションが含まれています。  <br/> |
|[ItemIds](itemids.md) <br/> | Exchange ストア内のアイテムの削除、送信、取得、移動、またはコピーに使用されるアイテム、オカレンスアイテム、定期的なマスターアイテムの一意の id が含まれています。 <br/><br/>この要素の XPath 式は次のとおりです。 <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/>**注**: [Moveitem](moveitem-operation.md)操作と[copyitem 操作](copyitem-operation.md)は、1つの予定表アイテムおよび定期的なマスターアイテムに対してのみ機能します。 アイテムの出現は、これらの操作では無効です。           |
|[ItemChange](itemchange.md) <br/> |アイテム識別子と、アイテムに適用する更新を含みます。<br/><br/> この要素の XPath 式を次に示します。  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

次の例では、id が34vswe4 である定期的なアイテムの4番目の発生を識別します。
  
```XML
<OccurrenceItemId RecurringMasterId="34vswe4" InstanceIndex="4" />
```

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [RecurringMasterItemId](recurringmasteritemid.md)
- [FindConversation 操作](findconversation-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


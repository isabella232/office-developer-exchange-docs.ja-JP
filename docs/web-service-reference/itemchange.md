---
title: ItemChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemChange
api_type:
- schema
ms.assetid: 5cb43b02-d444-4d9c-9075-cdc5a4427daf
description: ItemChange 要素には、アイテムの識別子と、アイテムに適用する更新が含まれています。
ms.openlocfilehash: 916ef1ba2c7a709ec1fd80ababd72999506773c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459918"
---
# <a name="itemchange"></a>ItemChange

**Itemchange**要素には、アイテムの識別子と、アイテムに適用する更新が含まれています。 
  
- [UpdateItem](updateitem.md) 
- [ItemChanges](itemchanges.md)
- [ItemChange](itemchange.md)
  
```xml
<ItemChange>
   <ItemId/>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <OccurrenceItemId>...</OccurrenceItemId>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <RecurringMasterItemId>...</RecurringMasterItemId>
   <Updates>...</Updates>
</ItemChange>
```

**ItemChangeType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。 この要素は、 [OccurrenceItemId](occurrenceitemid.md)または[RecurringMasterItemId](recurringmasteritemid.md)要素が使用されていない場合に必要です。  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |定期的なアイテムの1回の出現を識別します。 この要素は、使用する場合は必須です。 この要素は、 [RecurringMasterItemId](recurringmasteritemid.md)または[ItemId](itemid.md)要素が使用されていない場合に必要です。  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |関連するオカレンスアイテムの識別子の1つを識別することによって、定期的なアイテムのマスターアイテムを識別します。 この要素は、使用する場合は必須です。 この要素は、 [OccurrenceItemId](occurrenceitemid.md)または[ItemId](itemid.md)要素が使用されていない場合に必要です。  <br/> |
|[Updates (Item)](updates-item.md) <br/> |アイテムのプロパティに対する追加、設定、および削除の変更を定義する配列を格納します。 この要素は必須です。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemChanges](itemchanges.md) <br/> |アイテムとアイテムに適用する更新を識別する[Itemchange](itemchange.md)要素の配列が含まれています。  <br/> この要素の XPath 式を次に示します。  <br/>  `/UpdateItem/ItemChanges` <br/> |
   
## <a name="remarks"></a>注釈

**Itemchange**要素に使用できる[ItemId](itemid.md)、 [OccurrenceItemId](occurrenceitemid.md)、または[RecurringMasterItemId](recurringmasteritemid.md)要素は1つだけです。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [UpdateItem 操作](updateitem-operation.md)


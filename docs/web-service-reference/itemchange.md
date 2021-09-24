---
title: ItemChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ItemChange
api_type:
- schema
ms.assetid: 5cb43b02-d444-4d9c-9075-cdc5a4427daf
description: ItemChange 要素には、アイテム識別子とアイテムに適用する更新プログラムが含まれています。
ms.openlocfilehash: 8ace3cf78eb902e48529a0534e39ce7d584bd164
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537750"
---
# <a name="itemchange"></a>ItemChange

**ItemChange 要素** には、アイテム識別子とアイテムに適用する更新プログラムが含まれています。 
  
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
|[ItemId](itemid.md) <br/> |ストア内のアイテムの一意の識別子と変更キー Exchangeします。 この要素は [、OccurrenceItemId](occurrenceitemid.md) または [RecurringMasterItemId](recurringmasteritemid.md) 要素が使用されていない場合に必要です。  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |定期的なアイテムの 1 回の出現を識別します。 この要素は、使用する場合に必要です。 この要素は [、RecurringMasterItemId](recurringmasteritemid.md) または [ItemId](itemid.md) 要素が使用されない場合に必要です。  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |関連するアイテムの識別子の 1 つを識別して、定期的なマスター アイテムを識別します。 この要素は、使用する場合に必要です。 この要素は [、OccurrenceItemId](occurrenceitemid.md) または [ItemId](itemid.md) 要素が使用されない場合に必要です。  <br/> |
|[Updates (Item)](updates-item.md) <br/> |アイテムプロパティの追加、設定、および削除の変更を定義する配列を含みます。 この要素は必須です。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemChanges](itemchanges.md) <br/> |アイテムとアイテムに適用する更新プログラムを識別する [ItemChange](itemchange.md) 要素の配列を格納します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/UpdateItem/ItemChanges` <br/> |
   
## <a name="remarks"></a>注釈

ItemChange 要素で使用できるのは、単一の[ItemId、OccurrenceItemId、](occurrenceitemid.md)または[](itemid.md)[RecurringMasterItemId](recurringmasteritemid.md)要素のみです。  
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [UpdateItem 操作](updateitem-operation.md)


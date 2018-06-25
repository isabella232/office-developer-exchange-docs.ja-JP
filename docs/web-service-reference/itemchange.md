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
description: ItemChange 要素には、項目 id と、アイテムに適用する更新プログラムが含まれています。
ms.openlocfilehash: d10ce96cacb0be7411c4e8230ebc9b2803b7a5b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832145"
---
# <a name="itemchange"></a>ItemChange

**ItemChange**要素には、項目 id と、アイテムに適用する更新プログラムが含まれています。 
  
[UpdateItem](updateitem.md)
  
[ItemChanges](itemchanges.md)
  
[ItemChange](itemchange.md)
  
```xml
<ItemChange>
   <ItemId/>
   <Updates>...</Updates>
</ItemChange>
```

 **ItemChangeType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。 [OccurrenceItemId](occurrenceitemid.md)または[RecurringMasterItemId](recurringmasteritemid.md)要素を使用しない場合、この要素が必要です。  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |定期的なアイテムの 1 回の発生を識別します。 使用する場合、この要素が必要です。 [RecurringMasterItemId](recurringmasteritemid.md)または[アイテム Id](itemid.md)要素を使用しない場合、この要素が必要です。  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |関連の出現アイテムの id のいずれかを識別することによって、定期的な予定のマスター アイテムを識別します。 使用する場合、この要素が必要です。 [OccurrenceItemId](occurrenceitemid.md)または[アイテム Id](itemid.md)要素を使用しない場合、この要素が必要です。  <br/> |
|[更新 (アイテム)](updates-item.md) <br/> |定義する配列が含まれていて、このオプションを設定すると、アイテムのプロパティの変更を削除します。 この要素は必須です。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemChanges](itemchanges.md) <br/> |アイテムと、アイテムに適用する更新プログラムを識別する[ItemChange](itemchange.md)要素の配列が含まれています。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/UpdateItem/ItemChanges` <br/> |
   
## <a name="remarks"></a>備考

**ItemChange**要素では、唯一の[アイテム Id](itemid.md)、 [OccurrenceItemId](occurrenceitemid.md)、または[RecurringMasterItemId](recurringmasteritemid.md)要素を使用できます。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [UpdateItem 操作](updateitem-operation.md)


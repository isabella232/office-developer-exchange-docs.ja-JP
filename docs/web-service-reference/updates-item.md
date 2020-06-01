---
title: Updates (Item)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Updates
api_type:
- schema
ms.assetid: 5c1a855e-390d-4713-9d10-6e86ca392814
description: Updates 要素には、アイテムのプロパティに対する追加、設定、および削除の変更を定義する一連の要素が含まれています。
ms.openlocfilehash: 6902ea4d3d3d9adc074745d5642cdfa6d91a9163
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456354"
---
# <a name="updates-item"></a>Updates (Item)

**Updates**要素には、アイテムのプロパティに対する追加、設定、および削除の変更を定義する一連の要素が含まれています。 
  
- [UpdateItem](updateitem.md)
  
- [ItemChanges](itemchanges.md)
  
- [ItemChange](itemchange.md)
  
- [Updates (Item)](updates-item.md)
  
```xml
<Updates>
   <AppendToItemField/>
   <SetItemField/>
   <DeleteItemField/>
</Updates>
```

**NonEmptyArrayOfItemChangeDescriptionsType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[AppendToItemField](appendtoitemfield.md) <br/> |[Updateitem 操作](updateitem-operation.md)中に、アイテムの1つのプロパティに追加するデータを表します。  <br/> |
|[SetItemField](setitemfield.md) <br/> |[Updateitem 操作](updateitem-operation.md)のアイテムの1つのプロパティに対する更新を表します。  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |[Updateitem 操作](updateitem-operation.md)中に、指定されたプロパティをアイテムから削除する操作を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemChange](itemchange.md) <br/> |アイテム識別子と、アイテムに適用する更新を含みます。  <br/> この要素の XPath 式を次に示します。`/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="remarks"></a>注釈

この要素によって定義された更新は、 [ItemId](itemid.md)、 [OccurrenceItemId](occurrenceitemid.md)、または[RecurringMasterItemId](recurringmasteritemid.md)要素によって識別されるアイテムに対して実行されます。 
  
この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- 
  [UpdateItem 操作](updateitem-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


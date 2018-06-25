---
title: 更新 (アイテム)
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
description: 更新プログラムの要素には、定義する要素のセットが含まれていて、このオプションを設定すると、アイテムのプロパティの変更を削除します。
ms.openlocfilehash: 13df458c783b942e1c868853c41b6247119cf123
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839890"
---
# <a name="updates-item"></a>更新 (アイテム)

**更新プログラム**の要素には、定義する要素のセットが含まれていて、このオプションを設定すると、アイテムのプロパティの変更を削除します。 
  
- [UpdateItem](updateitem.md)
  
- [ItemChanges](itemchanges.md)
  
- [ItemChange](itemchange.md)
  
- [更新 (アイテム)](updates-item.md)
  
```xml
<Updates>
   <AppendToItemField/>
   <SetItemField/>
   <DeleteItemField/>
</Updates>
```

**NonEmptyArrayOfItemChangeDescriptionsType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[AppendToItemField](appendtoitemfield.md) <br/> |[UpdateItem 操作](updateitem-operation.md)中に 1 つのアイテムのプロパティを追加するデータを表します。  <br/> |
|[SetItemField](setitemfield.md) <br/> |[UpdateItem 操作](updateitem-operation.md)内の項目の 1 つのプロパティには、更新プログラムを表します。  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |[UpdateItem 操作](updateitem-operation.md)中に、アイテムから指定されたプロパティを削除する操作を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemChange](itemchange.md) <br/> |アイテム識別子と、アイテムに適用する更新プログラムが含まれています。  <br/> この要素への XPath 式は、次のようにします。`/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="remarks"></a>備考

[アイテム Id](itemid.md)、 [OccurrenceItemId](occurrenceitemid.md)、または[RecurringMasterItemId](recurringmasteritemid.md)の要素で識別される項目には、この要素で定義されている更新プログラムが実行されます。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- 
  [UpdateItem 操作](updateitem-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


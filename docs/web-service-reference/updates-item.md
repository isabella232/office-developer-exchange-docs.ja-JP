---
title: Updates (Item)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Updates
api_type:
- schema
ms.assetid: 5c1a855e-390d-4713-9d10-6e86ca392814
description: Updates 要素には、アイテムのプロパティに対する追加、設定、および削除の変更を定義する一連の要素が含まれています。
ms.openlocfilehash: b4a343d941d29e9b25ebedfbf25894c7ec9b22d7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517407"
---
# <a name="updates-item"></a>Updates (Item)

**Updates 要素には**、アイテムのプロパティに対する追加、設定、および削除の変更を定義する一連の要素が含まれています。 
  
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
|[AppendToItemField](appendtoitemfield.md) <br/> |UpdateItem 操作中にアイテムの 1 つのプロパティに追加する [データを表します](updateitem-operation.md)。  <br/> |
|[SetItemField](setitemfield.md) <br/> |UpdateItem 操作内のアイテムの 1 つのプロパティへの更新 [を表します](updateitem-operation.md)。  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |UpdateItem 操作中にアイテムから特定のプロパティを削除する [操作を表します](updateitem-operation.md)。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemChange](itemchange.md) <br/> |アイテム識別子とアイテムに適用する更新プログラムが含まれています。  <br/> 次に、この要素の XPath 式を示します。  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="remarks"></a>注釈

この要素によって定義される更新は[、ItemId、OccurrenceItemId、](occurrenceitemid.md)[または RecurringMasterItemId](recurringmasteritemid.md)要素によって識別されるアイテムに対して実行されます。 [](itemid.md) 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [UpdateItem 操作](updateitem-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


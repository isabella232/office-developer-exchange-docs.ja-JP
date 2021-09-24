---
title: ItemChanges
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ItemChanges
api_type:
- schema
ms.assetid: cd307892-2f69-4494-8325-219bdb5c3ad5
description: ItemChanges 要素には、アイテムを識別する ItemChange 要素の配列と、アイテムに適用する更新プログラムが含まれます。
ms.openlocfilehash: 69a90f7bce330910b9ff44c63656f38509438981
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516686"
---
# <a name="itemchanges"></a>ItemChanges

**ItemChanges 要素には**、アイテムを識別する [ItemChange](itemchange.md)要素の配列と、アイテムに適用する更新プログラムが含まれます。 
  
[UpdateItem](updateitem.md)
  
[ItemChanges](itemchanges.md)
  
```xml
<ItemChanges>
   <ItemChange/>
</ItemChanges>
```

 **NonEmptyArrayOfItemChangesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ItemChange](itemchange.md) <br/> |アイテム識別子とアイテムに適用する更新プログラムが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[UpdateItem](updateitem.md) <br/> |メールボックス内のアイテムを更新する要求を定義します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/UpdateItem` <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[UpdateItem 操作](updateitem-operation.md)


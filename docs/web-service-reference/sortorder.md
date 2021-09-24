---
title: SortOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SortOrder
api_type:
- schema
ms.assetid: c2413f0b-8c03-46ae-9990-13338b3c53a6
description: SortOrder 要素は、FindItem または FindConversation 要求でアイテムを並べ替える方法を定義します。
ms.openlocfilehash: eefa10c4af32d550414d83f8f524b5b088fcfa7c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531702"
---
# <a name="sortorder"></a>SortOrder

**SortOrder 要素** は、FindItem または **FindConversation** 要求でアイテムを並べ替える方法を定義します。  
  
```xml
<SortOrder>
   <FieldOrder/>
</SortOrder>
```

 **NonEmptyArrayOfFieldOrdersType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FieldOrder](fieldorder.md) <br/> |結果を並べ替える 1 つのフィールドを表し、並べ替えの方向を示します。 これらの要素の 1 つ以上が含まれる場合があります。 [FieldOrder](fieldorder.md) 要素は、並べ替えに指定された順序で適用されます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索する要求を定義します。  <br/> 次に、この要素の XPath 式を示します。  `/FindItem` <br/> |
|[FindConversation](findconversation.md) <br/> |メールボックス内の会話を検索する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[FindItem 操作](finditem-operation.md)
  
[FindConversation 操作](findconversation-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


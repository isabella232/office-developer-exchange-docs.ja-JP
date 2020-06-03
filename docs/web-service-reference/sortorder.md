---
title: SortOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SortOrder
api_type:
- schema
ms.assetid: c2413f0b-8c03-46ae-9990-13338b3c53a6
description: 並べ替え要素は、FindItem または FindConversation 会話要求でアイテムを並べ替える方法を定義します。
ms.openlocfilehash: b520bb3ca6daadc777e7235b2b7420a12e425048
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468370"
---
# <a name="sortorder"></a>SortOrder

並べ替え**要素は**、 **FindItem**または**findconversation 会話**要求でアイテムを並べ替える方法を定義します。 
  
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
|[FieldOrder](fieldorder.md) <br/> |結果を並べ替えるための1つのフィールドを表し、並べ替えの方向を示します。 これらの要素の1つ以上を含めることができます。 [Fieldorder](fieldorder.md)要素は、並べ替えに指定された順序で適用されます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索するための要求を定義します。  <br/> この要素の XPath 式を次に示します。`/FindItem` <br/> |
|[FindConversation](findconversation.md) <br/> |メールボックス内のスレッドを検索する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[FindItem 操作](finditem-operation.md)
  
[FindConversation 操作](findconversation-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


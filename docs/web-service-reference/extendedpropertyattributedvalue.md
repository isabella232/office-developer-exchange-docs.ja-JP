---
title: ExtendedPropertyAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 90f3c5c5-f612-4e1b-b1f5-f92dd8524179
description: ExtendedPropertyAttributedValue 要素は、ペルシャの拡張プロパティを指定します。
ms.openlocfilehash: 338c2a12d89cd7b1305be2fc75692782b1b3a466
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535381"
---
# <a name="extendedpropertyattributedvalue"></a>ExtendedPropertyAttributedValue

**ExtendedPropertyAttributedValue** 要素は、ペルシャの拡張プロパティを指定します。 
  
```XML
<ExtendedPropertyAttributedValue>
    <Value/>
    <Attributions/>
</ExtendedPropertyAttributedValue>
```

 **ExtendedPropertyAttributedValueType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Value (ExtendedPropertyType)](value-extendedpropertytype.md) <br/> |ペルサの拡張プロパティの配列を指定します。  <br/> |
|[Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md) <br/> |関連付けられた Value 要素の属性の配列を **指定** します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)](extendedproperties-arrayofextendedpropertyattributedvaluetype.md) <br/> |統合連絡先ストア操作に使用される拡張プロパティが含まれます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


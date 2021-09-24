---
title: CarPhones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ad096246-113c-42ea-9e63-861b546003e8
description: CarPhone 要素は、自動車の電話番号の配列と、関連付けられたペルサのソース属性の識別子を指定します。
ms.openlocfilehash: dedcaa3403945c12c1717c1d7fb0f995cacaf267
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518813"
---
# <a name="carphones"></a>CarPhones

**CarPhone 要素は**、自動車の電話番号の配列と、関連付けられたペルサのソース属性の識別子を指定します。 
  
```XML
<CarPhones>
    <Value></Value>
    <Attributions></Attributions>
</CarPhones>
```

 **ArrayOfPhoneNumberAttributedValuesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Value (PersonaPhoneNumberType)](value-personaphonenumbertype.md) <br/> |電話番号と種類の情報を指定し、属性のセットに関連付けられる。  <br/> |
|[Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md) <br/> |関連付けられた Value 要素の属性の配列を **指定** します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ユーザー](persona.md) <br/> |**GetPersona** 要求によって返されるペルソナ データのセットを指定します。  <br/> |
   
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


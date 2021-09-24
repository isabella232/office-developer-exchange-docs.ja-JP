---
title: EmailAddressAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ebdf224d-3796-4179-aa0a-87942e7585ff
description: EmailAddressAttributedValue 要素は、電子メール アドレスの配列とその関連付けられた属性のインスタンスを指定します。
ms.openlocfilehash: 2b5e9b431b6a62c63e815bfee190c923f454c867
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519766"
---
# <a name="emailaddressattributedvalue"></a>EmailAddressAttributedValue

**EmailAddressAttributedValue** 要素は、電子メール アドレスの配列とその関連付けられた属性のインスタンスを指定します。 
  
```XML
<EmailAddressAttributedValue>
    <Value></Value>
    <Attributions></Attributions>
<EmailAddressAttributedValue>
```

 **EmailAddressAttributedValueType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Value (EmailAddressType)](value-emailaddresstype.md) <br/> |属性配列に関連付 **けられた EmailAddress** の値を指定します。  <br/> |
|[Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md) <br/> |関連付けられた Value 要素の属性の配列を **指定** します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Emails1](emails1.md) <br/> |電子メール値の配列と、関連付けられたペルサのソース属性の識別子を指定します。  <br/> |
|[Emails2](emails2.md) <br/> |電子メール値の配列と、関連付けられたペルサのソース属性の識別子を指定します。  <br/> |
|[Emails3](emails3.md) <br/> |電子メール値の配列と、関連付けられたペルサのソース属性の識別子を指定します。  <br/> |
   
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


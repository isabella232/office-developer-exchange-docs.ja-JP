---
title: EmailAddressAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ebdf224d-3796-4179-aa0a-87942e7585ff
description: EmailAddressAttributedValue 要素は、電子メール アドレスの配列と、関連付けられている帰属のインスタンスを指定します。
ms.openlocfilehash: 3bcbb5c0a2bc9a2dc24516b5fc62e6e3363a360b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760233"
---
# <a name="emailaddressattributedvalue"></a>EmailAddressAttributedValue

**EmailAddressAttributedValue**要素は、電子メール アドレスの配列と、関連付けられている帰属のインスタンスを指定します。 
  
```XML
<EmailAddressAttributedValue>
    <Value></Value>
    <Attributions></Attributions>
<EmailAddressAttributedValue>
```

 **EmailAddressAttributedValueType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[値 (EmailAddressType)](value-emailaddresstype.md) <br/> |帰属配列に関連付け、 **EmailAddress**の値を指定します。  <br/> |
|[帰属 (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md) <br/> |帰属、関連付けられている**値**の要素の配列を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Emails1](emails1.md) <br/> |電子メールの値の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。  <br/> |
|[Emails2](emails2.md) <br/> |電子メールの値の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。  <br/> |
|[Emails3](emails3.md) <br/> |電子メールの値の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


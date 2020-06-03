---
title: Attributions (ArrayOfValueAttributionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7f36b6ee-8ecf-48c9-8cb6-dfb2da0ce2a2
description: Attributions 要素は、関連付けられた Value 要素の Attributions の配列を指定します。
ms.openlocfilehash: 9fd552670c529009838125063869f65e130c1e63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463994"
---
# <a name="attributions-arrayofvalueattributionstype"></a>Attributions (ArrayOfValueAttributionsType)

**Attributions**要素は、関連付けられた**Value**要素の Attributions の配列を指定します。 
  
```XML
<Attributions>
    <Attribution></Attribution>
</Attribution>
```

 **ArrayOfValueAttributionsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[属性 (string)](attribution-string.md) <br/> |属性を識別するために使用する文字列を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[BodyContentAttributedValue](bodycontentattributedvalue.md) <br/> |アイテムの本文のコンテンツを指定します。  <br/> |
|[EmailAddressAttributedValue](emailaddressattributedvalue.md) <br/> |電子メールアドレスの配列のインスタンスと、それに関連付けられている attributions を指定します。  <br/> |
|[ExtendedPropertyAttributedValue](extendedpropertyattributedvalue.md) <br/> |ペルソナの拡張プロパティを指定します。  <br/> |
|[PhoneNumberAttributedValue](phonenumberattributedvalue.md) <br/> |電話番号の配列のインスタンスと、それに関連付けられている attributions を指定します。  <br/> |
|[PostalAddressAttributedValue](postaladdressattributedvalue.md) <br/> |郵送先住所の配列のインスタンスと、それに関連付けられている attributions を指定します。  <br/> |
|[StringArrayAttributedValue](stringarrayattributedvalue.md) <br/> |Persona 要素の文字列データの配列のインスタンスを指定します。  <br/> |
|[StringAttributedValue](stringattributedvalue.md) <br/> |Persona 要素に関連付けられている属性の配列のインスタンスを指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


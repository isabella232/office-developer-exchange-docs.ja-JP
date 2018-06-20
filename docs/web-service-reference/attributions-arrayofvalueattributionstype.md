---
title: 帰属 (ArrayOfValueAttributionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7f36b6ee-8ecf-48c9-8cb6-dfb2da0ce2a2
description: 帰属要素は、その関連付けられている値要素の帰属の配列を指定します。
ms.openlocfilehash: a64510cacb9923682418ca8a9b203c765a129bdd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759471"
---
# <a name="attributions-arrayofvalueattributionstype"></a>帰属 (ArrayOfValueAttributionsType)

**帰属**要素は、その関連付けられている**値**要素の帰属の配列を指定します。 
  
```XML
<Attributions>
    <Attribution></Attribution>
</Attribution>
```

 **ArrayOfValueAttributionsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[属性 (文字列)](attribution-string.md) <br/> |属性を識別するために使う文字列を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[BodyContentAttributedValue](bodycontentattributedvalue.md) <br/> |アイテムの本文の内容を指定します。  <br/> |
|[EmailAddressAttributedValue](emailaddressattributedvalue.md) <br/> |電子メール アドレスと関連付けられている、帰属の配列のインスタンスを指定します。  <br/> |
|[ExtendedPropertyAttributedValue](extendedpropertyattributedvalue.md) <br/> |ペルソナの拡張プロパティを指定します。  <br/> |
|[PhoneNumberAttributedValue](phonenumberattributedvalue.md) <br/> |電話番号と、関連付けられている帰属の配列のインスタンスを指定します。  <br/> |
|[PostalAddressAttributedValue](postaladdressattributedvalue.md) <br/> |郵送先住所と、関連付けられている帰属の配列のインスタンスを指定します。  <br/> |
|[StringArrayAttributedValue](stringarrayattributedvalue.md) <br/> |ペルソナの要素のデータを文字列の配列のインスタンスを指定します。  <br/> |
|[StringAttributedValue](stringattributedvalue.md) <br/> |ペルソナの要素に関連付けられている属性の配列のインスタンスを指定します。  <br/> |
   
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


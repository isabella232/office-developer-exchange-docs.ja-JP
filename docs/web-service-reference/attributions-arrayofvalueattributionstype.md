---
title: Attributions (ArrayOfValueAttributionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7f36b6ee-8ecf-48c9-8cb6-dfb2da0ce2a2
description: Attributions 要素は、関連付けられた Value 要素の属性の配列を指定します。
ms.openlocfilehash: e5483e8e7ef4745e8025106ae1f1c52e91987183
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529329"
---
# <a name="attributions-arrayofvalueattributionstype"></a>Attributions (ArrayOfValueAttributionsType)

**Attributions 要素** は、関連付けられた Value 要素の属性の配列 **を指定** します。 
  
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
|[Attribution (string)](attribution-string.md) <br/> |属性の識別に使用する文字列を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[BodyContentAttributedValue](bodycontentattributedvalue.md) <br/> |アイテムの本文の内容を指定します。  <br/> |
|[EmailAddressAttributedValue](emailaddressattributedvalue.md) <br/> |電子メール アドレスの配列とその関連付けられた属性のインスタンスを指定します。  <br/> |
|[ExtendedPropertyAttributedValue](extendedpropertyattributedvalue.md) <br/> |ペルサの拡張プロパティを指定します。  <br/> |
|[PhoneNumberAttributedValue](phonenumberattributedvalue.md) <br/> |電話番号の配列とその関連付けられた属性のインスタンスを指定します。  <br/> |
|[PostalAddressAttributedValue](postaladdressattributedvalue.md) <br/> |住所の配列とその関連付けられた属性のインスタンスを指定します。  <br/> |
|[StringArrayAttributedValue](stringarrayattributedvalue.md) <br/> |ペルサ要素の文字列データの配列のインスタンスを指定します。  <br/> |
|[StringAttributedValue](stringattributedvalue.md) <br/> |ペルサ要素に関連付けられた属性の配列内のインスタンスを指定します。  <br/> |
   
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


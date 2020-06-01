---
title: FormattedAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 643f8663-1fab-4625-a7e9-5724e352972b
description: FormattedAddress 要素は、関連付けられている郵便番号の書式設定された表示値を指定します。
ms.openlocfilehash: 9150a3bb5bc81f7afecdafbf0cc33fafff597578
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461941"
---
# <a name="formattedaddress"></a>FormattedAddress

**FormattedAddress**要素は、関連付けられている郵便番号の書式設定された表示値を指定します。 
  
```XML
<FormattedAddress></FormattedAddress>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md) <br/> |住所に関連付けられている情報を指定します。  <br/> |
|["Postaladdress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md) <br/> |場所の住所を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**FormattedAddress**要素のテキスト値は、書式設定されたアドレスを指定する文字列型 (string) の値です。 
  
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


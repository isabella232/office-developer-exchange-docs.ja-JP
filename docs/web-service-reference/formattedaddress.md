---
title: FormattedAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 643f8663-1fab-4625-a7e9-5724e352972b
description: FormattedAddress 要素は、関連付けられている住所の書式設定された表示値を指定します。
ms.openlocfilehash: 14c970fcbe20567546e99e637c9c78c6003d9c0f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760581"
---
# <a name="formattedaddress"></a>FormattedAddress

**FormattedAddress**要素は、関連付けられている住所の書式設定された表示値を指定します。 
  
```XML
<FormattedAddress></FormattedAddress>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[値 (PersonaPostalAddressType)](value-personapostaladdresstype.md) <br/> |郵送先住所に関連付けられている情報を指定します。  <br/> |
|[住所 (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md) <br/> |場所の郵便の宛先を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**FormattedAddress**要素のテキスト値は、書式設定されたアドレスを指定する文字列値です。 
  
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


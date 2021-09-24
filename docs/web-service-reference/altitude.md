---
title: Altitude
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 14c2c8bd-db54-4b03-9a97-190ff9e908b3
description: Altitude 要素は、住所の高度を指定します。
ms.openlocfilehash: e3f4559b3baf99bf60fa7da85b363450a65d8747
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518961"
---
# <a name="altitude"></a>Altitude

**Altitude 要素** は、住所の高度を指定します。 
  
```XML
<Altitude></Altitude>
```

 **xs:double**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md) <br/> |場所の郵便番号を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

Altitude 要素のテキスト値は、郵便番号の高度です。
  
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


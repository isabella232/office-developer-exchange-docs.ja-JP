---
title: 型 (文字列)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d5eea7a8-c40d-42a6-8e0d-67f3252496cf
description: 型の要素では、郵便住所、電話番号、たとえば、HomeorBusiness の種類を指定します。
ms.openlocfilehash: b2262a01b03922e36daa3b13436f1e070918b72c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839760"
---
# <a name="type-string"></a>型 (文字列)

**型**の要素では、郵便番号と住所や電話番号、たとえば、「自宅」または「ビジネス」の種類を指定します。 
  
```XML
<Type></Type>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[電話](phone.md) | [電話番号](phonenumber.md) | [値 (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [(PersonaPostalAddressType) の住所](postaladdress-personapostaladdresstype.md)
  
## <a name="text-value"></a>テキスト値

**型**の要素のテキスト値は、郵便番号と住所や電話番号の種類です。 たとえば、「自宅」または「ビジネス」の値は、**型**の要素の予期される値です。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> ||
   


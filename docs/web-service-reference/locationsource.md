---
title: LocationSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: LocationSource 要素は、関連付けられている住所、連絡先、電話番号帳の発生元に関する情報を指定します。
ms.openlocfilehash: 7f5cf5fcca0a72287593349fcf5090a74225d012
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832248"
---
# <a name="locationsource"></a>LocationSource

**LocationSource**要素は、関連付けられている住所、連絡先、電話番号帳の発生元に関する情報を指定します。 
  
```XML
<LocationSource> None | LocationServices | PhonebookServices | Device | Contact | Resource </LocationSource>
```

 **LocationSourceType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[値 (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [(PersonaPostalAddressType) の住所](postaladdress-personapostaladdresstype.md)
  
## <a name="text-value"></a>テキスト値

**LocationSource**要素のテキスト値は、次の表のとおりです。 
  
**LocationSource 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |場所のソースがありません。  <br/> |
|LocationServices  <br/> |情報は、サービスの場所から入手されました。  <br/> |
|PhonebookServices  <br/> |電話帳サービスから情報を取得しました。  <br/> |
|デバイス  <br/> |デバイスから情報を取得しました。  <br/> |
|連絡先  <br/> |情報は、取引先担当者から入手されました。  <br/> |
|リソース  <br/> |リソースから情報を取得しました。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  


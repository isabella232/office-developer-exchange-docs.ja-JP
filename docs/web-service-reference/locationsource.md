---
title: LocationSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: LocationSource 要素は、連絡先や電話帳など、関連付けられた郵送先住所の発生元に関する情報を指定します。
ms.openlocfilehash: f3569494d3e662fbc46060944c8bd399b62d656b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543262"
---
# <a name="locationsource"></a>LocationSource

**LocationSource 要素** は、連絡先や電話帳など、関連付けられた郵送先住所の発生元に関する情報を指定します。 
  
```XML
<LocationSource> None | LocationServices | PhonebookServices | Device | Contact | Resource </LocationSource>
```

 **LocationSourceType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md)  | [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)
  
## <a name="text-value"></a>テキスト値

**LocationSource** 要素のテキスト値を次の表に示します。 
  
**LocationSource 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |場所のソースはありません。  <br/> |
|LocationServices  <br/> |この情報は、位置情報サービスから取得しました。  <br/> |
|PhonebookServices  <br/> |情報は電話帳サービスから取得しました。  <br/> |
|デバイス  <br/> |情報はデバイスから取得しました。  <br/> |
|Contact  <br/> |情報は連絡先から取得しました。  <br/> |
|リソース  <br/> |情報はリソースから取得しました。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  


---
title: LocationSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: LocationSource 要素は、関連付けられた郵便番号の発信元に関する情報を指定します。たとえば、連絡先または電話帳などです。
ms.openlocfilehash: ceba52c43d1c798bb8f5492b779c7c45d7d00b0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467103"
---
# <a name="locationsource"></a>LocationSource

**Locationsource**要素は、関連付けられた郵便番号の発信元に関する情報を指定します。たとえば、連絡先または電話帳などです。 
  
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

[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md)  | ["Postaladdress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)
  
## <a name="text-value"></a>テキスト値

次の表に、 **Locationsource**要素のテキスト値を示します。 
  
**LocationSource 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |場所のソースはありません。  <br/> |
|LocationServices  <br/> |情報は場所サービスから取得されました。  <br/> |
|電話帳サービス  <br/> |情報は、電話帳サービスから取得されました。  <br/> |
|Device  <br/> |情報はデバイスから取得されました。  <br/> |
|Contact  <br/> |連絡先から情報を取得しました。  <br/> |
|関連情報  <br/> |情報はリソースから取得されました。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  


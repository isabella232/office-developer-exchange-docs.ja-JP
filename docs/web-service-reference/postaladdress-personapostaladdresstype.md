---
title: "\"Postaladdress (PersonaPostalAddressType)"
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 075f7d65-9d05-47cb-af26-0dd6d5593439
description: "\"Postaladdress 要素は、ペルソナの郵送先住所を指定します。"
ms.openlocfilehash: 9e316e5e0135c2d18fab4067241988c65eceec66
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465388"
---
# <a name="postaladdress-personapostaladdresstype"></a>"Postaladdress (PersonaPostalAddressType)

**"Postaladdress**要素は、ペルソナの郵送先住所を指定します。 
  
```XML
<PostalAddress>
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
   <PostOfficeBox/>
   <Type/>
   <Latitude/>
   <Longitude/>
   <Accuracy/>
   <Altitude/>
   <AltitudeAccuracy/>
   <FormattedAddress/>
   <LocationUri/>
   <LocationSource/>
</PostalAddress>
```

 **PersonaPostalAddressType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[番地](street.md)  | [市区町村](city.md)  | [状態](state-ex15websvcsotherref.md)  | [国](country.md)  | [郵便](postalcode.md)  |  番号[Postofficebox が](postofficebox.md)  | [型 (string)](type-string.md)  | [緯度](latitude.md)  | [経度](longitude.md)  | [精度](accuracy.md)  | [高度](altitude.md)  | [AltitudeAccuracy](altitudeaccuracy.md)  | [FormattedAddress](formattedaddress.md)  | [Locationuri](locationuri.md)  | [Locationsource](locationsource.md)
  
### <a name="parent-elements"></a>親要素

[EnhancedLocation](enhancedlocation.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   


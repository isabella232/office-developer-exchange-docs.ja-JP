---
title: 住所 (PersonaPostalAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 075f7d65-9d05-47cb-af26-0dd6d5593439
description: 住所要素は、ペルソナの郵便の宛先を指定します。
ms.openlocfilehash: fb418154867aebb4d284e75be579003c0ddc88f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832855"
---
# <a name="postaladdress-personapostaladdresstype"></a>住所 (PersonaPostalAddressType)

**住所**要素は、ペルソナの郵便の宛先を指定します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[番地](street.md) | [市](city.md) | [状態](state-ex15websvcsotherref.md) | [国](country.md) | [[郵便番号]](postalcode.md) | [PostOfficeBox](postofficebox.md) | [(string) 型](type-string.md) | [緯度](latitude.md) |  [経度](longitude.md) | [精度](accuracy.md) | [高](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)
  
### <a name="parent-elements"></a>親要素

[EnhancedLocation](enhancedlocation.md)
  
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
   


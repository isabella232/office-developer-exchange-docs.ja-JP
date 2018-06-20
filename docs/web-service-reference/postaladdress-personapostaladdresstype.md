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
# <a name="postaladdress-personapostaladdresstype"></a><span data-ttu-id="05059-103">住所 (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="05059-103">PostalAddress (PersonaPostalAddressType)</span></span>

<span data-ttu-id="05059-104">**住所**要素は、ペルソナの郵便の宛先を指定します。</span><span class="sxs-lookup"><span data-stu-id="05059-104">The **PostalAddress** element specifies the postal address for a persona.</span></span> 
  
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

 <span data-ttu-id="05059-105">**PersonaPostalAddressType**</span><span class="sxs-lookup"><span data-stu-id="05059-105">**PersonaPostalAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05059-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="05059-106">Attributes and elements</span></span>

<span data-ttu-id="05059-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="05059-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05059-108">属性</span><span class="sxs-lookup"><span data-stu-id="05059-108">Attributes</span></span>

<span data-ttu-id="05059-109">なし。</span><span class="sxs-lookup"><span data-stu-id="05059-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05059-110">子要素</span><span class="sxs-lookup"><span data-stu-id="05059-110">Child elements</span></span>

<span data-ttu-id="05059-111">[番地](street.md) | [市](city.md) | [状態](state-ex15websvcsotherref.md) | [国](country.md) | [[郵便番号]](postalcode.md) | [PostOfficeBox](postofficebox.md) | [(string) 型](type-string.md) | [緯度](latitude.md) |  [経度](longitude.md) | [精度](accuracy.md) | [高](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span><span class="sxs-lookup"><span data-stu-id="05059-111">[Street](street.md) | [City](city.md) | [State](state-ex15websvcsotherref.md) | [Country](country.md) | [PostalCode](postalcode.md) | [PostOfficeBox](postofficebox.md) | [Type (string)](type-string.md) | [Latitude](latitude.md) | [Longitude](longitude.md) | [Accuracy](accuracy.md) | [Altitude](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05059-112">親要素</span><span class="sxs-lookup"><span data-stu-id="05059-112">Parent elements</span></span>

[<span data-ttu-id="05059-113">EnhancedLocation</span><span class="sxs-lookup"><span data-stu-id="05059-113">EnhancedLocation</span></span>](enhancedlocation.md)
  
## <a name="remarks"></a><span data-ttu-id="05059-114">備考</span><span class="sxs-lookup"><span data-stu-id="05059-114">Remarks</span></span>

<span data-ttu-id="05059-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="05059-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="05059-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="05059-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05059-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="05059-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05059-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="05059-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05059-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="05059-119">Schema name</span></span>  <br/> |<span data-ttu-id="05059-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="05059-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="05059-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="05059-121">Validation file</span></span>  <br/> |<span data-ttu-id="05059-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="05059-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05059-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="05059-123">Can be empty</span></span>  <br/> ||
   


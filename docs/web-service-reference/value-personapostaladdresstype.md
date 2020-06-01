---
title: Value (PersonaPostalAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: be838fc2-cfcb-4856-b095-a8e5366bb6c6
description: Value 要素は、住所に関連付けられている情報を指定します。
ms.openlocfilehash: 2d644ff45fe89061ccd90279773f3a5a5b7fe7cc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466473"
---
# <a name="value-personapostaladdresstype"></a><span data-ttu-id="6a402-103">Value (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="6a402-103">Value (PersonaPostalAddressType)</span></span>

<span data-ttu-id="6a402-104">**Value**要素は、住所に関連付けられている情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="6a402-104">The **Value** element specifies information associated with a postal address.</span></span> 
  
```XML
<Value>
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
</Value>
```

<span data-ttu-id="6a402-105">**PersonaPostalAddressType**</span><span class="sxs-lookup"><span data-stu-id="6a402-105">**PersonaPostalAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6a402-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6a402-106">Attributes and elements</span></span>

<span data-ttu-id="6a402-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6a402-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a402-108">属性</span><span class="sxs-lookup"><span data-stu-id="6a402-108">Attributes</span></span>

<span data-ttu-id="6a402-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6a402-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a402-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6a402-110">Child elements</span></span>

<span data-ttu-id="6a402-111">[番地](street.md)  | [市区町村](city.md)  | [状態](state-ex15websvcsotherref.md)  | [国](country.md)  | [郵便](postalcode.md)  |  番号[Postofficebox が](postofficebox.md)  | [型 (string)](type-string.md)  | [緯度](latitude.md)  | [経度](longitude.md)  | [精度](accuracy.md)  | [高度](altitude.md)  | [AltitudeAccuracy](altitudeaccuracy.md)  | [FormattedAddress](formattedaddress.md)  | [Locationuri](locationuri.md)  | [Locationsource](locationsource.md)</span><span class="sxs-lookup"><span data-stu-id="6a402-111">[Street](street.md) | [City](city.md) | [State](state-ex15websvcsotherref.md) | [Country](country.md) | [PostalCode](postalcode.md) | [PostOfficeBox](postofficebox.md) | [Type (string)](type-string.md) | [Latitude](latitude.md) | [Longitude](longitude.md) | [Accuracy](accuracy.md) | [Altitude](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6a402-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6a402-112">Parent elements</span></span>

[<span data-ttu-id="6a402-113">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="6a402-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md)
  
## <a name="remarks"></a><span data-ttu-id="6a402-114">注釈</span><span class="sxs-lookup"><span data-stu-id="6a402-114">Remarks</span></span>

<span data-ttu-id="6a402-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6a402-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6a402-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6a402-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a402-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6a402-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a402-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="6a402-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6a402-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6a402-119">Schema name</span></span>  <br/> |<span data-ttu-id="6a402-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6a402-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="6a402-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6a402-121">Validation file</span></span>  <br/> |<span data-ttu-id="6a402-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6a402-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6a402-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6a402-123">Can be empty</span></span>  <br/> ||
   


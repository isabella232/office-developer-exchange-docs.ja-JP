---
title: 値 (PersonaPostalAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: be838fc2-cfcb-4856-b095-a8e5366bb6c6
description: 情報が住所に関連付けられている値の要素を指定します。
ms.openlocfilehash: 048d3a49552f1a9e89744e4cd16ec1745417e923
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839974"
---
# <a name="value-personapostaladdresstype"></a><span data-ttu-id="9ca7f-103">値 (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="9ca7f-103">Value (PersonaPostalAddressType)</span></span>

<span data-ttu-id="9ca7f-104">**値**要素は、郵送先住所に関連付けられている情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="9ca7f-104">The **Value** element specifies information associated with a postal address.</span></span> 
  
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

<span data-ttu-id="9ca7f-105">**PersonaPostalAddressType**</span><span class="sxs-lookup"><span data-stu-id="9ca7f-105">**PersonaPostalAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9ca7f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9ca7f-106">Attributes and elements</span></span>

<span data-ttu-id="9ca7f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9ca7f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ca7f-108">属性</span><span class="sxs-lookup"><span data-stu-id="9ca7f-108">Attributes</span></span>

<span data-ttu-id="9ca7f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9ca7f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ca7f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9ca7f-110">Child elements</span></span>

<span data-ttu-id="9ca7f-111">[番地](street.md) | [市](city.md) | [状態](state-ex15websvcsotherref.md) | [国](country.md) | [[郵便番号]](postalcode.md) | [PostOfficeBox](postofficebox.md) | [(string) 型](type-string.md) | [緯度](latitude.md) |  [経度](longitude.md) | [精度](accuracy.md) | [高](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span><span class="sxs-lookup"><span data-stu-id="9ca7f-111">[Street](street.md) | [City](city.md) | [State](state-ex15websvcsotherref.md) | [Country](country.md) | [PostalCode](postalcode.md) | [PostOfficeBox](postofficebox.md) | [Type (string)](type-string.md) | [Latitude](latitude.md) | [Longitude](longitude.md) | [Accuracy](accuracy.md) | [Altitude](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9ca7f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9ca7f-112">Parent elements</span></span>

[<span data-ttu-id="9ca7f-113">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="9ca7f-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md)
  
## <a name="remarks"></a><span data-ttu-id="9ca7f-114">備考</span><span class="sxs-lookup"><span data-stu-id="9ca7f-114">Remarks</span></span>

<span data-ttu-id="9ca7f-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9ca7f-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9ca7f-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9ca7f-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ca7f-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="9ca7f-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ca7f-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="9ca7f-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9ca7f-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9ca7f-119">Schema name</span></span>  <br/> |<span data-ttu-id="9ca7f-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9ca7f-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="9ca7f-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9ca7f-121">Validation file</span></span>  <br/> |<span data-ttu-id="9ca7f-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9ca7f-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9ca7f-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9ca7f-123">Can be empty</span></span>  <br/> ||
   


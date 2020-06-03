---
title: DayOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOrder
api_type:
- schema
ms.assetid: 3022f839-12a2-42a9-820e-3ea585ce8657
description: DayOrder 要素は、期間から標準時および夏時間に移行する日付を表す、DayOfWeek (TimeZone) 要素で指定された日の n 番目の出現を表します。
ms.openlocfilehash: 53a8cb979bdb7aefead5623b4680f4c1a4ef5509
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526964"
---
# <a name="dayorder"></a><span data-ttu-id="70e23-103">DayOrder</span><span class="sxs-lookup"><span data-stu-id="70e23-103">DayOrder</span></span>

<span data-ttu-id="70e23-104">**Dayorder**要素は、期間から標準時および夏時間に移行する日付を表す[DayOfWeek (TimeZone)](dayofweek-timezone.md)要素で指定された日の _n_th を表します。</span><span class="sxs-lookup"><span data-stu-id="70e23-104">The **DayOrder** element represents the  _n_th occurrence of the day specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span> 
  
```xml
<DayOrder>...</DayOrder>
```

<span data-ttu-id="70e23-105">**短い**</span><span class="sxs-lookup"><span data-stu-id="70e23-105">**short**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="70e23-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="70e23-106">Attributes and elements</span></span>

<span data-ttu-id="70e23-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="70e23-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70e23-108">属性</span><span class="sxs-lookup"><span data-stu-id="70e23-108">Attributes</span></span>

<span data-ttu-id="70e23-109">なし。</span><span class="sxs-lookup"><span data-stu-id="70e23-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70e23-110">子要素</span><span class="sxs-lookup"><span data-stu-id="70e23-110">Child elements</span></span>

<span data-ttu-id="70e23-111">なし。</span><span class="sxs-lookup"><span data-stu-id="70e23-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="70e23-112">親要素</span><span class="sxs-lookup"><span data-stu-id="70e23-112">Parent elements</span></span>

|<span data-ttu-id="70e23-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="70e23-113">**Element**</span></span>|<span data-ttu-id="70e23-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="70e23-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70e23-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="70e23-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="70e23-116">時間のオフセット (協定世界時 (UTC) を基準として、 [Bias (utc)](bias-utc.md)要素で表される) を表します。</span><span class="sxs-lookup"><span data-stu-id="70e23-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span><br/><br/><span data-ttu-id="70e23-117">この要素には、夏時間が計測される地域で夏時間から標準時への切り替えに関する情報も含まれます。</span><span class="sxs-lookup"><span data-stu-id="70e23-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="70e23-118">[Standardtime](standardtime.md)要素に対する XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="70e23-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="70e23-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="70e23-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="70e23-120">夏時間が計測される地域で、 [Bias (utc)](bias-utc.md)要素によって表される utc を基準とした時刻からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="70e23-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="70e23-121">この要素には、標準時から夏時間への切り替えが行われるタイミングに関する情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="70e23-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span><br/><br/><span data-ttu-id="70e23-122">[Daylighttime](daylighttime.md)要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="70e23-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="70e23-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="70e23-123">Text value</span></span>

<span data-ttu-id="70e23-124">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="70e23-124">A text value is required.</span></span> <span data-ttu-id="70e23-125">**Dayorder**要素の値は、1 ~ 5 にすることができます。</span><span class="sxs-lookup"><span data-stu-id="70e23-125">The value for the **DayOrder** element can be 1 through 5.</span></span> <span data-ttu-id="70e23-126">この要素の最大値は、月と年に応じて4または5のいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="70e23-126">The maximum value for this element can be either 4 or 5, depending on the month and year.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="70e23-127">注釈</span><span class="sxs-lookup"><span data-stu-id="70e23-127">Remarks</span></span>

<span data-ttu-id="70e23-128">値5、値10を持つ[Month](month.md)要素、および値が日曜日である[DayOfWeek (TimeZone)](dayofweek-timezone.md)要素を含む**Dayorder**要素を含む[standardtime](standardtime.md)要素は、標準時から夏時間への切り替えが10月の5番目の日曜日に行われることを意味します。</span><span class="sxs-lookup"><span data-stu-id="70e23-128">A [StandardTime](standardtime.md) element that contains a **DayOrder** element that has a value of 5, a [Month](month.md) element that has a value of 10, and a [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="70e23-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="70e23-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70e23-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="70e23-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="70e23-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="70e23-131">Schema Name</span></span>  <br/> |<span data-ttu-id="70e23-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="70e23-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="70e23-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="70e23-133">Validation File</span></span>  <br/> |<span data-ttu-id="70e23-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="70e23-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="70e23-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="70e23-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="70e23-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="70e23-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="70e23-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="70e23-137">See also</span></span>

- [<span data-ttu-id="70e23-138">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="70e23-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="70e23-139">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="70e23-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


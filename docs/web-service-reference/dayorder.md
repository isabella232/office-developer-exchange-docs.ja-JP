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
description: DayOrder 要素は、標準時間と夏時間との切り替えの日付を表す曜日 (タイムゾーン) の要素で指定された日の n 番目の発生を表します。
ms.openlocfilehash: 03ee678611a6cf58a7256ded67ab4d0a8a06a7ee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759940"
---
# <a name="dayorder"></a><span data-ttu-id="35ae4-103">DayOrder</span><span class="sxs-lookup"><span data-stu-id="35ae4-103">DayOrder</span></span>

<span data-ttu-id="35ae4-104">**DayOrder**要素は、標準時間と夏時間との切り替えの日付を表す[曜日 (タイムゾーン)](dayofweek-timezone.md)の要素で指定された日の _n_th の発生を表します。</span><span class="sxs-lookup"><span data-stu-id="35ae4-104">The **DayOrder** element represents the  _n_th occurrence of the day specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span> 
  
```xml
<DayOrder>...</DayOrder>
```

<span data-ttu-id="35ae4-105">**短い**</span><span class="sxs-lookup"><span data-stu-id="35ae4-105">**short**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="35ae4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="35ae4-106">Attributes and elements</span></span>

<span data-ttu-id="35ae4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="35ae4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="35ae4-108">属性</span><span class="sxs-lookup"><span data-stu-id="35ae4-108">Attributes</span></span>

<span data-ttu-id="35ae4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="35ae4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="35ae4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="35ae4-110">Child elements</span></span>

<span data-ttu-id="35ae4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="35ae4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="35ae4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="35ae4-112">Parent elements</span></span>

|<span data-ttu-id="35ae4-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="35ae4-113">**Element**</span></span>|<span data-ttu-id="35ae4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="35ae4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35ae4-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="35ae4-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="35ae4-116">基準にして世界協定時刻 (UTC)[バイアス (UTC)](bias-utc.md)の要素で表される時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="35ae4-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span><br/><br/><span data-ttu-id="35ae4-117">この要素は、夏時間が発生した地域で夏時間から切り替えに関する情報を標準時も含みます。</span><span class="sxs-lookup"><span data-stu-id="35ae4-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="35ae4-118">[StandardTime](standardtime.md)要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="35ae4-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="35ae4-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="35ae4-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="35ae4-120">夏時間が発生した地域の[バイアス (UTC)](bias-utc.md)の要素で表される UTC 時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="35ae4-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="35ae4-121">この要素には、標準時間から夏時間への切り替えが発生した場合についての情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="35ae4-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span><br/><br/><span data-ttu-id="35ae4-122">[DaylightTime](daylighttime.md)要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="35ae4-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="35ae4-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="35ae4-123">Text value</span></span>

<span data-ttu-id="35ae4-124">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="35ae4-124">A text value is required.</span></span> <span data-ttu-id="35ae4-125">**DayOrder**要素の値は 1 ~ 5 にできます。</span><span class="sxs-lookup"><span data-stu-id="35ae4-125">The value for the **DayOrder** element can be 1 through 5.</span></span> <span data-ttu-id="35ae4-126">この要素の最大値は 4 または 5、月、年によってのいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="35ae4-126">The maximum value for this element can be either 4 or 5, depending on the month and year.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="35ae4-127">備考</span><span class="sxs-lookup"><span data-stu-id="35ae4-127">Remarks</span></span>

<span data-ttu-id="35ae4-128">5 の値を持つ**DayOrder**要素、10 の値を持つ[月](month.md)の要素と、日曜日の値を持つ[DayOfWeek (タイムゾーン)](dayofweek-timezone.md)の要素を含む[StandardTime](standardtime.md)要素を意味する (標準時) からの移行夏時間は、10 月の 5 番目の日曜日に発生します。</span><span class="sxs-lookup"><span data-stu-id="35ae4-128">A [StandardTime](standardtime.md) element that contains a **DayOrder** element that has a value of 5, a [Month](month.md) element that has a value of 10, and a [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="35ae4-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="35ae4-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="35ae4-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="35ae4-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="35ae4-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="35ae4-131">Schema Name</span></span>  <br/> |<span data-ttu-id="35ae4-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="35ae4-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="35ae4-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="35ae4-133">Validation File</span></span>  <br/> |<span data-ttu-id="35ae4-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="35ae4-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="35ae4-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="35ae4-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="35ae4-136">False</span><span class="sxs-lookup"><span data-stu-id="35ae4-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="35ae4-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="35ae4-137">See also</span></span>

- [<span data-ttu-id="35ae4-138">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="35ae4-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="35ae4-139">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="35ae4-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


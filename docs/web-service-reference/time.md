---
title: 時刻
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Time
api_type:
- schema
ms.assetid: c4b98be7-141c-4ba8-97ef-9ad1ed19f61f
description: Time 要素は、標準時と夏時間の切り替え時間を表します。
ms.openlocfilehash: 97c89fbcbdb85fcdd4d32a1d44075ac42adef053
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460296"
---
# <a name="time"></a><span data-ttu-id="47171-103">Time</span><span class="sxs-lookup"><span data-stu-id="47171-103">Time</span></span>

<span data-ttu-id="47171-104">**Time**要素は、標準時と夏時間の切り替え時間を表します。</span><span class="sxs-lookup"><span data-stu-id="47171-104">The **Time** element represents the transition time of day to and from standard time and daylight saving time.</span></span> 
  
```xml
<Time>...</Time>
```

 <span data-ttu-id="47171-105">**string**</span><span class="sxs-lookup"><span data-stu-id="47171-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="47171-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="47171-106">Attributes and elements</span></span>

<span data-ttu-id="47171-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="47171-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47171-108">属性</span><span class="sxs-lookup"><span data-stu-id="47171-108">Attributes</span></span>

<span data-ttu-id="47171-109">なし。</span><span class="sxs-lookup"><span data-stu-id="47171-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="47171-110">子要素</span><span class="sxs-lookup"><span data-stu-id="47171-110">Child elements</span></span>

<span data-ttu-id="47171-111">なし。</span><span class="sxs-lookup"><span data-stu-id="47171-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="47171-112">親要素</span><span class="sxs-lookup"><span data-stu-id="47171-112">Parent elements</span></span>

|<span data-ttu-id="47171-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="47171-113">**Element**</span></span>|<span data-ttu-id="47171-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="47171-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47171-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="47171-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="47171-116">時間のオフセット (協定世界時 (UTC) を基準として、 [Bias (utc)](bias-utc.md)要素で表される) を表します。</span><span class="sxs-lookup"><span data-stu-id="47171-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="47171-117">この要素には、夏時間が計測される地域で夏時間から標準時への切り替えに関する情報も含まれます。</span><span class="sxs-lookup"><span data-stu-id="47171-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span>  <br/><br/>  <span data-ttu-id="47171-118">[Standardtime](standardtime.md)要素に対する XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="47171-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/> <br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="47171-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="47171-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="47171-120">夏時間が計測される地域で、 [Bias (utc)](bias-utc.md)要素によって表される utc を基準とした時刻からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="47171-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="47171-121">この要素には、標準時から夏時間への切り替えが行われるタイミングに関する情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="47171-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/>  <span data-ttu-id="47171-122">[Daylighttime](daylighttime.md)要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="47171-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span>  <br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="47171-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="47171-123">Text value</span></span>

<span data-ttu-id="47171-124">Text 値は、時間、分、秒を次の形式で表します。 hh: mm: ss。</span><span class="sxs-lookup"><span data-stu-id="47171-124">The text value represents hours, minutes, and seconds in the following format: hh:mm:ss.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="47171-125">注釈</span><span class="sxs-lookup"><span data-stu-id="47171-125">Remarks</span></span>

<span data-ttu-id="47171-126">[Daylighttime](daylighttime.md)要素に**time**要素がある場合は、夏時間から標準時への切り替えが行われる時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="47171-126">When the **Time** element occurs in the [DaylightTime](daylighttime.md) element, it represents the time of day that the transition from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="47171-127">[Standardtime](standardtime.md)要素に[time](time.md)要素がある場合は、標準時から夏時間への切り替えが行われる時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="47171-127">When the [Time](time.md) element occurs in the [StandardTime](standardtime.md) element, it represents the time of day that the transition from standard time to daylight saving time occurs.</span></span> 
  
<span data-ttu-id="47171-128">この要素の最小出現回数は0で、最大出現回数は1です。</span><span class="sxs-lookup"><span data-stu-id="47171-128">This element has a minimum occurrence of zero and a maximum occurrence of one.</span></span>
  
## <a name="example"></a><span data-ttu-id="47171-129">例</span><span class="sxs-lookup"><span data-stu-id="47171-129">Example</span></span>

<span data-ttu-id="47171-130">要求の次の部分は、2 A.M. に移行する時間を表します。</span><span class="sxs-lookup"><span data-stu-id="47171-130">The following part of a request represents a transition time of 2 A.M.</span></span> <span data-ttu-id="47171-131">標準時から夏時間への間隔。</span><span class="sxs-lookup"><span data-stu-id="47171-131">from standard time to daylight saving time.</span></span>
  
```xml
<StandardTime>
   <Bias>0</Bias>
   <Time>02:00:00</Time>
   <DayOrder>5</DayOrder>
   <Month>10</Month>
   <DayOfWeek>Sunday</DayOfWeek>
</StandardTime
```

## <a name="element-information"></a><span data-ttu-id="47171-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="47171-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47171-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="47171-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="47171-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="47171-134">Schema Name</span></span>  <br/> |<span data-ttu-id="47171-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="47171-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="47171-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="47171-136">Validation File</span></span>  <br/> |<span data-ttu-id="47171-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="47171-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="47171-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="47171-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="47171-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="47171-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="47171-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="47171-140">See also</span></span>

- [<span data-ttu-id="47171-141">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="47171-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="47171-142">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="47171-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


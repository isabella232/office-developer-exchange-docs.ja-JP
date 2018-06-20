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
description: 時刻要素は、標準時間と夏時間との間に 1 日の切り替え時間を表します。
ms.openlocfilehash: 716487fb7ed64dbaa6fa97caf1ea608e4673d2ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839676"
---
# <a name="time"></a><span data-ttu-id="33f68-103">時刻型 (Time)</span><span class="sxs-lookup"><span data-stu-id="33f68-103">Time</span></span>

<span data-ttu-id="33f68-104">**時刻**要素は、標準時間と夏時間との間に 1 日の切り替え時間を表します。</span><span class="sxs-lookup"><span data-stu-id="33f68-104">The **Time** element represents the transition time of day to and from standard time and daylight saving time.</span></span> 
  
```xml
<Time>...</Time>
```

 <span data-ttu-id="33f68-105">**string**</span><span class="sxs-lookup"><span data-stu-id="33f68-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33f68-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="33f68-106">Attributes and elements</span></span>

<span data-ttu-id="33f68-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="33f68-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33f68-108">属性</span><span class="sxs-lookup"><span data-stu-id="33f68-108">Attributes</span></span>

<span data-ttu-id="33f68-109">なし。</span><span class="sxs-lookup"><span data-stu-id="33f68-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33f68-110">子要素</span><span class="sxs-lookup"><span data-stu-id="33f68-110">Child elements</span></span>

<span data-ttu-id="33f68-111">なし。</span><span class="sxs-lookup"><span data-stu-id="33f68-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="33f68-112">親要素</span><span class="sxs-lookup"><span data-stu-id="33f68-112">Parent elements</span></span>

|<span data-ttu-id="33f68-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="33f68-113">**Element**</span></span>|<span data-ttu-id="33f68-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="33f68-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33f68-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="33f68-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="33f68-116">基準にして世界協定時刻 (UTC)[バイアス (UTC)](bias-utc.md)の要素で表される時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="33f68-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="33f68-117">この要素は、夏時間が発生した地域で夏時間から切り替えに関する情報を標準時も含みます。</span><span class="sxs-lookup"><span data-stu-id="33f68-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span>  <br/><br/>  <span data-ttu-id="33f68-118">[StandardTime](standardtime.md)要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="33f68-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/> <br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="33f68-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="33f68-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="33f68-120">夏時間が発生した地域の[バイアス (UTC)](bias-utc.md)の要素で表される UTC 時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="33f68-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="33f68-121">この要素には、標準時間から夏時間への切り替えが発生した場合についての情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="33f68-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/>  <span data-ttu-id="33f68-122">[DaylightTime](daylighttime.md)要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="33f68-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span>  <br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="33f68-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="33f68-123">Text value</span></span>

<span data-ttu-id="33f68-124">テキスト値は、時間、分、および次の形式で秒を表します: hh:mm:ss です。</span><span class="sxs-lookup"><span data-stu-id="33f68-124">The text value represents hours, minutes, and seconds in the following format: hh:mm:ss.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="33f68-125">備考</span><span class="sxs-lookup"><span data-stu-id="33f68-125">Remarks</span></span>

<span data-ttu-id="33f68-126">[DaylightTime](daylighttime.md)要素では、**時間**の要素が発生する場合は、夏時間から標準時への移行が発生する時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="33f68-126">When the **Time** element occurs in the [DaylightTime](daylighttime.md) element, it represents the time of day that the transition from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="33f68-127">[時刻](time.md)要素は、 [StandardTime](standardtime.md)要素で発生した場合、標準時間から夏時間への切り替えが発生する時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="33f68-127">When the [Time](time.md) element occurs in the [StandardTime](standardtime.md) element, it represents the time of day that the transition from standard time to daylight saving time occurs.</span></span> 
  
<span data-ttu-id="33f68-128">この要素には、最小出現回数が 0 と 1 つの最大出現します。</span><span class="sxs-lookup"><span data-stu-id="33f68-128">This element has a minimum occurrence of zero and a maximum occurrence of one.</span></span>
  
## <a name="example"></a><span data-ttu-id="33f68-129">例</span><span class="sxs-lookup"><span data-stu-id="33f68-129">Example</span></span>

<span data-ttu-id="33f68-130">要求の次の部分は、午前 2 時の遷移時間を表します</span><span class="sxs-lookup"><span data-stu-id="33f68-130">The following part of a request represents a transition time of 2 A.M.</span></span> <span data-ttu-id="33f68-131">夏時間への標準時間です。</span><span class="sxs-lookup"><span data-stu-id="33f68-131">from standard time to daylight saving time.</span></span>
  
```xml
<StandardTime>
   <Bias>0</Bias>
   <Time>02:00:00</Time>
   <DayOrder>5</DayOrder>
   <Month>10</Month>
   <DayOfWeek>Sunday</DayOfWeek>
</StandardTime
```

## <a name="element-information"></a><span data-ttu-id="33f68-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="33f68-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33f68-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="33f68-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="33f68-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="33f68-134">Schema Name</span></span>  <br/> |<span data-ttu-id="33f68-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="33f68-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="33f68-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="33f68-136">Validation File</span></span>  <br/> |<span data-ttu-id="33f68-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="33f68-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="33f68-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="33f68-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="33f68-139">False</span><span class="sxs-lookup"><span data-stu-id="33f68-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33f68-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="33f68-140">See also</span></span>

- [<span data-ttu-id="33f68-141">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="33f68-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="33f68-142">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="33f68-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


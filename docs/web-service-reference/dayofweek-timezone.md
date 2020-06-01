---
title: DayOfWeek (TimeZone)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 416e8892-ebb1-4fac-82cf-e27549a6c175
description: DayOfWeek 要素は、タイムゾーンの切り替えが行われる曜日を表します。
ms.openlocfilehash: 7bc05f417268ccfb20adae12e2694d8360023ab2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457845"
---
# <a name="dayofweek-timezone"></a><span data-ttu-id="5f04f-103">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="5f04f-103">DayOfWeek (TimeZone)</span></span>

<span data-ttu-id="5f04f-104">**DayOfWeek**要素は、タイムゾーンの切り替えが行われる曜日を表します。</span><span class="sxs-lookup"><span data-stu-id="5f04f-104">The **DayOfWeek** element represents the day of the week on which the time zone transition occurs.</span></span> 
  
```xml
<DayOfWeek>...</DayOfWeek>
```

<span data-ttu-id="5f04f-105">**DayOfWeekType**</span><span class="sxs-lookup"><span data-stu-id="5f04f-105">**DayOfWeekType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5f04f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5f04f-106">Attributes and elements</span></span>

<span data-ttu-id="5f04f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5f04f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5f04f-108">属性</span><span class="sxs-lookup"><span data-stu-id="5f04f-108">Attributes</span></span>

<span data-ttu-id="5f04f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5f04f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5f04f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5f04f-110">Child elements</span></span>

<span data-ttu-id="5f04f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5f04f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5f04f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5f04f-112">Parent elements</span></span>

|<span data-ttu-id="5f04f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5f04f-113">**Element**</span></span>|<span data-ttu-id="5f04f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5f04f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f04f-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="5f04f-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="5f04f-116">時間のオフセット (協定世界時 (UTC) を基準として、 [Bias (utc)](bias-utc.md)要素で表される) を表します。</span><span class="sxs-lookup"><span data-stu-id="5f04f-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span><br/><br/><span data-ttu-id="5f04f-117">この要素には、夏時間が計測される地域で夏時間から標準時への切り替えに関する情報も含まれます。</span><span class="sxs-lookup"><span data-stu-id="5f04f-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="5f04f-118">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="5f04f-118">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="5f04f-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="5f04f-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="5f04f-120">夏時間が計測される地域で、 [Bias (utc)](bias-utc.md)要素によって表される utc を基準とした時刻からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="5f04f-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="5f04f-121">この要素には、標準時から夏時間への切り替えが行われるタイミングに関する情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="5f04f-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span><br/><br/><span data-ttu-id="5f04f-122">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="5f04f-122">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
|[<span data-ttu-id="5f04f-123">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="5f04f-123">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="5f04f-124">毎年同じ日に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="5f04f-124">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5f04f-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5f04f-125">Text value</span></span>

<span data-ttu-id="5f04f-126">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="5f04f-126">A text value is required.</span></span> <span data-ttu-id="5f04f-127">テキスト値は、次の値を持つ列挙型で表されます。</span><span class="sxs-lookup"><span data-stu-id="5f04f-127">The text value is represented by an enumeration that has the following possible values:</span></span>
  
- <span data-ttu-id="5f04f-128">日曜日</span><span class="sxs-lookup"><span data-stu-id="5f04f-128">Sunday</span></span>    
- <span data-ttu-id="5f04f-129">月曜日</span><span class="sxs-lookup"><span data-stu-id="5f04f-129">Monday</span></span>    
- <span data-ttu-id="5f04f-130">火曜日</span><span class="sxs-lookup"><span data-stu-id="5f04f-130">Tuesday</span></span>    
- <span data-ttu-id="5f04f-131">水曜日</span><span class="sxs-lookup"><span data-stu-id="5f04f-131">Wednesday</span></span>    
- <span data-ttu-id="5f04f-132">木曜日</span><span class="sxs-lookup"><span data-stu-id="5f04f-132">Thursday</span></span>    
- <span data-ttu-id="5f04f-133">金曜日</span><span class="sxs-lookup"><span data-stu-id="5f04f-133">Friday</span></span>    
- <span data-ttu-id="5f04f-134">土曜日</span><span class="sxs-lookup"><span data-stu-id="5f04f-134">Saturday</span></span>    
- <span data-ttu-id="5f04f-135">Day</span><span class="sxs-lookup"><span data-stu-id="5f04f-135">Day</span></span>    
- <span data-ttu-id="5f04f-136">平日</span><span class="sxs-lookup"><span data-stu-id="5f04f-136">Weekday</span></span>   
- <span data-ttu-id="5f04f-137">WeekendDay</span><span class="sxs-lookup"><span data-stu-id="5f04f-137">WeekendDay</span></span>
    
## <a name="remarks"></a><span data-ttu-id="5f04f-138">注釈</span><span class="sxs-lookup"><span data-stu-id="5f04f-138">Remarks</span></span>

<span data-ttu-id="5f04f-139">値5、値が10の[month](month.md)要素、日曜日という値を持つ**DayOfWeek**要素を含む[Dayorder](dayorder.md)要素を含む[standardtime](standardtime.md)要素は、標準時から夏時間への切り替えが10月の5番目の日曜日に行われることを意味します。</span><span class="sxs-lookup"><span data-stu-id="5f04f-139">A [StandardTime](standardtime.md) element that contains a [DayOrder](dayorder.md) element that has a value of 5, a [Month](month.md) element that has a value of 10, and a **DayOfWeek** element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
<span data-ttu-id="5f04f-140">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5f04f-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5f04f-141">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5f04f-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5f04f-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="5f04f-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5f04f-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5f04f-143">Schema Name</span></span>  <br/> |<span data-ttu-id="5f04f-144">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="5f04f-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="5f04f-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5f04f-145">Validation File</span></span>  <br/> |<span data-ttu-id="5f04f-146">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="5f04f-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5f04f-147">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5f04f-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="5f04f-148">正しくない</span><span class="sxs-lookup"><span data-stu-id="5f04f-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5f04f-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="5f04f-149">See also</span></span>

- [<span data-ttu-id="5f04f-150">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="5f04f-150">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="5f04f-151">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="5f04f-151">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


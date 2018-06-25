---
title: DayOfWeek (タイムゾーン)
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
description: DayOfWeek の要素では、タイム ゾーンの切り替えが発生する曜日を表します。
ms.openlocfilehash: 7816b90000be36cf3a3354d26d978684bfdcfe40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759935"
---
# <a name="dayofweek-timezone"></a><span data-ttu-id="144c3-103">DayOfWeek (タイムゾーン)</span><span class="sxs-lookup"><span data-stu-id="144c3-103">DayOfWeek (TimeZone)</span></span>

<span data-ttu-id="144c3-104">**DayOfWeek**の要素では、タイム ゾーンの切り替えが発生する曜日を表します。</span><span class="sxs-lookup"><span data-stu-id="144c3-104">The **DayOfWeek** element represents the day of the week on which the time zone transition occurs.</span></span> 
  
```xml
<DayOfWeek>...</DayOfWeek>
```

<span data-ttu-id="144c3-105">**DayOfWeekType**</span><span class="sxs-lookup"><span data-stu-id="144c3-105">**DayOfWeekType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="144c3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="144c3-106">Attributes and elements</span></span>

<span data-ttu-id="144c3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="144c3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="144c3-108">属性</span><span class="sxs-lookup"><span data-stu-id="144c3-108">Attributes</span></span>

<span data-ttu-id="144c3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="144c3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="144c3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="144c3-110">Child elements</span></span>

<span data-ttu-id="144c3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="144c3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="144c3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="144c3-112">Parent elements</span></span>

|<span data-ttu-id="144c3-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="144c3-113">**Element**</span></span>|<span data-ttu-id="144c3-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="144c3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="144c3-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="144c3-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="144c3-116">基準にして世界協定時刻 (UTC)[バイアス (UTC)](bias-utc.md)の要素で表される時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="144c3-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span><br/><br/><span data-ttu-id="144c3-117">この要素は、夏時間が発生した地域で夏時間から切り替えに関する情報を標準時も含みます。</span><span class="sxs-lookup"><span data-stu-id="144c3-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="144c3-118">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="144c3-118">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="144c3-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="144c3-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="144c3-120">夏時間が発生した地域の[バイアス (UTC)](bias-utc.md)の要素で表される UTC 時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="144c3-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="144c3-121">この要素には、標準時間から夏時間への切り替えが発生した場合についての情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="144c3-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span><br/><br/><span data-ttu-id="144c3-122">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="144c3-122">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
|[<span data-ttu-id="144c3-123">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="144c3-123">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="144c3-124">毎年同じ日に発生するタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="144c3-124">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="144c3-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="144c3-125">Text value</span></span>

<span data-ttu-id="144c3-126">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="144c3-126">A text value is required.</span></span> <span data-ttu-id="144c3-127">テキスト値は、次の値を持つ列挙型で表されます。</span><span class="sxs-lookup"><span data-stu-id="144c3-127">The text value is represented by an enumeration that has the following possible values:</span></span>
  
- <span data-ttu-id="144c3-128">日曜日</span><span class="sxs-lookup"><span data-stu-id="144c3-128">Sunday</span></span>    
- <span data-ttu-id="144c3-129">月曜日</span><span class="sxs-lookup"><span data-stu-id="144c3-129">Monday</span></span>    
- <span data-ttu-id="144c3-130">火曜日</span><span class="sxs-lookup"><span data-stu-id="144c3-130">Tuesday</span></span>    
- <span data-ttu-id="144c3-131">水曜日</span><span class="sxs-lookup"><span data-stu-id="144c3-131">Wednesday</span></span>    
- <span data-ttu-id="144c3-132">木曜日</span><span class="sxs-lookup"><span data-stu-id="144c3-132">Thursday</span></span>    
- <span data-ttu-id="144c3-133">金曜日</span><span class="sxs-lookup"><span data-stu-id="144c3-133">Friday</span></span>    
- <span data-ttu-id="144c3-134">土曜日</span><span class="sxs-lookup"><span data-stu-id="144c3-134">Saturday</span></span>    
- <span data-ttu-id="144c3-135">日</span><span class="sxs-lookup"><span data-stu-id="144c3-135">Day</span></span>    
- <span data-ttu-id="144c3-136">週日</span><span class="sxs-lookup"><span data-stu-id="144c3-136">Weekday</span></span>   
- <span data-ttu-id="144c3-137">WeekendDay</span><span class="sxs-lookup"><span data-stu-id="144c3-137">WeekendDay</span></span>
    
## <a name="remarks"></a><span data-ttu-id="144c3-138">備考</span><span class="sxs-lookup"><span data-stu-id="144c3-138">Remarks</span></span>

<span data-ttu-id="144c3-139">5 の値を持つ[DayOrder](dayorder.md)要素、10 の値を持つ[月](month.md)の要素、および**日曜日の値を持つ値**が含まれている[StandardTime](standardtime.md)要素は、標準時間から夏時間への移行を提供します。時間の節約は、10 月の 5 番目の日曜日に発生します。</span><span class="sxs-lookup"><span data-stu-id="144c3-139">A [StandardTime](standardtime.md) element that contains a [DayOrder](dayorder.md) element that has a value of 5, a [Month](month.md) element that has a value of 10, and a **DayOfWeek** element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
<span data-ttu-id="144c3-140">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="144c3-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="144c3-141">要素情報</span><span class="sxs-lookup"><span data-stu-id="144c3-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="144c3-142">名前空間</span><span class="sxs-lookup"><span data-stu-id="144c3-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="144c3-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="144c3-143">Schema Name</span></span>  <br/> |<span data-ttu-id="144c3-144">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="144c3-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="144c3-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="144c3-145">Validation File</span></span>  <br/> |<span data-ttu-id="144c3-146">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="144c3-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="144c3-147">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="144c3-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="144c3-148">False</span><span class="sxs-lookup"><span data-stu-id="144c3-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="144c3-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="144c3-149">See also</span></span>

- [<span data-ttu-id="144c3-150">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="144c3-150">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="144c3-151">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="144c3-151">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


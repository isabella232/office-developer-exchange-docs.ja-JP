---
title: StandardTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StandardTime
api_type:
- schema
ms.assetid: 13084726-ab24-4009-be99-c4a4273c9e05
description: StandardTime 要素を基準にして世界協定時刻 (UTC) バイアス (UTC) の要素で表される時間からのオフセットを表します。 この要素は、夏時間が発生した地域で夏時間から切り替えに関する情報を標準時も含みます。
ms.openlocfilehash: 726c31ffba06c1c437711b88444ec5eba45b520d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833546"
---
# <a name="standardtime"></a><span data-ttu-id="8666c-104">StandardTime</span><span class="sxs-lookup"><span data-stu-id="8666c-104">StandardTime</span></span>

<span data-ttu-id="8666c-105">**StandardTime**要素を基準にして世界協定時刻 (UTC)[バイアス (UTC)](bias-utc.md)の要素で表される時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="8666c-105">The **StandardTime** element represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="8666c-106">この要素は、夏時間が発生した地域で夏時間から切り替えに関する情報を標準時も含みます。</span><span class="sxs-lookup"><span data-stu-id="8666c-106">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span> 
  
- [<span data-ttu-id="8666c-107">タイムゾーン (可用性)</span><span class="sxs-lookup"><span data-stu-id="8666c-107">TimeZone (Availability)</span></span>](timezone-availability.md)
- [<span data-ttu-id="8666c-108">StandardTime</span><span class="sxs-lookup"><span data-stu-id="8666c-108">StandardTime</span></span>](standardtime.md)
  
```xml
<StandardTime>
   <Bias>int</Bias>
   <Time>string</Time>
   <DayOrder>short</DayOrder>
   <Month>short</Month>
   <DayOfWeek>Sunday or Monday or Tuesday or Wednesday or Thursday or Friday or Saturday</DayOfWeek>
   <Year>string</Year>
</StandardTime>
```

 <span data-ttu-id="8666c-109">**SerializableTimeZoneTime**</span><span class="sxs-lookup"><span data-stu-id="8666c-109">**SerializableTimeZoneTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8666c-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8666c-110">Attributes and elements</span></span>

<span data-ttu-id="8666c-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8666c-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8666c-112">属性</span><span class="sxs-lookup"><span data-stu-id="8666c-112">Attributes</span></span>

<span data-ttu-id="8666c-113">なし。</span><span class="sxs-lookup"><span data-stu-id="8666c-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8666c-114">子要素</span><span class="sxs-lookup"><span data-stu-id="8666c-114">Child elements</span></span>

|<span data-ttu-id="8666c-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="8666c-115">**Element**</span></span>|<span data-ttu-id="8666c-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="8666c-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8666c-117">Bias</span><span class="sxs-lookup"><span data-stu-id="8666c-117">Bias</span></span>](bias.md) <br/> |<span data-ttu-id="8666c-118">標準時間と夏時間の[時差 (UTC)](bias-utc.md)の要素で識別されている UTC オフセットからのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="8666c-118">Represents the offset from the UTC offset that is identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="8666c-119">この値は分単位です。</span><span class="sxs-lookup"><span data-stu-id="8666c-119">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="8666c-120">時間</span><span class="sxs-lookup"><span data-stu-id="8666c-120">Time</span></span>](time.md) <br/> |<span data-ttu-id="8666c-121">標準時間と夏時間との間に 1 日の切り替え時間を表します。</span><span class="sxs-lookup"><span data-stu-id="8666c-121">Represents the transition time of day to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="8666c-122">DayOrder</span><span class="sxs-lookup"><span data-stu-id="8666c-122">DayOrder</span></span>](dayorder.md) <br/> |<span data-ttu-id="8666c-123">標準時間と夏時間との切り替えの日付を表す[曜日 (タイムゾーン)](dayofweek-timezone.md)の要素で指定されている日の _n_th の発生を表します。</span><span class="sxs-lookup"><span data-stu-id="8666c-123">Represents the  _n_th occurrence of the day that is specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="8666c-124">Month</span><span class="sxs-lookup"><span data-stu-id="8666c-124">Month</span></span>](month.md) <br/> |<span data-ttu-id="8666c-125">標準時間と夏時間との間の切り替えの月を表します。</span><span class="sxs-lookup"><span data-stu-id="8666c-125">Represents the transition month of the year to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="8666c-126">DayOfWeek (タイムゾーン)</span><span class="sxs-lookup"><span data-stu-id="8666c-126">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="8666c-127">標準時間と夏時間からの切り替えが発生する曜日を表します。</span><span class="sxs-lookup"><span data-stu-id="8666c-127">Represents the day of the week when the transition to and from standard time and daylight saving time occurs.</span></span>  <br/> |
|[<span data-ttu-id="8666c-128">年</span><span class="sxs-lookup"><span data-stu-id="8666c-128">Year</span></span>](year.md) <br/> |<span data-ttu-id="8666c-129">年によって変更されるタイム ゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="8666c-129">Defines a time zone that changes depending on the year.</span></span> <span data-ttu-id="8666c-130">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="8666c-130">This element is optional.</span></span> <span data-ttu-id="8666c-131">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8666c-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8666c-132">親要素</span><span class="sxs-lookup"><span data-stu-id="8666c-132">Parent elements</span></span>

|<span data-ttu-id="8666c-133">**要素**</span><span class="sxs-lookup"><span data-stu-id="8666c-133">**Element**</span></span>|<span data-ttu-id="8666c-134">**説明**</span><span class="sxs-lookup"><span data-stu-id="8666c-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8666c-135">タイムゾーン (可用性)</span><span class="sxs-lookup"><span data-stu-id="8666c-135">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="8666c-136">タイム ゾーン情報を識別する要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8666c-136">Contains elements that identify time zone information.</span></span> <span data-ttu-id="8666c-137">この要素には、標準時と夏時間の切り替えに関する情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="8666c-137">This element also contains information about the transition between standard time and daylight saving time.</span></span> <br/><br/><span data-ttu-id="8666c-138">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="8666c-138">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/> <br/> `/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8666c-139">備考</span><span class="sxs-lookup"><span data-stu-id="8666c-139">Remarks</span></span>

<span data-ttu-id="8666c-140">**StandardTime**要素は、[バイアス (UTC)](bias-utc.md)の要素で表されるオフセットの時間を表します。</span><span class="sxs-lookup"><span data-stu-id="8666c-140">The **StandardTime** element represents an offset time that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="8666c-141">[バイアス](bias.md)の子要素には、0 が等しくなると、標準時はバイアス オフセット[バイアス (UTC)](bias-utc.md)の要素で表される UTC からです。</span><span class="sxs-lookup"><span data-stu-id="8666c-141">When the child [Bias](bias.md) element equals 0, the standard time is equal to the bias offset from UTC that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="8666c-142">例</span><span class="sxs-lookup"><span data-stu-id="8666c-142">Example</span></span>

<span data-ttu-id="8666c-143">次の使用例は、夏時間の期間が守られている領域を示しています。</span><span class="sxs-lookup"><span data-stu-id="8666c-143">The following example shows a region where daylight saving time is observed.</span></span> <span data-ttu-id="8666c-144">午前 2 時に夏時間から標準時への移行が発生しました。</span><span class="sxs-lookup"><span data-stu-id="8666c-144">The transition from daylight saving time to standard time is observed at 2 A.M.</span></span> <span data-ttu-id="8666c-145">10 か月目の 5 番目の日曜日。</span><span class="sxs-lookup"><span data-stu-id="8666c-145">on the fifth Sunday of the tenth month.</span></span>
  
```xml
<TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>5</DayOrder>
    <Month>10</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>4</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </DaylightTime>
</TimeZone>
```

## <a name="element-information"></a><span data-ttu-id="8666c-146">要素情報</span><span class="sxs-lookup"><span data-stu-id="8666c-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8666c-147">名前空間</span><span class="sxs-lookup"><span data-stu-id="8666c-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8666c-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8666c-148">Schema Name</span></span>  <br/> |<span data-ttu-id="8666c-149">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8666c-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="8666c-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8666c-150">Validation File</span></span>  <br/> |<span data-ttu-id="8666c-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8666c-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8666c-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8666c-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="8666c-153">False</span><span class="sxs-lookup"><span data-stu-id="8666c-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8666c-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="8666c-154">See also</span></span>

- [<span data-ttu-id="8666c-155">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="8666c-155">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="8666c-156">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="8666c-156">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


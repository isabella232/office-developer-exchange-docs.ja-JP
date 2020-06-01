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
description: StandardTime 要素は、バイアス (UTC) 要素で表される協定世界時 (UTC) を基準とした時刻からのオフセットを表します。 この要素には、夏時間が計測される地域で夏時間から標準時への切り替えに関する情報も含まれます。
ms.openlocfilehash: 793f058840d4fd9216f03e660f5be0f7564906cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456403"
---
# <a name="standardtime"></a><span data-ttu-id="d3ffd-104">StandardTime</span><span class="sxs-lookup"><span data-stu-id="d3ffd-104">StandardTime</span></span>

<span data-ttu-id="d3ffd-105">**Standardtime**要素は、[バイアス (utc](bias-utc.md) ) 要素で表される協定世界時 (utc) を基準とした時刻からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-105">The **StandardTime** element represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="d3ffd-106">この要素には、夏時間が計測される地域で夏時間から標準時への切り替えに関する情報も含まれます。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-106">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span> 
  
- [<span data-ttu-id="d3ffd-107">TimeZone (Availability)</span><span class="sxs-lookup"><span data-stu-id="d3ffd-107">TimeZone (Availability)</span></span>](timezone-availability.md)
- [<span data-ttu-id="d3ffd-108">StandardTime</span><span class="sxs-lookup"><span data-stu-id="d3ffd-108">StandardTime</span></span>](standardtime.md)
  
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

 <span data-ttu-id="d3ffd-109">**SerializableTimeZoneTime**</span><span class="sxs-lookup"><span data-stu-id="d3ffd-109">**SerializableTimeZoneTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3ffd-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d3ffd-110">Attributes and elements</span></span>

<span data-ttu-id="d3ffd-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3ffd-112">属性</span><span class="sxs-lookup"><span data-stu-id="d3ffd-112">Attributes</span></span>

<span data-ttu-id="d3ffd-113">なし。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3ffd-114">子要素</span><span class="sxs-lookup"><span data-stu-id="d3ffd-114">Child elements</span></span>

|<span data-ttu-id="d3ffd-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="d3ffd-115">**Element**</span></span>|<span data-ttu-id="d3ffd-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="d3ffd-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3ffd-117">バイアス</span><span class="sxs-lookup"><span data-stu-id="d3ffd-117">Bias</span></span>](bias.md) <br/> |<span data-ttu-id="d3ffd-118">標準時と夏時間の[時差 (utc)](bias-utc.md)要素によって識別される utc オフセットからのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-118">Represents the offset from the UTC offset that is identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="d3ffd-119">この値は分単位です。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-119">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="d3ffd-120">Time</span><span class="sxs-lookup"><span data-stu-id="d3ffd-120">Time</span></span>](time.md) <br/> |<span data-ttu-id="d3ffd-121">標準時と夏時間の切り替え時間を表します。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-121">Represents the transition time of day to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="d3ffd-122">DayOrder</span><span class="sxs-lookup"><span data-stu-id="d3ffd-122">DayOrder</span></span>](dayorder.md) <br/> |<span data-ttu-id="d3ffd-123">標準時および夏時間への切り替えの日付を表す、 [DayOfWeek (TimeZone)](dayofweek-timezone.md)要素で指定された日の _n_th 発生を表します。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-123">Represents the  _n_th occurrence of the day that is specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="d3ffd-124">Month</span><span class="sxs-lookup"><span data-stu-id="d3ffd-124">Month</span></span>](month.md) <br/> |<span data-ttu-id="d3ffd-125">標準時と夏時間との間の年間の移行月を表します。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-125">Represents the transition month of the year to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="d3ffd-126">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="d3ffd-126">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="d3ffd-127">標準時および夏時間からの切り替えが行われる曜日を表します。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-127">Represents the day of the week when the transition to and from standard time and daylight saving time occurs.</span></span>  <br/> |
|[<span data-ttu-id="d3ffd-128">Year</span><span class="sxs-lookup"><span data-stu-id="d3ffd-128">Year</span></span>](year.md) <br/> |<span data-ttu-id="d3ffd-129">年に応じて変更されるタイムゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-129">Defines a time zone that changes depending on the year.</span></span> <span data-ttu-id="d3ffd-130">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-130">This element is optional.</span></span> <span data-ttu-id="d3ffd-131">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3ffd-132">親要素</span><span class="sxs-lookup"><span data-stu-id="d3ffd-132">Parent elements</span></span>

|<span data-ttu-id="d3ffd-133">**要素**</span><span class="sxs-lookup"><span data-stu-id="d3ffd-133">**Element**</span></span>|<span data-ttu-id="d3ffd-134">**説明**</span><span class="sxs-lookup"><span data-stu-id="d3ffd-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3ffd-135">TimeZone (Availability)</span><span class="sxs-lookup"><span data-stu-id="d3ffd-135">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="d3ffd-136">タイムゾーン情報を識別する要素を格納します。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-136">Contains elements that identify time zone information.</span></span> <span data-ttu-id="d3ffd-137">この要素には、標準時から夏時間への切り替えに関する情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-137">This element also contains information about the transition between standard time and daylight saving time.</span></span> <br/><br/><span data-ttu-id="d3ffd-138">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-138">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/> <br/> `/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d3ffd-139">注釈</span><span class="sxs-lookup"><span data-stu-id="d3ffd-139">Remarks</span></span>

<span data-ttu-id="d3ffd-140">**Standardtime**要素は、 [Bias (UTC)](bias-utc.md)要素で表されるオフセット時間を表します。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-140">The **StandardTime** element represents an offset time that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="d3ffd-141">子[バイアス](bias.md)要素が0と等しい場合、標準時は[bias (utc)](bias-utc.md)要素で表される、utc からのバイアスオフセットと等しくなります。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-141">When the child [Bias](bias.md) element equals 0, the standard time is equal to the bias offset from UTC that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="d3ffd-142">例</span><span class="sxs-lookup"><span data-stu-id="d3ffd-142">Example</span></span>

<span data-ttu-id="d3ffd-143">次の例は、夏時間が測定される地域を示しています。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-143">The following example shows a region where daylight saving time is observed.</span></span> <span data-ttu-id="d3ffd-144">夏時間から標準時への切り替えは午前2時に発生します。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-144">The transition from daylight saving time to standard time is observed at 2 A.M.</span></span> <span data-ttu-id="d3ffd-145">10月の5番目の日曜日。</span><span class="sxs-lookup"><span data-stu-id="d3ffd-145">on the fifth Sunday of the tenth month.</span></span>
  
```xml
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="d3ffd-146">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d3ffd-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3ffd-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="d3ffd-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d3ffd-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d3ffd-148">Schema Name</span></span>  <br/> |<span data-ttu-id="d3ffd-149">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d3ffd-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="d3ffd-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d3ffd-150">Validation File</span></span>  <br/> |<span data-ttu-id="d3ffd-151">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d3ffd-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d3ffd-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d3ffd-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="d3ffd-153">正しくない</span><span class="sxs-lookup"><span data-stu-id="d3ffd-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3ffd-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="d3ffd-154">See also</span></span>

- [<span data-ttu-id="d3ffd-155">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="d3ffd-155">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="d3ffd-156">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="d3ffd-156">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


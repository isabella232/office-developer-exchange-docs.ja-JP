---
title: DaylightTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DaylightTime
api_type:
- schema
ms.assetid: 9f551ee4-d945-477c-b981-9554b197d26d
description: DaylightTime 要素は、夏時間 (utc) を基準とした時刻からのオフセットを表し、夏時間が発生する地域の時差 (UTC) 要素によって表されます。 この要素には、標準時から夏時間への切り替えが行われるタイミングに関する情報も含まれています。
ms.openlocfilehash: 350fcb4ce278f423c62fcc5ecaa160eda71e4a2c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455654"
---
# <a name="daylighttime"></a><span data-ttu-id="b3591-104">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="b3591-104">DaylightTime</span></span>

<span data-ttu-id="b3591-105">**Daylighttime**要素は、夏時間 (utc) を基準とした時刻からのオフセットを表し、夏時間が発生する地域の[時差 (utc)](bias-utc.md)要素によって表されます。</span><span class="sxs-lookup"><span data-stu-id="b3591-105">The **DaylightTime** element represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="b3591-106">この要素には、標準時から夏時間への切り替えが行われるタイミングに関する情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="b3591-106">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span> 
  
- [<span data-ttu-id="b3591-107">TimeZone (Availability)</span><span class="sxs-lookup"><span data-stu-id="b3591-107">TimeZone (Availability)</span></span>](timezone-availability.md) 
- [<span data-ttu-id="b3591-108">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="b3591-108">DaylightTime</span></span>](daylighttime.md)
  
```xml
<DaylightTime>
   <Bias>int</Bias>
   <Time>string</Time>
   <DayOrder>short</DayOrder>
   <Month>short</Month>
   <DayOfWeek>Sunday or Monday or Tuesday or Wednesday or Thursday or Friday or Saturday</DayOfWeek>
   <Year>string</Year>
</DaylightTime>
```

<span data-ttu-id="b3591-109">**SerializableTimeZoneTime**</span><span class="sxs-lookup"><span data-stu-id="b3591-109">**SerializableTimeZoneTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b3591-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b3591-110">Attributes and elements</span></span>

<span data-ttu-id="b3591-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b3591-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b3591-112">属性</span><span class="sxs-lookup"><span data-stu-id="b3591-112">Attributes</span></span>

<span data-ttu-id="b3591-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b3591-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b3591-114">子要素</span><span class="sxs-lookup"><span data-stu-id="b3591-114">Child elements</span></span>

|<span data-ttu-id="b3591-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="b3591-115">**Element**</span></span>|<span data-ttu-id="b3591-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="b3591-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3591-117">バイアス</span><span class="sxs-lookup"><span data-stu-id="b3591-117">Bias</span></span>](bias.md) <br/> |<span data-ttu-id="b3591-118">標準時と夏時間の[時差 (utc)](bias-utc.md)要素によって識別される utc オフセットからのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="b3591-118">Represents the offset from the UTC offset that is identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="b3591-119">この値は分単位です。</span><span class="sxs-lookup"><span data-stu-id="b3591-119">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="b3591-120">Time</span><span class="sxs-lookup"><span data-stu-id="b3591-120">Time</span></span>](time.md) <br/> |<span data-ttu-id="b3591-121">標準時と夏時間の切り替え時間を表します。</span><span class="sxs-lookup"><span data-stu-id="b3591-121">Represents the transition time of day to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="b3591-122">DayOrder</span><span class="sxs-lookup"><span data-stu-id="b3591-122">DayOrder</span></span>](dayorder.md) <br/> |<span data-ttu-id="b3591-123">標準時および夏時間への切り替えの日付を表す、 [DayOfWeek (TimeZone)](dayofweek-timezone.md)要素で指定された日の _n_th 発生を表します。</span><span class="sxs-lookup"><span data-stu-id="b3591-123">Represents the  _n_th occurrence of the day that is specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="b3591-124">Month</span><span class="sxs-lookup"><span data-stu-id="b3591-124">Month</span></span>](month.md) <br/> |<span data-ttu-id="b3591-125">標準時と夏時間との間の年間の移行月を表します。</span><span class="sxs-lookup"><span data-stu-id="b3591-125">Represents the transition month of the year to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="b3591-126">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="b3591-126">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="b3591-127">標準時および夏時間からの切り替えが行われる曜日を表します。</span><span class="sxs-lookup"><span data-stu-id="b3591-127">Represents the day of the week when the transition to and from standard time and daylight saving time occurs.</span></span>  <br/> |
|[<span data-ttu-id="b3591-128">Year</span><span class="sxs-lookup"><span data-stu-id="b3591-128">Year</span></span>](year.md) <br/> |<span data-ttu-id="b3591-129">年に応じて変更されるタイムゾーンを定義するために使用します。</span><span class="sxs-lookup"><span data-stu-id="b3591-129">Used to define a time zone that changes depending on the year.</span></span> <span data-ttu-id="b3591-130">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="b3591-130">This element is optional.</span></span> <span data-ttu-id="b3591-131">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b3591-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b3591-132">親要素</span><span class="sxs-lookup"><span data-stu-id="b3591-132">Parent elements</span></span>

|<span data-ttu-id="b3591-133">**要素**</span><span class="sxs-lookup"><span data-stu-id="b3591-133">**Element**</span></span>|<span data-ttu-id="b3591-134">**説明**</span><span class="sxs-lookup"><span data-stu-id="b3591-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3591-135">TimeZone (Availability)</span><span class="sxs-lookup"><span data-stu-id="b3591-135">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="b3591-136">タイムゾーン情報を識別する要素を格納します。</span><span class="sxs-lookup"><span data-stu-id="b3591-136">Contains elements that identify time zone information.</span></span><br/><br/><span data-ttu-id="b3591-137">この要素には、標準時から夏時間への切り替えに関する情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="b3591-137">This element also contains information about the transition between standard time and daylight saving time.</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="example"></a><span data-ttu-id="b3591-138">例</span><span class="sxs-lookup"><span data-stu-id="b3591-138">Example</span></span>

<span data-ttu-id="b3591-139">次の部分的な GetUserAvailability 要求は、夏時間を認識する場所にあるクライアントアプリケーションを表します。</span><span class="sxs-lookup"><span data-stu-id="b3591-139">The following partial GetUserAvailability request represents a client application in a location that recognizes daylight saving time.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="b3591-140">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b3591-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b3591-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="b3591-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b3591-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b3591-142">Schema Name</span></span>  <br/> |<span data-ttu-id="b3591-143">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b3591-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="b3591-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b3591-144">Validation File</span></span>  <br/> |<span data-ttu-id="b3591-145">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b3591-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b3591-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b3591-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="b3591-147">正しくない</span><span class="sxs-lookup"><span data-stu-id="b3591-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b3591-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="b3591-148">See also</span></span>

- [<span data-ttu-id="b3591-149">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="b3591-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="b3591-150">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="b3591-150">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


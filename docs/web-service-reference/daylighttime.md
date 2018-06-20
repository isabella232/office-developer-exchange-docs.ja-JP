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
description: DaylightTime 要素を基準にして世界協定時刻 (UTC) 夏時間が発生した地域のバイアス (UTC) の要素で表される時間からのオフセットを表します。 この要素には、標準時間から夏時間への切り替えが発生した場合についての情報も含まれています。
ms.openlocfilehash: 07ec4b1a5f84669aca33d46cdf1fa2e578f3b43b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759934"
---
# <a name="daylighttime"></a><span data-ttu-id="7d668-104">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="7d668-104">DaylightTime</span></span>

<span data-ttu-id="7d668-105">**DaylightTime**要素を基準にして世界協定時刻 (UTC) 夏時間が発生した地域の[バイアス (UTC)](bias-utc.md)の要素で表される時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="7d668-105">The **DaylightTime** element represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="7d668-106">この要素には、標準時間から夏時間への切り替えが発生した場合についての情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="7d668-106">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span> 
  
- [<span data-ttu-id="7d668-107">タイムゾーン (可用性)</span><span class="sxs-lookup"><span data-stu-id="7d668-107">TimeZone (Availability)</span></span>](timezone-availability.md) 
- [<span data-ttu-id="7d668-108">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="7d668-108">DaylightTime</span></span>](daylighttime.md)
  
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

<span data-ttu-id="7d668-109">**SerializableTimeZoneTime**</span><span class="sxs-lookup"><span data-stu-id="7d668-109">**SerializableTimeZoneTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7d668-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7d668-110">Attributes and elements</span></span>

<span data-ttu-id="7d668-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7d668-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d668-112">属性</span><span class="sxs-lookup"><span data-stu-id="7d668-112">Attributes</span></span>

<span data-ttu-id="7d668-113">なし。</span><span class="sxs-lookup"><span data-stu-id="7d668-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d668-114">子要素</span><span class="sxs-lookup"><span data-stu-id="7d668-114">Child elements</span></span>

|<span data-ttu-id="7d668-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="7d668-115">**Element**</span></span>|<span data-ttu-id="7d668-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="7d668-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d668-117">Bias</span><span class="sxs-lookup"><span data-stu-id="7d668-117">Bias</span></span>](bias.md) <br/> |<span data-ttu-id="7d668-118">標準時間と夏時間の[時差 (UTC)](bias-utc.md)の要素で識別されている UTC オフセットからのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="7d668-118">Represents the offset from the UTC offset that is identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="7d668-119">この値は分単位です。</span><span class="sxs-lookup"><span data-stu-id="7d668-119">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="7d668-120">時間</span><span class="sxs-lookup"><span data-stu-id="7d668-120">Time</span></span>](time.md) <br/> |<span data-ttu-id="7d668-121">標準時間と夏時間との間に 1 日の切り替え時間を表します。</span><span class="sxs-lookup"><span data-stu-id="7d668-121">Represents the transition time of day to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="7d668-122">DayOrder</span><span class="sxs-lookup"><span data-stu-id="7d668-122">DayOrder</span></span>](dayorder.md) <br/> |<span data-ttu-id="7d668-123">標準時間と夏時間との切り替えの日付を表す[曜日 (タイムゾーン)](dayofweek-timezone.md)の要素で指定されている日の _n_th の発生を表します。</span><span class="sxs-lookup"><span data-stu-id="7d668-123">Represents the  _n_th occurrence of the day that is specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="7d668-124">Month</span><span class="sxs-lookup"><span data-stu-id="7d668-124">Month</span></span>](month.md) <br/> |<span data-ttu-id="7d668-125">標準時間と夏時間との間の切り替えの月を表します。</span><span class="sxs-lookup"><span data-stu-id="7d668-125">Represents the transition month of the year to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="7d668-126">DayOfWeek (タイムゾーン)</span><span class="sxs-lookup"><span data-stu-id="7d668-126">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="7d668-127">標準時間と夏時間からの切り替えが発生する曜日を表します。</span><span class="sxs-lookup"><span data-stu-id="7d668-127">Represents the day of the week when the transition to and from standard time and daylight saving time occurs.</span></span>  <br/> |
|[<span data-ttu-id="7d668-128">年</span><span class="sxs-lookup"><span data-stu-id="7d668-128">Year</span></span>](year.md) <br/> |<span data-ttu-id="7d668-129">年によって変更されるタイム ゾーンの定義に使用されます。</span><span class="sxs-lookup"><span data-stu-id="7d668-129">Used to define a time zone that changes depending on the year.</span></span> <span data-ttu-id="7d668-130">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="7d668-130">This element is optional.</span></span> <span data-ttu-id="7d668-131">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7d668-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7d668-132">親要素</span><span class="sxs-lookup"><span data-stu-id="7d668-132">Parent elements</span></span>

|<span data-ttu-id="7d668-133">**要素**</span><span class="sxs-lookup"><span data-stu-id="7d668-133">**Element**</span></span>|<span data-ttu-id="7d668-134">**説明**</span><span class="sxs-lookup"><span data-stu-id="7d668-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d668-135">タイムゾーン (可用性)</span><span class="sxs-lookup"><span data-stu-id="7d668-135">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="7d668-136">タイム ゾーン情報を識別する要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7d668-136">Contains elements that identify time zone information.</span></span><br/><br/><span data-ttu-id="7d668-137">この要素には、標準時と夏時間の切り替えに関する情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="7d668-137">This element also contains information about the transition between standard time and daylight saving time.</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="example"></a><span data-ttu-id="7d668-138">例</span><span class="sxs-lookup"><span data-stu-id="7d668-138">Example</span></span>

<span data-ttu-id="7d668-139">次のような GetUserAvailability の部分の要求では、夏時間を認識する場所にクライアント アプリケーションを表します。</span><span class="sxs-lookup"><span data-stu-id="7d668-139">The following partial GetUserAvailability request represents a client application in a location that recognizes daylight saving time.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="7d668-140">要素情報</span><span class="sxs-lookup"><span data-stu-id="7d668-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d668-141">名前空間</span><span class="sxs-lookup"><span data-stu-id="7d668-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7d668-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7d668-142">Schema Name</span></span>  <br/> |<span data-ttu-id="7d668-143">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7d668-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="7d668-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7d668-144">Validation File</span></span>  <br/> |<span data-ttu-id="7d668-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7d668-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7d668-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7d668-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="7d668-147">False</span><span class="sxs-lookup"><span data-stu-id="7d668-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d668-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="7d668-148">See also</span></span>

- [<span data-ttu-id="7d668-149">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="7d668-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="7d668-150">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="7d668-150">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


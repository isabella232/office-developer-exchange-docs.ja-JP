---
title: TimeZone (Availability)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZone
api_type:
- schema
ms.assetid: d662ffae-1f93-4c08-85a4-c69de2f7c681
description: TimeZone 要素には、タイムゾーン情報を識別する要素が含まれています。 この要素には、標準時から夏時間への切り替えに関する情報も含まれています。
ms.openlocfilehash: ba4b0a4805dba54450e01e89c5e9ef746404b716
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460275"
---
# <a name="timezone-availability"></a><span data-ttu-id="6c240-104">TimeZone (Availability)</span><span class="sxs-lookup"><span data-stu-id="6c240-104">TimeZone (Availability)</span></span>

<span data-ttu-id="6c240-105">**TimeZone**要素には、タイムゾーン情報を識別する要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c240-105">The **TimeZone** element contains elements that identify time zone information.</span></span> <span data-ttu-id="6c240-106">この要素には、標準時から夏時間への切り替えに関する情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c240-106">This element also contains information about the transition between standard time and daylight saving time.</span></span> 
  
```xml
<TimeZone>
   <Bias/>
   <StandardTime/>
   <DaylightTime/>
</TimeZone>
```

 <span data-ttu-id="6c240-107">**SerializableTimeZone**</span><span class="sxs-lookup"><span data-stu-id="6c240-107">**SerializableTimeZone**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c240-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6c240-108">Attributes and elements</span></span>

<span data-ttu-id="6c240-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6c240-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c240-110">属性</span><span class="sxs-lookup"><span data-stu-id="6c240-110">Attributes</span></span>

<span data-ttu-id="6c240-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6c240-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c240-112">子要素</span><span class="sxs-lookup"><span data-stu-id="6c240-112">Child elements</span></span>

|<span data-ttu-id="6c240-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="6c240-113">**Element**</span></span>|<span data-ttu-id="6c240-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c240-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c240-115">Bias (UTC)</span><span class="sxs-lookup"><span data-stu-id="6c240-115">Bias (UTC)</span></span>](bias-utc.md) <br/> |<span data-ttu-id="6c240-116">協定世界時 (UTC) からの一般的なオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="6c240-116">Represents the general offset from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="6c240-117">この値は分単位です。</span><span class="sxs-lookup"><span data-stu-id="6c240-117">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="6c240-118">StandardTime</span><span class="sxs-lookup"><span data-stu-id="6c240-118">StandardTime</span></span>](standardtime.md) <br/> |<span data-ttu-id="6c240-119">[Bias (utc)](bias-utc.md)要素で表される utc を基準とした時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="6c240-119">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="6c240-120">この要素には、夏時間が計測される地域で夏時間から標準時への切り替えに関する情報も含まれます。</span><span class="sxs-lookup"><span data-stu-id="6c240-120">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span>  <br/> |
|[<span data-ttu-id="6c240-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="6c240-121">DaylightTime</span></span>](daylighttime.md) <br/> |<span data-ttu-id="6c240-122">夏時間が計測される地域で、 [Bias (utc)](bias-utc.md)要素によって表される utc を基準とした時刻からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="6c240-122">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="6c240-123">この要素には、標準時から夏時間への切り替えが行われるタイミングに関する情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c240-123">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6c240-124">親要素</span><span class="sxs-lookup"><span data-stu-id="6c240-124">Parent elements</span></span>

|<span data-ttu-id="6c240-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="6c240-125">**Element**</span></span>|<span data-ttu-id="6c240-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c240-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c240-127">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="6c240-127">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="6c240-128">ユーザーの空き時間情報を取得するために使用する引数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c240-128">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="6c240-129">これはルート要素です。</span><span class="sxs-lookup"><span data-stu-id="6c240-129">This is a root element.</span></span>  <br/> <span data-ttu-id="6c240-130">GetUserAvailabilityRequest message の**TimeZone**要素は、要求の DateTime 値が指定されているタイムゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="6c240-130">The **TimeZone** element in the GetUserAvailabilityRequest message represents the time zone in which the DateTime values in the request are specified.</span></span> <span data-ttu-id="6c240-131">Availability service によって返される DateTime 値もこのタイムゾーンに含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c240-131">The DateTime values returned by the Availability service are also in this time zone.</span></span>  <br/> <span data-ttu-id="6c240-132">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6c240-132">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[<span data-ttu-id="6c240-133">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="6c240-133">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6c240-134">要求されたメールボックスユーザーのタイムゾーン設定および稼働時間を表します。</span><span class="sxs-lookup"><span data-stu-id="6c240-134">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> <span data-ttu-id="6c240-135">GetUserAvailabilityResponse message の**TimeZone**要素は、要求されたメールボックスユーザーのタイムゾーン設定を表します。</span><span class="sxs-lookup"><span data-stu-id="6c240-135">The **TimeZone** element in the GetUserAvailabilityResponse message represents the time zone settings of the requested mailbox user.</span></span>  <br/> <span data-ttu-id="6c240-136">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6c240-136">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6c240-137">注釈</span><span class="sxs-lookup"><span data-stu-id="6c240-137">Remarks</span></span>

<span data-ttu-id="6c240-138">この要素は[GetUserAvailabilityRequest](getuseravailabilityrequest.md)要素で必要です。</span><span class="sxs-lookup"><span data-stu-id="6c240-138">This element is required in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md) element.</span></span> <span data-ttu-id="6c240-139">この要素は、親要素が[WorkingHours](workinghours-ex15websvcsotherref.md)要素の数回または少なくとも0回発生します。</span><span class="sxs-lookup"><span data-stu-id="6c240-139">This element occurs at most once or at least zero times when the parent element is the [WorkingHours](workinghours-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="6c240-140">例</span><span class="sxs-lookup"><span data-stu-id="6c240-140">Example</span></span>

<span data-ttu-id="6c240-141">次の例は、クライアントアプリケーションで8時間の UTC からのオフセットを識別する XML 要求の一部を示しています。</span><span class="sxs-lookup"><span data-stu-id="6c240-141">The following example shows part of an XML request that identifies an offset from UTC of 8 hours in the client application.</span></span>
  
```XML
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>11</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>2</DayOrder>
    <Month>3</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </DaylightTime>
</TimeZone>
```

## <a name="element-information"></a><span data-ttu-id="6c240-142">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6c240-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c240-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="6c240-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6c240-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6c240-144">Schema Name</span></span>  <br/> |<span data-ttu-id="6c240-145">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6c240-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="6c240-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6c240-146">Validation File</span></span>  <br/> |<span data-ttu-id="6c240-147">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6c240-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6c240-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6c240-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="6c240-149">正しくない</span><span class="sxs-lookup"><span data-stu-id="6c240-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c240-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="6c240-150">See also</span></span>



[<span data-ttu-id="6c240-151">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="6c240-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="6c240-152">バイアス</span><span class="sxs-lookup"><span data-stu-id="6c240-152">Bias</span></span>](bias.md)


[<span data-ttu-id="6c240-153">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="6c240-153">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


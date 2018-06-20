---
title: タイムゾーン (可用性)
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
description: タイム ゾーン要素には、タイム ゾーン情報を識別する要素が含まれています。 この要素には、標準時と夏時間の切り替えに関する情報も含まれています。
ms.openlocfilehash: dc2466e8039819edc82294ff05f1746ada64cb43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839717"
---
# <a name="timezone-availability"></a><span data-ttu-id="c9be8-104">タイムゾーン (可用性)</span><span class="sxs-lookup"><span data-stu-id="c9be8-104">TimeZone (Availability)</span></span>

<span data-ttu-id="c9be8-105">**タイム ゾーン**要素には、タイム ゾーン情報を識別する要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c9be8-105">The **TimeZone** element contains elements that identify time zone information.</span></span> <span data-ttu-id="c9be8-106">この要素には、標準時と夏時間の切り替えに関する情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="c9be8-106">This element also contains information about the transition between standard time and daylight saving time.</span></span> 
  
```xml
<TimeZone>
   <Bias/>
   <StandardTime/>
   <DaylightTime/>
</TimeZone>
```

 <span data-ttu-id="c9be8-107">**SerializableTimeZone**</span><span class="sxs-lookup"><span data-stu-id="c9be8-107">**SerializableTimeZone**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9be8-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c9be8-108">Attributes and elements</span></span>

<span data-ttu-id="c9be8-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c9be8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9be8-110">属性</span><span class="sxs-lookup"><span data-stu-id="c9be8-110">Attributes</span></span>

<span data-ttu-id="c9be8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c9be8-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9be8-112">子要素</span><span class="sxs-lookup"><span data-stu-id="c9be8-112">Child elements</span></span>

|<span data-ttu-id="c9be8-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c9be8-113">**Element**</span></span>|<span data-ttu-id="c9be8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c9be8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9be8-115">バイアス (UTC)</span><span class="sxs-lookup"><span data-stu-id="c9be8-115">Bias (UTC)</span></span>](bias-utc.md) <br/> |<span data-ttu-id="c9be8-116">世界協定時刻 (UTC) から一般のオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="c9be8-116">Represents the general offset from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="c9be8-117">この値は分単位です。</span><span class="sxs-lookup"><span data-stu-id="c9be8-117">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="c9be8-118">StandardTime</span><span class="sxs-lookup"><span data-stu-id="c9be8-118">StandardTime</span></span>](standardtime.md) <br/> |<span data-ttu-id="c9be8-119">[バイアス (UTC)](bias-utc.md)の要素で表される UTC 時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="c9be8-119">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="c9be8-120">この要素は、夏時間が発生した地域で夏時間から切り替えに関する情報を標準時も含みます。</span><span class="sxs-lookup"><span data-stu-id="c9be8-120">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span>  <br/> |
|[<span data-ttu-id="c9be8-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="c9be8-121">DaylightTime</span></span>](daylighttime.md) <br/> |<span data-ttu-id="c9be8-122">夏時間が発生した地域の[バイアス (UTC)](bias-utc.md)の要素で表される UTC 時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="c9be8-122">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="c9be8-123">この要素には、標準時間から夏時間への切り替えが発生した場合についての情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="c9be8-123">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c9be8-124">親要素</span><span class="sxs-lookup"><span data-stu-id="c9be8-124">Parent elements</span></span>

|<span data-ttu-id="c9be8-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="c9be8-125">**Element**</span></span>|<span data-ttu-id="c9be8-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="c9be8-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9be8-127">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="c9be8-127">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="c9be8-128">ユーザーの利用可能時間情報を取得するための引数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c9be8-128">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="c9be8-129">これは、ルート要素です。</span><span class="sxs-lookup"><span data-stu-id="c9be8-129">This is a root element.</span></span>  <br/> <span data-ttu-id="c9be8-130">GetUserAvailabilityRequest メッセージの**タイム ゾーン**の要素は、要求内の DateTime 値が指定されているタイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="c9be8-130">The **TimeZone** element in the GetUserAvailabilityRequest message represents the time zone in which the DateTime values in the request are specified.</span></span> <span data-ttu-id="c9be8-131">可用性サービスによって返される DateTime 値は、このタイム ゾーンでもあります。</span><span class="sxs-lookup"><span data-stu-id="c9be8-131">The DateTime values returned by the Availability service are also in this time zone.</span></span>  <br/> <span data-ttu-id="c9be8-132">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="c9be8-132">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[<span data-ttu-id="c9be8-133">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="c9be8-133">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c9be8-134">要求されたメールボックスのユーザーの作業時間とタイム ゾーンの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="c9be8-134">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> <span data-ttu-id="c9be8-135">GetUserAvailabilityResponse メッセージの**タイム ゾーン**の要素は、要求されたメールボックス ユーザーのタイム ゾーンの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="c9be8-135">The **TimeZone** element in the GetUserAvailabilityResponse message represents the time zone settings of the requested mailbox user.</span></span>  <br/> <span data-ttu-id="c9be8-136">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="c9be8-136">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c9be8-137">備考</span><span class="sxs-lookup"><span data-stu-id="c9be8-137">Remarks</span></span>

<span data-ttu-id="c9be8-138">[GetUserAvailabilityRequest](getuseravailabilityrequest.md)要素では、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="c9be8-138">This element is required in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md) element.</span></span> <span data-ttu-id="c9be8-139">0 回以上すると、親要素は、 [WorkingHours](workinghours-ex15websvcsotherref.md)要素またはこの要素は最大で 1 回に発生します。</span><span class="sxs-lookup"><span data-stu-id="c9be8-139">This element occurs at most once or at least zero times when the parent element is the [WorkingHours](workinghours-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="c9be8-140">例</span><span class="sxs-lookup"><span data-stu-id="c9be8-140">Example</span></span>

<span data-ttu-id="c9be8-141">次の使用例は、クライアント アプリケーションで 8 時間の UTC からのオフセットを識別する XML 要求の一部を示しています。</span><span class="sxs-lookup"><span data-stu-id="c9be8-141">The following example shows part of an XML request that identifies an offset from UTC of 8 hours in the client application.</span></span>
  
```XML
<TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="c9be8-142">要素情報</span><span class="sxs-lookup"><span data-stu-id="c9be8-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9be8-143">名前空間</span><span class="sxs-lookup"><span data-stu-id="c9be8-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c9be8-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c9be8-144">Schema Name</span></span>  <br/> |<span data-ttu-id="c9be8-145">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c9be8-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="c9be8-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c9be8-146">Validation File</span></span>  <br/> |<span data-ttu-id="c9be8-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c9be8-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c9be8-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c9be8-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="c9be8-149">False</span><span class="sxs-lookup"><span data-stu-id="c9be8-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9be8-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="c9be8-150">See also</span></span>



[<span data-ttu-id="c9be8-151">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="c9be8-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="c9be8-152">Bias</span><span class="sxs-lookup"><span data-stu-id="c9be8-152">Bias</span></span>](bias.md)


[<span data-ttu-id="c9be8-153">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="c9be8-153">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


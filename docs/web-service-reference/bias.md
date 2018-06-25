---
title: Bias
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bias
api_type:
- schema
ms.assetid: ae10aa44-e6d3-483d-a3e6-bb9c45966810
description: バイアスの要素は、標準時間と夏時間の時差 (UTC) の要素で識別される、世界協定時刻 (UTC) オフセットからのオフセットを表します。 この値は分単位です。
ms.openlocfilehash: 770bf97b030ac1293595560bc269f54896e35a15
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759505"
---
# <a name="bias"></a><span data-ttu-id="86fa8-104">Bias</span><span class="sxs-lookup"><span data-stu-id="86fa8-104">Bias</span></span>

<span data-ttu-id="86fa8-105">**バイアス**の要素は、標準時間と夏時間の[時差 (UTC)](bias-utc.md)の要素で識別される、世界協定時刻 (UTC) オフセットからのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="86fa8-105">The **Bias** element represents the offset from the Coordinated Universal Time (UTC) offset identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="86fa8-106">この値は分単位です。</span><span class="sxs-lookup"><span data-stu-id="86fa8-106">This value is in minutes.</span></span> 
  
```xml
<Bias>...</Bias>
```

<span data-ttu-id="86fa8-107">**int**</span><span class="sxs-lookup"><span data-stu-id="86fa8-107">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="86fa8-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="86fa8-108">Attributes and elements</span></span>

<span data-ttu-id="86fa8-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="86fa8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86fa8-110">属性</span><span class="sxs-lookup"><span data-stu-id="86fa8-110">Attributes</span></span>

<span data-ttu-id="86fa8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="86fa8-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86fa8-112">子要素</span><span class="sxs-lookup"><span data-stu-id="86fa8-112">Child elements</span></span>

<span data-ttu-id="86fa8-113">なし。</span><span class="sxs-lookup"><span data-stu-id="86fa8-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="86fa8-114">親要素</span><span class="sxs-lookup"><span data-stu-id="86fa8-114">Parent elements</span></span>

|<span data-ttu-id="86fa8-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="86fa8-115">**Element**</span></span>|<span data-ttu-id="86fa8-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="86fa8-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86fa8-117">StandardTime</span><span class="sxs-lookup"><span data-stu-id="86fa8-117">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="86fa8-118">[バイアス (UTC)](bias-utc.md)の要素で表される UTC 時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="86fa8-118">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="86fa8-119">この要素は、夏時間が発生した地域で夏時間から切り替えに関する情報を標準時も含みます。</span><span class="sxs-lookup"><span data-stu-id="86fa8-119">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="86fa8-120">[StandardTime](standardtime.md)要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="86fa8-120">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span><br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="86fa8-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="86fa8-121">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="86fa8-122">夏時間が発生した地域の[バイアス (UTC)](bias-utc.md)の要素で表される UTC 時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="86fa8-122">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="86fa8-123">この要素には、標準時間から夏時間への切り替えが発生した場合についての情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="86fa8-123">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/><span data-ttu-id="86fa8-124">[DaylightTime](daylighttime.md)要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="86fa8-124">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span><br/><br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="86fa8-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="86fa8-125">Text value</span></span>

<span data-ttu-id="86fa8-126">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="86fa8-126">A text value is required.</span></span> <span data-ttu-id="86fa8-127">テキスト値は、整数を表します。</span><span class="sxs-lookup"><span data-stu-id="86fa8-127">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="86fa8-128">備考</span><span class="sxs-lookup"><span data-stu-id="86fa8-128">Remarks</span></span>

<span data-ttu-id="86fa8-129">現地時刻を決定するために使用するオフセットは、**バイアス**の要素の 1 つでのみ指定できます。</span><span class="sxs-lookup"><span data-stu-id="86fa8-129">The offset used to determine the local time can only be provided by one of the **Bias** elements.</span></span> <span data-ttu-id="86fa8-130">[DaylightTime](daylighttime.md)要素または[StandardTime](standardtime.md)要素と要素[のバイアス (UTC)](bias-utc.md)によって提供されるバイアスの要素の値の合計は、現地時刻を識別します。</span><span class="sxs-lookup"><span data-stu-id="86fa8-130">The sum of the values of the Bias element provided by the [DaylightTime](daylighttime.md) element or the [StandardTime](standardtime.md) element plus the [Bias (UTC)](bias-utc.md) element identifies the local time.</span></span> 
  
## <a name="example"></a><span data-ttu-id="86fa8-131">例</span><span class="sxs-lookup"><span data-stu-id="86fa8-131">Example</span></span>

<span data-ttu-id="86fa8-132">夏時間に従って ~ 60 分で、UTC からのオフセットを調整することによってユーザーを識別する XML 要求の一部を次の例に示します。</span><span class="sxs-lookup"><span data-stu-id="86fa8-132">The following example shows part of an XML request that identifies a user who observes daylight saving time by adjusting the offset from UTC by -60 minutes.</span></span> <span data-ttu-id="86fa8-133">これにより、バイアス 420 分 utc を基準とします。</span><span class="sxs-lookup"><span data-stu-id="86fa8-133">This effectively makes the bias 420 minutes from UTC.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="86fa8-134">要素情報</span><span class="sxs-lookup"><span data-stu-id="86fa8-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86fa8-135">名前空間</span><span class="sxs-lookup"><span data-stu-id="86fa8-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="86fa8-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="86fa8-136">Schema Name</span></span>  <br/> |<span data-ttu-id="86fa8-137">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="86fa8-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="86fa8-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="86fa8-138">Validation File</span></span>  <br/> |<span data-ttu-id="86fa8-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="86fa8-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="86fa8-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="86fa8-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="86fa8-141">False</span><span class="sxs-lookup"><span data-stu-id="86fa8-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="86fa8-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="86fa8-142">See also</span></span>

- [<span data-ttu-id="86fa8-143">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="86fa8-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="86fa8-144">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="86fa8-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


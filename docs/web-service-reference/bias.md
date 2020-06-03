---
title: バイアス
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
description: Bias 要素は、標準時および夏時間時に Bias (UTC) 要素によって識別される協定世界時 (UTC) オフセットからのオフセットを表します。 この値は分単位です。
ms.openlocfilehash: 6c9dce88f3eece9c793fb018114f07a85c7cb89b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460240"
---
# <a name="bias"></a><span data-ttu-id="04a43-104">バイアス</span><span class="sxs-lookup"><span data-stu-id="04a43-104">Bias</span></span>

<span data-ttu-id="04a43-105">**Bias**要素は、標準時および夏時間時に[bias (utc)](bias-utc.md)要素によって識別される協定世界時 (utc) オフセットからのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="04a43-105">The **Bias** element represents the offset from the Coordinated Universal Time (UTC) offset identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="04a43-106">この値は分単位です。</span><span class="sxs-lookup"><span data-stu-id="04a43-106">This value is in minutes.</span></span> 
  
```xml
<Bias>...</Bias>
```

<span data-ttu-id="04a43-107">**int**</span><span class="sxs-lookup"><span data-stu-id="04a43-107">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="04a43-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="04a43-108">Attributes and elements</span></span>

<span data-ttu-id="04a43-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="04a43-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04a43-110">属性</span><span class="sxs-lookup"><span data-stu-id="04a43-110">Attributes</span></span>

<span data-ttu-id="04a43-111">なし。</span><span class="sxs-lookup"><span data-stu-id="04a43-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04a43-112">子要素</span><span class="sxs-lookup"><span data-stu-id="04a43-112">Child elements</span></span>

<span data-ttu-id="04a43-113">なし。</span><span class="sxs-lookup"><span data-stu-id="04a43-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="04a43-114">親要素</span><span class="sxs-lookup"><span data-stu-id="04a43-114">Parent elements</span></span>

|<span data-ttu-id="04a43-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="04a43-115">**Element**</span></span>|<span data-ttu-id="04a43-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="04a43-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04a43-117">StandardTime</span><span class="sxs-lookup"><span data-stu-id="04a43-117">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="04a43-118">[Bias (utc)](bias-utc.md)要素で表される utc を基準とした時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="04a43-118">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="04a43-119">この要素には、夏時間が計測される地域で夏時間から標準時への切り替えに関する情報も含まれます。</span><span class="sxs-lookup"><span data-stu-id="04a43-119">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="04a43-120">[Standardtime](standardtime.md)要素に対する XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="04a43-120">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span><br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="04a43-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="04a43-121">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="04a43-122">夏時間が計測される地域で、 [Bias (utc)](bias-utc.md)要素によって表される utc を基準とした時刻からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="04a43-122">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="04a43-123">この要素には、標準時から夏時間への切り替えが行われるタイミングに関する情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="04a43-123">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/><span data-ttu-id="04a43-124">[Daylighttime](daylighttime.md)要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="04a43-124">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span><br/><br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="04a43-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="04a43-125">Text value</span></span>

<span data-ttu-id="04a43-126">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="04a43-126">A text value is required.</span></span> <span data-ttu-id="04a43-127">テキスト値は、整数を表します。</span><span class="sxs-lookup"><span data-stu-id="04a43-127">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="04a43-128">注釈</span><span class="sxs-lookup"><span data-stu-id="04a43-128">Remarks</span></span>

<span data-ttu-id="04a43-129">現地時刻を決定するために使用されるオフセットは、 **Bias**要素のいずれかによってのみ提供されます。</span><span class="sxs-lookup"><span data-stu-id="04a43-129">The offset used to determine the local time can only be provided by one of the **Bias** elements.</span></span> <span data-ttu-id="04a43-130">[Daylighttime](daylighttime.md)要素、 [standardtime](standardtime.md)要素、および[bias (UTC)](bias-utc.md)要素によって提供される bias 要素の値の合計は、現地時刻を示します。</span><span class="sxs-lookup"><span data-stu-id="04a43-130">The sum of the values of the Bias element provided by the [DaylightTime](daylighttime.md) element or the [StandardTime](standardtime.md) element plus the [Bias (UTC)](bias-utc.md) element identifies the local time.</span></span> 
  
## <a name="example"></a><span data-ttu-id="04a43-131">例</span><span class="sxs-lookup"><span data-stu-id="04a43-131">Example</span></span>

<span data-ttu-id="04a43-132">次の例は、UTC を60分間で調整して夏時間を管理するユーザーを識別する、XML 要求の一部を示しています。</span><span class="sxs-lookup"><span data-stu-id="04a43-132">The following example shows part of an XML request that identifies a user who observes daylight saving time by adjusting the offset from UTC by -60 minutes.</span></span> <span data-ttu-id="04a43-133">これにより、実質的に UTC から420分のずれが生じます。</span><span class="sxs-lookup"><span data-stu-id="04a43-133">This effectively makes the bias 420 minutes from UTC.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="04a43-134">要素の情報</span><span class="sxs-lookup"><span data-stu-id="04a43-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04a43-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="04a43-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04a43-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="04a43-136">Schema Name</span></span>  <br/> |<span data-ttu-id="04a43-137">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="04a43-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="04a43-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="04a43-138">Validation File</span></span>  <br/> |<span data-ttu-id="04a43-139">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="04a43-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="04a43-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="04a43-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="04a43-141">正しくない</span><span class="sxs-lookup"><span data-stu-id="04a43-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04a43-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="04a43-142">See also</span></span>

- [<span data-ttu-id="04a43-143">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="04a43-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="04a43-144">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="04a43-144">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


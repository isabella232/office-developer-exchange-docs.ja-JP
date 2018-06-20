---
title: バイアス (UTC)
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
ms.assetid: 15790d5a-5134-457b-8f2b-d9dee1f807a2
description: バイアス要素では、世界協定時刻 (UTC) から一般のオフセットを表します。 この値は分単位です。
ms.openlocfilehash: 43613593565ca15be97bd2a98dbe5c512dbe5fc7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759501"
---
# <a name="bias-utc"></a><span data-ttu-id="e2558-104">バイアス (UTC)</span><span class="sxs-lookup"><span data-stu-id="e2558-104">Bias (UTC)</span></span>

<span data-ttu-id="e2558-105">**バイアス**要素では、世界協定時刻 (UTC) から一般のオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="e2558-105">The **Bias** element represents the general offset from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="e2558-106">この値は分単位です。</span><span class="sxs-lookup"><span data-stu-id="e2558-106">This value is in minutes.</span></span> 
  
```xml
<TimeZone>
   <Bias>int</Bias>
</TimeZone>
```

<span data-ttu-id="e2558-107">**int**</span><span class="sxs-lookup"><span data-stu-id="e2558-107">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e2558-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e2558-108">Attributes and elements</span></span>

<span data-ttu-id="e2558-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e2558-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2558-110">属性</span><span class="sxs-lookup"><span data-stu-id="e2558-110">Attributes</span></span>

<span data-ttu-id="e2558-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e2558-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2558-112">子要素</span><span class="sxs-lookup"><span data-stu-id="e2558-112">Child elements</span></span>

<span data-ttu-id="e2558-113">なし。</span><span class="sxs-lookup"><span data-stu-id="e2558-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e2558-114">親要素</span><span class="sxs-lookup"><span data-stu-id="e2558-114">Parent elements</span></span>

|<span data-ttu-id="e2558-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="e2558-115">**Element**</span></span>|<span data-ttu-id="e2558-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="e2558-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2558-117">タイムゾーン (可用性)</span><span class="sxs-lookup"><span data-stu-id="e2558-117">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="e2558-118">要求の日付と時刻の情報を識別するコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="e2558-118">The container that identifies the date-time information of the request.</span></span> <span data-ttu-id="e2558-119">この要素には、標準時と夏時間の切り替えに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e2558-119">This element contains information about the transition between standard time and daylight saving time.</span></span>  <br/><br/><span data-ttu-id="e2558-120">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="e2558-120">The following are the XPath expressions to this element:</span></span><br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e2558-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e2558-121">Text value</span></span>

<span data-ttu-id="e2558-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="e2558-122">A text value is required.</span></span> <span data-ttu-id="e2558-123">テキスト値は、整数を表します。</span><span class="sxs-lookup"><span data-stu-id="e2558-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e2558-124">備考</span><span class="sxs-lookup"><span data-stu-id="e2558-124">Remarks</span></span>

<span data-ttu-id="e2558-125">スキーマ内の 2 番目の[バイアス](bias.md)要素は、世界協定時刻 (UTC) オフセットからのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="e2558-125">A second [Bias](bias.md) element in the schema represents the offset from the Coordinated Universal Time (UTC) offset.</span></span> 
  
## <a name="example"></a><span data-ttu-id="e2558-126">例</span><span class="sxs-lookup"><span data-stu-id="e2558-126">Example</span></span>

<span data-ttu-id="e2558-127">次の使用例は、クライアント アプリケーションで、UTC から 8 時間のオフセットを識別する XML 要求の一部を示しています。</span><span class="sxs-lookup"><span data-stu-id="e2558-127">The following example shows part of an XML request that identifies an offset of 8 hours from UTC on the client application.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="e2558-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="e2558-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2558-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="e2558-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e2558-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e2558-130">Schema Name</span></span>  <br/> |<span data-ttu-id="e2558-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e2558-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="e2558-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e2558-132">Validation File</span></span>  <br/> |<span data-ttu-id="e2558-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e2558-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e2558-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e2558-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="e2558-135">False</span><span class="sxs-lookup"><span data-stu-id="e2558-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e2558-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="e2558-136">See also</span></span>

- [<span data-ttu-id="e2558-137">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="e2558-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="e2558-138">Bias</span><span class="sxs-lookup"><span data-stu-id="e2558-138">Bias</span></span>](bias.md)
- [<span data-ttu-id="e2558-139">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="e2558-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


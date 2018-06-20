---
title: Month
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Month
api_type:
- schema
ms.assetid: b12ac64f-b230-4573-be05-c86a428c4965
description: 月要素は、標準時間と夏時間との間の切り替えの月を表します。
ms.openlocfilehash: 73d052ef16bc51cd574eb8b04e21546f97347258
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832476"
---
# <a name="month"></a><span data-ttu-id="411d1-103">Month</span><span class="sxs-lookup"><span data-stu-id="411d1-103">Month</span></span>

<span data-ttu-id="411d1-104">**月**要素は、標準時間と夏時間との間の切り替えの月を表します。</span><span class="sxs-lookup"><span data-stu-id="411d1-104">The **Month** element represents the transition month of the year to and from standard time and daylight saving time.</span></span> 
  
```xml
<Month>...</Month>
```

 <span data-ttu-id="411d1-105">**短い**</span><span class="sxs-lookup"><span data-stu-id="411d1-105">**Short**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="411d1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="411d1-106">Attributes and elements</span></span>

<span data-ttu-id="411d1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="411d1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="411d1-108">属性</span><span class="sxs-lookup"><span data-stu-id="411d1-108">Attributes</span></span>

<span data-ttu-id="411d1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="411d1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="411d1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="411d1-110">Child elements</span></span>

<span data-ttu-id="411d1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="411d1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="411d1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="411d1-112">Parent elements</span></span>

|<span data-ttu-id="411d1-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="411d1-113">**Element**</span></span>|<span data-ttu-id="411d1-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="411d1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="411d1-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="411d1-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="411d1-116">基準にして世界協定時刻 (UTC)[バイアス (UTC)](bias-utc.md)の要素で表される時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="411d1-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="411d1-117">この要素は、夏時間が発生した地域で夏時間から切り替えに関する情報を標準時も含みます。</span><span class="sxs-lookup"><span data-stu-id="411d1-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span> <br/> <br/>  <span data-ttu-id="411d1-118">[StandardTime](standardtime.md)要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="411d1-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="411d1-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="411d1-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="411d1-120">夏時間が発生した地域の[バイアス (UTC)](bias-utc.md)の要素で表される UTC 時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="411d1-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="411d1-121">この要素には、標準時間から夏時間への切り替えが発生した場合についての情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="411d1-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/>  <span data-ttu-id="411d1-122">[DaylightTime](daylighttime.md)要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="411d1-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span>  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="411d1-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="411d1-123">Text value</span></span>

<span data-ttu-id="411d1-124">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="411d1-124">A text value is required.</span></span> <span data-ttu-id="411d1-125">値が現れることにより、月の順序のランクを表す、1 から 12 までの数値である必要があります。</span><span class="sxs-lookup"><span data-stu-id="411d1-125">The value represents the ordinal rank of the month by occurrence and must be a number between 1 and 12.</span></span> <span data-ttu-id="411d1-126">これは、short 型の整数データ型です。</span><span class="sxs-lookup"><span data-stu-id="411d1-126">This is a short integer data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="411d1-127">備考</span><span class="sxs-lookup"><span data-stu-id="411d1-127">Remarks</span></span>

<span data-ttu-id="411d1-128">5 の値を持つ[DayOrder](dayorder.md)要素、10 の値を持つ**月**の要素と、日曜日の値を持つ[DayOfWeek (タイムゾーン)](dayofweek-timezone.md)の要素を含む[StandardTime](standardtime.md)要素を意味する (標準時) からの移行夏時間は、10 月の 5 番目の日曜日に発生します。</span><span class="sxs-lookup"><span data-stu-id="411d1-128">A [StandardTime](standardtime.md) element that contains a [DayOrder](dayorder.md) element that has a value of 5, a **Month** element that has a value of 10, and a [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="411d1-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="411d1-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="411d1-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="411d1-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="411d1-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="411d1-131">Schema Name</span></span>  <br/> |<span data-ttu-id="411d1-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="411d1-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="411d1-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="411d1-133">Validation File</span></span>  <br/> |<span data-ttu-id="411d1-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="411d1-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="411d1-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="411d1-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="411d1-136">False</span><span class="sxs-lookup"><span data-stu-id="411d1-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="411d1-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="411d1-137">See also</span></span>

- [<span data-ttu-id="411d1-138">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="411d1-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="411d1-139">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="411d1-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


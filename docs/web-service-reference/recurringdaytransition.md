---
title: RecurringDayTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringDayTransition
api_type:
- schema
ms.assetid: 1ae28d14-c2b8-4084-9e76-e2e347a884ce
description: RecurringDayTransition 要素は、毎年同じ日に発生するタイム ゾーンの移行を表します。
ms.openlocfilehash: 913345188547ce9903809fdc1cbbbe3e20ae7f36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833012"
---
# <a name="recurringdaytransition"></a><span data-ttu-id="5c6d8-103">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="5c6d8-103">RecurringDayTransition</span></span>

<span data-ttu-id="5c6d8-104">**RecurringDayTransition**要素は、毎年同じ日に発生するタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="5c6d8-104">The **RecurringDayTransition** element represents a time zone transition that occurs on the same day each year.</span></span> 
  
```xml
<RecurringDayTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <DayOfWeek/>
   <Occurrence/>
</RecurringDayTransition>
```

 <span data-ttu-id="5c6d8-105">**RecurringDayTransitionType**</span><span class="sxs-lookup"><span data-stu-id="5c6d8-105">**RecurringDayTransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c6d8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5c6d8-106">Attributes and elements</span></span>

<span data-ttu-id="5c6d8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5c6d8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c6d8-108">属性</span><span class="sxs-lookup"><span data-stu-id="5c6d8-108">Attributes</span></span>

<span data-ttu-id="5c6d8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5c6d8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c6d8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5c6d8-110">Child elements</span></span>

|<span data-ttu-id="5c6d8-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="5c6d8-111">**Element**</span></span>|<span data-ttu-id="5c6d8-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5c6d8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c6d8-113">To</span><span class="sxs-lookup"><span data-stu-id="5c6d8-113">To</span></span>](to.md) <br/> |<span data-ttu-id="5c6d8-114">[TransitionsGroup](transitionsgroup.md)タイム ゾーンの移行の対象となる[期間](period.md)を指定します。</span><span class="sxs-lookup"><span data-stu-id="5c6d8-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="5c6d8-115">TimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c6d8-115">TimeOffset</span></span>](timeoffset.md) <br/> |<span data-ttu-id="5c6d8-116">タイム ゾーンの移行の世界協定時刻 (UTC) からの期間のオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="5c6d8-116">Represents the duration offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="5c6d8-117">月 (タイム ゾーンの切り替え)</span><span class="sxs-lookup"><span data-stu-id="5c6d8-117">Month (Time Zone Transition)</span></span>](month-time-zone-transition.md) <br/> |<span data-ttu-id="5c6d8-118">タイム ゾーンの切り替えが発生する月を表します。</span><span class="sxs-lookup"><span data-stu-id="5c6d8-118">Represents the month in which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="5c6d8-119">DayOfWeek (タイムゾーン)</span><span class="sxs-lookup"><span data-stu-id="5c6d8-119">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="5c6d8-120">タイム ゾーンの切り替えが発生する曜日を表します。</span><span class="sxs-lookup"><span data-stu-id="5c6d8-120">Represents the day of the week on which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="5c6d8-121">発生 (タイム ゾーンの切り替え)</span><span class="sxs-lookup"><span data-stu-id="5c6d8-121">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="5c6d8-122">タイム ゾーンの切り替えが発生する月の週の日の発生を表します。</span><span class="sxs-lookup"><span data-stu-id="5c6d8-122">Represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5c6d8-123">親要素</span><span class="sxs-lookup"><span data-stu-id="5c6d8-123">Parent elements</span></span>

|<span data-ttu-id="5c6d8-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="5c6d8-124">**Element**</span></span>|<span data-ttu-id="5c6d8-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="5c6d8-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c6d8-126">遷移</span><span class="sxs-lookup"><span data-stu-id="5c6d8-126">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="5c6d8-127">タイム ゾーンの切り替え効果のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="5c6d8-127">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="5c6d8-128">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="5c6d8-128">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="5c6d8-129">タイム ゾーンの切り替え効果のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="5c6d8-129">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5c6d8-130">備考</span><span class="sxs-lookup"><span data-stu-id="5c6d8-130">Remarks</span></span>

<span data-ttu-id="5c6d8-131">[RecurringDayTransition](recurringdaytransition.md)要素によって表すことができるタイム ゾーンの切り替えの例としては毎年 2 月の第 2 火曜日に移行します。</span><span class="sxs-lookup"><span data-stu-id="5c6d8-131">An example of a time zone transition that could be represented by the [RecurringDayTransition](recurringdaytransition.md) element is a transition that occurs on the second Tuesday of February each year.</span></span> 
  
<span data-ttu-id="5c6d8-132">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5c6d8-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c6d8-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="5c6d8-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c6d8-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="5c6d8-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5c6d8-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5c6d8-135">Schema Name</span></span>  <br/> |<span data-ttu-id="5c6d8-136">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5c6d8-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="5c6d8-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5c6d8-137">Validation File</span></span>  <br/> |<span data-ttu-id="5c6d8-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5c6d8-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5c6d8-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5c6d8-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c6d8-140">False</span><span class="sxs-lookup"><span data-stu-id="5c6d8-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c6d8-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="5c6d8-141">See also</span></span>



- [<span data-ttu-id="5c6d8-142">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5c6d8-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


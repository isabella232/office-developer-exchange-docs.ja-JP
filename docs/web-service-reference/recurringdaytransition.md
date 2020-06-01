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
description: RecurringDayTransition 要素は、毎年同じ日に発生するタイムゾーンの切り替えを表します。
ms.openlocfilehash: 44c2a6ec4dbaaa52a2772cb5c35a84b14dd77f97
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468468"
---
# <a name="recurringdaytransition"></a><span data-ttu-id="ca400-103">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="ca400-103">RecurringDayTransition</span></span>

<span data-ttu-id="ca400-104">**RecurringDayTransition**要素は、毎年同じ日に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="ca400-104">The **RecurringDayTransition** element represents a time zone transition that occurs on the same day each year.</span></span> 
  
```xml
<RecurringDayTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <DayOfWeek/>
   <Occurrence/>
</RecurringDayTransition>
```

 <span data-ttu-id="ca400-105">**RecurringDayTransitionType**</span><span class="sxs-lookup"><span data-stu-id="ca400-105">**RecurringDayTransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ca400-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ca400-106">Attributes and elements</span></span>

<span data-ttu-id="ca400-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ca400-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ca400-108">属性</span><span class="sxs-lookup"><span data-stu-id="ca400-108">Attributes</span></span>

<span data-ttu-id="ca400-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ca400-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ca400-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ca400-110">Child elements</span></span>

|<span data-ttu-id="ca400-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="ca400-111">**Element**</span></span>|<span data-ttu-id="ca400-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ca400-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca400-113">To</span><span class="sxs-lookup"><span data-stu-id="ca400-113">To</span></span>](to.md) <br/> |<span data-ttu-id="ca400-114">タイムゾーンの遷移のターゲットである[期間](period.md)[または時間を指定](transitionsgroup.md)します。</span><span class="sxs-lookup"><span data-stu-id="ca400-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="ca400-115">TimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca400-115">TimeOffset</span></span>](timeoffset.md) <br/> |<span data-ttu-id="ca400-116">タイムゾーンの切り替えについて、世界協定時刻 (UTC) からの時間オフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="ca400-116">Represents the duration offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="ca400-117">月 (タイムゾーン切り替え)</span><span class="sxs-lookup"><span data-stu-id="ca400-117">Month (Time Zone Transition)</span></span>](month-time-zone-transition.md) <br/> |<span data-ttu-id="ca400-118">タイムゾーンの切り替えが行われる月を表します。</span><span class="sxs-lookup"><span data-stu-id="ca400-118">Represents the month in which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="ca400-119">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="ca400-119">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="ca400-120">タイムゾーンの切り替えが行われる曜日を表します。</span><span class="sxs-lookup"><span data-stu-id="ca400-120">Represents the day of the week on which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="ca400-121">発生 (タイムゾーンの切り替え)</span><span class="sxs-lookup"><span data-stu-id="ca400-121">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="ca400-122">タイムゾーンの切り替えが行われる月の曜日の発生を表します。</span><span class="sxs-lookup"><span data-stu-id="ca400-122">Represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ca400-123">親要素</span><span class="sxs-lookup"><span data-stu-id="ca400-123">Parent elements</span></span>

|<span data-ttu-id="ca400-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="ca400-124">**Element**</span></span>|<span data-ttu-id="ca400-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="ca400-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca400-126">切り替わる</span><span class="sxs-lookup"><span data-stu-id="ca400-126">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="ca400-127">タイムゾーンの遷移のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ca400-127">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="ca400-128">遷移 Tionsgroup</span><span class="sxs-lookup"><span data-stu-id="ca400-128">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="ca400-129">タイムゾーンの遷移のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ca400-129">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ca400-130">注釈</span><span class="sxs-lookup"><span data-stu-id="ca400-130">Remarks</span></span>

<span data-ttu-id="ca400-131">[RecurringDayTransition](recurringdaytransition.md)要素によって表される可能性があるタイムゾーンの遷移の例としては、各年2月2日の火曜日に発生する遷移があります。</span><span class="sxs-lookup"><span data-stu-id="ca400-131">An example of a time zone transition that could be represented by the [RecurringDayTransition](recurringdaytransition.md) element is a transition that occurs on the second Tuesday of February each year.</span></span> 
  
<span data-ttu-id="ca400-132">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="ca400-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ca400-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ca400-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ca400-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="ca400-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ca400-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ca400-135">Schema Name</span></span>  <br/> |<span data-ttu-id="ca400-136">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ca400-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="ca400-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ca400-137">Validation File</span></span>  <br/> |<span data-ttu-id="ca400-138">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ca400-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ca400-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ca400-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="ca400-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="ca400-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ca400-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="ca400-141">See also</span></span>



- [<span data-ttu-id="ca400-142">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ca400-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: 遷移
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Transitions
api_type:
- schema
ms.assetid: 26f38f1c-96a3-440e-805c-1437886d11c5
description: 遷移要素では、タイム ゾーンの移行の配列を表します。
ms.openlocfilehash: df7cacdef71c3fdfaa3ecadb486843ea30e6109d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839747"
---
# <a name="transitions"></a><span data-ttu-id="9becb-103">遷移</span><span class="sxs-lookup"><span data-stu-id="9becb-103">Transitions</span></span>

<span data-ttu-id="9becb-104">**遷移**要素では、タイム ゾーンの移行の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="9becb-104">The **Transitions** element represents an array of time zone transitions.</span></span> 
  
```xml
<Transitions Id="">
   <Transition/>
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</Transitions>
```

 <span data-ttu-id="9becb-105">**ArrayOfTransitionsType**</span><span class="sxs-lookup"><span data-stu-id="9becb-105">**ArrayOfTransitionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9becb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9becb-106">Attributes and elements</span></span>

<span data-ttu-id="9becb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9becb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9becb-108">属性</span><span class="sxs-lookup"><span data-stu-id="9becb-108">Attributes</span></span>

|<span data-ttu-id="9becb-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="9becb-109">**Attribute**</span></span>|<span data-ttu-id="9becb-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="9becb-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9becb-111">ID</span><span class="sxs-lookup"><span data-stu-id="9becb-111">Id</span></span>  <br/> |<span data-ttu-id="9becb-112">タイム ゾーン定義の一意の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="9becb-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9becb-113">子要素</span><span class="sxs-lookup"><span data-stu-id="9becb-113">Child elements</span></span>

|<span data-ttu-id="9becb-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="9becb-114">**Element**</span></span>|<span data-ttu-id="9becb-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="9becb-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9becb-116">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="9becb-116">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="9becb-117">特定の日付と、特定の時刻に表示されるタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="9becb-117">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="9becb-118">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="9becb-118">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="9becb-119">毎年同じ日に発生するタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="9becb-119">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="9becb-120">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="9becb-120">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="9becb-121">年の指定された日に発生するタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="9becb-121">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
|[<span data-ttu-id="9becb-122">Transition</span><span class="sxs-lookup"><span data-stu-id="9becb-122">Transition</span></span>](transition.md) <br/> |<span data-ttu-id="9becb-123">タイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="9becb-123">Represents a time zone transition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9becb-124">親要素</span><span class="sxs-lookup"><span data-stu-id="9becb-124">Parent elements</span></span>

|<span data-ttu-id="9becb-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="9becb-125">**Element**</span></span>|<span data-ttu-id="9becb-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="9becb-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9becb-127">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="9becb-127">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="9becb-128">[カレンダー項目](calendaritem.md)または[MeetingRequest](meetingrequest.md)の開始時刻のタイム ゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="9becb-128">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="9becb-129">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="9becb-129">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="9becb-130">[カレンダー項目](calendaritem.md)または[MeetingRequest](meetingrequest.md)の終了時刻のタイム ゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="9becb-130">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="9becb-131">タイム</span><span class="sxs-lookup"><span data-stu-id="9becb-131">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="9becb-132">タイム ゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="9becb-132">Defines a time zone.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9becb-133">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9becb-133">Text value</span></span>

<span data-ttu-id="9becb-134">なし。</span><span class="sxs-lookup"><span data-stu-id="9becb-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9becb-135">備考</span><span class="sxs-lookup"><span data-stu-id="9becb-135">Remarks</span></span>

<span data-ttu-id="9becb-136">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9becb-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9becb-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="9becb-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9becb-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="9becb-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9becb-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9becb-139">Schema Name</span></span>  <br/> |<span data-ttu-id="9becb-140">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9becb-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="9becb-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9becb-141">Validation File</span></span>  <br/> |<span data-ttu-id="9becb-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9becb-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9becb-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9becb-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="9becb-144">False</span><span class="sxs-lookup"><span data-stu-id="9becb-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9becb-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="9becb-145">See also</span></span>



- [<span data-ttu-id="9becb-146">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9becb-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: 切り替わる
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
description: トランジションビュー要素は、タイムゾーンの遷移の配列を表します。
ms.openlocfilehash: d48fb8872b2f7e052f733c32e5dd1c9b4d04d898
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467439"
---
# <a name="transitions"></a><span data-ttu-id="f5f9d-103">切り替わる</span><span class="sxs-lookup"><span data-stu-id="f5f9d-103">Transitions</span></span>

<span data-ttu-id="f5f9d-104">**トランジションビュー**要素は、タイムゾーンの遷移の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="f5f9d-104">The **Transitions** element represents an array of time zone transitions.</span></span> 
  
```xml
<Transitions Id="">
   <Transition/>
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</Transitions>
```

 <span data-ttu-id="f5f9d-105">**Arrayofstype Tionstype**</span><span class="sxs-lookup"><span data-stu-id="f5f9d-105">**ArrayOfTransitionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f5f9d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f5f9d-106">Attributes and elements</span></span>

<span data-ttu-id="f5f9d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f5f9d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f5f9d-108">属性</span><span class="sxs-lookup"><span data-stu-id="f5f9d-108">Attributes</span></span>

|<span data-ttu-id="f5f9d-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="f5f9d-109">**Attribute**</span></span>|<span data-ttu-id="f5f9d-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="f5f9d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f5f9d-111">ID</span><span class="sxs-lookup"><span data-stu-id="f5f9d-111">Id</span></span>  <br/> |<span data-ttu-id="f5f9d-112">タイムゾーン定義の一意識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="f5f9d-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f5f9d-113">子要素</span><span class="sxs-lookup"><span data-stu-id="f5f9d-113">Child elements</span></span>

|<span data-ttu-id="f5f9d-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="f5f9d-114">**Element**</span></span>|<span data-ttu-id="f5f9d-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="f5f9d-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5f9d-116">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="f5f9d-116">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="f5f9d-117">特定の日付および特定の時刻に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="f5f9d-117">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="f5f9d-118">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="f5f9d-118">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="f5f9d-119">毎年同じ日に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="f5f9d-119">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="f5f9d-120">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="f5f9d-120">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="f5f9d-121">指定した日に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="f5f9d-121">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
|[<span data-ttu-id="f5f9d-122">Transition</span><span class="sxs-lookup"><span data-stu-id="f5f9d-122">Transition</span></span>](transition.md) <br/> |<span data-ttu-id="f5f9d-123">タイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="f5f9d-123">Represents a time zone transition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f5f9d-124">親要素</span><span class="sxs-lookup"><span data-stu-id="f5f9d-124">Parent elements</span></span>

|<span data-ttu-id="f5f9d-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="f5f9d-125">**Element**</span></span>|<span data-ttu-id="f5f9d-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="f5f9d-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5f9d-127">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="f5f9d-127">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="f5f9d-128">[Calendaritem](calendaritem.md)または[会議要求](meetingrequest.md)の開始時刻のタイムゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="f5f9d-128">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="f5f9d-129">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="f5f9d-129">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="f5f9d-130">[Calendaritem](calendaritem.md)または[会議の要求](meetingrequest.md)の終了時刻のタイムゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="f5f9d-130">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="f5f9d-131">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="f5f9d-131">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="f5f9d-132">タイムゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="f5f9d-132">Defines a time zone.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f5f9d-133">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f5f9d-133">Text value</span></span>

<span data-ttu-id="f5f9d-134">なし。</span><span class="sxs-lookup"><span data-stu-id="f5f9d-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f5f9d-135">注釈</span><span class="sxs-lookup"><span data-stu-id="f5f9d-135">Remarks</span></span>

<span data-ttu-id="f5f9d-136">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f5f9d-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f5f9d-137">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f5f9d-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f5f9d-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="f5f9d-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f5f9d-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f5f9d-139">Schema Name</span></span>  <br/> |<span data-ttu-id="f5f9d-140">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f5f9d-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="f5f9d-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f5f9d-141">Validation File</span></span>  <br/> |<span data-ttu-id="f5f9d-142">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f5f9d-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f5f9d-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f5f9d-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="f5f9d-144">正しくない</span><span class="sxs-lookup"><span data-stu-id="f5f9d-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f5f9d-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="f5f9d-145">See also</span></span>



- [<span data-ttu-id="f5f9d-146">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f5f9d-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


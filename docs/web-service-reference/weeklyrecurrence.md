---
title: WeeklyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WeeklyRecurrence
api_type:
- schema
ms.assetid: 69c41dd5-597c-45bc-be3f-e2f2b5615aa3
description: WeeklyRecurrence 要素では、毎週の定期的なパターンについて説明します。
ms.openlocfilehash: 78bc76dd63c6737786df02f336217dc8de9a3a67
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840017"
---
# <a name="weeklyrecurrence"></a><span data-ttu-id="19edb-103">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="19edb-103">WeeklyRecurrence</span></span>

<span data-ttu-id="19edb-104">**WeeklyRecurrence**要素では、毎週の定期的なパターンについて説明します。</span><span class="sxs-lookup"><span data-stu-id="19edb-104">The **WeeklyRecurrence** element describes a weekly recurrence pattern.</span></span> 
  
```XML
<WeeklyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <FirstDayOfWeek/>
</WeeklyRecurrence>
```

 <span data-ttu-id="19edb-105">**WeeklyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="19edb-105">**WeeklyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19edb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="19edb-106">Attributes and elements</span></span>

<span data-ttu-id="19edb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="19edb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19edb-108">属性</span><span class="sxs-lookup"><span data-stu-id="19edb-108">Attributes</span></span>

<span data-ttu-id="19edb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="19edb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19edb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="19edb-110">Child elements</span></span>

|<span data-ttu-id="19edb-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="19edb-111">**Element**</span></span>|<span data-ttu-id="19edb-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="19edb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19edb-113">間隔</span><span class="sxs-lookup"><span data-stu-id="19edb-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="19edb-114">週、2 つの連続した週 1 回定期的なアイテムのパターン ・項目間の間隔を定義します。</span><span class="sxs-lookup"><span data-stu-id="19edb-114">Defines the interval, in weeks, between two consecutive weekly recurrence pattern items.</span></span> <span data-ttu-id="19edb-115">1 から 99 の範囲で指定できます。</span><span class="sxs-lookup"><span data-stu-id="19edb-115">The value can be in the range from 1 to 99.</span></span>  <br/> |
|[<span data-ttu-id="19edb-116">DaysOfWeek (DaysOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="19edb-116">DaysOfWeek (DaysOfWeekType)</span></span>](daysofweek-daysofweektype.md) <br/> |<span data-ttu-id="19edb-117">毎週の定期的なパターンでは、週の曜日について説明します。</span><span class="sxs-lookup"><span data-stu-id="19edb-117">Describes which days of the week are in the weekly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="19edb-118">FirstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="19edb-118">FirstDayOfWeek</span></span>](firstdayofweek.md) <br/> |<span data-ttu-id="19edb-119">週の最初の日を指定します。</span><span class="sxs-lookup"><span data-stu-id="19edb-119">Specifies the first day of the week.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="19edb-120">親要素</span><span class="sxs-lookup"><span data-stu-id="19edb-120">Parent elements</span></span>

|<span data-ttu-id="19edb-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="19edb-121">**Element**</span></span>|<span data-ttu-id="19edb-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="19edb-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19edb-123">定期的な予定 (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="19edb-123">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="19edb-124">定期タスクの頻度に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="19edb-124">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="19edb-125">定期的なアイテム (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="19edb-125">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="19edb-126">予定表アイテムおよび会議出席依頼に定期的なパターンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="19edb-126">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="19edb-127">テキスト値</span><span class="sxs-lookup"><span data-stu-id="19edb-127">Text value</span></span>

<span data-ttu-id="19edb-128">なし。</span><span class="sxs-lookup"><span data-stu-id="19edb-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="19edb-129">備考</span><span class="sxs-lookup"><span data-stu-id="19edb-129">Remarks</span></span>

<span data-ttu-id="19edb-130">定期的なマスター アイテムの[開始](start.md)と[終了](end-ex15websvcsotherref.md)日が毎週の定期的なパターンの 1 番目の日付があるない場合、タイム ゾーン オフセット情報は失われます。</span><span class="sxs-lookup"><span data-stu-id="19edb-130">The time zone offset information is lost if the [Start](start.md) and [End ](end-ex15websvcsotherref.md) dates of the recurring master item do not have a date that is equal to the first occurrence of a weekly recurrence pattern.</span></span> 
  
<span data-ttu-id="19edb-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="19edb-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19edb-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="19edb-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19edb-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="19edb-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="19edb-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="19edb-134">Schema Name</span></span>  <br/> |<span data-ttu-id="19edb-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="19edb-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="19edb-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="19edb-136">Validation File</span></span>  <br/> |<span data-ttu-id="19edb-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="19edb-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="19edb-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="19edb-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="19edb-139">False</span><span class="sxs-lookup"><span data-stu-id="19edb-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19edb-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="19edb-140">See also</span></span>



- [<span data-ttu-id="19edb-141">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="19edb-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


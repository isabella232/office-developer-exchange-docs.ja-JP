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
description: WeeklyRecurrence 要素は、週単位の定期的なパターンを記述します。
ms.openlocfilehash: 5006238590c4cd7556a92fb1fbe13292383412b8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530367"
---
# <a name="weeklyrecurrence"></a><span data-ttu-id="a8901-103">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="a8901-103">WeeklyRecurrence</span></span>

<span data-ttu-id="a8901-104">**WeeklyRecurrence**要素は、週単位の定期的なパターンを記述します。</span><span class="sxs-lookup"><span data-stu-id="a8901-104">The **WeeklyRecurrence** element describes a weekly recurrence pattern.</span></span> 
  
```XML
<WeeklyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <FirstDayOfWeek/>
</WeeklyRecurrence>
```

 <span data-ttu-id="a8901-105">**WeeklyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="a8901-105">**WeeklyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8901-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a8901-106">Attributes and elements</span></span>

<span data-ttu-id="a8901-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a8901-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8901-108">属性</span><span class="sxs-lookup"><span data-stu-id="a8901-108">Attributes</span></span>

<span data-ttu-id="a8901-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a8901-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8901-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a8901-110">Child elements</span></span>

|<span data-ttu-id="a8901-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="a8901-111">**Element**</span></span>|<span data-ttu-id="a8901-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a8901-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8901-113">間隔</span><span class="sxs-lookup"><span data-stu-id="a8901-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="a8901-114">週単位の定期的な繰り返しパターンアイテム間の間隔 (週単位) を定義します。</span><span class="sxs-lookup"><span data-stu-id="a8901-114">Defines the interval, in weeks, between two consecutive weekly recurrence pattern items.</span></span> <span data-ttu-id="a8901-115">この値は 1 ~ 99 の範囲で指定できます。</span><span class="sxs-lookup"><span data-stu-id="a8901-115">The value can be in the range from 1 to 99.</span></span>  <br/> |
|[<span data-ttu-id="a8901-116">DaysOfWeek (DaysOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="a8901-116">DaysOfWeek (DaysOfWeekType)</span></span>](daysofweek-daysofweektype.md) <br/> |<span data-ttu-id="a8901-117">毎週の定期的なパターンに含まれる曜日を指定します。</span><span class="sxs-lookup"><span data-stu-id="a8901-117">Describes which days of the week are in the weekly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="a8901-118">FirstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="a8901-118">FirstDayOfWeek</span></span>](firstdayofweek.md) <br/> |<span data-ttu-id="a8901-119">週の最初の曜日を指定します。</span><span class="sxs-lookup"><span data-stu-id="a8901-119">Specifies the first day of the week.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a8901-120">親要素</span><span class="sxs-lookup"><span data-stu-id="a8901-120">Parent elements</span></span>

|<span data-ttu-id="a8901-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="a8901-121">**Element**</span></span>|<span data-ttu-id="a8901-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="a8901-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8901-123">定期的なアイテム (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="a8901-123">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="a8901-124">定期的なタスクの定期的なアイテムの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a8901-124">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="a8901-125">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="a8901-125">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="a8901-126">予定表アイテムと会議出席依頼の定期的なパターンを含みます。</span><span class="sxs-lookup"><span data-stu-id="a8901-126">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a8901-127">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a8901-127">Text value</span></span>

<span data-ttu-id="a8901-128">なし。</span><span class="sxs-lookup"><span data-stu-id="a8901-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a8901-129">注釈</span><span class="sxs-lookup"><span data-stu-id="a8901-129">Remarks</span></span>

<span data-ttu-id="a8901-130">定期的なマスターアイテムの[開始](start.md)日と[終了](end-ex15websvcsotherref.md)日に、最初に週単位の定期的なパターンと同じ日付が設定されていない場合は、タイムゾーンのオフセット情報は失われます。</span><span class="sxs-lookup"><span data-stu-id="a8901-130">The time zone offset information is lost if the [Start](start.md) and [End ](end-ex15websvcsotherref.md) dates of the recurring master item do not have a date that is equal to the first occurrence of a weekly recurrence pattern.</span></span> 
  
<span data-ttu-id="a8901-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a8901-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8901-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a8901-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8901-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="a8901-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8901-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a8901-134">Schema Name</span></span>  <br/> |<span data-ttu-id="a8901-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a8901-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="a8901-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a8901-136">Validation File</span></span>  <br/> |<span data-ttu-id="a8901-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a8901-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8901-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a8901-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8901-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="a8901-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8901-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="a8901-140">See also</span></span>



- [<span data-ttu-id="a8901-141">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a8901-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


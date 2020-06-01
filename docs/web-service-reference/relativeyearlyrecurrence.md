---
title: RelativeYearlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RelativeYearlyRecurrence
api_type:
- schema
ms.assetid: 25b67876-9979-4a30-a637-357ea10a93b8
description: RelativeYearlyRecurrence 要素は、相対的な年単位の定期的なパターンを記述します。
ms.openlocfilehash: 2abe09ddfe52c24211ef5d0a392ddecaf15bf7bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456735"
---
# <a name="relativeyearlyrecurrence"></a><span data-ttu-id="663a5-103">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="663a5-103">RelativeYearlyRecurrence</span></span>

<span data-ttu-id="663a5-104">**RelativeYearlyRecurrence**要素は、相対的な年単位の定期的なパターンを記述します。</span><span class="sxs-lookup"><span data-stu-id="663a5-104">The **RelativeYearlyRecurrence** element describes a relative yearly recurrence pattern.</span></span> 
  
```xml
<RelativeYearlyRecurrence>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
   <Month/>
</RelativeYearlyRecurrence>
```

 <span data-ttu-id="663a5-105">**RelativeYearlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="663a5-105">**RelativeYearlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="663a5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="663a5-106">Attributes and elements</span></span>

<span data-ttu-id="663a5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="663a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="663a5-108">属性</span><span class="sxs-lookup"><span data-stu-id="663a5-108">Attributes</span></span>

<span data-ttu-id="663a5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="663a5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="663a5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="663a5-110">Child elements</span></span>

|<span data-ttu-id="663a5-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="663a5-111">**Element**</span></span>|<span data-ttu-id="663a5-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="663a5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="663a5-113">DaysOfWeek (DayOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="663a5-113">DaysOfWeek (DayOfWeekType)</span></span>](daysofweek-dayofweektype.md) <br/> |<span data-ttu-id="663a5-114">アイテムの定期的なパターンで使用される曜日を表します。</span><span class="sxs-lookup"><span data-stu-id="663a5-114">Describes the days of the week that are used in item recurrence patterns.</span></span>  <br/> |
|[<span data-ttu-id="663a5-115">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="663a5-115">DayOfWeekIndex</span></span>](dayofweekindex.md) <br/> |<span data-ttu-id="663a5-116">1月の週が、相対的な年単位の定期的なパターンで使用されることを説明します。</span><span class="sxs-lookup"><span data-stu-id="663a5-116">Describes which week in a month is used in a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="663a5-117">月 (アイテムの定期的な予定)</span><span class="sxs-lookup"><span data-stu-id="663a5-117">Month (Item Recurrence)</span></span>](month-item-recurrence.md) <br/> |<span data-ttu-id="663a5-118">年単位の定期的なアイテムが発生する月を表します。</span><span class="sxs-lookup"><span data-stu-id="663a5-118">Describes the month when a yearly recurring item occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="663a5-119">親要素</span><span class="sxs-lookup"><span data-stu-id="663a5-119">Parent elements</span></span>

|<span data-ttu-id="663a5-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="663a5-120">**Element**</span></span>|<span data-ttu-id="663a5-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="663a5-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="663a5-122">定期的なアイテム (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="663a5-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="663a5-123">定期的なタスクの定期的なアイテムの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="663a5-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="663a5-124">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="663a5-124">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="663a5-125">予定表アイテムと会議出席依頼の定期的なパターンを含みます。</span><span class="sxs-lookup"><span data-stu-id="663a5-125">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="663a5-126">Standard</span><span class="sxs-lookup"><span data-stu-id="663a5-126">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="663a5-127">夏時間から標準時までの時刻が変更された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="663a5-127">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="663a5-128">日光</span><span class="sxs-lookup"><span data-stu-id="663a5-128">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="663a5-129">時刻が標準時から夏時間に変更された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="663a5-129">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="663a5-130">注釈</span><span class="sxs-lookup"><span data-stu-id="663a5-130">Remarks</span></span>

<span data-ttu-id="663a5-131">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="663a5-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="663a5-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="663a5-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="663a5-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="663a5-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="663a5-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="663a5-134">Schema Name</span></span>  <br/> |<span data-ttu-id="663a5-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="663a5-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="663a5-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="663a5-136">Validation File</span></span>  <br/> |<span data-ttu-id="663a5-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="663a5-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="663a5-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="663a5-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="663a5-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="663a5-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="663a5-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="663a5-140">See also</span></span>



- [<span data-ttu-id="663a5-141">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="663a5-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


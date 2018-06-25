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
description: RelativeYearlyRecurrence 要素では、相対的な年間の定期的なパターンについて説明します。
ms.openlocfilehash: ce8d2b134ce1fa34cbce8bd2fa921cab18d908a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833057"
---
# <a name="relativeyearlyrecurrence"></a><span data-ttu-id="07844-103">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="07844-103">RelativeYearlyRecurrence</span></span>

<span data-ttu-id="07844-104">**RelativeYearlyRecurrence**要素では、相対的な年間の定期的なパターンについて説明します。</span><span class="sxs-lookup"><span data-stu-id="07844-104">The **RelativeYearlyRecurrence** element describes a relative yearly recurrence pattern.</span></span> 
  
```xml
<RelativeYearlyRecurrence>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
   <Month/>
</RelativeYearlyRecurrence>
```

 <span data-ttu-id="07844-105">**RelativeYearlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="07844-105">**RelativeYearlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07844-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="07844-106">Attributes and elements</span></span>

<span data-ttu-id="07844-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="07844-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07844-108">属性</span><span class="sxs-lookup"><span data-stu-id="07844-108">Attributes</span></span>

<span data-ttu-id="07844-109">なし。</span><span class="sxs-lookup"><span data-stu-id="07844-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07844-110">子要素</span><span class="sxs-lookup"><span data-stu-id="07844-110">Child elements</span></span>

|<span data-ttu-id="07844-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="07844-111">**Element**</span></span>|<span data-ttu-id="07844-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="07844-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07844-113">DaysOfWeek (DayOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="07844-113">DaysOfWeek (DayOfWeekType)</span></span>](daysofweek-dayofweektype.md) <br/> |<span data-ttu-id="07844-114">項目の定期的なパターンで使用されている週の日について説明します。</span><span class="sxs-lookup"><span data-stu-id="07844-114">Describes the days of the week that are used in item recurrence patterns.</span></span>  <br/> |
|[<span data-ttu-id="07844-115">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="07844-115">DayOfWeekIndex</span></span>](dayofweekindex.md) <br/> |<span data-ttu-id="07844-116">1 か月の週が相対的な年間の定期的なパターンの使用について説明します。</span><span class="sxs-lookup"><span data-stu-id="07844-116">Describes which week in a month is used in a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="07844-117">月 (定期的なアイテム)</span><span class="sxs-lookup"><span data-stu-id="07844-117">Month (Item Recurrence)</span></span>](month-item-recurrence.md) <br/> |<span data-ttu-id="07844-118">年間の定期的なアイテムが発生する場合について説明します。</span><span class="sxs-lookup"><span data-stu-id="07844-118">Describes the month when a yearly recurring item occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="07844-119">親要素</span><span class="sxs-lookup"><span data-stu-id="07844-119">Parent elements</span></span>

|<span data-ttu-id="07844-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="07844-120">**Element**</span></span>|<span data-ttu-id="07844-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="07844-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07844-122">定期的な予定 (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="07844-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="07844-123">定期タスクの頻度に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="07844-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="07844-124">定期的なアイテム (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="07844-124">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="07844-125">予定表アイテムおよび会議出席依頼に定期的なパターンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="07844-125">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="07844-126">Standard</span><span class="sxs-lookup"><span data-stu-id="07844-126">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="07844-127">日付と時刻が変更されたとき夏時間から標準時間への時間を表します。</span><span class="sxs-lookup"><span data-stu-id="07844-127">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="07844-128">(夏時間)</span><span class="sxs-lookup"><span data-stu-id="07844-128">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="07844-129">日付と時刻が変更されたとき標準時間から夏時間への時間を表します。</span><span class="sxs-lookup"><span data-stu-id="07844-129">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="07844-130">備考</span><span class="sxs-lookup"><span data-stu-id="07844-130">Remarks</span></span>

<span data-ttu-id="07844-131">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="07844-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07844-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="07844-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07844-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="07844-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="07844-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="07844-134">Schema Name</span></span>  <br/> |<span data-ttu-id="07844-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="07844-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="07844-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="07844-136">Validation File</span></span>  <br/> |<span data-ttu-id="07844-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="07844-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="07844-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="07844-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="07844-139">False</span><span class="sxs-lookup"><span data-stu-id="07844-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="07844-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="07844-140">See also</span></span>



- [<span data-ttu-id="07844-141">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="07844-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


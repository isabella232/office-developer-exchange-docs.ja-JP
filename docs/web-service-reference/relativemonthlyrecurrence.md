---
title: RelativeMonthlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RelativeMonthlyRecurrence
api_type:
- schema
ms.assetid: a76595db-7460-44ac-ac2a-53241caa33a7
description: RelativeMonthlyRecurrence 要素では、相対的な毎月の定期的なパターンについて説明します。
ms.openlocfilehash: 9b695052c38e2693946837bf99f03baea093df08
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833053"
---
# <a name="relativemonthlyrecurrence"></a><span data-ttu-id="d89ff-103">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="d89ff-103">RelativeMonthlyRecurrence</span></span>

<span data-ttu-id="d89ff-104">**RelativeMonthlyRecurrence**要素では、相対的な毎月の定期的なパターンについて説明します。</span><span class="sxs-lookup"><span data-stu-id="d89ff-104">The **RelativeMonthlyRecurrence** element describes a relative monthly recurrence pattern.</span></span> 
  
```xml
<RelativeMonthlyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
</RelativeMonthlyRecurrence>
```

 <span data-ttu-id="d89ff-105">**RelativeMonthlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="d89ff-105">**RelativeMonthlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d89ff-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d89ff-106">Attributes and elements</span></span>

<span data-ttu-id="d89ff-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d89ff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d89ff-108">属性</span><span class="sxs-lookup"><span data-stu-id="d89ff-108">Attributes</span></span>

<span data-ttu-id="d89ff-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d89ff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d89ff-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d89ff-110">Child elements</span></span>

|<span data-ttu-id="d89ff-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d89ff-111">**Element**</span></span>|<span data-ttu-id="d89ff-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d89ff-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d89ff-113">間隔</span><span class="sxs-lookup"><span data-stu-id="d89ff-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="d89ff-114">2 つ連続の定期的なパターンの毎月アイテム間の間隔を定義します。</span><span class="sxs-lookup"><span data-stu-id="d89ff-114">Defines the interval between two consecutive monthly recurring pattern items.</span></span> <span data-ttu-id="d89ff-115">この値の範囲は、1 から 99 までです。</span><span class="sxs-lookup"><span data-stu-id="d89ff-115">The range for this value is 1 to 99.</span></span>  <br/> |
|[<span data-ttu-id="d89ff-116">DaysOfWeek (DayOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="d89ff-116">DaysOfWeek (DayOfWeekType)</span></span>](daysofweek-dayofweektype.md) <br/> |<span data-ttu-id="d89ff-117">相対の毎月の定期的なパターンでは、週の曜日について説明します。</span><span class="sxs-lookup"><span data-stu-id="d89ff-117">Describes which days of the week are in the relative monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="d89ff-118">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="d89ff-118">DayOfWeekIndex</span></span>](dayofweekindex.md) <br/> |<span data-ttu-id="d89ff-119">どの週が相対的な毎月の定期的なパターンの使用について説明します。</span><span class="sxs-lookup"><span data-stu-id="d89ff-119">Describes which week is used in a relative monthly recurrence pattern.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d89ff-120">親要素</span><span class="sxs-lookup"><span data-stu-id="d89ff-120">Parent elements</span></span>

|<span data-ttu-id="d89ff-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="d89ff-121">**Element**</span></span>|<span data-ttu-id="d89ff-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="d89ff-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d89ff-123">定期的なアイテム (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="d89ff-123">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="d89ff-124">予定表アイテムおよび会議出席依頼に定期的なパターンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d89ff-124">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="d89ff-125">定期的な予定 (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="d89ff-125">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="d89ff-126">定期タスクの頻度に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d89ff-126">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d89ff-127">備考</span><span class="sxs-lookup"><span data-stu-id="d89ff-127">Remarks</span></span>

<span data-ttu-id="d89ff-128">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d89ff-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d89ff-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="d89ff-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d89ff-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="d89ff-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d89ff-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d89ff-131">Schema Name</span></span>  <br/> |<span data-ttu-id="d89ff-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d89ff-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="d89ff-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d89ff-133">Validation File</span></span>  <br/> |<span data-ttu-id="d89ff-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d89ff-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d89ff-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d89ff-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="d89ff-136">False</span><span class="sxs-lookup"><span data-stu-id="d89ff-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d89ff-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="d89ff-137">See also</span></span>



- [<span data-ttu-id="d89ff-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d89ff-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


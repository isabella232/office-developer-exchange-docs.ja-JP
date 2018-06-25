---
title: AbsoluteMonthlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteMonthlyRecurrence
api_type:
- schema
ms.assetid: 178fa0ae-9dfc-417f-933c-d657d31c2161
description: AbsoluteMonthlyRecurrence 要素は、毎月の定期的なパターンを表します。
ms.openlocfilehash: f4613fa71a9164c45b60a82f675959817cd4bdd5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760415"
---
# <a name="absolutemonthlyrecurrence"></a><span data-ttu-id="cda09-103">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="cda09-103">AbsoluteMonthlyRecurrence</span></span>

<span data-ttu-id="cda09-104">**AbsoluteMonthlyRecurrence**要素は、毎月の定期的なパターンを表します。</span><span class="sxs-lookup"><span data-stu-id="cda09-104">The **AbsoluteMonthlyRecurrence** element represents a monthly recurrence pattern.</span></span> 
  
```xml
<AbsoluteMonthlyRecurrence>
   <Interval/>
   <DayOfMonth/>
</AbsoluteMonthlyRecurrence>
```

 <span data-ttu-id="cda09-105">**AbsoluteMonthlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="cda09-105">**AbsoluteMonthlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cda09-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cda09-106">Attributes and elements</span></span>

<span data-ttu-id="cda09-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cda09-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cda09-108">属性</span><span class="sxs-lookup"><span data-stu-id="cda09-108">Attributes</span></span>

<span data-ttu-id="cda09-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cda09-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cda09-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cda09-110">Child elements</span></span>

|<span data-ttu-id="cda09-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="cda09-111">**Element**</span></span>|<span data-ttu-id="cda09-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="cda09-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cda09-113">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="cda09-113">DayOfMonth</span></span>](dayofmonth.md) <br/> |<span data-ttu-id="cda09-114">定期的なアイテムに発生する月の日について説明します。</span><span class="sxs-lookup"><span data-stu-id="cda09-114">Describes the day in a month that a recurring item occurs.</span></span> <span data-ttu-id="cda09-115">このプロパティの値の範囲は、1 から 31 です。</span><span class="sxs-lookup"><span data-stu-id="cda09-115">The range of values for this property is 1 to 31.</span></span> <span data-ttu-id="cda09-116">特定の月のこの値が大きい場合、月の日数よりも、月の最後の日がこのプロパティと見なされます。</span><span class="sxs-lookup"><span data-stu-id="cda09-116">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed for this property.</span></span>  <br/> |
|[<span data-ttu-id="cda09-117">間隔</span><span class="sxs-lookup"><span data-stu-id="cda09-117">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="cda09-118">連続する 2 つの定期的なアイテムの間隔を定義します。</span><span class="sxs-lookup"><span data-stu-id="cda09-118">Defines the interval between two consecutive recurring items.</span></span> <span data-ttu-id="cda09-119">たとえば、**間隔**の要素の値が 5 の場合は、定期的なアイテムはすべて 5 月に発生します。</span><span class="sxs-lookup"><span data-stu-id="cda09-119">For example, if the **Interval** element has a value of 5, the recurring item occurs every 5 months.</span></span> <span data-ttu-id="cda09-120">有効値の範囲は、1 から 99 までです。</span><span class="sxs-lookup"><span data-stu-id="cda09-120">The range of valid values is from 1 to 99.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cda09-121">親要素</span><span class="sxs-lookup"><span data-stu-id="cda09-121">Parent elements</span></span>

|<span data-ttu-id="cda09-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="cda09-122">**Element**</span></span>|<span data-ttu-id="cda09-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="cda09-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cda09-124">定期的な予定 (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="cda09-124">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="cda09-125">定期タスクの頻度に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cda09-125">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="cda09-126">定期的なアイテム (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="cda09-126">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="cda09-127">予定表アイテムおよび会議出席依頼に定期的なパターンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cda09-127">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cda09-128">備考</span><span class="sxs-lookup"><span data-stu-id="cda09-128">Remarks</span></span>

<span data-ttu-id="cda09-129">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="cda09-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cda09-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="cda09-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cda09-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="cda09-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cda09-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cda09-132">Schema Name</span></span>  <br/> |<span data-ttu-id="cda09-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="cda09-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="cda09-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cda09-134">Validation File</span></span>  <br/> |<span data-ttu-id="cda09-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cda09-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cda09-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cda09-136">Can Be Empty</span></span>  <br/> |<span data-ttu-id="cda09-137">False</span><span class="sxs-lookup"><span data-stu-id="cda09-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cda09-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="cda09-138">See also</span></span>

- [<span data-ttu-id="cda09-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="cda09-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


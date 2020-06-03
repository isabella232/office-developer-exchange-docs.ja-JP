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
description: AbsoluteMonthlyRecurrence 要素は、月単位の定期的なパターンを表します。
ms.openlocfilehash: 3176cd30a1cfe7b2310f960ce377ab7a277e795a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460436"
---
# <a name="absolutemonthlyrecurrence"></a><span data-ttu-id="dcda4-103">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="dcda4-103">AbsoluteMonthlyRecurrence</span></span>

<span data-ttu-id="dcda4-104">**AbsoluteMonthlyRecurrence**要素は、月単位の定期的なパターンを表します。</span><span class="sxs-lookup"><span data-stu-id="dcda4-104">The **AbsoluteMonthlyRecurrence** element represents a monthly recurrence pattern.</span></span> 
  
```xml
<AbsoluteMonthlyRecurrence>
   <Interval/>
   <DayOfMonth/>
</AbsoluteMonthlyRecurrence>
```

 <span data-ttu-id="dcda4-105">**AbsoluteMonthlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="dcda4-105">**AbsoluteMonthlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dcda4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="dcda4-106">Attributes and elements</span></span>

<span data-ttu-id="dcda4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dcda4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dcda4-108">属性</span><span class="sxs-lookup"><span data-stu-id="dcda4-108">Attributes</span></span>

<span data-ttu-id="dcda4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dcda4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dcda4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dcda4-110">Child elements</span></span>

|<span data-ttu-id="dcda4-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="dcda4-111">**Element**</span></span>|<span data-ttu-id="dcda4-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="dcda4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dcda4-113">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="dcda4-113">DayOfMonth</span></span>](dayofmonth.md) <br/> |<span data-ttu-id="dcda4-114">定期的なアイテムが発生する月の日付を表します。</span><span class="sxs-lookup"><span data-stu-id="dcda4-114">Describes the day in a month that a recurring item occurs.</span></span> <span data-ttu-id="dcda4-115">このプロパティの値の範囲は、1 ~ 31 です。</span><span class="sxs-lookup"><span data-stu-id="dcda4-115">The range of values for this property is 1 to 31.</span></span> <span data-ttu-id="dcda4-116">特定の月の場合、この値はその月の日数よりも長くなるため、月の最後の日はこのプロパティの値と見なされます。</span><span class="sxs-lookup"><span data-stu-id="dcda4-116">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed for this property.</span></span>  <br/> |
|[<span data-ttu-id="dcda4-117">間隔</span><span class="sxs-lookup"><span data-stu-id="dcda4-117">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="dcda4-118">連続する2つのアイテム間の間隔を定義します。</span><span class="sxs-lookup"><span data-stu-id="dcda4-118">Defines the interval between two consecutive recurring items.</span></span> <span data-ttu-id="dcda4-119">たとえば、 **Interval**要素の値が5の場合、定期的なアイテムは5か月ごとに発生します。</span><span class="sxs-lookup"><span data-stu-id="dcda4-119">For example, if the **Interval** element has a value of 5, the recurring item occurs every 5 months.</span></span> <span data-ttu-id="dcda4-120">有効な値の範囲は、1 ~ 99 です。</span><span class="sxs-lookup"><span data-stu-id="dcda4-120">The range of valid values is from 1 to 99.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dcda4-121">親要素</span><span class="sxs-lookup"><span data-stu-id="dcda4-121">Parent elements</span></span>

|<span data-ttu-id="dcda4-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="dcda4-122">**Element**</span></span>|<span data-ttu-id="dcda4-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="dcda4-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dcda4-124">定期的なアイテム (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="dcda4-124">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="dcda4-125">定期的なタスクの定期的なアイテムの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dcda4-125">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="dcda4-126">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="dcda4-126">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="dcda4-127">予定表アイテムと会議出席依頼の定期的なパターンを含みます。</span><span class="sxs-lookup"><span data-stu-id="dcda4-127">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dcda4-128">注釈</span><span class="sxs-lookup"><span data-stu-id="dcda4-128">Remarks</span></span>

<span data-ttu-id="dcda4-129">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="dcda4-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dcda4-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="dcda4-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dcda4-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="dcda4-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dcda4-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dcda4-132">Schema Name</span></span>  <br/> |<span data-ttu-id="dcda4-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="dcda4-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="dcda4-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dcda4-134">Validation File</span></span>  <br/> |<span data-ttu-id="dcda4-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="dcda4-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dcda4-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="dcda4-136">Can Be Empty</span></span>  <br/> |<span data-ttu-id="dcda4-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="dcda4-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dcda4-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="dcda4-138">See also</span></span>

- [<span data-ttu-id="dcda4-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="dcda4-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


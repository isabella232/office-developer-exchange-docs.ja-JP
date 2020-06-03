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
description: RelativeMonthlyRecurrence 要素は、相対的な月単位の定期的なパターンを記述します。
ms.openlocfilehash: 90aa0e43684bfb09a3e13cf86ec96f680e80a714
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457509"
---
# <a name="relativemonthlyrecurrence"></a><span data-ttu-id="9bcba-103">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="9bcba-103">RelativeMonthlyRecurrence</span></span>

<span data-ttu-id="9bcba-104">**RelativeMonthlyRecurrence**要素は、相対的な月単位の定期的なパターンを記述します。</span><span class="sxs-lookup"><span data-stu-id="9bcba-104">The **RelativeMonthlyRecurrence** element describes a relative monthly recurrence pattern.</span></span> 
  
```xml
<RelativeMonthlyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
</RelativeMonthlyRecurrence>
```

 <span data-ttu-id="9bcba-105">**RelativeMonthlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="9bcba-105">**RelativeMonthlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9bcba-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9bcba-106">Attributes and elements</span></span>

<span data-ttu-id="9bcba-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9bcba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9bcba-108">属性</span><span class="sxs-lookup"><span data-stu-id="9bcba-108">Attributes</span></span>

<span data-ttu-id="9bcba-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9bcba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9bcba-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9bcba-110">Child elements</span></span>

|<span data-ttu-id="9bcba-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="9bcba-111">**Element**</span></span>|<span data-ttu-id="9bcba-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9bcba-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9bcba-113">間隔</span><span class="sxs-lookup"><span data-stu-id="9bcba-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="9bcba-114">2つの連続する定期的なパターンアイテム間の間隔を定義します。</span><span class="sxs-lookup"><span data-stu-id="9bcba-114">Defines the interval between two consecutive monthly recurring pattern items.</span></span> <span data-ttu-id="9bcba-115">この値の範囲は、1 ~ 99 です。</span><span class="sxs-lookup"><span data-stu-id="9bcba-115">The range for this value is 1 to 99.</span></span>  <br/> |
|[<span data-ttu-id="9bcba-116">DaysOfWeek (DayOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="9bcba-116">DaysOfWeek (DayOfWeekType)</span></span>](daysofweek-dayofweektype.md) <br/> |<span data-ttu-id="9bcba-117">相対的な月単位の定期的なパターンに含まれる曜日を指定します。</span><span class="sxs-lookup"><span data-stu-id="9bcba-117">Describes which days of the week are in the relative monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="9bcba-118">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="9bcba-118">DayOfWeekIndex</span></span>](dayofweekindex.md) <br/> |<span data-ttu-id="9bcba-119">相対的な月単位の定期的なパターンで使用される週を示します。</span><span class="sxs-lookup"><span data-stu-id="9bcba-119">Describes which week is used in a relative monthly recurrence pattern.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9bcba-120">親要素</span><span class="sxs-lookup"><span data-stu-id="9bcba-120">Parent elements</span></span>

|<span data-ttu-id="9bcba-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="9bcba-121">**Element**</span></span>|<span data-ttu-id="9bcba-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="9bcba-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9bcba-123">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="9bcba-123">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="9bcba-124">予定表アイテムと会議出席依頼の定期的なパターンを含みます。</span><span class="sxs-lookup"><span data-stu-id="9bcba-124">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="9bcba-125">定期的なアイテム (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="9bcba-125">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="9bcba-126">定期的なタスクの定期的なアイテムの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9bcba-126">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9bcba-127">注釈</span><span class="sxs-lookup"><span data-stu-id="9bcba-127">Remarks</span></span>

<span data-ttu-id="9bcba-128">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="9bcba-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9bcba-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9bcba-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9bcba-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="9bcba-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9bcba-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9bcba-131">Schema Name</span></span>  <br/> |<span data-ttu-id="9bcba-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9bcba-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="9bcba-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9bcba-133">Validation File</span></span>  <br/> |<span data-ttu-id="9bcba-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9bcba-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9bcba-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9bcba-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="9bcba-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="9bcba-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9bcba-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="9bcba-137">See also</span></span>



- [<span data-ttu-id="9bcba-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9bcba-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


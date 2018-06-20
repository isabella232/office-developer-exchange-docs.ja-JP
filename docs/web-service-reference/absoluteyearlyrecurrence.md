---
title: AbsoluteYearlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteYearlyRecurrence
api_type:
- schema
ms.assetid: 96f53e2c-3893-4f6e-a78a-ac179f45c5db
description: AbsoluteYearlyRecurrence 要素は、年間の定期的なパターンを表します。
ms.openlocfilehash: 205da336a6a6ca4fd39120e83ab264e1543354e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760410"
---
# <a name="absoluteyearlyrecurrence"></a><span data-ttu-id="69797-103">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="69797-103">AbsoluteYearlyRecurrence</span></span>

<span data-ttu-id="69797-104">**AbsoluteYearlyRecurrence**要素は、年間の定期的なパターンを表します。</span><span class="sxs-lookup"><span data-stu-id="69797-104">The **AbsoluteYearlyRecurrence** element represents a yearly recurrence pattern.</span></span> 
  
```xml
<AbsoluteYearlyRecurrence>
   <DayOfMonth/>
   <Month/>
</AbsoluteYearlyRecurrence>
```

 <span data-ttu-id="69797-105">**AbsoluteYearlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="69797-105">**AbsoluteYearlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="69797-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="69797-106">Attributes and elements</span></span>

<span data-ttu-id="69797-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="69797-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69797-108">属性</span><span class="sxs-lookup"><span data-stu-id="69797-108">Attributes</span></span>

<span data-ttu-id="69797-109">なし。</span><span class="sxs-lookup"><span data-stu-id="69797-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="69797-110">子要素</span><span class="sxs-lookup"><span data-stu-id="69797-110">Child elements</span></span>

|<span data-ttu-id="69797-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="69797-111">**Element**</span></span>|<span data-ttu-id="69797-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="69797-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69797-113">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="69797-113">DayOfMonth</span></span>](dayofmonth.md) <br/> |<span data-ttu-id="69797-114">定期的なアイテムが発生する月の日について説明します。</span><span class="sxs-lookup"><span data-stu-id="69797-114">Describes the day in a month on which a recurring item occurs.</span></span> <span data-ttu-id="69797-115">このプロパティの値の範囲は、1 から 31 です。</span><span class="sxs-lookup"><span data-stu-id="69797-115">The range of values for this property is 1 to 31.</span></span> <span data-ttu-id="69797-116">特定の月のこの値が大きい場合、月の日数よりも、月の最後の日がこのプロパティと見なされます。</span><span class="sxs-lookup"><span data-stu-id="69797-116">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed for this property.</span></span>  <br/> |
|[<span data-ttu-id="69797-117">月 (定期的なアイテム)</span><span class="sxs-lookup"><span data-stu-id="69797-117">Month (Item Recurrence)</span></span>](month-item-recurrence.md) <br/> |<span data-ttu-id="69797-118">年間の定期的なアイテムが発生する月をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="69797-118">Describes the month in which a yearly recurring item occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="69797-119">親要素</span><span class="sxs-lookup"><span data-stu-id="69797-119">Parent elements</span></span>

|<span data-ttu-id="69797-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="69797-120">**Element**</span></span>|<span data-ttu-id="69797-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="69797-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69797-122">定期的な予定 (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="69797-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="69797-123">定期タスクの頻度に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="69797-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="69797-124">定期的なアイテム (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="69797-124">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="69797-125">予定表アイテムおよび会議出席依頼に定期的なパターンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="69797-125">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="69797-126">備考</span><span class="sxs-lookup"><span data-stu-id="69797-126">Remarks</span></span>

<span data-ttu-id="69797-127">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="69797-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69797-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="69797-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69797-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="69797-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="69797-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="69797-130">Schema Name</span></span>  <br/> |<span data-ttu-id="69797-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="69797-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="69797-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="69797-132">Validation File</span></span>  <br/> |<span data-ttu-id="69797-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="69797-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="69797-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="69797-134">Can Be Empty</span></span>  <br/> |<span data-ttu-id="69797-135">False</span><span class="sxs-lookup"><span data-stu-id="69797-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69797-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="69797-136">See also</span></span>

- [<span data-ttu-id="69797-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="69797-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


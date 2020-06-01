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
description: AbsoluteYearlyRecurrence 要素は、年単位の定期的なパターンを表します。
ms.openlocfilehash: 19b617dfd5c0a3d206d62439c880da084fd5f5f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460415"
---
# <a name="absoluteyearlyrecurrence"></a><span data-ttu-id="d5252-103">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="d5252-103">AbsoluteYearlyRecurrence</span></span>

<span data-ttu-id="d5252-104">**AbsoluteYearlyRecurrence**要素は、年単位の定期的なパターンを表します。</span><span class="sxs-lookup"><span data-stu-id="d5252-104">The **AbsoluteYearlyRecurrence** element represents a yearly recurrence pattern.</span></span> 
  
```xml
<AbsoluteYearlyRecurrence>
   <DayOfMonth/>
   <Month/>
</AbsoluteYearlyRecurrence>
```

 <span data-ttu-id="d5252-105">**AbsoluteYearlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="d5252-105">**AbsoluteYearlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d5252-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d5252-106">Attributes and elements</span></span>

<span data-ttu-id="d5252-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d5252-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5252-108">属性</span><span class="sxs-lookup"><span data-stu-id="d5252-108">Attributes</span></span>

<span data-ttu-id="d5252-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d5252-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5252-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d5252-110">Child elements</span></span>

|<span data-ttu-id="d5252-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d5252-111">**Element**</span></span>|<span data-ttu-id="d5252-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d5252-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5252-113">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="d5252-113">DayOfMonth</span></span>](dayofmonth.md) <br/> |<span data-ttu-id="d5252-114">定期的なアイテムが発生する月の日付を表します。</span><span class="sxs-lookup"><span data-stu-id="d5252-114">Describes the day in a month on which a recurring item occurs.</span></span> <span data-ttu-id="d5252-115">このプロパティの値の範囲は、1 ~ 31 です。</span><span class="sxs-lookup"><span data-stu-id="d5252-115">The range of values for this property is 1 to 31.</span></span> <span data-ttu-id="d5252-116">特定の月の場合、この値はその月の日数よりも長くなるため、月の最後の日はこのプロパティの値と見なされます。</span><span class="sxs-lookup"><span data-stu-id="d5252-116">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed for this property.</span></span>  <br/> |
|[<span data-ttu-id="d5252-117">月 (アイテムの定期的な予定)</span><span class="sxs-lookup"><span data-stu-id="d5252-117">Month (Item Recurrence)</span></span>](month-item-recurrence.md) <br/> |<span data-ttu-id="d5252-118">年単位の定期的なアイテムが発生する月を表します。</span><span class="sxs-lookup"><span data-stu-id="d5252-118">Describes the month in which a yearly recurring item occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d5252-119">親要素</span><span class="sxs-lookup"><span data-stu-id="d5252-119">Parent elements</span></span>

|<span data-ttu-id="d5252-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="d5252-120">**Element**</span></span>|<span data-ttu-id="d5252-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="d5252-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5252-122">定期的なアイテム (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="d5252-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="d5252-123">定期的なタスクの定期的なアイテムの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d5252-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="d5252-124">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="d5252-124">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="d5252-125">予定表アイテムと会議出席依頼の定期的なパターンを含みます。</span><span class="sxs-lookup"><span data-stu-id="d5252-125">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d5252-126">注釈</span><span class="sxs-lookup"><span data-stu-id="d5252-126">Remarks</span></span>

<span data-ttu-id="d5252-127">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d5252-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d5252-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d5252-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5252-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="d5252-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d5252-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d5252-130">Schema Name</span></span>  <br/> |<span data-ttu-id="d5252-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d5252-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="d5252-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d5252-132">Validation File</span></span>  <br/> |<span data-ttu-id="d5252-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d5252-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d5252-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d5252-134">Can Be Empty</span></span>  <br/> |<span data-ttu-id="d5252-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="d5252-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5252-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="d5252-136">See also</span></span>

- [<span data-ttu-id="d5252-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d5252-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


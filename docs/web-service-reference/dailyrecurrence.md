---
title: DailyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DailyRecurrence
api_type:
- schema
ms.assetid: 0aaf265d-b723-49c6-8e9c-9ba60141e9ab
description: DailyRecurrence 要素では、日、予定表アイテム、またはタスクを定期的に、頻度について説明します。
ms.openlocfilehash: d02c1f7425372d60c10b40527dc5f0d65f923b45
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759900"
---
# <a name="dailyrecurrence"></a><span data-ttu-id="d083e-103">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="d083e-103">DailyRecurrence</span></span>

<span data-ttu-id="d083e-104">**DailyRecurrence**要素では、日、予定表アイテム、またはタスクを定期的に、頻度について説明します。</span><span class="sxs-lookup"><span data-stu-id="d083e-104">The **DailyRecurrence** element describes the frequency, in days, in which a calendar item or a task recurs.</span></span> 
  
```xml
<DailyRecurrence>
   <Interval/>
</DailyRecurrence>
```

<span data-ttu-id="d083e-105">**DailyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="d083e-105">**DailyRecurrencePatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d083e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d083e-106">Attributes and elements</span></span>

<span data-ttu-id="d083e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d083e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d083e-108">属性</span><span class="sxs-lookup"><span data-stu-id="d083e-108">Attributes</span></span>

<span data-ttu-id="d083e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d083e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d083e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d083e-110">Child elements</span></span>

|<span data-ttu-id="d083e-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d083e-111">**Element**</span></span>|<span data-ttu-id="d083e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d083e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d083e-113">間隔</span><span class="sxs-lookup"><span data-stu-id="d083e-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="d083e-114">差の日数、連続する 2 つの定期的なアイテムの間隔を定義します。</span><span class="sxs-lookup"><span data-stu-id="d083e-114">Defines the interval, in days, between two consecutive recurring items.</span></span> <span data-ttu-id="d083e-115">値は 1 から 999 の範囲である必要があります。</span><span class="sxs-lookup"><span data-stu-id="d083e-115">The value must be in the range from 1 to 999.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d083e-116">親要素</span><span class="sxs-lookup"><span data-stu-id="d083e-116">Parent elements</span></span>

|<span data-ttu-id="d083e-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="d083e-117">**Element**</span></span>|<span data-ttu-id="d083e-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="d083e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d083e-119">定期的な予定 (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="d083e-119">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="d083e-120">定期タスクの頻度に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d083e-120">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="d083e-121">定期的なアイテム (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="d083e-121">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="d083e-122">予定表アイテムおよび会議出席依頼に定期的なパターンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d083e-122">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d083e-123">備考</span><span class="sxs-lookup"><span data-stu-id="d083e-123">Remarks</span></span>

<span data-ttu-id="d083e-124">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="d083e-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d083e-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="d083e-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d083e-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="d083e-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d083e-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d083e-127">Schema name</span></span>  <br/> |<span data-ttu-id="d083e-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d083e-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="d083e-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d083e-129">Validation file</span></span>  <br/> |<span data-ttu-id="d083e-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d083e-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d083e-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d083e-131">Can be empty</span></span>  <br/> |<span data-ttu-id="d083e-132">False</span><span class="sxs-lookup"><span data-stu-id="d083e-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d083e-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="d083e-133">See also</span></span>

- [<span data-ttu-id="d083e-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d083e-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


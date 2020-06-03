---
title: Interval/間隔
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Interval
api_type:
- schema
ms.assetid: d0c97a5f-96be-40c6-b7d4-abf4c3870adf
description: Interval 要素は、連続する2つのアイテム間の間隔を定義します。
ms.openlocfilehash: 70a41cfc438f057cbe11d792f0004d46d0abcc85
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526565"
---
# <a name="interval"></a><span data-ttu-id="56f81-103">Interval/間隔</span><span class="sxs-lookup"><span data-stu-id="56f81-103">Interval</span></span>

<span data-ttu-id="56f81-104">**Interval**要素は、連続する2つのアイテム間の間隔を定義します。</span><span class="sxs-lookup"><span data-stu-id="56f81-104">The **Interval** element defines the interval between two consecutive recurring items.</span></span> 
  
```xml
<Interval/>
```

 <span data-ttu-id="56f81-105">**int**</span><span class="sxs-lookup"><span data-stu-id="56f81-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="56f81-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="56f81-106">Attributes and elements</span></span>

<span data-ttu-id="56f81-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="56f81-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56f81-108">属性</span><span class="sxs-lookup"><span data-stu-id="56f81-108">Attributes</span></span>

<span data-ttu-id="56f81-109">なし。</span><span class="sxs-lookup"><span data-stu-id="56f81-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="56f81-110">子要素</span><span class="sxs-lookup"><span data-stu-id="56f81-110">Child elements</span></span>

<span data-ttu-id="56f81-111">なし。</span><span class="sxs-lookup"><span data-stu-id="56f81-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="56f81-112">親要素</span><span class="sxs-lookup"><span data-stu-id="56f81-112">Parent elements</span></span>

|<span data-ttu-id="56f81-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="56f81-113">**Element**</span></span>|<span data-ttu-id="56f81-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="56f81-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56f81-115">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="56f81-115">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="56f81-116">1 か月ごと。</span><span class="sxs-lookup"><span data-stu-id="56f81-116">Represents a monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="56f81-117">DailyRegeneration</span><span class="sxs-lookup"><span data-stu-id="56f81-117">DailyRegeneration</span></span>](dailyregeneration.md) <br/> |<span data-ttu-id="56f81-118">タスクが再生成される頻度 (日単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="56f81-118">Describes the frequency, in days, in which a task is regenerated.</span></span>  <br/> |
|[<span data-ttu-id="56f81-119">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="56f81-119">DailyRecurrence</span></span>](dailyrecurrence.md) <br/> |<span data-ttu-id="56f81-120">タスクが繰り返される頻度 (日単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="56f81-120">Describes the frequency, in days, in which a task recurs.</span></span>  <br/> |
|[<span data-ttu-id="56f81-121">月の明示再生</span><span class="sxs-lookup"><span data-stu-id="56f81-121">MonthlyRegeneration</span></span>](monthlyregeneration.md) <br/> |<span data-ttu-id="56f81-122">タスクが再生成される頻度 (月単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="56f81-122">Describes the frequency, in months, in which a task is regenerated.</span></span>  <br/> |
|[<span data-ttu-id="56f81-123">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="56f81-123">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="56f81-124">定期的なタスクの相対月パターンを表します。</span><span class="sxs-lookup"><span data-stu-id="56f81-124">Describes a relative monthly pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="56f81-125">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="56f81-125">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="56f81-126">頻度 (週単位) と、タスクが繰り返される曜日を表します。</span><span class="sxs-lookup"><span data-stu-id="56f81-126">Describes the frequency, in weeks, in which and the days on which a task recurs.</span></span>  <br/> |
|[<span data-ttu-id="56f81-127">WeeklyRegeneration</span><span class="sxs-lookup"><span data-stu-id="56f81-127">WeeklyRegeneration</span></span>](weeklyregeneration.md) <br/> |<span data-ttu-id="56f81-128">タスクが再生成される頻度 (週単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="56f81-128">Describes the frequency, in weeks, in which a task is regenerated.</span></span>  <br/> |
|[<span data-ttu-id="56f81-129">YearlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="56f81-129">YearlyRegeneration</span></span>](yearlyregeneration.md) <br/> |<span data-ttu-id="56f81-130">タスクが再生成される頻度 (年単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="56f81-130">Describes the frequency, in years, in which a task is regenerated.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="56f81-131">テキスト値</span><span class="sxs-lookup"><span data-stu-id="56f81-131">Text value</span></span>

<span data-ttu-id="56f81-132">整数を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="56f81-132">A text value that represents an integer is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="56f81-133">注釈</span><span class="sxs-lookup"><span data-stu-id="56f81-133">Remarks</span></span>

<span data-ttu-id="56f81-134">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="56f81-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="56f81-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="56f81-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56f81-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="56f81-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="56f81-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="56f81-137">Schema name</span></span>  <br/> |<span data-ttu-id="56f81-138">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="56f81-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="56f81-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="56f81-139">Validation file</span></span>  <br/> |<span data-ttu-id="56f81-140">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="56f81-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="56f81-141">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="56f81-141">Can be empty</span></span>  <br/> |<span data-ttu-id="56f81-142">正しくない</span><span class="sxs-lookup"><span data-stu-id="56f81-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="56f81-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="56f81-143">See also</span></span>



- [<span data-ttu-id="56f81-144">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="56f81-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


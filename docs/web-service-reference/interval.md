---
title: Interval
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
description: 間隔の要素は、連続する 2 つの定期的なアイテムの間隔を定義します。
ms.openlocfilehash: 55d26b5b1b51aca3effa93a2e6852c1ae57ef4b0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831962"
---
# <a name="interval"></a><span data-ttu-id="475db-103">Interval</span><span class="sxs-lookup"><span data-stu-id="475db-103">Interval</span></span>

<span data-ttu-id="475db-104">**間隔**の要素は、連続する 2 つの定期的なアイテムの間隔を定義します。</span><span class="sxs-lookup"><span data-stu-id="475db-104">The **Interval** element defines the interval between two consecutive recurring items.</span></span> 
  
```xml
<Interval/>
```

 <span data-ttu-id="475db-105">**int**</span><span class="sxs-lookup"><span data-stu-id="475db-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="475db-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="475db-106">Attributes and elements</span></span>

<span data-ttu-id="475db-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="475db-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="475db-108">属性</span><span class="sxs-lookup"><span data-stu-id="475db-108">Attributes</span></span>

<span data-ttu-id="475db-109">なし。</span><span class="sxs-lookup"><span data-stu-id="475db-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="475db-110">子要素</span><span class="sxs-lookup"><span data-stu-id="475db-110">Child elements</span></span>

<span data-ttu-id="475db-111">なし。</span><span class="sxs-lookup"><span data-stu-id="475db-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="475db-112">親要素</span><span class="sxs-lookup"><span data-stu-id="475db-112">Parent elements</span></span>

|<span data-ttu-id="475db-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="475db-113">**Element**</span></span>|<span data-ttu-id="475db-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="475db-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="475db-115">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="475db-115">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="475db-116">1 か月ごと。</span><span class="sxs-lookup"><span data-stu-id="475db-116">Represents a monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="475db-117">DailyRegeneration</span><span class="sxs-lookup"><span data-stu-id="475db-117">DailyRegeneration</span></span>](dailyregeneration.md) <br/> |<span data-ttu-id="475db-118">日後にタスクが再生成される頻度を説明します。</span><span class="sxs-lookup"><span data-stu-id="475db-118">Describes the frequency, in days, in which a task is regenerated.</span></span>  <br/> |
|[<span data-ttu-id="475db-119">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="475db-119">DailyRecurrence</span></span>](dailyrecurrence.md) <br/> |<span data-ttu-id="475db-120">頻度を日数でタスクが繰り返し発生するについて説明します。</span><span class="sxs-lookup"><span data-stu-id="475db-120">Describes the frequency, in days, in which a task recurs.</span></span>  <br/> |
|[<span data-ttu-id="475db-121">MonthlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="475db-121">MonthlyRegeneration</span></span>](monthlyregeneration.md) <br/> |<span data-ttu-id="475db-122">月のタスクが再生成される頻度を説明します。</span><span class="sxs-lookup"><span data-stu-id="475db-122">Describes the frequency, in months, in which a task is regenerated.</span></span>  <br/> |
|[<span data-ttu-id="475db-123">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="475db-123">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="475db-124">定期的なタスクの相対的な月単位のパターンについて説明します。</span><span class="sxs-lookup"><span data-stu-id="475db-124">Describes a relative monthly pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="475db-125">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="475db-125">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="475db-126">週単位、およびタスクが繰り返し発生する日は、頻度について説明します。</span><span class="sxs-lookup"><span data-stu-id="475db-126">Describes the frequency, in weeks, in which and the days on which a task recurs.</span></span>  <br/> |
|[<span data-ttu-id="475db-127">WeeklyRegeneration</span><span class="sxs-lookup"><span data-stu-id="475db-127">WeeklyRegeneration</span></span>](weeklyregeneration.md) <br/> |<span data-ttu-id="475db-128">週間後、タスクが再生成される頻度を説明します。</span><span class="sxs-lookup"><span data-stu-id="475db-128">Describes the frequency, in weeks, in which a task is regenerated.</span></span>  <br/> |
|[<span data-ttu-id="475db-129">YearlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="475db-129">YearlyRegeneration</span></span>](yearlyregeneration.md) <br/> |<span data-ttu-id="475db-130">年間で、タスクが再生成される頻度を説明します。</span><span class="sxs-lookup"><span data-stu-id="475db-130">Describes the frequency, in years, in which a task is regenerated.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="475db-131">テキスト値</span><span class="sxs-lookup"><span data-stu-id="475db-131">Text value</span></span>

<span data-ttu-id="475db-132">整数値を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="475db-132">A text value that represents an integer is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="475db-133">備考</span><span class="sxs-lookup"><span data-stu-id="475db-133">Remarks</span></span>

<span data-ttu-id="475db-134">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="475db-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="475db-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="475db-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="475db-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="475db-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="475db-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="475db-137">Schema name</span></span>  <br/> |<span data-ttu-id="475db-138">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="475db-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="475db-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="475db-139">Validation file</span></span>  <br/> |<span data-ttu-id="475db-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="475db-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="475db-141">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="475db-141">Can be empty</span></span>  <br/> |<span data-ttu-id="475db-142">False</span><span class="sxs-lookup"><span data-stu-id="475db-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="475db-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="475db-143">See also</span></span>



- [<span data-ttu-id="475db-144">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="475db-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


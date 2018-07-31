---
title: Recurrence (TaskRecurrenceType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recurrence
api_type:
- schema
ms.assetid: 99f8414a-9110-4721-a6e5-ebf225d7ed0a
description: 定期的なアイテムの要素には、定期タスクの頻度に関する情報が含まれています。
ms.openlocfilehash: 0ec43447e47050a0bd483d8441da88e4a7f08923
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354422"
---
# <a name="recurrence-taskrecurrencetype"></a><span data-ttu-id="1c673-103">Recurrence (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="1c673-103">Recurrence (TaskRecurrenceType)</span></span>

<span data-ttu-id="1c673-104">**定期的なアイテム**の要素には、定期タスクの頻度に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1c673-104">The **Recurrence** element contains recurrence information for recurring tasks.</span></span> 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <MonthlyRegeneration/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <DailyRegeneration/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
       <DailyRegeneration/> 
       <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <DailyRegeneration/> 
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
       <MonthlyRegeneration/> 
       <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <YearlyRegeneration/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <YearlyRegeneration/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRegeneration/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeYearlyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRegeneration/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <YearlyRegeneration/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeYearlyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
       <MonthlyRegeneration/> 
       <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
       <DailyRecurrence/> 
       <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRegeneration/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```


<span data-ttu-id="1c673-105">**TaskRecurrenceType**</span><span class="sxs-lookup"><span data-stu-id="1c673-105">**TaskRecurrenceType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1c673-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1c673-106">Attributes and elements</span></span>

<span data-ttu-id="1c673-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1c673-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1c673-108">属性</span><span class="sxs-lookup"><span data-stu-id="1c673-108">Attributes</span></span>

<span data-ttu-id="1c673-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1c673-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1c673-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1c673-110">Child elements</span></span>

|<span data-ttu-id="1c673-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="1c673-111">**Element**</span></span>|<span data-ttu-id="1c673-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1c673-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c673-113">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="1c673-113">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="1c673-114">定期的なタスクの相対的な年 1 回定期的なパターンをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1c673-114">Describes a relative yearly recurrence pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="1c673-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="1c673-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="1c673-116">定期的な仕事の年間の定期的なパターンを表します。</span><span class="sxs-lookup"><span data-stu-id="1c673-116">Represents a yearly recurrence pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="1c673-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="1c673-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="1c673-118">定期的なタスクの相対的な毎月定期的なパターンをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1c673-118">Describes a relative monthly recurrence pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="1c673-119">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="1c673-119">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="1c673-120">定期的な仕事の毎月の定期的なパターンを表します。</span><span class="sxs-lookup"><span data-stu-id="1c673-120">Represents a monthly recurrence pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="1c673-121">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="1c673-121">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="1c673-122">週、および日のタスクが繰り返し発生する頻度について説明します。</span><span class="sxs-lookup"><span data-stu-id="1c673-122">Describes the frequency, in weeks, and the days on which a task recurs.</span></span>  <br/> |
|[<span data-ttu-id="1c673-123">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="1c673-123">DailyRecurrence</span></span>](dailyrecurrence.md) <br/> |<span data-ttu-id="1c673-124">頻度を日数でタスクが繰り返し発生するについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1c673-124">Describes the frequency, in days, in which a task recurs.</span></span>  <br/> |
|[<span data-ttu-id="1c673-125">DailyRegeneration</span><span class="sxs-lookup"><span data-stu-id="1c673-125">DailyRegeneration</span></span>](dailyregeneration.md) <br/> |<span data-ttu-id="1c673-126">次の項目の現在のタスクの完了の期限後、何日間について説明します。</span><span class="sxs-lookup"><span data-stu-id="1c673-126">Describes how many days after the completion of the current task the next occurrence will be due.</span></span>  <br/> |
|[<span data-ttu-id="1c673-127">WeeklyRegeneration</span><span class="sxs-lookup"><span data-stu-id="1c673-127">WeeklyRegeneration</span></span>](weeklyregeneration.md) <br/> |<span data-ttu-id="1c673-128">次の項目の現在のタスクの完了の期限後の数週間をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1c673-128">Describes how many weeks after the completion of the current task the next occurrence will be due.</span></span>  <br/> |
|[<span data-ttu-id="1c673-129">MonthlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="1c673-129">MonthlyRegeneration</span></span>](monthlyregeneration.md) <br/> |<span data-ttu-id="1c673-130">次に一致する現在のタスクの完了が原因である後数か月間について説明します。</span><span class="sxs-lookup"><span data-stu-id="1c673-130">Describes how many months after the completion of the current task the next occurrence will be due.</span></span>  <br/> |
|[<span data-ttu-id="1c673-131">YearlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="1c673-131">YearlyRegeneration</span></span>](yearlyregeneration.md) <br/> |<span data-ttu-id="1c673-132">数年の後、次に一致する現在のタスクの完了が原因であるについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1c673-132">Describes how many years after the completion of the current task the next occurrence will be due.</span></span>  <br/> |
|[<span data-ttu-id="1c673-133">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="1c673-133">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="1c673-134">定義された終了日がない定期的なパターンをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1c673-134">Describes a recurrence pattern that does not have a defined end date.</span></span>  <br/> <span data-ttu-id="1c673-135">この要素の使用は、 [EndDateRecurrence](enddaterecurrence.md)と[NumberedRecurrence](numberedrecurrence.md)の要素の使用を除外します。</span><span class="sxs-lookup"><span data-stu-id="1c673-135">The use of this element excludes the use of the [EndDateRecurrence](enddaterecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="1c673-136">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="1c673-136">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="1c673-137">開始日と終了日の項目の定期的なパターンについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1c673-137">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> <span data-ttu-id="1c673-138">この要素の使用は、 [NoEndRecurrence](noendrecurrence.md)と[NumberedRecurrence](numberedrecurrence.md)の要素の使用を除外します。</span><span class="sxs-lookup"><span data-stu-id="1c673-138">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> <span data-ttu-id="1c673-139">再生のパターンとは、 [EndDateRecurrence](enddaterecurrence.md)を使用できません。</span><span class="sxs-lookup"><span data-stu-id="1c673-139">[EndDateRecurrence](enddaterecurrence.md) cannot be used together with a regeneration pattern.</span></span>  <br/> |
|[<span data-ttu-id="1c673-140">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="1c673-140">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="1c673-141">開始日と定期的なアイテムの出現回数を説明します。</span><span class="sxs-lookup"><span data-stu-id="1c673-141">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> <span data-ttu-id="1c673-142">この要素の使用は、 [NoEndRecurrence](noendrecurrence.md)と[EndDateRecurrence](enddaterecurrence.md)の要素の使用を除外します。</span><span class="sxs-lookup"><span data-stu-id="1c673-142">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [EndDateRecurrence](enddaterecurrence.md) elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1c673-143">親要素</span><span class="sxs-lookup"><span data-stu-id="1c673-143">Parent elements</span></span>

|<span data-ttu-id="1c673-144">**要素**</span><span class="sxs-lookup"><span data-stu-id="1c673-144">**Element**</span></span>|<span data-ttu-id="1c673-145">**説明**</span><span class="sxs-lookup"><span data-stu-id="1c673-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c673-146">タスク</span><span class="sxs-lookup"><span data-stu-id="1c673-146">Task</span></span>](task.md) <br/> |<span data-ttu-id="1c673-147">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="1c673-147">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1c673-148">注釈</span><span class="sxs-lookup"><span data-stu-id="1c673-148">Remarks</span></span>

<span data-ttu-id="1c673-149">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="1c673-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1c673-150">要素情報</span><span class="sxs-lookup"><span data-stu-id="1c673-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1c673-151">名前空間</span><span class="sxs-lookup"><span data-stu-id="1c673-151">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1c673-152">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1c673-152">Schema name</span></span>  <br/> |<span data-ttu-id="1c673-153">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1c673-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="1c673-154">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1c673-154">Validation file</span></span>  <br/> |<span data-ttu-id="1c673-155">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1c673-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1c673-156">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1c673-156">Can be empty</span></span>  <br/> |<span data-ttu-id="1c673-157">False</span><span class="sxs-lookup"><span data-stu-id="1c673-157">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1c673-158">関連項目</span><span class="sxs-lookup"><span data-stu-id="1c673-158">See also</span></span>

- [<span data-ttu-id="1c673-159">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1c673-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


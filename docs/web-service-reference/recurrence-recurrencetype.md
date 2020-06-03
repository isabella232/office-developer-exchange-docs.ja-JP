---
title: Recurrence (RecurrenceType)
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
ms.assetid: 3d1c2c1c-4103-47ce-ad3c-ad16ec6e9b12
description: 繰り返し要素には、予定表アイテムと会議出席依頼の定期的なパターンが含まれています。
ms.openlocfilehash: d00445c75fb35c3bb99eeed06e30cb1cf2883597
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529890"
---
# <a name="recurrence-recurrencetype"></a><span data-ttu-id="8d793-103">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="8d793-103">Recurrence (RecurrenceType)</span></span>

<span data-ttu-id="8d793-104">**繰り返し**要素には、予定表アイテムと会議出席依頼の定期的なパターンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8d793-104">The **Recurrence** element contains the recurrence pattern for calendar items and meeting requests.</span></span> 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
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
      <RelativeMonthlyRecurrence/> 
      <NumberedRecurrence/>
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
      <RelativeYearlyRecurrence/> 
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
      <DailyRecurrence/> 
      <NoEndRecurrence/>
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
      <DailyRecurrence/> 
      <EndDateRecurrence/>
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
      <DailyRecurrence/> 
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
      <AbsoluteMonthlyRecurrence/> 
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
      <WeeklyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <NumberedRecurrence/> 
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
      <RelativeMonthlyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

<span data-ttu-id="8d793-105">**RecurrenceType**</span><span class="sxs-lookup"><span data-stu-id="8d793-105">**RecurrenceType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8d793-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8d793-106">Attributes and elements</span></span>

<span data-ttu-id="8d793-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8d793-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d793-108">属性</span><span class="sxs-lookup"><span data-stu-id="8d793-108">Attributes</span></span>

<span data-ttu-id="8d793-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8d793-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d793-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8d793-110">Child elements</span></span>

|<span data-ttu-id="8d793-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="8d793-111">**Element**</span></span>|<span data-ttu-id="8d793-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="8d793-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d793-113">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="8d793-113">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="8d793-114">相対的な年単位の定期的なパターンを記述します。</span><span class="sxs-lookup"><span data-stu-id="8d793-114">Describes a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="8d793-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="8d793-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="8d793-116">1 年ごと。</span><span class="sxs-lookup"><span data-stu-id="8d793-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="8d793-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="8d793-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="8d793-118">定期的な予定表アイテムの相対的な月単位のパターンを記述します。</span><span class="sxs-lookup"><span data-stu-id="8d793-118">Describes a relative monthly recurrence pattern for a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8d793-119">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="8d793-119">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="8d793-120">1 か月ごと。</span><span class="sxs-lookup"><span data-stu-id="8d793-120">Represents a monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="8d793-121">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="8d793-121">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="8d793-122">頻度 (週単位) と予定表アイテムまたはタスクが繰り返される日数を示します。</span><span class="sxs-lookup"><span data-stu-id="8d793-122">Describes the frequency, in weeks, and the days that a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="8d793-123">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="8d793-123">DailyRecurrence</span></span>](dailyrecurrence.md) <br/> |<span data-ttu-id="8d793-124">予定表アイテムまたはタスクが繰り返される頻度 (日単位) を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d793-124">Describes the frequency, in days, in which a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="8d793-125">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="8d793-125">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="8d793-126">定義済みの終了日がない定期的なパターンを記述します。</span><span class="sxs-lookup"><span data-stu-id="8d793-126">Describes a recurrence pattern that does not have a defined end date.</span></span>  <br/> <span data-ttu-id="8d793-127">この要素を使用すると、 [EndDateRecurrence](enddaterecurrence.md)要素と[番号 ed再発](numberedrecurrence.md)要素の使用が除外されます。</span><span class="sxs-lookup"><span data-stu-id="8d793-127">The use of this element excludes the use of the [EndDateRecurrence](enddaterecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="8d793-128">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="8d793-128">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="8d793-129">アイテムの定期的なパターンの開始日と終了日を示します。</span><span class="sxs-lookup"><span data-stu-id="8d793-129">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> <span data-ttu-id="8d793-130">この要素を使用すると、 [Noendrecurrence なパターン](noendrecurrence.md)要素と[番号 ed再発](numberedrecurrence.md)要素の使用が除外されます。</span><span class="sxs-lookup"><span data-stu-id="8d793-130">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="8d793-131">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="8d793-131">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="8d793-132">定期的なアイテムの開始日と発生回数を表します。</span><span class="sxs-lookup"><span data-stu-id="8d793-132">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> <span data-ttu-id="8d793-133">この要素を使用すると、 [Noendrecurrence](noendrecurrence.md)要素と[EndDateRecurrence](enddaterecurrence.md)要素の使用が除外されます。</span><span class="sxs-lookup"><span data-stu-id="8d793-133">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [EndDateRecurrence](enddaterecurrence.md) elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8d793-134">親要素</span><span class="sxs-lookup"><span data-stu-id="8d793-134">Parent elements</span></span>

|<span data-ttu-id="8d793-135">**要素**</span><span class="sxs-lookup"><span data-stu-id="8d793-135">**Element**</span></span>|<span data-ttu-id="8d793-136">**説明**</span><span class="sxs-lookup"><span data-stu-id="8d793-136">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d793-137">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="8d793-137">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="8d793-138">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="8d793-138">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8d793-139">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="8d793-139">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="8d793-140">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="8d793-140">Represents a meeting request in the Exchange store</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8d793-141">注釈</span><span class="sxs-lookup"><span data-stu-id="8d793-141">Remarks</span></span>

<span data-ttu-id="8d793-142">[Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。</span><span class="sxs-lookup"><span data-stu-id="8d793-142">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="8d793-143">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="8d793-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8d793-144">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8d793-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d793-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="8d793-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8d793-146">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8d793-146">Schema name</span></span>  <br/> |<span data-ttu-id="8d793-147">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8d793-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="8d793-148">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8d793-148">Validation file</span></span>  <br/> |<span data-ttu-id="8d793-149">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8d793-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8d793-150">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8d793-150">Can be empty</span></span>  <br/> |<span data-ttu-id="8d793-151">正しくない</span><span class="sxs-lookup"><span data-stu-id="8d793-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8d793-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="8d793-152">See also</span></span>

- [<span data-ttu-id="8d793-153">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8d793-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


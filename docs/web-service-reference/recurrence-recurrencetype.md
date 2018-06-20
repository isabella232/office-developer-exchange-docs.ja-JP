---
title: 定期的なアイテム (RecurrenceType)
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
description: 定期的なアイテムの要素には、予定表アイテムおよび会議出席依頼に定期的なパターンが含まれています。
ms.openlocfilehash: f26ccf5912848a6d7fbbfa7d0a19d41635c896e0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833004"
---
# <a name="recurrence-recurrencetype"></a><span data-ttu-id="caf61-103">定期的なアイテム (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="caf61-103">Recurrence (RecurrenceType)</span></span>

<span data-ttu-id="caf61-104">**定期的なアイテム**の要素には、予定表アイテムおよび会議出席依頼に定期的なパターンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="caf61-104">The **Recurrence** element contains the recurrence pattern for calendar items and meeting requests.</span></span> 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

 <span data-ttu-id="caf61-105">**RecurrenceType**</span><span class="sxs-lookup"><span data-stu-id="caf61-105">**RecurrenceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="caf61-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="caf61-106">Attributes and elements</span></span>

<span data-ttu-id="caf61-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="caf61-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="caf61-108">属性</span><span class="sxs-lookup"><span data-stu-id="caf61-108">Attributes</span></span>

<span data-ttu-id="caf61-109">なし。</span><span class="sxs-lookup"><span data-stu-id="caf61-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="caf61-110">子要素</span><span class="sxs-lookup"><span data-stu-id="caf61-110">Child elements</span></span>

|<span data-ttu-id="caf61-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="caf61-111">**Element**</span></span>|<span data-ttu-id="caf61-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="caf61-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="caf61-113">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="caf61-113">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="caf61-114">相対年間の定期的なパターンをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="caf61-114">Describes a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="caf61-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="caf61-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="caf61-116">1 年ごと。</span><span class="sxs-lookup"><span data-stu-id="caf61-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="caf61-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="caf61-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="caf61-118">定期的な予定表アイテムの相対的な毎月定期的なパターンをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="caf61-118">Describes a relative monthly recurrence pattern for a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="caf61-119">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="caf61-119">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="caf61-120">1 か月ごと。</span><span class="sxs-lookup"><span data-stu-id="caf61-120">Represents a monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="caf61-121">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="caf61-121">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="caf61-122">週、および定期的に繰り返されるタスクの予定表アイテムで、頻度を説明します。</span><span class="sxs-lookup"><span data-stu-id="caf61-122">Describes the frequency, in weeks, and the days that a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="caf61-123">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="caf61-123">DailyRecurrence</span></span>](dailyrecurrence.md) <br/> |<span data-ttu-id="caf61-124">日単位での周波数を表すタスクの予定表アイテムが再発するのです。</span><span class="sxs-lookup"><span data-stu-id="caf61-124">Describes the frequency, in days, in which a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="caf61-125">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="caf61-125">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="caf61-126">定義された終了日がない定期的なパターンをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="caf61-126">Describes a recurrence pattern that does not have a defined end date.</span></span>  <br/> <span data-ttu-id="caf61-127">この要素の使用は、 [EndDateRecurrence](enddaterecurrence.md)と[NumberedRecurrence](numberedrecurrence.md)の要素の使用を除外します。</span><span class="sxs-lookup"><span data-stu-id="caf61-127">The use of this element excludes the use of the [EndDateRecurrence](enddaterecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="caf61-128">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="caf61-128">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="caf61-129">開始日と終了日の項目の定期的なパターンについて説明します。</span><span class="sxs-lookup"><span data-stu-id="caf61-129">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> <span data-ttu-id="caf61-130">この要素の使用は、 [NoEndRecurrence](noendrecurrence.md)と[NumberedRecurrence](numberedrecurrence.md)の要素の使用を除外します。</span><span class="sxs-lookup"><span data-stu-id="caf61-130">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="caf61-131">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="caf61-131">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="caf61-132">開始日と定期的なアイテムの出現回数を説明します。</span><span class="sxs-lookup"><span data-stu-id="caf61-132">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> <span data-ttu-id="caf61-133">この要素の使用は、 [NoEndRecurrence](noendrecurrence.md)と[EndDateRecurrence](enddaterecurrence.md)の要素の使用を除外します。</span><span class="sxs-lookup"><span data-stu-id="caf61-133">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [EndDateRecurrence](enddaterecurrence.md) elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="caf61-134">親要素</span><span class="sxs-lookup"><span data-stu-id="caf61-134">Parent elements</span></span>

|<span data-ttu-id="caf61-135">**要素**</span><span class="sxs-lookup"><span data-stu-id="caf61-135">**Element**</span></span>|<span data-ttu-id="caf61-136">**説明**</span><span class="sxs-lookup"><span data-stu-id="caf61-136">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="caf61-137">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="caf61-137">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="caf61-138">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="caf61-138">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="caf61-139">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="caf61-139">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="caf61-140">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="caf61-140">Represents a meeting request in the Exchange store</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="caf61-141">備考</span><span class="sxs-lookup"><span data-stu-id="caf61-141">Remarks</span></span>

<span data-ttu-id="caf61-142">この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。</span><span class="sxs-lookup"><span data-stu-id="caf61-142">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="caf61-143">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="caf61-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="caf61-144">要素情報</span><span class="sxs-lookup"><span data-stu-id="caf61-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="caf61-145">名前空間</span><span class="sxs-lookup"><span data-stu-id="caf61-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="caf61-146">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="caf61-146">Schema name</span></span>  <br/> |<span data-ttu-id="caf61-147">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="caf61-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="caf61-148">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="caf61-148">Validation file</span></span>  <br/> |<span data-ttu-id="caf61-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="caf61-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="caf61-150">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="caf61-150">Can be empty</span></span>  <br/> |<span data-ttu-id="caf61-151">False</span><span class="sxs-lookup"><span data-stu-id="caf61-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="caf61-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="caf61-152">See also</span></span>



- [<span data-ttu-id="caf61-153">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="caf61-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: IsRecurring
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsRecurring
api_type:
- schema
ms.assetid: f4df6997-8d5b-4893-a4a5-fc7047e0a9c3
description: IsRecurring 要素では、予定表アイテム、会議出席依頼、またはタスクの定期的なアイテムの一部であるかどうかを示します。 この要素は、読み取り専用です。
ms.openlocfilehash: dfb0c28fe225792c7128409a8cf010627c624fe0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832104"
---
# <a name="isrecurring"></a><span data-ttu-id="96bbb-104">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="96bbb-104">IsRecurring</span></span>

<span data-ttu-id="96bbb-105">**IsRecurring**要素では、予定表アイテム、会議出席依頼、またはタスクの定期的なアイテムの一部であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="96bbb-105">The **IsRecurring** element indicates whether a calendar item, meeting request, or task is part of a recurring item.</span></span> <span data-ttu-id="96bbb-106">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96bbb-106">This element is read-only.</span></span> 
  
```xml
<IsRecurring/>
```

 <span data-ttu-id="96bbb-107">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="96bbb-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96bbb-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="96bbb-108">Attributes and elements</span></span>

<span data-ttu-id="96bbb-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="96bbb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96bbb-110">属性</span><span class="sxs-lookup"><span data-stu-id="96bbb-110">Attributes</span></span>

<span data-ttu-id="96bbb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="96bbb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96bbb-112">子要素</span><span class="sxs-lookup"><span data-stu-id="96bbb-112">Child elements</span></span>

<span data-ttu-id="96bbb-113">なし。</span><span class="sxs-lookup"><span data-stu-id="96bbb-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="96bbb-114">親要素</span><span class="sxs-lookup"><span data-stu-id="96bbb-114">Parent elements</span></span>

|<span data-ttu-id="96bbb-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="96bbb-115">**Element**</span></span>|<span data-ttu-id="96bbb-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="96bbb-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96bbb-117">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="96bbb-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="96bbb-118">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="96bbb-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="96bbb-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="96bbb-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="96bbb-120">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="96bbb-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="96bbb-121">タスク</span><span class="sxs-lookup"><span data-stu-id="96bbb-121">Task</span></span>](task.md) <br/> |<span data-ttu-id="96bbb-122">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="96bbb-122">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="96bbb-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="96bbb-123">Text value</span></span>

<span data-ttu-id="96bbb-124">ブール値を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="96bbb-124">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="96bbb-125">備考</span><span class="sxs-lookup"><span data-stu-id="96bbb-125">Remarks</span></span>

<span data-ttu-id="96bbb-126">次の表は、開催者と出席者と会議出席依頼と更新プログラムの別の予定表アイテムの種類に対して、 **IsRecurring**プロパティを設定する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="96bbb-126">The following table shows how the **IsRecurring** property is set for different calendar item types for organizers and attendees and for meeting requests and updates.</span></span> 
  
|<span data-ttu-id="96bbb-127">**カレンダー項目の種類**</span><span class="sxs-lookup"><span data-stu-id="96bbb-127">**CalendarItem Type**</span></span>|<span data-ttu-id="96bbb-128">**オーガナイザー <br/> (IsRecurring)**</span><span class="sxs-lookup"><span data-stu-id="96bbb-128">**Organizer  <br/> (IsRecurring)**</span></span>|<span data-ttu-id="96bbb-129">**出席者<br/>(IsRecurring)**</span><span class="sxs-lookup"><span data-stu-id="96bbb-129">**Attendee  <br/> (IsRecurring)**</span></span>|<span data-ttu-id="96bbb-130">**会議の更新の要求/ <br/> (IsRecurring)**</span><span class="sxs-lookup"><span data-stu-id="96bbb-130">**Meeting request/update  <br/> (IsRecurring)**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="96bbb-131">1 回</span><span class="sxs-lookup"><span data-stu-id="96bbb-131">Single Occurrence</span></span>  <br/> |<span data-ttu-id="96bbb-132">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="96bbb-132">**FALSE**</span></span> <br/> |<span data-ttu-id="96bbb-133">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="96bbb-133">**FALSE**</span></span> <br/> |<span data-ttu-id="96bbb-134">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="96bbb-134">**FALSE**</span></span> <br/> |
|<span data-ttu-id="96bbb-135">定期的なマスター</span><span class="sxs-lookup"><span data-stu-id="96bbb-135">Recurring Master</span></span>  <br/> |<span data-ttu-id="96bbb-136">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="96bbb-136">**FALSE**</span></span> <br/> |<span data-ttu-id="96bbb-137">**場合は TRUE。**</span><span class="sxs-lookup"><span data-stu-id="96bbb-137">**TRUE**</span></span> <br/> |<span data-ttu-id="96bbb-138">**場合は TRUE。**</span><span class="sxs-lookup"><span data-stu-id="96bbb-138">**TRUE**</span></span> <br/> |
|<span data-ttu-id="96bbb-139">定期的な例外</span><span class="sxs-lookup"><span data-stu-id="96bbb-139">Recurring Exception</span></span>  <br/> |<span data-ttu-id="96bbb-140">**場合は TRUE。**</span><span class="sxs-lookup"><span data-stu-id="96bbb-140">**TRUE**</span></span> <br/> |<span data-ttu-id="96bbb-141">**場合は TRUE。**</span><span class="sxs-lookup"><span data-stu-id="96bbb-141">**TRUE**</span></span> <br/> |<span data-ttu-id="96bbb-142">**場合は TRUE。**</span><span class="sxs-lookup"><span data-stu-id="96bbb-142">**TRUE**</span></span> <br/> |
   
<span data-ttu-id="96bbb-143">開催者の定期的なマスターの予定表のアイテムに設定されている**IsRecurring**プロパティの値が正しくありません。この値を**TRUE**に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="96bbb-143">The **IsRecurring** property value that is set for recurring master calendar items for the organizer is incorrect; this value should be set to **TRUE**.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="96bbb-144">GetUserAvailability 操作では、 [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md)の要素もあります。</span><span class="sxs-lookup"><span data-stu-id="96bbb-144">The GetUserAvailability operation also has an [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) element.</span></span> 
  
<span data-ttu-id="96bbb-145">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="96bbb-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96bbb-146">要素情報</span><span class="sxs-lookup"><span data-stu-id="96bbb-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96bbb-147">名前空間</span><span class="sxs-lookup"><span data-stu-id="96bbb-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="96bbb-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="96bbb-148">Schema name</span></span>  <br/> |<span data-ttu-id="96bbb-149">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="96bbb-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="96bbb-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="96bbb-150">Validation file</span></span>  <br/> |<span data-ttu-id="96bbb-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="96bbb-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="96bbb-152">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="96bbb-152">Can be empty</span></span>  <br/> |<span data-ttu-id="96bbb-153">False</span><span class="sxs-lookup"><span data-stu-id="96bbb-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96bbb-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="96bbb-154">See also</span></span>



[<span data-ttu-id="96bbb-155">TaskType.IsRecurring</span><span class="sxs-lookup"><span data-stu-id="96bbb-155">TaskType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurring.aspx)
  
[<span data-ttu-id="96bbb-156">CalendarEventDetails.IsRecurring</span><span class="sxs-lookup"><span data-stu-id="96bbb-156">CalendarEventDetails.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarEventDetails.IsRecurring.aspx)
  
[<span data-ttu-id="96bbb-157">CalendarItemType.IsRecurring</span><span class="sxs-lookup"><span data-stu-id="96bbb-157">CalendarItemType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurring.aspx)
  
[<span data-ttu-id="96bbb-158">MeetingRequestMessageType.IsRecurring</span><span class="sxs-lookup"><span data-stu-id="96bbb-158">MeetingRequestMessageType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurring.aspx)
  
[<span data-ttu-id="96bbb-159">CalendarItemType.IsRecurringSpecified</span><span class="sxs-lookup"><span data-stu-id="96bbb-159">CalendarItemType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurringSpecified.aspx)
  
[<span data-ttu-id="96bbb-160">MeetingRequestMessageType.IsRecurringSpecified</span><span class="sxs-lookup"><span data-stu-id="96bbb-160">MeetingRequestMessageType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurringSpecified.aspx)
  
[<span data-ttu-id="96bbb-161">TaskType.IsRecurringSpecified</span><span class="sxs-lookup"><span data-stu-id="96bbb-161">TaskType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurringSpecified.aspx)


- [<span data-ttu-id="96bbb-162">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="96bbb-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


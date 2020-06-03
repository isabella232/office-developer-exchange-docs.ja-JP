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
description: IsRecurring 要素は、予定表アイテム、会議出席依頼、またはタスクが定期的なアイテムの一部であるかどうかを示します。 この要素は値の取得のみ可能です。
ms.openlocfilehash: 72c71c1955b69f1c0df855ce4bd0ed02d4c89122
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526488"
---
# <a name="isrecurring"></a><span data-ttu-id="8e79b-104">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="8e79b-104">IsRecurring</span></span>

<span data-ttu-id="8e79b-105">**Isrecurring**要素は、予定表アイテム、会議出席依頼、またはタスクが定期的なアイテムの一部であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8e79b-105">The **IsRecurring** element indicates whether a calendar item, meeting request, or task is part of a recurring item.</span></span> <span data-ttu-id="8e79b-106">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8e79b-106">This element is read-only.</span></span> 
  
```xml
<IsRecurring/>
```

 <span data-ttu-id="8e79b-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="8e79b-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8e79b-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8e79b-108">Attributes and elements</span></span>

<span data-ttu-id="8e79b-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8e79b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e79b-110">属性</span><span class="sxs-lookup"><span data-stu-id="8e79b-110">Attributes</span></span>

<span data-ttu-id="8e79b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8e79b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8e79b-112">子要素</span><span class="sxs-lookup"><span data-stu-id="8e79b-112">Child elements</span></span>

<span data-ttu-id="8e79b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="8e79b-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8e79b-114">親要素</span><span class="sxs-lookup"><span data-stu-id="8e79b-114">Parent elements</span></span>

|<span data-ttu-id="8e79b-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="8e79b-115">**Element**</span></span>|<span data-ttu-id="8e79b-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="8e79b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e79b-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="8e79b-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="8e79b-118">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="8e79b-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8e79b-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="8e79b-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="8e79b-120">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="8e79b-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8e79b-121">タスク</span><span class="sxs-lookup"><span data-stu-id="8e79b-121">Task</span></span>](task.md) <br/> |<span data-ttu-id="8e79b-122">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="8e79b-122">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8e79b-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8e79b-123">Text value</span></span>

<span data-ttu-id="8e79b-124">ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="8e79b-124">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8e79b-125">注釈</span><span class="sxs-lookup"><span data-stu-id="8e79b-125">Remarks</span></span>

<span data-ttu-id="8e79b-126">次の表は、開催者と出席者、および会議出席依頼と更新について、さまざまな予定表アイテムの種類に対して**Isrecurring**プロパティを設定する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="8e79b-126">The following table shows how the **IsRecurring** property is set for different calendar item types for organizers and attendees and for meeting requests and updates.</span></span> 
  
|<span data-ttu-id="8e79b-127">**CalendarItem 型**</span><span class="sxs-lookup"><span data-stu-id="8e79b-127">**CalendarItem Type**</span></span>|<span data-ttu-id="8e79b-128">**開催者 <br/> (isrecurring)**</span><span class="sxs-lookup"><span data-stu-id="8e79b-128">**Organizer  <br/> (IsRecurring)**</span></span>|<span data-ttu-id="8e79b-129">**出席者 <br/> (isrecurring)**</span><span class="sxs-lookup"><span data-stu-id="8e79b-129">**Attendee  <br/> (IsRecurring)**</span></span>|<span data-ttu-id="8e79b-130">**会議出席依頼/更新 <br/> (isrecurring)**</span><span class="sxs-lookup"><span data-stu-id="8e79b-130">**Meeting request/update  <br/> (IsRecurring)**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="8e79b-131">単一の発生</span><span class="sxs-lookup"><span data-stu-id="8e79b-131">Single Occurrence</span></span>  <br/> |<span data-ttu-id="8e79b-132">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="8e79b-132">**FALSE**</span></span> <br/> |<span data-ttu-id="8e79b-133">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="8e79b-133">**FALSE**</span></span> <br/> |<span data-ttu-id="8e79b-134">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="8e79b-134">**FALSE**</span></span> <br/> |
|<span data-ttu-id="8e79b-135">定期的なマスター</span><span class="sxs-lookup"><span data-stu-id="8e79b-135">Recurring Master</span></span>  <br/> |<span data-ttu-id="8e79b-136">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="8e79b-136">**FALSE**</span></span> <br/> |<span data-ttu-id="8e79b-137">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="8e79b-137">**TRUE**</span></span> <br/> |<span data-ttu-id="8e79b-138">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="8e79b-138">**TRUE**</span></span> <br/> |
|<span data-ttu-id="8e79b-139">定期的な例外</span><span class="sxs-lookup"><span data-stu-id="8e79b-139">Recurring Exception</span></span>  <br/> |<span data-ttu-id="8e79b-140">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="8e79b-140">**TRUE**</span></span> <br/> |<span data-ttu-id="8e79b-141">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="8e79b-141">**TRUE**</span></span> <br/> |<span data-ttu-id="8e79b-142">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="8e79b-142">**TRUE**</span></span> <br/> |
   
<span data-ttu-id="8e79b-143">開催者の定期的なマスター予定表アイテムに対して設定されている**Isrecurring**なプロパティの値が正しくありません。この値は**TRUE**に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8e79b-143">The **IsRecurring** property value that is set for recurring master calendar items for the organizer is incorrect; this value should be set to **TRUE**.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="8e79b-144">GetUserAvailability 操作には、 [Isrecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md)要素もあります。</span><span class="sxs-lookup"><span data-stu-id="8e79b-144">The GetUserAvailability operation also has an [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) element.</span></span> 
  
<span data-ttu-id="8e79b-145">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="8e79b-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e79b-146">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8e79b-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e79b-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="8e79b-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8e79b-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8e79b-148">Schema name</span></span>  <br/> |<span data-ttu-id="8e79b-149">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8e79b-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="8e79b-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8e79b-150">Validation file</span></span>  <br/> |<span data-ttu-id="8e79b-151">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8e79b-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8e79b-152">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8e79b-152">Can be empty</span></span>  <br/> |<span data-ttu-id="8e79b-153">正しくない</span><span class="sxs-lookup"><span data-stu-id="8e79b-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8e79b-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="8e79b-154">See also</span></span>



[<span data-ttu-id="8e79b-155">TaskType IsRecurring</span><span class="sxs-lookup"><span data-stu-id="8e79b-155">TaskType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurring.aspx)
  
[<span data-ttu-id="8e79b-156">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="8e79b-156">CalendarEventDetails.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarEventDetails.IsRecurring.aspx)
  
[<span data-ttu-id="8e79b-157">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="8e79b-157">CalendarItemType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurring.aspx)
  
[<span data-ttu-id="8e79b-158">会議の要求の Messagetype。 IsRecurring</span><span class="sxs-lookup"><span data-stu-id="8e79b-158">MeetingRequestMessageType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurring.aspx)
  
[<span data-ttu-id="8e79b-159">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="8e79b-159">CalendarItemType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurringSpecified.aspx)
  
[<span data-ttu-id="8e79b-160">会議の IsRecurringSpecified</span><span class="sxs-lookup"><span data-stu-id="8e79b-160">MeetingRequestMessageType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurringSpecified.aspx)
  
[<span data-ttu-id="8e79b-161">IsRecurringSpecified</span><span class="sxs-lookup"><span data-stu-id="8e79b-161">TaskType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurringSpecified.aspx)


- [<span data-ttu-id="8e79b-162">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8e79b-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


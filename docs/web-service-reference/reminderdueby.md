---
title: ReminderDueBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReminderDueBy
api_type:
- schema
ms.assetid: e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f
description: ReminderDueBy 要素は、イベントが発生した日付と時刻を表します。 これは、アラームがいつ表示されるかを決定するために ReminderMinutesBeforeStart 要素によって使用されます。
ms.openlocfilehash: 206534da4498e871e99635b236e500dec573eb5a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528728"
---
# <a name="reminderdueby"></a><span data-ttu-id="a8f24-104">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="a8f24-104">ReminderDueBy</span></span>

<span data-ttu-id="a8f24-105">**ReminderDueBy**要素は、イベントが発生した日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="a8f24-105">The **ReminderDueBy** element represents the date and time when the event occurs.</span></span> <span data-ttu-id="a8f24-106">これは、アラームがいつ表示されるかを決定するために[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="a8f24-106">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span> 
  
```xml
<ReminderDueBy/>
```

 <span data-ttu-id="a8f24-107">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="a8f24-107">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8f24-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a8f24-108">Attributes and elements</span></span>

<span data-ttu-id="a8f24-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a8f24-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8f24-110">属性</span><span class="sxs-lookup"><span data-stu-id="a8f24-110">Attributes</span></span>

<span data-ttu-id="a8f24-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a8f24-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8f24-112">子要素</span><span class="sxs-lookup"><span data-stu-id="a8f24-112">Child elements</span></span>

<span data-ttu-id="a8f24-113">なし。</span><span class="sxs-lookup"><span data-stu-id="a8f24-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a8f24-114">親要素</span><span class="sxs-lookup"><span data-stu-id="a8f24-114">Parent elements</span></span>

|<span data-ttu-id="a8f24-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="a8f24-115">**Element**</span></span>|<span data-ttu-id="a8f24-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="a8f24-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8f24-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="a8f24-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="a8f24-118">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="a8f24-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="a8f24-119">Contact</span><span class="sxs-lookup"><span data-stu-id="a8f24-119">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="a8f24-120">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="a8f24-120">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="a8f24-121">DistributionList</span><span class="sxs-lookup"><span data-stu-id="a8f24-121">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="a8f24-122">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="a8f24-122">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="a8f24-123">Item</span><span class="sxs-lookup"><span data-stu-id="a8f24-123">Item</span></span>](item.md) <br/> |<span data-ttu-id="a8f24-124">Exchange ストア内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="a8f24-124">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a8f24-125">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="a8f24-125">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="a8f24-126">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="a8f24-126">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a8f24-127">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="a8f24-127">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="a8f24-128">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="a8f24-128">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a8f24-129">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="a8f24-129">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a8f24-130">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="a8f24-130">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a8f24-131">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="a8f24-131">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="a8f24-132">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="a8f24-132">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a8f24-133">Message</span><span class="sxs-lookup"><span data-stu-id="a8f24-133">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a8f24-134">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="a8f24-134">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="a8f24-135">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="a8f24-135">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="a8f24-136">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="a8f24-136">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a8f24-137">タスク</span><span class="sxs-lookup"><span data-stu-id="a8f24-137">Task</span></span>](task.md) <br/> |<span data-ttu-id="a8f24-138">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="a8f24-138">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a8f24-139">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a8f24-139">Text value</span></span>

<span data-ttu-id="a8f24-140">Text 値は、アラームの期限の日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="a8f24-140">The text value represents the date and time when a reminder is due.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a8f24-141">注釈</span><span class="sxs-lookup"><span data-stu-id="a8f24-141">Remarks</span></span>

<span data-ttu-id="a8f24-142">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a8f24-142">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8f24-143">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a8f24-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8f24-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="a8f24-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8f24-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a8f24-145">Schema Name</span></span>  <br/> |<span data-ttu-id="a8f24-146">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a8f24-146">Types schema</span></span>  <br/> |
|<span data-ttu-id="a8f24-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a8f24-147">Validation File</span></span>  <br/> |<span data-ttu-id="a8f24-148">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a8f24-148">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8f24-149">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a8f24-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8f24-150">正しくない</span><span class="sxs-lookup"><span data-stu-id="a8f24-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8f24-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="a8f24-151">See also</span></span>



- [<span data-ttu-id="a8f24-152">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a8f24-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


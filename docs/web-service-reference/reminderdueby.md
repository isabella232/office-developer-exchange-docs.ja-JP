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
description: ReminderDueBy 要素は、イベントが発生したときの日時を表します。 ReminderMinutesBeforeStart 要素によってアラームが表示されたときを決定する使用されます。
ms.openlocfilehash: cff8142958108635dd9dfaec425af135dee2f2eb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833061"
---
# <a name="reminderdueby"></a><span data-ttu-id="95405-104">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="95405-104">ReminderDueBy</span></span>

<span data-ttu-id="95405-105">**ReminderDueBy**要素は、イベントが発生したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="95405-105">The **ReminderDueBy** element represents the date and time when the event occurs.</span></span> <span data-ttu-id="95405-106">[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によってアラームが表示されたときを決定する使用されます。</span><span class="sxs-lookup"><span data-stu-id="95405-106">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span> 
  
```xml
<ReminderDueBy/>
```

 <span data-ttu-id="95405-107">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="95405-107">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95405-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="95405-108">Attributes and elements</span></span>

<span data-ttu-id="95405-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="95405-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95405-110">属性</span><span class="sxs-lookup"><span data-stu-id="95405-110">Attributes</span></span>

<span data-ttu-id="95405-111">なし。</span><span class="sxs-lookup"><span data-stu-id="95405-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="95405-112">子要素</span><span class="sxs-lookup"><span data-stu-id="95405-112">Child elements</span></span>

<span data-ttu-id="95405-113">なし。</span><span class="sxs-lookup"><span data-stu-id="95405-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="95405-114">親要素</span><span class="sxs-lookup"><span data-stu-id="95405-114">Parent elements</span></span>

|<span data-ttu-id="95405-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="95405-115">**Element**</span></span>|<span data-ttu-id="95405-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="95405-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95405-117">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="95405-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="95405-118">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="95405-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="95405-119">Contact</span><span class="sxs-lookup"><span data-stu-id="95405-119">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="95405-120">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="95405-120">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="95405-121">DistributionList</span><span class="sxs-lookup"><span data-stu-id="95405-121">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="95405-122">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="95405-122">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="95405-123">アイテム</span><span class="sxs-lookup"><span data-stu-id="95405-123">Item</span></span>](item.md) <br/> |<span data-ttu-id="95405-124">Exchange ストア内の項目を表します。</span><span class="sxs-lookup"><span data-stu-id="95405-124">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="95405-125">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="95405-125">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="95405-126">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="95405-126">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="95405-127">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="95405-127">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="95405-128">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="95405-128">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="95405-129">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="95405-129">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="95405-130">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="95405-130">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="95405-131">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="95405-131">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="95405-132">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="95405-132">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="95405-133">Message</span><span class="sxs-lookup"><span data-stu-id="95405-133">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="95405-134">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="95405-134">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="95405-135">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="95405-135">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="95405-136">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="95405-136">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="95405-137">タスク</span><span class="sxs-lookup"><span data-stu-id="95405-137">Task</span></span>](task.md) <br/> |<span data-ttu-id="95405-138">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="95405-138">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="95405-139">テキスト値</span><span class="sxs-lookup"><span data-stu-id="95405-139">Text value</span></span>

<span data-ttu-id="95405-140">テキスト値は、日付とアラームは予定時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="95405-140">The text value represents the date and time when a reminder is due.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="95405-141">備考</span><span class="sxs-lookup"><span data-stu-id="95405-141">Remarks</span></span>

<span data-ttu-id="95405-142">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="95405-142">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95405-143">要素情報</span><span class="sxs-lookup"><span data-stu-id="95405-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95405-144">名前空間</span><span class="sxs-lookup"><span data-stu-id="95405-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="95405-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="95405-145">Schema Name</span></span>  <br/> |<span data-ttu-id="95405-146">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="95405-146">Types schema</span></span>  <br/> |
|<span data-ttu-id="95405-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="95405-147">Validation File</span></span>  <br/> |<span data-ttu-id="95405-148">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="95405-148">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="95405-149">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="95405-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="95405-150">False</span><span class="sxs-lookup"><span data-stu-id="95405-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="95405-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="95405-151">See also</span></span>



- [<span data-ttu-id="95405-152">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="95405-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: 通知
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Notification
api_type:
- schema
ms.assetid: c9070936-0930-438e-839c-91127256a6c8
description: 通知の要素には、サブスクリプション、および最後の通知以降に発生したイベントに関する情報が含まれています。
ms.openlocfilehash: a769d8988eb68d0fa0b02f3838cd891e714571b6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832547"
---
# <a name="notification"></a><span data-ttu-id="fb1ec-103">通知</span><span class="sxs-lookup"><span data-stu-id="fb1ec-103">Notification</span></span>

<span data-ttu-id="fb1ec-104">**通知**の要素には、サブスクリプション、および最後の通知以降に発生したイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-104">The **Notification** element contains information about the subscription and the events that have occurred since the last notification.</span></span> 
  
```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <CopiedEvent/>
</Notification>
```

 <span data-ttu-id="fb1ec-105">**NotificationType**</span><span class="sxs-lookup"><span data-stu-id="fb1ec-105">**NotificationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb1ec-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fb1ec-106">Attributes and elements</span></span>

<span data-ttu-id="fb1ec-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb1ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="fb1ec-108">Attributes</span></span>

<span data-ttu-id="fb1ec-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb1ec-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fb1ec-110">Child elements</span></span>

|<span data-ttu-id="fb1ec-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="fb1ec-111">**Element**</span></span>|<span data-ttu-id="fb1ec-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb1ec-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb1ec-113">サブスクリプション Id (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="fb1ec-113">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="fb1ec-114">サブスクリプションの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-114">Represents the identifier for a subscription.</span></span>  <br/> |
|[<span data-ttu-id="fb1ec-115">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="fb1ec-115">PreviousWatermark</span></span>](previouswatermark.md) <br/> |<span data-ttu-id="fb1ec-116">サブスクリプションでクライアントに正常に通信された最新イベントのウォーターマークを表します。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-116">Represents the watermark of the latest event that was successfully communicated to the client for the subscription.</span></span>  <br/> |
|[<span data-ttu-id="fb1ec-117">イベント</span><span class="sxs-lookup"><span data-stu-id="fb1ec-117">MoreEvents</span></span>](moreevents.md) <br/> |<span data-ttu-id="fb1ec-118">クライアントに配信するキューにその他のイベントがあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-118">Indicates whether there are more events in the queue to be delivered to the client.</span></span>  <br/> |
|[<span data-ttu-id="fb1ec-119">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="fb1ec-119">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="fb1ec-120">アイテムまたはフォルダーのコピー先のイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-120">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="fb1ec-121">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="fb1ec-121">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="fb1ec-122">アイテムまたはフォルダーが作成されているイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-122">Represents an event in which an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="fb1ec-123">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="fb1ec-123">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="fb1ec-124">アイテムまたはフォルダーが削除されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-124">Represents an event in which an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="fb1ec-125">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="fb1ec-125">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="fb1ec-126">アイテムまたはフォルダーが変更されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-126">Represents an event in which an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="fb1ec-127">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="fb1ec-127">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="fb1ec-128">アイテムまたはフォルダーが 1 つの親フォルダー間で移動して別の親フォルダー イベントを表します。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-128">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="fb1ec-129">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="fb1ec-129">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="fb1ec-130">メールボックス内の新しいメール アイテムによって発生するイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-130">Represents an event that is triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="fb1ec-131">StatusEvent</span><span class="sxs-lookup"><span data-stu-id="fb1ec-131">StatusEvent</span></span>](statusevent.md) <br/> |<span data-ttu-id="fb1ec-132">通知メールボックスに新しいアクティビティが発生していないことを表します。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-132">Represents a notification that no new activity has occurred in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="fb1ec-133">FreeBusyChangedEvent</span><span class="sxs-lookup"><span data-stu-id="fb1ec-133">FreeBusyChangedEvent</span></span>](freebusychangedevent.md) <br/> |<span data-ttu-id="fb1ec-134">アイテムの空き時間情報が変更されたイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-134">Represents an event in which an item's free/busy time has changed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fb1ec-135">親要素</span><span class="sxs-lookup"><span data-stu-id="fb1ec-135">Parent elements</span></span>

|<span data-ttu-id="fb1ec-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="fb1ec-136">**Element**</span></span>|<span data-ttu-id="fb1ec-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb1ec-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb1ec-138">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fb1ec-138">GetEventsResponseMessage</span></span>](geteventsresponsemessage.md) <br/> |<span data-ttu-id="fb1ec-139">状態および 1 つの GetEvents 要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-139">Contains the status and result of a single GetEvents request.</span></span>  <br/> |
|[<span data-ttu-id="fb1ec-140">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fb1ec-140">SendNotificationResponseMessage</span></span>](sendnotificationresponsemessage.md) <br/> |<span data-ttu-id="fb1ec-141">状態および 1 つの SendNotification 要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-141">Contains the status and result of a single SendNotification request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fb1ec-142">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fb1ec-142">Text value</span></span>

<span data-ttu-id="fb1ec-143">なし。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fb1ec-144">備考</span><span class="sxs-lookup"><span data-stu-id="fb1ec-144">Remarks</span></span>

<span data-ttu-id="fb1ec-145">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fb1ec-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb1ec-146">要素情報</span><span class="sxs-lookup"><span data-stu-id="fb1ec-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb1ec-147">名前空間</span><span class="sxs-lookup"><span data-stu-id="fb1ec-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fb1ec-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fb1ec-148">Schema Name</span></span>  <br/> |<span data-ttu-id="fb1ec-149">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="fb1ec-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="fb1ec-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fb1ec-150">Validation File</span></span>  <br/> |<span data-ttu-id="fb1ec-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fb1ec-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fb1ec-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fb1ec-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="fb1ec-153">False</span><span class="sxs-lookup"><span data-stu-id="fb1ec-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb1ec-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="fb1ec-154">See also</span></span>



[<span data-ttu-id="fb1ec-155">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="fb1ec-155">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="fb1ec-156">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="fb1ec-156">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="fb1ec-157">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="fb1ec-157">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="fb1ec-158">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="fb1ec-158">Unsubscribe operation</span></span>](unsubscribe-operation.md)


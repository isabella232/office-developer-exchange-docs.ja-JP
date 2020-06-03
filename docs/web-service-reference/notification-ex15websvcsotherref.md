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
description: Notification 要素には、サブスクリプションに関する情報と、最後の通知以降に発生したイベントが含まれます。
ms.openlocfilehash: c4a5206c14985ec46cf40162a9ce4eaec68242ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530388"
---
# <a name="notification"></a><span data-ttu-id="9256c-103">通知</span><span class="sxs-lookup"><span data-stu-id="9256c-103">Notification</span></span>

<span data-ttu-id="9256c-104">**Notification**要素には、サブスクリプションに関する情報と、最後の通知以降に発生したイベントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="9256c-104">The **Notification** element contains information about the subscription and the events that have occurred since the last notification.</span></span> 
  
```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <CopiedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <CreatedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <DeletedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <ModifiedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <MovedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <NewMailEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <StatusEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <FreeBusyChangedEvent/>
</Notification>
```

<span data-ttu-id="9256c-105">**NotificationType**</span><span class="sxs-lookup"><span data-stu-id="9256c-105">**NotificationType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9256c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9256c-106">Attributes and elements</span></span>

<span data-ttu-id="9256c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9256c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9256c-108">属性</span><span class="sxs-lookup"><span data-stu-id="9256c-108">Attributes</span></span>

<span data-ttu-id="9256c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9256c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9256c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9256c-110">Child elements</span></span>

|<span data-ttu-id="9256c-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="9256c-111">**Element**</span></span>|<span data-ttu-id="9256c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9256c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9256c-113">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="9256c-113">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="9256c-114">サブスクリプションの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="9256c-114">Represents the identifier for a subscription.</span></span>  <br/> |
|[<span data-ttu-id="9256c-115">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="9256c-115">PreviousWatermark</span></span>](previouswatermark.md) <br/> |<span data-ttu-id="9256c-116">サブスクリプションのためにクライアントに正常に伝達された最新のイベントのウォーターマークを表します。</span><span class="sxs-lookup"><span data-stu-id="9256c-116">Represents the watermark of the latest event that was successfully communicated to the client for the subscription.</span></span>  <br/> |
|[<span data-ttu-id="9256c-117">その他のイベント</span><span class="sxs-lookup"><span data-stu-id="9256c-117">MoreEvents</span></span>](moreevents.md) <br/> |<span data-ttu-id="9256c-118">クライアントに配信されるキューに、さらにイベントがあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9256c-118">Indicates whether there are more events in the queue to be delivered to the client.</span></span>  <br/> |
|[<span data-ttu-id="9256c-119">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="9256c-119">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="9256c-120">アイテムまたはフォルダーがコピーされるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="9256c-120">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="9256c-121">対する createdevent</span><span class="sxs-lookup"><span data-stu-id="9256c-121">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="9256c-122">アイテムまたはフォルダーが作成されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="9256c-122">Represents an event in which an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="9256c-123">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="9256c-123">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="9256c-124">アイテムまたはフォルダーが削除されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="9256c-124">Represents an event in which an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="9256c-125">対する modifiedevent</span><span class="sxs-lookup"><span data-stu-id="9256c-125">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="9256c-126">アイテムまたはフォルダーが変更されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="9256c-126">Represents an event in which an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="9256c-127">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="9256c-127">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="9256c-128">ある親フォルダーから別の親フォルダーにアイテムまたはフォルダーを移動するイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="9256c-128">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="9256c-129">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="9256c-129">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="9256c-130">メールボックス内の新しいメールアイテムによってトリガーされるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="9256c-130">Represents an event that is triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9256c-131">StatusEvent</span><span class="sxs-lookup"><span data-stu-id="9256c-131">StatusEvent</span></span>](statusevent.md) <br/> |<span data-ttu-id="9256c-132">メールボックス内で新しいアクティビティが発生していないことを示す通知を表します。</span><span class="sxs-lookup"><span data-stu-id="9256c-132">Represents a notification that no new activity has occurred in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9256c-133">FreeBusyChangedEvent</span><span class="sxs-lookup"><span data-stu-id="9256c-133">FreeBusyChangedEvent</span></span>](freebusychangedevent.md) <br/> |<span data-ttu-id="9256c-134">アイテムの空き時間情報が変更されたイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="9256c-134">Represents an event in which an item's free/busy time has changed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9256c-135">親要素</span><span class="sxs-lookup"><span data-stu-id="9256c-135">Parent elements</span></span>

|<span data-ttu-id="9256c-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="9256c-136">**Element**</span></span>|<span data-ttu-id="9256c-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="9256c-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9256c-138">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9256c-138">GetEventsResponseMessage</span></span>](geteventsresponsemessage.md) <br/> |<span data-ttu-id="9256c-139">単一の GetEvents 要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="9256c-139">Contains the status and result of a single GetEvents request.</span></span>  <br/> |
|[<span data-ttu-id="9256c-140">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9256c-140">SendNotificationResponseMessage</span></span>](sendnotificationresponsemessage.md) <br/> |<span data-ttu-id="9256c-141">1回の SendNotification 要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="9256c-141">Contains the status and result of a single SendNotification request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9256c-142">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9256c-142">Text value</span></span>

<span data-ttu-id="9256c-143">なし。</span><span class="sxs-lookup"><span data-stu-id="9256c-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9256c-144">注釈</span><span class="sxs-lookup"><span data-stu-id="9256c-144">Remarks</span></span>

<span data-ttu-id="9256c-145">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9256c-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9256c-146">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9256c-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9256c-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="9256c-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9256c-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9256c-148">Schema Name</span></span>  <br/> |<span data-ttu-id="9256c-149">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9256c-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="9256c-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9256c-150">Validation File</span></span>  <br/> |<span data-ttu-id="9256c-151">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9256c-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9256c-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9256c-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="9256c-153">正しくない</span><span class="sxs-lookup"><span data-stu-id="9256c-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9256c-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="9256c-154">See also</span></span>

- [<span data-ttu-id="9256c-155">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="9256c-155">Subscribe operation</span></span>](subscribe-operation.md) 
- [<span data-ttu-id="9256c-156">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="9256c-156">GetEvents operation</span></span>](getevents-operation.md) 
- [<span data-ttu-id="9256c-157">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="9256c-157">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md) 
- [<span data-ttu-id="9256c-158">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="9256c-158">Unsubscribe operation</span></span>](unsubscribe-operation.md)


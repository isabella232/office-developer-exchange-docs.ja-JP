---
title: StatusEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StatusEvent
api_type:
- schema
ms.assetid: d3901818-2640-4bed-aad8-21a61aee62a1
description: StatusEvent 要素は、メールボックスに新しいアクティビティが発生していないことの通知を表します。
ms.openlocfilehash: e214918f9795e9e29061d4aac72ab144d2b24267
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833592"
---
# <a name="statusevent"></a><span data-ttu-id="bb5d3-103">StatusEvent</span><span class="sxs-lookup"><span data-stu-id="bb5d3-103">StatusEvent</span></span>

<span data-ttu-id="bb5d3-104">**StatusEvent**要素は、メールボックスに新しいアクティビティが発生していないことの通知を表します。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-104">The **StatusEvent** element represents a notification that no new activity has occurred in the mailbox.</span></span> 
  
```xml
<StatusEvent>
   <Watermark/>
</StatusEvent>
```

 <span data-ttu-id="bb5d3-105">**BaseNotificationEventType**</span><span class="sxs-lookup"><span data-stu-id="bb5d3-105">**BaseNotificationEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb5d3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bb5d3-106">Attributes and elements</span></span>

<span data-ttu-id="bb5d3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb5d3-108">属性</span><span class="sxs-lookup"><span data-stu-id="bb5d3-108">Attributes</span></span>

<span data-ttu-id="bb5d3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bb5d3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bb5d3-110">Child elements</span></span>

|<span data-ttu-id="bb5d3-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="bb5d3-111">**Element**</span></span>|<span data-ttu-id="bb5d3-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="bb5d3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb5d3-113">透かし</span><span class="sxs-lookup"><span data-stu-id="bb5d3-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="bb5d3-114">サブスクリプションの有効な最新のウォーターマークを表します。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-114">Represents the last valid watermark for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bb5d3-115">親要素</span><span class="sxs-lookup"><span data-stu-id="bb5d3-115">Parent elements</span></span>

|<span data-ttu-id="bb5d3-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="bb5d3-116">**Element**</span></span>|<span data-ttu-id="bb5d3-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="bb5d3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb5d3-118">通知</span><span class="sxs-lookup"><span data-stu-id="bb5d3-118">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="bb5d3-119">サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-119">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bb5d3-120">備考</span><span class="sxs-lookup"><span data-stu-id="bb5d3-120">Remarks</span></span>

<span data-ttu-id="bb5d3-121">**StatusEvent**要素は次の理由の 1 つの通知で返されます。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-121">The **StatusEvent** element is returned in a notification for one of the following reasons:</span></span> 
  
- <span data-ttu-id="bb5d3-122">プル クライアントでは、アクティビティがサブスクリプションの GetEvents 要求を発行しません。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-122">A pull client issues a GetEvents request on a subscription that has no activity.</span></span>
    
- <span data-ttu-id="bb5d3-123">プッシュ クライアント イベントがありません。 キュー内の[StatusFrequency](statusfrequency.md)に到達したとき。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-123">A push client has no events in the queue when the [StatusFrequency](statusfrequency.md) has been reached.</span></span> 
    
<span data-ttu-id="bb5d3-124">**StatusEvent**[ウォーターマーク](watermark.md)は、他のイベントの種類のウォーターマークと同じ方法でクライアント アプリケーションによって使用されます。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-124">The **StatusEvent**[Watermark](watermark.md) is used by a client application in the same manner as the other event type watermarks.</span></span> <span data-ttu-id="bb5d3-125">ただし、 **StatusEvent**のウォーターマークは他のイベントに使用されるウォーターマークと同じです。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-125">However, the watermark for the **StatusEvent** is not the same as the watermarks used for other events.</span></span> <span data-ttu-id="bb5d3-126">などの透かし 1 を使用してイベントをサブスクリプションには、2 と 3 とこれらのイベント通知されていること正常に通知します。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-126">For example, a subscription has events with watermarks 1, 2, and 3 and those events have been successfully communicated in a notification.</span></span> <span data-ttu-id="bb5d3-127">一定の期間が発生し、 **GetEvents**要求が送信されます。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-127">A period of inactivity occurs and a **GetEvents** request is sent.</span></span> <span data-ttu-id="bb5d3-128">クライアント アクセス サーバー (CAS) は、状態イベントを返し、 [PreviousWatermark](previouswatermark.md)と現在の[透かし](watermark.md)の両方として、3、最新のウォーターマークが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-128">The Client Access server (CAS) returns a status event and includes the last watermark, 3, as both the [PreviousWatermark](previouswatermark.md) and the current [Watermark](watermark.md).</span></span>
  
<span data-ttu-id="bb5d3-129">透かしのすべてのケースで同じままになりません。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-129">The watermark will not remain the same in all cases.</span></span> <span data-ttu-id="bb5d3-130">イベント エントリは、30 日間保持されます。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-130">Event entries are maintained for 30 days.</span></span> <span data-ttu-id="bb5d3-131">アクティブなサブスクリプションを維持するために、CA は、サブスクリプションのキューの透かしを定期的に更新します。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-131">To maintain an active subscription, the CAS periodically updates the watermarks for subscription queues.</span></span> <span data-ttu-id="bb5d3-132">最新のウォーターマークは、アクティブなサブスクリプションを維持するために、クライアントに送信されます。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-132">The updated watermarks are sent to clients to maintain an active subscription.</span></span>
  
<span data-ttu-id="bb5d3-133">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb5d3-134">要素情報</span><span class="sxs-lookup"><span data-stu-id="bb5d3-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb5d3-135">名前空間</span><span class="sxs-lookup"><span data-stu-id="bb5d3-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bb5d3-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bb5d3-136">Schema name</span></span>  <br/> |<span data-ttu-id="bb5d3-137">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="bb5d3-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="bb5d3-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bb5d3-138">Validation file</span></span>  <br/> |<span data-ttu-id="bb5d3-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bb5d3-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bb5d3-140">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="bb5d3-140">Can be empty</span></span>  <br/> |<span data-ttu-id="bb5d3-141">False</span><span class="sxs-lookup"><span data-stu-id="bb5d3-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bb5d3-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="bb5d3-142">See also</span></span>



[<span data-ttu-id="bb5d3-143">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="bb5d3-143">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="bb5d3-144">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="bb5d3-144">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="bb5d3-145">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="bb5d3-145">Unsubscribe operation</span></span>](unsubscribe-operation.md)


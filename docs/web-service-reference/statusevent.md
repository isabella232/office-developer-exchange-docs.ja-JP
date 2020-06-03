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
description: StatusEvent 要素は、メールボックス内で新しいアクティビティが発生していないことを示す通知を表します。
ms.openlocfilehash: 8158a47937a810be2ea22346384b4e61da56ac48
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468258"
---
# <a name="statusevent"></a><span data-ttu-id="e43eb-103">StatusEvent</span><span class="sxs-lookup"><span data-stu-id="e43eb-103">StatusEvent</span></span>

<span data-ttu-id="e43eb-104">**Statusevent**要素は、メールボックス内で新しいアクティビティが発生していないことを示す通知を表します。</span><span class="sxs-lookup"><span data-stu-id="e43eb-104">The **StatusEvent** element represents a notification that no new activity has occurred in the mailbox.</span></span> 
  
```xml
<StatusEvent>
   <Watermark/>
</StatusEvent>
```

 <span data-ttu-id="e43eb-105">**BaseNotificationEventType**</span><span class="sxs-lookup"><span data-stu-id="e43eb-105">**BaseNotificationEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e43eb-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e43eb-106">Attributes and elements</span></span>

<span data-ttu-id="e43eb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e43eb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e43eb-108">属性</span><span class="sxs-lookup"><span data-stu-id="e43eb-108">Attributes</span></span>

<span data-ttu-id="e43eb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e43eb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e43eb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e43eb-110">Child elements</span></span>

|<span data-ttu-id="e43eb-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="e43eb-111">**Element**</span></span>|<span data-ttu-id="e43eb-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e43eb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e43eb-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="e43eb-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="e43eb-114">サブスクリプションの最後の有効なウォーターマークを表します。</span><span class="sxs-lookup"><span data-stu-id="e43eb-114">Represents the last valid watermark for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e43eb-115">親要素</span><span class="sxs-lookup"><span data-stu-id="e43eb-115">Parent elements</span></span>

|<span data-ttu-id="e43eb-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="e43eb-116">**Element**</span></span>|<span data-ttu-id="e43eb-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="e43eb-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e43eb-118">通知</span><span class="sxs-lookup"><span data-stu-id="e43eb-118">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e43eb-119">サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e43eb-119">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e43eb-120">注釈</span><span class="sxs-lookup"><span data-stu-id="e43eb-120">Remarks</span></span>

<span data-ttu-id="e43eb-121">**Statusevent**要素は、次のいずれかの理由で通知で返されます。</span><span class="sxs-lookup"><span data-stu-id="e43eb-121">The **StatusEvent** element is returned in a notification for one of the following reasons:</span></span> 
  
- <span data-ttu-id="e43eb-122">プルクライアントが、アクティビティのないサブスクリプションに対して GetEvents 要求を発行します。</span><span class="sxs-lookup"><span data-stu-id="e43eb-122">A pull client issues a GetEvents request on a subscription that has no activity.</span></span>
    
- <span data-ttu-id="e43eb-123">[Statusfrequency](statusfrequency.md)に達した場合、プッシュクライアントにはキューにイベントがありません。</span><span class="sxs-lookup"><span data-stu-id="e43eb-123">A push client has no events in the queue when the [StatusFrequency](statusfrequency.md) has been reached.</span></span> 
    
<span data-ttu-id="e43eb-124">**Statusevent**[ウォーターマーク](watermark.md)は、クライアントアプリケーションによって、他のイベントの種類のウォーターマークと同じ方法で使用されます。</span><span class="sxs-lookup"><span data-stu-id="e43eb-124">The **StatusEvent**[Watermark](watermark.md) is used by a client application in the same manner as the other event type watermarks.</span></span> <span data-ttu-id="e43eb-125">ただし、 **Statusevent**のウォーターマークは、他のイベントで使用されるウォーターマークとは異なります。</span><span class="sxs-lookup"><span data-stu-id="e43eb-125">However, the watermark for the **StatusEvent** is not the same as the watermarks used for other events.</span></span> <span data-ttu-id="e43eb-126">たとえば、サブスクリプションにはウォーターマーク1、2、および3のイベントがあり、それらのイベントは通知で正常に伝達されています。</span><span class="sxs-lookup"><span data-stu-id="e43eb-126">For example, a subscription has events with watermarks 1, 2, and 3 and those events have been successfully communicated in a notification.</span></span> <span data-ttu-id="e43eb-127">非アクティブな期間が発生し、 **GetEvents**要求が送信されます。</span><span class="sxs-lookup"><span data-stu-id="e43eb-127">A period of inactivity occurs and a **GetEvents** request is sent.</span></span> <span data-ttu-id="e43eb-128">クライアントアクセスサーバー (CAS) は状態イベントを返し、最後のウォーターマーク3を[PreviousWatermark](previouswatermark.md)と現在の[ウォーターマーク](watermark.md)の両方として含みます。</span><span class="sxs-lookup"><span data-stu-id="e43eb-128">The Client Access server (CAS) returns a status event and includes the last watermark, 3, as both the [PreviousWatermark](previouswatermark.md) and the current [Watermark](watermark.md).</span></span>
  
<span data-ttu-id="e43eb-129">ウォーターマークは、すべての場合に変わりません。</span><span class="sxs-lookup"><span data-stu-id="e43eb-129">The watermark will not remain the same in all cases.</span></span> <span data-ttu-id="e43eb-130">イベントエントリは、30日間保持されます。</span><span class="sxs-lookup"><span data-stu-id="e43eb-130">Event entries are maintained for 30 days.</span></span> <span data-ttu-id="e43eb-131">アクティブなサブスクリプションを維持するために、CAS はサブスクリプションキューのウォーターマークを定期的に更新します。</span><span class="sxs-lookup"><span data-stu-id="e43eb-131">To maintain an active subscription, the CAS periodically updates the watermarks for subscription queues.</span></span> <span data-ttu-id="e43eb-132">更新されたウォーターマークは、アクティブなサブスクリプションを維持するためにクライアントに送信されます。</span><span class="sxs-lookup"><span data-stu-id="e43eb-132">The updated watermarks are sent to clients to maintain an active subscription.</span></span>
  
<span data-ttu-id="e43eb-133">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e43eb-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e43eb-134">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e43eb-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e43eb-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="e43eb-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e43eb-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e43eb-136">Schema name</span></span>  <br/> |<span data-ttu-id="e43eb-137">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e43eb-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="e43eb-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e43eb-138">Validation file</span></span>  <br/> |<span data-ttu-id="e43eb-139">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e43eb-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e43eb-140">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e43eb-140">Can be empty</span></span>  <br/> |<span data-ttu-id="e43eb-141">正しくない</span><span class="sxs-lookup"><span data-stu-id="e43eb-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e43eb-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="e43eb-142">See also</span></span>



[<span data-ttu-id="e43eb-143">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="e43eb-143">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="e43eb-144">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="e43eb-144">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="e43eb-145">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="e43eb-145">Unsubscribe operation</span></span>](unsubscribe-operation.md)


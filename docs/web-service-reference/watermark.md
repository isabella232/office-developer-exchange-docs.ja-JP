---
title: Watermark
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Watermark
api_type:
- schema
ms.assetid: e1545046-94f9-4ac7-af1c-ea81dfb6822c
description: ウォーターマーク要素は、メールボックスイベントキュー内のイベントブックマークを表します。
ms.openlocfilehash: a717196101fea698b0b8c66f92a3d420fda9a421
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459764"
---
# <a name="watermark"></a><span data-ttu-id="673ad-103">Watermark</span><span class="sxs-lookup"><span data-stu-id="673ad-103">Watermark</span></span>

<span data-ttu-id="673ad-104">**ウォーターマーク**要素は、メールボックスイベントキュー内のイベントブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="673ad-104">The **Watermark** element represents an event bookmark in the mailbox event queue.</span></span> 
  
```xml
<Watermark/>
```

 <span data-ttu-id="673ad-105">**WatermarkType**</span><span class="sxs-lookup"><span data-stu-id="673ad-105">**WatermarkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="673ad-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="673ad-106">Attributes and elements</span></span>

<span data-ttu-id="673ad-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="673ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="673ad-108">属性</span><span class="sxs-lookup"><span data-stu-id="673ad-108">Attributes</span></span>

<span data-ttu-id="673ad-109">なし。</span><span class="sxs-lookup"><span data-stu-id="673ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="673ad-110">子要素</span><span class="sxs-lookup"><span data-stu-id="673ad-110">Child elements</span></span>

<span data-ttu-id="673ad-111">なし。</span><span class="sxs-lookup"><span data-stu-id="673ad-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="673ad-112">親要素</span><span class="sxs-lookup"><span data-stu-id="673ad-112">Parent elements</span></span>

|<span data-ttu-id="673ad-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="673ad-113">**Element**</span></span>|<span data-ttu-id="673ad-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="673ad-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="673ad-115">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="673ad-115">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="673ad-116">プルベースのイベント通知サブスクリプションに対するサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="673ad-116">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="673ad-117">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="673ad-117">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="673ad-118">プッシュベースのイベント通知サブスクリプションのサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="673ad-118">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="673ad-119">GetEvents</span><span class="sxs-lookup"><span data-stu-id="673ad-119">GetEvents</span></span>](getevents.md) <br/> |<span data-ttu-id="673ad-120">プルクライアントがサーバーからの通知を要求するために使用する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="673ad-120">Represents the operation used by pull clients to request notifications from the server.</span></span>  <br/> |
|[<span data-ttu-id="673ad-121">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="673ad-121">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="673ad-122">アイテムまたはフォルダーがコピーされるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="673ad-122">Represents an event where an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="673ad-123">対する createdevent</span><span class="sxs-lookup"><span data-stu-id="673ad-123">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="673ad-124">アイテムまたはフォルダーが作成されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="673ad-124">Represents an event where an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="673ad-125">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="673ad-125">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="673ad-126">アイテムまたはフォルダーが削除されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="673ad-126">Represents an event where an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="673ad-127">対する modifiedevent</span><span class="sxs-lookup"><span data-stu-id="673ad-127">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="673ad-128">アイテムまたはフォルダーが変更されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="673ad-128">Represents an event where an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="673ad-129">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="673ad-129">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="673ad-130">ある親フォルダーから別の親フォルダーにアイテムまたはフォルダーを移動するイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="673ad-130">Represents an event where an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="673ad-131">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="673ad-131">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="673ad-132">メールボックス内の新しいメールアイテムによってトリガーされるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="673ad-132">Represents an event triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="673ad-133">StatusEvent</span><span class="sxs-lookup"><span data-stu-id="673ad-133">StatusEvent</span></span>](statusevent.md) <br/> |<span data-ttu-id="673ad-134">メールボックス内で新しいアクティビティが発生していないことを示す通知を表します。</span><span class="sxs-lookup"><span data-stu-id="673ad-134">Represents a notification that no new activity has occurred in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="673ad-135">メッセージの表示</span><span class="sxs-lookup"><span data-stu-id="673ad-135">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md) <br/> |<span data-ttu-id="673ad-136">サブスクライブ要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="673ad-136">Contains the status and result of a Subscribe request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="673ad-137">テキスト値</span><span class="sxs-lookup"><span data-stu-id="673ad-137">Text value</span></span>

<span data-ttu-id="673ad-138">この要素の使用方法によっては、テキスト値が必須または省略可能である場合があります。</span><span class="sxs-lookup"><span data-stu-id="673ad-138">A text value may be required or optional depending on how this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="673ad-139">注釈</span><span class="sxs-lookup"><span data-stu-id="673ad-139">Remarks</span></span>

<span data-ttu-id="673ad-140">Subscribe 要求にウォーターマークが含まれている場合、サブスクリプションはウォーターマークの前から作成されます。</span><span class="sxs-lookup"><span data-stu-id="673ad-140">If a Subscribe request contains a watermark, the subscription is created from the watermark forward.</span></span> <span data-ttu-id="673ad-141">Subscribe 要求に、メールボックスの events テーブルにないウォーターマークが含まれる場合、 `ErrorInvalidWatermark` クライアントアプリケーションにエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="673ad-141">If the Subscribe request contains a watermark that is not found in the mailbox events table, an  `ErrorInvalidWatermark` error is returned to the client application.</span></span> <span data-ttu-id="673ad-142">これは、ウォーターマークが古すぎ、[イベント] テーブルの30日間のウィンドウから削除されている場合、またはウォーターマークが events テーブルに存在しない場合に発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="673ad-142">This may occur if the watermark is too old and has been removed from the 30 day window of the events table or if the watermark was not ever present in the events table.</span></span> <span data-ttu-id="673ad-143">これは、たとえば、別のデータベースにあるメールボックスの別のサブスクリプションからウォーターマークが取得された場合などに発生します。</span><span class="sxs-lookup"><span data-stu-id="673ad-143">This can happen, for example, if a watermark is obtained from a different subscription for a mailbox in a different database.</span></span> 
  
<span data-ttu-id="673ad-144">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="673ad-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="673ad-145">要素の情報</span><span class="sxs-lookup"><span data-stu-id="673ad-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="673ad-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="673ad-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="673ad-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="673ad-147">Schema name</span></span>  <br/> |<span data-ttu-id="673ad-148">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="673ad-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="673ad-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="673ad-149">Validation file</span></span>  <br/> |<span data-ttu-id="673ad-150">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="673ad-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="673ad-151">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="673ad-151">Can be empty</span></span>  <br/> |<span data-ttu-id="673ad-152">正しくない</span><span class="sxs-lookup"><span data-stu-id="673ad-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="673ad-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="673ad-153">See also</span></span>



[<span data-ttu-id="673ad-154">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="673ad-154">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="673ad-155">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="673ad-155">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="673ad-156">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="673ad-156">Unsubscribe operation</span></span>](unsubscribe-operation.md)


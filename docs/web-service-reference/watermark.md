---
title: ウォーターマーク
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
description: 透かしの要素は、メールボックス イベント キュー内のイベント ブックマークを表します。
ms.openlocfilehash: 1867aa781bc24f5eb3bdb4648fa494a2a7ea396a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839999"
---
# <a name="watermark"></a><span data-ttu-id="31087-103">ウォーターマーク</span><span class="sxs-lookup"><span data-stu-id="31087-103">Watermark</span></span>

<span data-ttu-id="31087-104">**透かし**の要素は、メールボックス イベント キュー内のイベント ブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="31087-104">The **Watermark** element represents an event bookmark in the mailbox event queue.</span></span> 
  
```xml
<Watermark/>
```

 <span data-ttu-id="31087-105">**WatermarkType**</span><span class="sxs-lookup"><span data-stu-id="31087-105">**WatermarkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31087-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="31087-106">Attributes and elements</span></span>

<span data-ttu-id="31087-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="31087-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31087-108">属性</span><span class="sxs-lookup"><span data-stu-id="31087-108">Attributes</span></span>

<span data-ttu-id="31087-109">なし。</span><span class="sxs-lookup"><span data-stu-id="31087-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31087-110">子要素</span><span class="sxs-lookup"><span data-stu-id="31087-110">Child elements</span></span>

<span data-ttu-id="31087-111">なし。</span><span class="sxs-lookup"><span data-stu-id="31087-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="31087-112">親要素</span><span class="sxs-lookup"><span data-stu-id="31087-112">Parent elements</span></span>

|<span data-ttu-id="31087-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="31087-113">**Element**</span></span>|<span data-ttu-id="31087-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="31087-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31087-115">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="31087-115">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="31087-116">プル ベースのイベント通知サブスクリプションをサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="31087-116">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="31087-117">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="31087-117">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="31087-118">プッシュ ベースのイベント通知サブスクリプションをサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="31087-118">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="31087-119">GetEvents</span><span class="sxs-lookup"><span data-stu-id="31087-119">GetEvents</span></span>](getevents.md) <br/> |<span data-ttu-id="31087-120">プル クライアントがサーバーからの通知を要求に使用する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="31087-120">Represents the operation used by pull clients to request notifications from the server.</span></span>  <br/> |
|[<span data-ttu-id="31087-121">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="31087-121">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="31087-122">アイテムまたはフォルダーがコピーされるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="31087-122">Represents an event where an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="31087-123">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="31087-123">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="31087-124">アイテムまたはフォルダーが作成されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="31087-124">Represents an event where an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="31087-125">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="31087-125">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="31087-126">アイテムまたはフォルダーが削除されたイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="31087-126">Represents an event where an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="31087-127">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="31087-127">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="31087-128">アイテムまたはフォルダーが変更されたイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="31087-128">Represents an event where an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="31087-129">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="31087-129">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="31087-130">アイテムまたはフォルダーの移動先フォルダーの 1 つの親から別の親フォルダー イベントを表します。</span><span class="sxs-lookup"><span data-stu-id="31087-130">Represents an event where an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="31087-131">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="31087-131">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="31087-132">メールボックス内の新しいメール アイテムによって発生したイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="31087-132">Represents an event triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="31087-133">StatusEvent</span><span class="sxs-lookup"><span data-stu-id="31087-133">StatusEvent</span></span>](statusevent.md) <br/> |<span data-ttu-id="31087-134">通知メールボックスに新しいアクティビティが発生していないことを表します。</span><span class="sxs-lookup"><span data-stu-id="31087-134">Represents a notification that no new activity has occurred in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="31087-135">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="31087-135">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md) <br/> |<span data-ttu-id="31087-136">Subscribe 要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="31087-136">Contains the status and result of a Subscribe request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="31087-137">テキスト値</span><span class="sxs-lookup"><span data-stu-id="31087-137">Text value</span></span>

<span data-ttu-id="31087-138">テキスト値には、必須またはオプションによっては、この要素を使用する方法があります。</span><span class="sxs-lookup"><span data-stu-id="31087-138">A text value may be required or optional depending on how this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="31087-139">備考</span><span class="sxs-lookup"><span data-stu-id="31087-139">Remarks</span></span>

<span data-ttu-id="31087-140">Subscribe 要求にウォーターマークが含まれている場合、サブスクリプションはウォーターマークから先作成されます。</span><span class="sxs-lookup"><span data-stu-id="31087-140">If a Subscribe request contains a watermark, the subscription is created from the watermark forward.</span></span> <span data-ttu-id="31087-141">Subscribe 要求にウォーターマークがメールボックス イベント テーブル内に見つからないことが含まれている場合、`ErrorInvalidWatermark`エラーがクライアント アプリケーションに返されます。</span><span class="sxs-lookup"><span data-stu-id="31087-141">If the Subscribe request contains a watermark that is not found in the mailbox events table, an  `ErrorInvalidWatermark` error is returned to the client application.</span></span> <span data-ttu-id="31087-142">ウォーターマークが古すぎるので、30 日間のウィンドウ イベント テーブルから削除された場合に発生することも透かしがかつてない場合は、イベント テーブルに表示します。</span><span class="sxs-lookup"><span data-stu-id="31087-142">This may occur if the watermark is too old and has been removed from the 30 day window of the events table or if the watermark was not ever present in the events table.</span></span> <span data-ttu-id="31087-143">これは、たとえば、ウォーターマークが別のデータベース内のメールボックスの別のサブスクリプションから取得した場合に発生します。</span><span class="sxs-lookup"><span data-stu-id="31087-143">This can happen, for example, if a watermark is obtained from a different subscription for a mailbox in a different database.</span></span> 
  
<span data-ttu-id="31087-144">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="31087-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31087-145">要素情報</span><span class="sxs-lookup"><span data-stu-id="31087-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31087-146">名前空間</span><span class="sxs-lookup"><span data-stu-id="31087-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="31087-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="31087-147">Schema name</span></span>  <br/> |<span data-ttu-id="31087-148">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="31087-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="31087-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="31087-149">Validation file</span></span>  <br/> |<span data-ttu-id="31087-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="31087-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="31087-151">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="31087-151">Can be empty</span></span>  <br/> |<span data-ttu-id="31087-152">False</span><span class="sxs-lookup"><span data-stu-id="31087-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="31087-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="31087-153">See also</span></span>



[<span data-ttu-id="31087-154">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="31087-154">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="31087-155">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="31087-155">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="31087-156">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="31087-156">Unsubscribe operation</span></span>](unsubscribe-operation.md)


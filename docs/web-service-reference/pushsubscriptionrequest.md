---
title: PushSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PushSubscriptionRequest
api_type:
- schema
ms.assetid: 70caa0ca-40a1-421f-b4e6-0658f22d0b8e
description: PushSubscriptionRequest 要素は、プッシュ ベースのイベント通知サブスクリプションをサブスクリプションを表します。
ms.openlocfilehash: 34717d37b8e5bb50c927e57088299fbcb18a2514
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832929"
---
# <a name="pushsubscriptionrequest"></a><span data-ttu-id="9df7f-103">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="9df7f-103">PushSubscriptionRequest</span></span>

<span data-ttu-id="9df7f-104">**PushSubscriptionRequest**要素は、プッシュ ベースのイベント通知サブスクリプションをサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="9df7f-104">The **PushSubscriptionRequest** element represents a subscription to a push-based event notification subscription.</span></span> 
  
[<span data-ttu-id="9df7f-105">購読</span><span class="sxs-lookup"><span data-stu-id="9df7f-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="9df7f-106">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="9df7f-106">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
```XML
<PushSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <StatusFrequency/>
   <URL/>
</PushSubscriptionRequest>
```

 <span data-ttu-id="9df7f-107">**PushSubscriptionRequestType**</span><span class="sxs-lookup"><span data-stu-id="9df7f-107">**PushSubscriptionRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9df7f-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9df7f-108">Attributes and elements</span></span>

<span data-ttu-id="9df7f-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9df7f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9df7f-110">属性</span><span class="sxs-lookup"><span data-stu-id="9df7f-110">Attributes</span></span>

|<span data-ttu-id="9df7f-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="9df7f-111">**Attribute**</span></span>|<span data-ttu-id="9df7f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9df7f-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9df7f-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="9df7f-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="9df7f-114">使用可能なすべてのフォルダーを購読するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9df7f-114">Indicates whether to subscribe to all available folders.</span></span> <span data-ttu-id="9df7f-115">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="9df7f-115">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9df7f-116">子要素</span><span class="sxs-lookup"><span data-stu-id="9df7f-116">Child elements</span></span>

|<span data-ttu-id="9df7f-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="9df7f-117">**Element**</span></span>|<span data-ttu-id="9df7f-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="9df7f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9df7f-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="9df7f-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="9df7f-120">イベント通知を監視するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9df7f-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="9df7f-121">EventTypes</span><span class="sxs-lookup"><span data-stu-id="9df7f-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="9df7f-122">サブスクリプションを作成するために使用されるイベント通知のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9df7f-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
|[<span data-ttu-id="9df7f-123">透かし</span><span class="sxs-lookup"><span data-stu-id="9df7f-123">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="9df7f-124">メールボックス イベント テーブル内のイベント ブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="9df7f-124">Represents an event bookmark in the mailbox events table.</span></span> <span data-ttu-id="9df7f-125">透かしによって表されるイベントからサブスクリプションの作成に使用されます。</span><span class="sxs-lookup"><span data-stu-id="9df7f-125">This is used to create a subscription starting at an event represented by the watermark.</span></span> <span data-ttu-id="9df7f-126">Subscribe 要求からのウォーターマークが見つからない場合、エラー応答がクライアントに返されます。</span><span class="sxs-lookup"><span data-stu-id="9df7f-126">If the watermark from a Subscribe request is not found, an error response will be returned to the client.</span></span> <span data-ttu-id="9df7f-127">これは、透かしは、30 日間またはウォーターマークがメールボックス内に存在しなかったかどうかよりも古い場合に発生します。</span><span class="sxs-lookup"><span data-stu-id="9df7f-127">This may occur if the watermark is older than 30 days or if the watermark was never present in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9df7f-128">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="9df7f-128">StatusFrequency</span></span>](statusfrequency.md) <br/> |<span data-ttu-id="9df7f-129">(分)、通知のメッセージがクライアントに送信、イベントが発生していない場合、頻度を表します。</span><span class="sxs-lookup"><span data-stu-id="9df7f-129">Represents the frequency, specified in minutes, at which notification messages will be sent to the client when no events have occurred.</span></span>  <br/> |
|[<span data-ttu-id="9df7f-130">Url</span><span class="sxs-lookup"><span data-stu-id="9df7f-130">Url </span></span>](url-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9df7f-131">クライアント プッシュ通知のための Web サービスの場所を表します。</span><span class="sxs-lookup"><span data-stu-id="9df7f-131">Represents the location of the client Web service for push notifications.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9df7f-132">親要素</span><span class="sxs-lookup"><span data-stu-id="9df7f-132">Parent elements</span></span>

|<span data-ttu-id="9df7f-133">**要素**</span><span class="sxs-lookup"><span data-stu-id="9df7f-133">**Element**</span></span>|<span data-ttu-id="9df7f-134">**説明**</span><span class="sxs-lookup"><span data-stu-id="9df7f-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9df7f-135">購読</span><span class="sxs-lookup"><span data-stu-id="9df7f-135">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="9df7f-136">サブスクリプションを作成するためのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9df7f-136">Contains the properties used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9df7f-137">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9df7f-137">Text value</span></span>

<span data-ttu-id="9df7f-138">なし。</span><span class="sxs-lookup"><span data-stu-id="9df7f-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9df7f-139">備考</span><span class="sxs-lookup"><span data-stu-id="9df7f-139">Remarks</span></span>

<span data-ttu-id="9df7f-140">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9df7f-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9df7f-141">要素情報</span><span class="sxs-lookup"><span data-stu-id="9df7f-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9df7f-142">名前空間</span><span class="sxs-lookup"><span data-stu-id="9df7f-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9df7f-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9df7f-143">Schema name</span></span>  <br/> |<span data-ttu-id="9df7f-144">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9df7f-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9df7f-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9df7f-145">Validation file</span></span>  <br/> |<span data-ttu-id="9df7f-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9df7f-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9df7f-147">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9df7f-147">Can be empty</span></span>  <br/> |<span data-ttu-id="9df7f-148">False</span><span class="sxs-lookup"><span data-stu-id="9df7f-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9df7f-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="9df7f-149">See also</span></span>



[<span data-ttu-id="9df7f-150">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="9df7f-150">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="9df7f-151">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="9df7f-151">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="9df7f-152">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="9df7f-152">Unsubscribe operation</span></span>](unsubscribe-operation.md)


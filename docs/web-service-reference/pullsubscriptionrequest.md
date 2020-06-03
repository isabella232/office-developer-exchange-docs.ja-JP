---
title: PullSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PullSubscriptionRequest
api_type:
- schema
ms.assetid: 145c5cc7-a894-4f0b-a6ea-358cddfb5c33
description: PullSubscriptionRequest 要素は、プルベースのイベント通知サブスクリプションに対するサブスクリプションを表します。
ms.openlocfilehash: fb9712c9e1481678c2821ee344052783d5c25bf9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468867"
---
# <a name="pullsubscriptionrequest"></a><span data-ttu-id="3986e-103">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="3986e-103">PullSubscriptionRequest</span></span>

<span data-ttu-id="3986e-104">**PullSubscriptionRequest**要素は、プルベースのイベント通知サブスクリプションに対するサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="3986e-104">The **PullSubscriptionRequest** element represents a subscription to a pull-based event notification subscription.</span></span> 
  
[<span data-ttu-id="3986e-105">登録</span><span class="sxs-lookup"><span data-stu-id="3986e-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="3986e-106">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="3986e-106">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
  
```XML
<PullSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <Timeout/>
</PullSubscriptionRequest>
```

 <span data-ttu-id="3986e-107">**PullSubscriptionRequestType**</span><span class="sxs-lookup"><span data-stu-id="3986e-107">**PullSubscriptionRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3986e-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3986e-108">Attributes and elements</span></span>

<span data-ttu-id="3986e-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3986e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3986e-110">属性</span><span class="sxs-lookup"><span data-stu-id="3986e-110">Attributes</span></span>

|<span data-ttu-id="3986e-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="3986e-111">**Attribute**</span></span>|<span data-ttu-id="3986e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3986e-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3986e-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="3986e-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="3986e-114">利用可能なすべてのフォルダーを購読するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3986e-114">Indicates whether to subscribe to all available folders.</span></span> <span data-ttu-id="3986e-115">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="3986e-115">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3986e-116">子要素</span><span class="sxs-lookup"><span data-stu-id="3986e-116">Child elements</span></span>

|<span data-ttu-id="3986e-117">**Element**</span><span class="sxs-lookup"><span data-stu-id="3986e-117">**Element**</span></span>|<span data-ttu-id="3986e-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="3986e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3986e-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="3986e-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="3986e-120">イベント通知を監視するフォルダーを識別するために使用されるフォルダー識別子の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="3986e-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="3986e-121">EventTypes</span><span class="sxs-lookup"><span data-stu-id="3986e-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="3986e-122">サブスクリプションの作成に使用されるイベント通知のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3986e-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
|[<span data-ttu-id="3986e-123">Watermark</span><span class="sxs-lookup"><span data-stu-id="3986e-123">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="3986e-124">メールボックスイベントテーブル内のイベントブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="3986e-124">Represents an event bookmark in the mailbox events table.</span></span> <span data-ttu-id="3986e-125">これは、ウォーターマークで表されるイベントで開始するサブスクリプションを作成するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="3986e-125">This is used to create a subscription that starts at an event that is represented by the watermark.</span></span> <span data-ttu-id="3986e-126">Subscribe 要求のウォーターマークが見つからない場合は、クライアントにエラー応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="3986e-126">If the watermark from a Subscribe request is not found, an error response will be returned to the client.</span></span> <span data-ttu-id="3986e-127">このエラーは、ウォーターマークが30日よりも古い場合、またはウォーターマークがメールボックスに存在しない場合に発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="3986e-127">This error may occur if the watermark is older than 30 days or if the watermark was never present in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3986e-128">Timeout</span><span class="sxs-lookup"><span data-stu-id="3986e-128">Timeout</span></span>](timeout.md) <br/> |<span data-ttu-id="3986e-129">クライアントからの GetEvents 要求なしで、サブスクリプションをアイドル状態のままにできる期間 (分単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="3986e-129">Represents the duration, in minutes, that the subscription can remain idle without a GetEvents request from the client.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3986e-130">親要素</span><span class="sxs-lookup"><span data-stu-id="3986e-130">Parent elements</span></span>

|<span data-ttu-id="3986e-131">**要素**</span><span class="sxs-lookup"><span data-stu-id="3986e-131">**Element**</span></span>|<span data-ttu-id="3986e-132">**説明**</span><span class="sxs-lookup"><span data-stu-id="3986e-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3986e-133">登録</span><span class="sxs-lookup"><span data-stu-id="3986e-133">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="3986e-134">サブスクリプションの作成に使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3986e-134">Contains the properties that are used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3986e-135">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3986e-135">Text value</span></span>

<span data-ttu-id="3986e-136">なし。</span><span class="sxs-lookup"><span data-stu-id="3986e-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3986e-137">注釈</span><span class="sxs-lookup"><span data-stu-id="3986e-137">Remarks</span></span>

<span data-ttu-id="3986e-138">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3986e-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3986e-139">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3986e-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3986e-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="3986e-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3986e-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3986e-141">Schema name</span></span>  <br/> |<span data-ttu-id="3986e-142">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="3986e-142">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3986e-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3986e-143">Validation file</span></span>  <br/> |<span data-ttu-id="3986e-144">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3986e-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3986e-145">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3986e-145">Can be empty</span></span>  <br/> |<span data-ttu-id="3986e-146">正しくない</span><span class="sxs-lookup"><span data-stu-id="3986e-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3986e-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="3986e-147">See also</span></span>



[<span data-ttu-id="3986e-148">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="3986e-148">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
[<span data-ttu-id="3986e-149">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="3986e-149">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="3986e-150">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="3986e-150">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="3986e-151">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="3986e-151">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="3986e-152">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3986e-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


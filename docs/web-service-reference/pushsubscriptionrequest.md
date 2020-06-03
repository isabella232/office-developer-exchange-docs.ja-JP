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
description: PushSubscriptionRequest 要素は、プッシュベースのイベント通知サブスクリプションへのサブスクリプションを表します。
ms.openlocfilehash: dcdb767ed175468aa4ec940f3147c164e4707e40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465514"
---
# <a name="pushsubscriptionrequest"></a><span data-ttu-id="e9ecb-103">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="e9ecb-103">PushSubscriptionRequest</span></span>

<span data-ttu-id="e9ecb-104">**Pushsubscriptionrequest**要素は、プッシュベースのイベント通知サブスクリプションへのサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="e9ecb-104">The **PushSubscriptionRequest** element represents a subscription to a push-based event notification subscription.</span></span> 
  
[<span data-ttu-id="e9ecb-105">登録</span><span class="sxs-lookup"><span data-stu-id="e9ecb-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="e9ecb-106">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="e9ecb-106">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
```XML
<PushSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <StatusFrequency/>
   <URL/>
</PushSubscriptionRequest>
```

 <span data-ttu-id="e9ecb-107">**PushSubscriptionRequestType**</span><span class="sxs-lookup"><span data-stu-id="e9ecb-107">**PushSubscriptionRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9ecb-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e9ecb-108">Attributes and elements</span></span>

<span data-ttu-id="e9ecb-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e9ecb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9ecb-110">属性</span><span class="sxs-lookup"><span data-stu-id="e9ecb-110">Attributes</span></span>

|<span data-ttu-id="e9ecb-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="e9ecb-111">**Attribute**</span></span>|<span data-ttu-id="e9ecb-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9ecb-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e9ecb-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="e9ecb-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="e9ecb-114">利用可能なすべてのフォルダーを購読するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e9ecb-114">Indicates whether to subscribe to all available folders.</span></span> <span data-ttu-id="e9ecb-115">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="e9ecb-115">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e9ecb-116">子要素</span><span class="sxs-lookup"><span data-stu-id="e9ecb-116">Child elements</span></span>

|<span data-ttu-id="e9ecb-117">**Element**</span><span class="sxs-lookup"><span data-stu-id="e9ecb-117">**Element**</span></span>|<span data-ttu-id="e9ecb-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9ecb-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9ecb-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="e9ecb-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="e9ecb-120">イベント通知を監視するフォルダーを識別するために使用されるフォルダー識別子の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="e9ecb-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="e9ecb-121">EventTypes</span><span class="sxs-lookup"><span data-stu-id="e9ecb-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="e9ecb-122">サブスクリプションの作成に使用されるイベント通知のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9ecb-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
|[<span data-ttu-id="e9ecb-123">Watermark</span><span class="sxs-lookup"><span data-stu-id="e9ecb-123">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="e9ecb-124">メールボックスイベントテーブル内のイベントブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="e9ecb-124">Represents an event bookmark in the mailbox events table.</span></span> <span data-ttu-id="e9ecb-125">これは、ウォーターマークで表されるイベントから開始するサブスクリプションを作成するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="e9ecb-125">This is used to create a subscription starting at an event represented by the watermark.</span></span> <span data-ttu-id="e9ecb-126">Subscribe 要求のウォーターマークが見つからない場合は、クライアントにエラー応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="e9ecb-126">If the watermark from a Subscribe request is not found, an error response will be returned to the client.</span></span> <span data-ttu-id="e9ecb-127">これは、ウォーターマークが30日よりも古い場合、またはウォーターマークがメールボックスに存在しない場合に発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="e9ecb-127">This may occur if the watermark is older than 30 days or if the watermark was never present in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e9ecb-128">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="e9ecb-128">StatusFrequency</span></span>](statusfrequency.md) <br/> |<span data-ttu-id="e9ecb-129">イベントが発生していない場合に通知メッセージがクライアントに送信される頻度 (分単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="e9ecb-129">Represents the frequency, specified in minutes, at which notification messages will be sent to the client when no events have occurred.</span></span>  <br/> |
|[<span data-ttu-id="e9ecb-130">.Url</span><span class="sxs-lookup"><span data-stu-id="e9ecb-130">Url </span></span>](url-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e9ecb-131">プッシュ通知用のクライアント Web サービスの場所を表します。</span><span class="sxs-lookup"><span data-stu-id="e9ecb-131">Represents the location of the client Web service for push notifications.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e9ecb-132">親要素</span><span class="sxs-lookup"><span data-stu-id="e9ecb-132">Parent elements</span></span>

|<span data-ttu-id="e9ecb-133">**要素**</span><span class="sxs-lookup"><span data-stu-id="e9ecb-133">**Element**</span></span>|<span data-ttu-id="e9ecb-134">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9ecb-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9ecb-135">登録</span><span class="sxs-lookup"><span data-stu-id="e9ecb-135">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="e9ecb-136">サブスクリプションの作成に使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9ecb-136">Contains the properties used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e9ecb-137">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e9ecb-137">Text value</span></span>

<span data-ttu-id="e9ecb-138">なし。</span><span class="sxs-lookup"><span data-stu-id="e9ecb-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e9ecb-139">注釈</span><span class="sxs-lookup"><span data-stu-id="e9ecb-139">Remarks</span></span>

<span data-ttu-id="e9ecb-140">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e9ecb-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9ecb-141">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e9ecb-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9ecb-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="e9ecb-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e9ecb-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e9ecb-143">Schema name</span></span>  <br/> |<span data-ttu-id="e9ecb-144">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="e9ecb-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e9ecb-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e9ecb-145">Validation file</span></span>  <br/> |<span data-ttu-id="e9ecb-146">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="e9ecb-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e9ecb-147">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e9ecb-147">Can be empty</span></span>  <br/> |<span data-ttu-id="e9ecb-148">正しくない</span><span class="sxs-lookup"><span data-stu-id="e9ecb-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9ecb-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="e9ecb-149">See also</span></span>



[<span data-ttu-id="e9ecb-150">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="e9ecb-150">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="e9ecb-151">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="e9ecb-151">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="e9ecb-152">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="e9ecb-152">Unsubscribe operation</span></span>](unsubscribe-operation.md)


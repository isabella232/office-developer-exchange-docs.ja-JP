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
description: PullSubscriptionRequest 要素は、プル ベースのイベント通知サブスクリプションをサブスクリプションを表します。
ms.openlocfilehash: 5f757bf1f79f7e2a00fb886db50e6ea0eaed1a4a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832932"
---
# <a name="pullsubscriptionrequest"></a><span data-ttu-id="8222e-103">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="8222e-103">PullSubscriptionRequest</span></span>

<span data-ttu-id="8222e-104">**PullSubscriptionRequest**要素は、プル ベースのイベント通知サブスクリプションをサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="8222e-104">The **PullSubscriptionRequest** element represents a subscription to a pull-based event notification subscription.</span></span> 
  
[<span data-ttu-id="8222e-105">購読</span><span class="sxs-lookup"><span data-stu-id="8222e-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="8222e-106">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="8222e-106">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
  
```XML
<PullSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <Timeout/>
</PullSubscriptionRequest>
```

 <span data-ttu-id="8222e-107">**PullSubscriptionRequestType**</span><span class="sxs-lookup"><span data-stu-id="8222e-107">**PullSubscriptionRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8222e-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8222e-108">Attributes and elements</span></span>

<span data-ttu-id="8222e-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8222e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8222e-110">属性</span><span class="sxs-lookup"><span data-stu-id="8222e-110">Attributes</span></span>

|<span data-ttu-id="8222e-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="8222e-111">**Attribute**</span></span>|<span data-ttu-id="8222e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="8222e-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8222e-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="8222e-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="8222e-114">使用可能なすべてのフォルダーを購読するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8222e-114">Indicates whether to subscribe to all available folders.</span></span> <span data-ttu-id="8222e-115">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="8222e-115">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8222e-116">子要素</span><span class="sxs-lookup"><span data-stu-id="8222e-116">Child elements</span></span>

|<span data-ttu-id="8222e-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="8222e-117">**Element**</span></span>|<span data-ttu-id="8222e-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="8222e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8222e-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="8222e-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="8222e-120">イベント通知を監視するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8222e-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="8222e-121">EventTypes</span><span class="sxs-lookup"><span data-stu-id="8222e-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="8222e-122">サブスクリプションを作成するために使用されるイベント通知のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8222e-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
|[<span data-ttu-id="8222e-123">透かし</span><span class="sxs-lookup"><span data-stu-id="8222e-123">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="8222e-124">メールボックス イベント テーブル内のイベント ブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="8222e-124">Represents an event bookmark in the mailbox events table.</span></span> <span data-ttu-id="8222e-125">ウォーターマークが表すイベントで開始されるサブスクリプションを作成するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="8222e-125">This is used to create a subscription that starts at an event that is represented by the watermark.</span></span> <span data-ttu-id="8222e-126">Subscribe 要求からのウォーターマークが見つからない場合、エラー応答がクライアントに返されます。</span><span class="sxs-lookup"><span data-stu-id="8222e-126">If the watermark from a Subscribe request is not found, an error response will be returned to the client.</span></span> <span data-ttu-id="8222e-127">ウォーターマークは、30 日間またはウォーターマークがメールボックス内に存在しなかったかどうかよりも古い場合、このエラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="8222e-127">This error may occur if the watermark is older than 30 days or if the watermark was never present in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8222e-128">Timeout</span><span class="sxs-lookup"><span data-stu-id="8222e-128">Timeout</span></span>](timeout.md) <br/> |<span data-ttu-id="8222e-129">サブスクリプションがクライアントからの GetEvents 要求なしアイドルを分単位で、期間を表します。</span><span class="sxs-lookup"><span data-stu-id="8222e-129">Represents the duration, in minutes, that the subscription can remain idle without a GetEvents request from the client.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8222e-130">親要素</span><span class="sxs-lookup"><span data-stu-id="8222e-130">Parent elements</span></span>

|<span data-ttu-id="8222e-131">**要素**</span><span class="sxs-lookup"><span data-stu-id="8222e-131">**Element**</span></span>|<span data-ttu-id="8222e-132">**説明**</span><span class="sxs-lookup"><span data-stu-id="8222e-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8222e-133">購読</span><span class="sxs-lookup"><span data-stu-id="8222e-133">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="8222e-134">サブスクリプションの作成に使用するプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8222e-134">Contains the properties that are used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8222e-135">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8222e-135">Text value</span></span>

<span data-ttu-id="8222e-136">なし。</span><span class="sxs-lookup"><span data-stu-id="8222e-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8222e-137">備考</span><span class="sxs-lookup"><span data-stu-id="8222e-137">Remarks</span></span>

<span data-ttu-id="8222e-138">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8222e-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8222e-139">要素情報</span><span class="sxs-lookup"><span data-stu-id="8222e-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8222e-140">名前空間</span><span class="sxs-lookup"><span data-stu-id="8222e-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8222e-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8222e-141">Schema name</span></span>  <br/> |<span data-ttu-id="8222e-142">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="8222e-142">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8222e-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8222e-143">Validation file</span></span>  <br/> |<span data-ttu-id="8222e-144">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8222e-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8222e-145">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8222e-145">Can be empty</span></span>  <br/> |<span data-ttu-id="8222e-146">False</span><span class="sxs-lookup"><span data-stu-id="8222e-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8222e-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="8222e-147">See also</span></span>



[<span data-ttu-id="8222e-148">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="8222e-148">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
[<span data-ttu-id="8222e-149">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="8222e-149">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="8222e-150">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="8222e-150">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="8222e-151">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="8222e-151">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="8222e-152">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8222e-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


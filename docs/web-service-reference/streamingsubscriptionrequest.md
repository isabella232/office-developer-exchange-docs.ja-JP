---
title: StreamingSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StreamingSubscriptionRequest
api_type:
- schema
ms.assetid: d18f3b60-ebb6-4133-b895-a6ec8942d039
description: StreamingSubscriptionRequest 要素は、ストリーミングイベント通知サブスクリプションへのサブスクリプションを表します。
ms.openlocfilehash: b469ba7598420189c1db0e2fe676a279390eb6bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468230"
---
# <a name="streamingsubscriptionrequest"></a><span data-ttu-id="189b6-103">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="189b6-103">StreamingSubscriptionRequest</span></span>

<span data-ttu-id="189b6-104">**Streamingsubscriptionrequest**要素は、ストリーミングイベント通知サブスクリプションへのサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="189b6-104">The **StreamingSubscriptionRequest** element represents a subscription to a streaming event notification subscription.</span></span> 
  
[<span data-ttu-id="189b6-105">登録</span><span class="sxs-lookup"><span data-stu-id="189b6-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="189b6-106">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="189b6-106">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md)
  
```xml
<StreamingSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
</StreamingSubscriptionRequest>
```

 <span data-ttu-id="189b6-107">**StreamingSubscriptionRequest**</span><span class="sxs-lookup"><span data-stu-id="189b6-107">**StreamingSubscriptionRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="189b6-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="189b6-108">Attributes and elements</span></span>

<span data-ttu-id="189b6-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="189b6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="189b6-110">属性</span><span class="sxs-lookup"><span data-stu-id="189b6-110">Attributes</span></span>

|<span data-ttu-id="189b6-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="189b6-111">**Attribute**</span></span>|<span data-ttu-id="189b6-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="189b6-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="189b6-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="189b6-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="189b6-114">サーバーがユーザーのメールボックス内のすべてのフォルダーをサブスクライブするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="189b6-114">Indicates whether the server will subscribe to all folders in the user's mailbox.</span></span> <span data-ttu-id="189b6-115">値が**true の場合**は、サーバーがサブスクライブすることを示します。</span><span class="sxs-lookup"><span data-stu-id="189b6-115">A value of **true** indicates that the server will subscribe.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="189b6-116">子要素</span><span class="sxs-lookup"><span data-stu-id="189b6-116">Child elements</span></span>

|<span data-ttu-id="189b6-117">**Element**</span><span class="sxs-lookup"><span data-stu-id="189b6-117">**Element**</span></span>|<span data-ttu-id="189b6-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="189b6-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="189b6-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="189b6-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="189b6-120">イベント通知を監視するフォルダーを識別するために使用されるフォルダー識別子の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="189b6-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="189b6-121">EventTypes</span><span class="sxs-lookup"><span data-stu-id="189b6-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="189b6-122">サブスクリプションの作成に使用されるイベント通知のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="189b6-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="189b6-123">親要素</span><span class="sxs-lookup"><span data-stu-id="189b6-123">Parent elements</span></span>

|<span data-ttu-id="189b6-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="189b6-124">**Element**</span></span>|<span data-ttu-id="189b6-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="189b6-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="189b6-126">登録</span><span class="sxs-lookup"><span data-stu-id="189b6-126">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="189b6-127">サブスクリプションの作成に使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="189b6-127">Contains the properties that are used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="189b6-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="189b6-128">Text value</span></span>

<span data-ttu-id="189b6-129">なし。</span><span class="sxs-lookup"><span data-stu-id="189b6-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="189b6-130">注釈</span><span class="sxs-lookup"><span data-stu-id="189b6-130">Remarks</span></span>

<span data-ttu-id="189b6-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="189b6-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="189b6-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="189b6-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="189b6-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="189b6-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="189b6-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="189b6-134">Schema name</span></span>  <br/> |<span data-ttu-id="189b6-135">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="189b6-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="189b6-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="189b6-136">Validation file</span></span>  <br/> |<span data-ttu-id="189b6-137">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="189b6-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="189b6-138">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="189b6-138">Can be empty</span></span>  <br/> |<span data-ttu-id="189b6-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="189b6-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="189b6-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="189b6-140">See also</span></span>



[<span data-ttu-id="189b6-141">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="189b6-141">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="189b6-142">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="189b6-142">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="189b6-143">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="189b6-143">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="189b6-144">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="189b6-144">Unsubscribe operation</span></span>](unsubscribe-operation.md)


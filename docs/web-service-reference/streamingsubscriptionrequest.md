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
description: StreamingSubscriptionRequest 要素は、ストリーミングのイベント通知サブスクリプションをサブスクリプションを表します。
ms.openlocfilehash: 088ec3b8048d70803b4837548ca918c0005d91bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833601"
---
# <a name="streamingsubscriptionrequest"></a><span data-ttu-id="17b44-103">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="17b44-103">StreamingSubscriptionRequest</span></span>

<span data-ttu-id="17b44-104">**StreamingSubscriptionRequest**要素は、ストリーミングのイベント通知サブスクリプションをサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="17b44-104">The **StreamingSubscriptionRequest** element represents a subscription to a streaming event notification subscription.</span></span> 
  
[<span data-ttu-id="17b44-105">購読</span><span class="sxs-lookup"><span data-stu-id="17b44-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="17b44-106">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="17b44-106">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md)
  
```xml
<StreamingSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
</StreamingSubscriptionRequest>
```

 <span data-ttu-id="17b44-107">**StreamingSubscriptionRequest**</span><span class="sxs-lookup"><span data-stu-id="17b44-107">**StreamingSubscriptionRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17b44-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="17b44-108">Attributes and elements</span></span>

<span data-ttu-id="17b44-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="17b44-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17b44-110">属性</span><span class="sxs-lookup"><span data-stu-id="17b44-110">Attributes</span></span>

|<span data-ttu-id="17b44-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="17b44-111">**Attribute**</span></span>|<span data-ttu-id="17b44-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="17b44-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="17b44-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="17b44-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="17b44-114">サーバーがユーザーのメールボックス内のすべてのフォルダーを購読するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="17b44-114">Indicates whether the server will subscribe to all folders in the user's mailbox.</span></span> <span data-ttu-id="17b44-115">**True**の場合は、サーバーがサブスクライブすることを示します。</span><span class="sxs-lookup"><span data-stu-id="17b44-115">A value of **true** indicates that the server will subscribe.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="17b44-116">子要素</span><span class="sxs-lookup"><span data-stu-id="17b44-116">Child elements</span></span>

|<span data-ttu-id="17b44-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="17b44-117">**Element**</span></span>|<span data-ttu-id="17b44-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="17b44-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17b44-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="17b44-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="17b44-120">イベント通知を監視するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="17b44-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="17b44-121">EventTypes</span><span class="sxs-lookup"><span data-stu-id="17b44-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="17b44-122">サブスクリプションを作成するために使用されるイベント通知のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="17b44-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="17b44-123">親要素</span><span class="sxs-lookup"><span data-stu-id="17b44-123">Parent elements</span></span>

|<span data-ttu-id="17b44-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="17b44-124">**Element**</span></span>|<span data-ttu-id="17b44-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="17b44-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17b44-126">購読</span><span class="sxs-lookup"><span data-stu-id="17b44-126">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="17b44-127">サブスクリプションの作成に使用するプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="17b44-127">Contains the properties that are used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="17b44-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="17b44-128">Text value</span></span>

<span data-ttu-id="17b44-129">なし。</span><span class="sxs-lookup"><span data-stu-id="17b44-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="17b44-130">備考</span><span class="sxs-lookup"><span data-stu-id="17b44-130">Remarks</span></span>

<span data-ttu-id="17b44-131">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="17b44-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="17b44-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="17b44-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17b44-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="17b44-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="17b44-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="17b44-134">Schema name</span></span>  <br/> |<span data-ttu-id="17b44-135">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="17b44-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="17b44-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="17b44-136">Validation file</span></span>  <br/> |<span data-ttu-id="17b44-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="17b44-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="17b44-138">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="17b44-138">Can be empty</span></span>  <br/> |<span data-ttu-id="17b44-139">False</span><span class="sxs-lookup"><span data-stu-id="17b44-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="17b44-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="17b44-140">See also</span></span>



[<span data-ttu-id="17b44-141">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="17b44-141">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="17b44-142">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="17b44-142">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="17b44-143">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="17b44-143">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="17b44-144">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="17b44-144">Unsubscribe operation</span></span>](unsubscribe-operation.md)


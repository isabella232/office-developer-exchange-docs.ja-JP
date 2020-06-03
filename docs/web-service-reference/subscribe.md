---
title: 登録
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subscribe
api_type:
- schema
ms.assetid: 6c2ee57d-e216-4a94-92db-faa3cb0e244a
description: Subscribe 要素には、サブスクリプションの作成に使用されるプロパティが含まれています。
ms.openlocfilehash: f60e67654fb6af76e8081036a3463f5be401862d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530959"
---
# <a name="subscribe"></a><span data-ttu-id="2bfaa-103">登録</span><span class="sxs-lookup"><span data-stu-id="2bfaa-103">Subscribe</span></span>

<span data-ttu-id="2bfaa-104">**Subscribe**要素には、サブスクリプションの作成に使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2bfaa-104">The **Subscribe** element contains the properties used to create subscriptions.</span></span> 
  
```XML
<Subscribe>
   <PullSubscriptionRequest/>
   <PushSubscriptionRequest/>
   <StreamingSubscriptionRequest/>
</Subscribe>
```

 <span data-ttu-id="2bfaa-105">**SubscribeType**</span><span class="sxs-lookup"><span data-stu-id="2bfaa-105">**SubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2bfaa-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2bfaa-106">Attributes and elements</span></span>

<span data-ttu-id="2bfaa-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2bfaa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2bfaa-108">属性</span><span class="sxs-lookup"><span data-stu-id="2bfaa-108">Attributes</span></span>

<span data-ttu-id="2bfaa-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2bfaa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2bfaa-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2bfaa-110">Child elements</span></span>

|<span data-ttu-id="2bfaa-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="2bfaa-111">**Element**</span></span>|<span data-ttu-id="2bfaa-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2bfaa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2bfaa-113">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="2bfaa-113">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="2bfaa-114">プルベースのイベント通知のサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="2bfaa-114">Represents a subscription to a pull-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="2bfaa-115">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="2bfaa-115">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="2bfaa-116">プッシュベースのイベント通知のサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="2bfaa-116">Represents a subscription to a push-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="2bfaa-117">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="2bfaa-117">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md) <br/> |<span data-ttu-id="2bfaa-118">ストリーミングイベント通知のサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="2bfaa-118">Represents a subscription to a streaming event notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2bfaa-119">親要素</span><span class="sxs-lookup"><span data-stu-id="2bfaa-119">Parent elements</span></span>

<span data-ttu-id="2bfaa-120">なし。</span><span class="sxs-lookup"><span data-stu-id="2bfaa-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2bfaa-121">注釈</span><span class="sxs-lookup"><span data-stu-id="2bfaa-121">Remarks</span></span>

<span data-ttu-id="2bfaa-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2bfaa-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2bfaa-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2bfaa-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2bfaa-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="2bfaa-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2bfaa-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2bfaa-125">Schema name</span></span>  <br/> |<span data-ttu-id="2bfaa-126">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2bfaa-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2bfaa-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2bfaa-127">Validation file</span></span>  <br/> |<span data-ttu-id="2bfaa-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2bfaa-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2bfaa-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2bfaa-129">Can be empty</span></span>  <br/> |<span data-ttu-id="2bfaa-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="2bfaa-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2bfaa-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="2bfaa-131">See also</span></span>



[<span data-ttu-id="2bfaa-132">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="2bfaa-132">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="2bfaa-133">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="2bfaa-133">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="2bfaa-134">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="2bfaa-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="2bfaa-135">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="2bfaa-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)


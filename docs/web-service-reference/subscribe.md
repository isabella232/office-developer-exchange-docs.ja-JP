---
title: 購読
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
description: 購読の要素には、サブスクリプションを作成するためのプロパティが含まれています。
ms.openlocfilehash: 9f23f566f9105c655b289ed9b434c5e7b917207f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833618"
---
# <a name="subscribe"></a><span data-ttu-id="2adbb-103">購読</span><span class="sxs-lookup"><span data-stu-id="2adbb-103">Subscribe</span></span>

<span data-ttu-id="2adbb-104">**購読**の要素には、サブスクリプションを作成するためのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2adbb-104">The **Subscribe** element contains the properties used to create subscriptions.</span></span> 
  
```XML
<Subscribe>
   <PullSubscriptionRequest/>
   <PushSubscriptionRequest/>
   <StreamingSubscriptionRequest/>
</Subscribe>
```

 <span data-ttu-id="2adbb-105">**SubscribeType**</span><span class="sxs-lookup"><span data-stu-id="2adbb-105">**SubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2adbb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2adbb-106">Attributes and elements</span></span>

<span data-ttu-id="2adbb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2adbb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2adbb-108">属性</span><span class="sxs-lookup"><span data-stu-id="2adbb-108">Attributes</span></span>

<span data-ttu-id="2adbb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2adbb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2adbb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2adbb-110">Child elements</span></span>

|<span data-ttu-id="2adbb-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="2adbb-111">**Element**</span></span>|<span data-ttu-id="2adbb-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2adbb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2adbb-113">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="2adbb-113">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="2adbb-114">プル ベースのイベント通知に対するサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="2adbb-114">Represents a subscription to a pull-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="2adbb-115">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="2adbb-115">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="2adbb-116">プッシュ ベースのイベント通知に対するサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="2adbb-116">Represents a subscription to a push-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="2adbb-117">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="2adbb-117">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md) <br/> |<span data-ttu-id="2adbb-118">ストリーミング イベント通知に対するサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="2adbb-118">Represents a subscription to a streaming event notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2adbb-119">親要素</span><span class="sxs-lookup"><span data-stu-id="2adbb-119">Parent elements</span></span>

<span data-ttu-id="2adbb-120">なし。</span><span class="sxs-lookup"><span data-stu-id="2adbb-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2adbb-121">備考</span><span class="sxs-lookup"><span data-stu-id="2adbb-121">Remarks</span></span>

<span data-ttu-id="2adbb-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2adbb-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2adbb-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="2adbb-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2adbb-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="2adbb-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2adbb-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2adbb-125">Schema name</span></span>  <br/> |<span data-ttu-id="2adbb-126">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="2adbb-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2adbb-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2adbb-127">Validation file</span></span>  <br/> |<span data-ttu-id="2adbb-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2adbb-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2adbb-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2adbb-129">Can be empty</span></span>  <br/> |<span data-ttu-id="2adbb-130">False</span><span class="sxs-lookup"><span data-stu-id="2adbb-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2adbb-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="2adbb-131">See also</span></span>



[<span data-ttu-id="2adbb-132">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="2adbb-132">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="2adbb-133">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="2adbb-133">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="2adbb-134">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="2adbb-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="2adbb-135">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="2adbb-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)


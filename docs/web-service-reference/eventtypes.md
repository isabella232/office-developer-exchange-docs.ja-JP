---
title: EventTypes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EventTypes
api_type:
- schema
ms.assetid: 29ded9e5-f191-4aa3-bc3e-500de2fc8818
description: EventTypes 要素には、サブスクリプションの作成に使用されるイベント通知の種類のコレクションが含まれています。
ms.openlocfilehash: f4c622376f6b607ed390511d7bb5f0f723889420
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760338"
---
# <a name="eventtypes"></a><span data-ttu-id="97a3d-103">EventTypes</span><span class="sxs-lookup"><span data-stu-id="97a3d-103">EventTypes</span></span>

<span data-ttu-id="97a3d-104">**EventTypes**要素には、サブスクリプションの作成に使用されるイベント通知の種類のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="97a3d-104">The **EventTypes** element contains a collection of event notification types that are used to create a subscription.</span></span> 
  
```xml
<EventTypes>
   <EventType/>
</EventTypes>
```

 <span data-ttu-id="97a3d-105">**NonEmptyArrayOfNotificationEventTypesType**</span><span class="sxs-lookup"><span data-stu-id="97a3d-105">**NonEmptyArrayOfNotificationEventTypesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97a3d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="97a3d-106">Attributes and elements</span></span>

<span data-ttu-id="97a3d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="97a3d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97a3d-108">属性</span><span class="sxs-lookup"><span data-stu-id="97a3d-108">Attributes</span></span>

<span data-ttu-id="97a3d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="97a3d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97a3d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="97a3d-110">Child elements</span></span>

|<span data-ttu-id="97a3d-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="97a3d-111">**Element**</span></span>|<span data-ttu-id="97a3d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="97a3d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97a3d-113">EventType</span><span class="sxs-lookup"><span data-stu-id="97a3d-113">EventType</span></span>](eventtype.md) <br/> |<span data-ttu-id="97a3d-114">サブスクリプションを作成するために使用される要求されたイベント通知の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="97a3d-114">Represents a requested event notification type that is used to create a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="97a3d-115">親要素</span><span class="sxs-lookup"><span data-stu-id="97a3d-115">Parent elements</span></span>

|<span data-ttu-id="97a3d-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="97a3d-116">**Element**</span></span>|<span data-ttu-id="97a3d-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="97a3d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97a3d-118">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="97a3d-118">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="97a3d-119">プル ベースのイベント通知サブスクリプションをサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="97a3d-119">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="97a3d-120">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="97a3d-120">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="97a3d-121">プッシュ ベースのイベント通知サブスクリプションをサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="97a3d-121">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="97a3d-122">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="97a3d-122">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md) <br/> |<span data-ttu-id="97a3d-123">ストリーミング イベント通知サブスクリプションをサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="97a3d-123">Represents a subscription to a streaming event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="97a3d-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="97a3d-124">Text value</span></span>

<span data-ttu-id="97a3d-125">なし。</span><span class="sxs-lookup"><span data-stu-id="97a3d-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="97a3d-126">備考</span><span class="sxs-lookup"><span data-stu-id="97a3d-126">Remarks</span></span>

<span data-ttu-id="97a3d-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="97a3d-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97a3d-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="97a3d-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97a3d-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="97a3d-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="97a3d-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="97a3d-130">Schema Name</span></span>  <br/> |<span data-ttu-id="97a3d-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="97a3d-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="97a3d-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="97a3d-132">Validation File</span></span>  <br/> |<span data-ttu-id="97a3d-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="97a3d-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="97a3d-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="97a3d-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="97a3d-135">False</span><span class="sxs-lookup"><span data-stu-id="97a3d-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97a3d-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="97a3d-136">See also</span></span>



[<span data-ttu-id="97a3d-137">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="97a3d-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="97a3d-138">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="97a3d-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="97a3d-139">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="97a3d-139">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="97a3d-140">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="97a3d-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


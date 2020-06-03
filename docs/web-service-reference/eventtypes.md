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
ms.openlocfilehash: 45ce1ed0699c8140029ae3fb7f667a5132f4731e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530629"
---
# <a name="eventtypes"></a><span data-ttu-id="eee50-103">EventTypes</span><span class="sxs-lookup"><span data-stu-id="eee50-103">EventTypes</span></span>

<span data-ttu-id="eee50-104">**Eventtypes**要素には、サブスクリプションの作成に使用されるイベント通知の種類のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="eee50-104">The **EventTypes** element contains a collection of event notification types that are used to create a subscription.</span></span> 
  
```xml
<EventTypes>
   <EventType/>
</EventTypes>
```

 <span data-ttu-id="eee50-105">**非 Emptyarrayofnotificationeventtypest/型**</span><span class="sxs-lookup"><span data-stu-id="eee50-105">**NonEmptyArrayOfNotificationEventTypesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eee50-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="eee50-106">Attributes and elements</span></span>

<span data-ttu-id="eee50-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="eee50-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eee50-108">属性</span><span class="sxs-lookup"><span data-stu-id="eee50-108">Attributes</span></span>

<span data-ttu-id="eee50-109">なし。</span><span class="sxs-lookup"><span data-stu-id="eee50-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eee50-110">子要素</span><span class="sxs-lookup"><span data-stu-id="eee50-110">Child elements</span></span>

|<span data-ttu-id="eee50-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="eee50-111">**Element**</span></span>|<span data-ttu-id="eee50-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="eee50-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eee50-113">EventType</span><span class="sxs-lookup"><span data-stu-id="eee50-113">EventType</span></span>](eventtype.md) <br/> |<span data-ttu-id="eee50-114">サブスクリプションの作成に使用される要求されたイベント通知の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="eee50-114">Represents a requested event notification type that is used to create a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eee50-115">親要素</span><span class="sxs-lookup"><span data-stu-id="eee50-115">Parent elements</span></span>

|<span data-ttu-id="eee50-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="eee50-116">**Element**</span></span>|<span data-ttu-id="eee50-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="eee50-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eee50-118">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="eee50-118">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="eee50-119">プルベースのイベント通知サブスクリプションに対するサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="eee50-119">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="eee50-120">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="eee50-120">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="eee50-121">プッシュベースのイベント通知サブスクリプションのサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="eee50-121">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="eee50-122">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="eee50-122">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md) <br/> |<span data-ttu-id="eee50-123">ストリーミングイベント通知サブスクリプションへのサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="eee50-123">Represents a subscription to a streaming event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eee50-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="eee50-124">Text value</span></span>

<span data-ttu-id="eee50-125">なし。</span><span class="sxs-lookup"><span data-stu-id="eee50-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="eee50-126">注釈</span><span class="sxs-lookup"><span data-stu-id="eee50-126">Remarks</span></span>

<span data-ttu-id="eee50-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="eee50-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eee50-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="eee50-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eee50-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="eee50-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eee50-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="eee50-130">Schema Name</span></span>  <br/> |<span data-ttu-id="eee50-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="eee50-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="eee50-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="eee50-132">Validation File</span></span>  <br/> |<span data-ttu-id="eee50-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="eee50-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eee50-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="eee50-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="eee50-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="eee50-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eee50-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="eee50-136">See also</span></span>



[<span data-ttu-id="eee50-137">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="eee50-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="eee50-138">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="eee50-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="eee50-139">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="eee50-139">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="eee50-140">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="eee50-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


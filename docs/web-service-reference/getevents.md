---
title: GetEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetEvents
api_type:
- schema
ms.assetid: 22d4da6b-d8a8-484f-82c4-3e4b8f5431cd
description: GetEvents 要素では、プル クライアントがサーバーからの通知を要求に使用する操作を表します。
ms.openlocfilehash: e7b24207bff579a2f5230676d6520452f96fe0ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760704"
---
# <a name="getevents"></a><span data-ttu-id="97003-103">GetEvents</span><span class="sxs-lookup"><span data-stu-id="97003-103">GetEvents</span></span>

<span data-ttu-id="97003-104">**GetEvents**要素では、プル クライアントがサーバーからの通知を要求に使用する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="97003-104">The **GetEvents** element represents the operation used by pull clients to request notifications from the server.</span></span> 
  
[<span data-ttu-id="97003-105">GetEvents</span><span class="sxs-lookup"><span data-stu-id="97003-105">GetEvents</span></span>](getevents.md)
  
```xml
<GetEvents>
   <SubscriptionId/>
   <Watermark/>
</GetEvents>
```

 <span data-ttu-id="97003-106">**GetEventsType**</span><span class="sxs-lookup"><span data-stu-id="97003-106">**GetEventsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97003-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="97003-107">Attributes and elements</span></span>

<span data-ttu-id="97003-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="97003-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97003-109">属性</span><span class="sxs-lookup"><span data-stu-id="97003-109">Attributes</span></span>

<span data-ttu-id="97003-110">なし。</span><span class="sxs-lookup"><span data-stu-id="97003-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97003-111">子要素</span><span class="sxs-lookup"><span data-stu-id="97003-111">Child elements</span></span>

|<span data-ttu-id="97003-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="97003-112">**Element**</span></span>|<span data-ttu-id="97003-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="97003-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97003-114">サブスクリプション Id (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="97003-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="97003-115">イベントを照会するサブスクリプションの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="97003-115">Represents the identifier for a subscription that is queried for events.</span></span>  <br/> |
|[<span data-ttu-id="97003-116">透かし</span><span class="sxs-lookup"><span data-stu-id="97003-116">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="97003-117">クライアントに返される最新のウォーターマークを表します。</span><span class="sxs-lookup"><span data-stu-id="97003-117">Represents the last watermark returned to the client.</span></span> <span data-ttu-id="97003-118">このサブスクリプションの GetEvents が呼び出されていない場合、クライアントは、Subscribe 要求から返された透かしを使用します。</span><span class="sxs-lookup"><span data-stu-id="97003-118">If GetEvents has not been called for this subscription, the client uses the watermark returned from the Subscribe request.</span></span> <span data-ttu-id="97003-119">それ以外の場合、最新の GetEvents 応答の最後のイベントからのウォーターマークが使用されます。</span><span class="sxs-lookup"><span data-stu-id="97003-119">Otherwise, the watermark from the last event in the last GetEvents response is used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="97003-120">親要素</span><span class="sxs-lookup"><span data-stu-id="97003-120">Parent elements</span></span>

<span data-ttu-id="97003-121">なし。</span><span class="sxs-lookup"><span data-stu-id="97003-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="97003-122">備考</span><span class="sxs-lookup"><span data-stu-id="97003-122">Remarks</span></span>

<span data-ttu-id="97003-123">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="97003-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97003-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="97003-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97003-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="97003-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="97003-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="97003-126">Schema name</span></span>  <br/> |<span data-ttu-id="97003-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="97003-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="97003-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="97003-128">Validation file</span></span>  <br/> |<span data-ttu-id="97003-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="97003-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="97003-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="97003-130">Can be empty</span></span>  <br/> |<span data-ttu-id="97003-131">false</span><span class="sxs-lookup"><span data-stu-id="97003-131">false</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97003-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="97003-132">See also</span></span>



[<span data-ttu-id="97003-133">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="97003-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="97003-134">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="97003-134">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="97003-135">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="97003-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)


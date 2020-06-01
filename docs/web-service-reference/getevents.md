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
description: GetEvents 要素は、サーバーからの通知を要求するためにプルクライアントによって使用される操作を表します。
ms.openlocfilehash: 004f782ccd32b3c5e501080bfc59419a6e7d9ce4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462501"
---
# <a name="getevents"></a><span data-ttu-id="c9bd0-103">GetEvents</span><span class="sxs-lookup"><span data-stu-id="c9bd0-103">GetEvents</span></span>

<span data-ttu-id="c9bd0-104">**GetEvents**要素は、サーバーからの通知を要求するためにプルクライアントによって使用される操作を表します。</span><span class="sxs-lookup"><span data-stu-id="c9bd0-104">The **GetEvents** element represents the operation used by pull clients to request notifications from the server.</span></span> 
  
[<span data-ttu-id="c9bd0-105">GetEvents</span><span class="sxs-lookup"><span data-stu-id="c9bd0-105">GetEvents</span></span>](getevents.md)
  
```xml
<GetEvents>
   <SubscriptionId/>
   <Watermark/>
</GetEvents>
```

 <span data-ttu-id="c9bd0-106">**GetEventsType**</span><span class="sxs-lookup"><span data-stu-id="c9bd0-106">**GetEventsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9bd0-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c9bd0-107">Attributes and elements</span></span>

<span data-ttu-id="c9bd0-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c9bd0-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9bd0-109">属性</span><span class="sxs-lookup"><span data-stu-id="c9bd0-109">Attributes</span></span>

<span data-ttu-id="c9bd0-110">なし。</span><span class="sxs-lookup"><span data-stu-id="c9bd0-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9bd0-111">子要素</span><span class="sxs-lookup"><span data-stu-id="c9bd0-111">Child elements</span></span>

|<span data-ttu-id="c9bd0-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="c9bd0-112">**Element**</span></span>|<span data-ttu-id="c9bd0-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="c9bd0-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9bd0-114">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="c9bd0-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="c9bd0-115">イベントを照会するサブスクリプションの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="c9bd0-115">Represents the identifier for a subscription that is queried for events.</span></span>  <br/> |
|[<span data-ttu-id="c9bd0-116">Watermark</span><span class="sxs-lookup"><span data-stu-id="c9bd0-116">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="c9bd0-117">クライアントに最後に返されたウォーターマークを表します。</span><span class="sxs-lookup"><span data-stu-id="c9bd0-117">Represents the last watermark returned to the client.</span></span> <span data-ttu-id="c9bd0-118">このサブスクリプションに対して GetEvents が呼び出されていない場合、クライアントは Subscribe 要求から返されたウォーターマークを使用します。</span><span class="sxs-lookup"><span data-stu-id="c9bd0-118">If GetEvents has not been called for this subscription, the client uses the watermark returned from the Subscribe request.</span></span> <span data-ttu-id="c9bd0-119">それ以外の場合は、最後の GetEvents 応答の最後のイベントのウォーターマークが使用されます。</span><span class="sxs-lookup"><span data-stu-id="c9bd0-119">Otherwise, the watermark from the last event in the last GetEvents response is used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c9bd0-120">親要素</span><span class="sxs-lookup"><span data-stu-id="c9bd0-120">Parent elements</span></span>

<span data-ttu-id="c9bd0-121">なし。</span><span class="sxs-lookup"><span data-stu-id="c9bd0-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c9bd0-122">注釈</span><span class="sxs-lookup"><span data-stu-id="c9bd0-122">Remarks</span></span>

<span data-ttu-id="c9bd0-123">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="c9bd0-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9bd0-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c9bd0-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9bd0-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="c9bd0-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c9bd0-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c9bd0-126">Schema name</span></span>  <br/> |<span data-ttu-id="c9bd0-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="c9bd0-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c9bd0-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c9bd0-128">Validation file</span></span>  <br/> |<span data-ttu-id="c9bd0-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c9bd0-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c9bd0-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c9bd0-130">Can be empty</span></span>  <br/> |<span data-ttu-id="c9bd0-131">false</span><span class="sxs-lookup"><span data-stu-id="c9bd0-131">false</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9bd0-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="c9bd0-132">See also</span></span>



[<span data-ttu-id="c9bd0-133">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="c9bd0-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="c9bd0-134">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="c9bd0-134">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="c9bd0-135">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="c9bd0-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)


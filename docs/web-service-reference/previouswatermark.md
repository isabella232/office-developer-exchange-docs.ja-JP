---
title: PreviousWatermark
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PreviousWatermark
api_type:
- schema
ms.assetid: 474f4f7c-47da-47d4-8126-230012172fb5
description: PreviousWatermark 要素は、サブスクリプションのためにクライアントに正常に通信された最新イベントのウォーターマークを表します。
ms.openlocfilehash: 93c6f90d0866ae13618391b8544ab593fe33922b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832886"
---
# <a name="previouswatermark"></a><span data-ttu-id="21388-103">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="21388-103">PreviousWatermark</span></span>

<span data-ttu-id="21388-104">**PreviousWatermark**要素は、サブスクリプションのためにクライアントに正常に通信された最新イベントのウォーターマークを表します。</span><span class="sxs-lookup"><span data-stu-id="21388-104">The **PreviousWatermark** element represents the watermark of the latest event that was successfully communicated to the client for the subscription.</span></span> 
  
```xml
<PreviousWatermark/>
```

 <span data-ttu-id="21388-105">**WatermarkType**</span><span class="sxs-lookup"><span data-stu-id="21388-105">**WatermarkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21388-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="21388-106">Attributes and elements</span></span>

<span data-ttu-id="21388-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="21388-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21388-108">属性</span><span class="sxs-lookup"><span data-stu-id="21388-108">Attributes</span></span>

<span data-ttu-id="21388-109">なし。</span><span class="sxs-lookup"><span data-stu-id="21388-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="21388-110">子要素</span><span class="sxs-lookup"><span data-stu-id="21388-110">Child elements</span></span>

<span data-ttu-id="21388-111">なし。</span><span class="sxs-lookup"><span data-stu-id="21388-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="21388-112">親要素</span><span class="sxs-lookup"><span data-stu-id="21388-112">Parent elements</span></span>

|<span data-ttu-id="21388-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="21388-113">**Element**</span></span>|<span data-ttu-id="21388-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="21388-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21388-115">通知</span><span class="sxs-lookup"><span data-stu-id="21388-115">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="21388-116">サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="21388-116">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="21388-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="21388-117">Text value</span></span>

<span data-ttu-id="21388-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="21388-118">A text value is required.</span></span> <span data-ttu-id="21388-119">テキスト値は、最新のウォーターマークを表します。</span><span class="sxs-lookup"><span data-stu-id="21388-119">The text value represents the latest watermark.</span></span> <span data-ttu-id="21388-120">テキスト値は、空の文字列にすることはできません。</span><span class="sxs-lookup"><span data-stu-id="21388-120">The text value cannot be an empty string.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="21388-121">備考</span><span class="sxs-lookup"><span data-stu-id="21388-121">Remarks</span></span>

<span data-ttu-id="21388-122">**PreviousWatermark**プロパティは、最後の成功の通知を決定するときにクライアントに便利です。</span><span class="sxs-lookup"><span data-stu-id="21388-122">The **PreviousWatermark** property is useful to the client in determining the last successful notification.</span></span> <span data-ttu-id="21388-123">たとえば、サブスクリプションには 1、2、および 3 の透かしを使用して次の 3 つのイベント、3 の**PreviousWatermark**値を持つ次の通知が送信される場合は、クライアントは受信した最後の通知のウォーターマークの値にこの値を比較できます。</span><span class="sxs-lookup"><span data-stu-id="21388-123">For example, if a subscription has three events with watermarks 1, 2, and 3, and the next notification is sent with a **PreviousWatermark** value of 3, the client can compare this value to the Watermark value of the last notification received.</span></span> <span data-ttu-id="21388-124">これにより、クライアントのイベントの継続性を確保します。</span><span class="sxs-lookup"><span data-stu-id="21388-124">This enables the client to ensure the continuity of events.</span></span> 
  
<span data-ttu-id="21388-125">プッシュ クライアントは、 **PreviousWatermark**は、クライアント側のローカル最新既知のウォーターマークと比較されます。</span><span class="sxs-lookup"><span data-stu-id="21388-125">For push clients, the **PreviousWatermark** is compared to the local, client-side last known watermark.</span></span> <span data-ttu-id="21388-126">値が異なる場合は、クライアントがイベント通知を見逃しているし、ローカルの最新のウォーターマークを使用してサブスクリプションを再確立する必要があります。</span><span class="sxs-lookup"><span data-stu-id="21388-126">If the values are different, the client has missed an event notification and should reestablish a subscription by using the latest local watermark.</span></span> <span data-ttu-id="21388-127">たとえば、プッシュ クライアントは、1、2、および 3 の透かしを使用してサブスクリプションの 3 つのイベントを受け取るし、次の通知は、5 の**PreviousWatermark**値が付属しています、クライアントが少なくとも 1 つの通知が失われた、新しいサブスクリプションを作成する必要があります。透かしとして 3 を渡しています。</span><span class="sxs-lookup"><span data-stu-id="21388-127">For example, if a push client receives three events for a subscription with watermarks 1, 2, and 3, and the next notification comes with a **PreviousWatermark** value of 5, the client has missed at least one notification and should create a new subscription, passing a 3 as the watermark.</span></span> 
  
<span data-ttu-id="21388-128">クライアントの場合、プル、 **PreviousWatermark**の値になります GetEvents 呼び出しのクライアントが含まれている[ウォーターマーク](watermark.md)と同じです。</span><span class="sxs-lookup"><span data-stu-id="21388-128">In the case of a pull client, the value of **PreviousWatermark** will be the same as the [Watermark](watermark.md) included by the client in the GetEvents call.</span></span> 
  
<span data-ttu-id="21388-129">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="21388-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21388-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="21388-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21388-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="21388-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="21388-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="21388-132">Schema Name</span></span>  <br/> |<span data-ttu-id="21388-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="21388-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="21388-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="21388-134">Validation File</span></span>  <br/> |<span data-ttu-id="21388-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="21388-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="21388-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="21388-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="21388-137">False</span><span class="sxs-lookup"><span data-stu-id="21388-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21388-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="21388-138">See also</span></span>



[<span data-ttu-id="21388-139">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="21388-139">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="21388-140">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="21388-140">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="21388-141">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="21388-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)


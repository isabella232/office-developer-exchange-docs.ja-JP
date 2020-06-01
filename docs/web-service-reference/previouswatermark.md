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
description: PreviousWatermark 要素は、サブスクリプションのためにクライアントに正常に伝達された最新のイベントのウォーターマークを表します。
ms.openlocfilehash: 1b26a645a5ec6dbbd2874b118f968866aadc32af
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461654"
---
# <a name="previouswatermark"></a><span data-ttu-id="5539f-103">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="5539f-103">PreviousWatermark</span></span>

<span data-ttu-id="5539f-104">**PreviousWatermark**要素は、サブスクリプションのためにクライアントに正常に伝達された最新のイベントのウォーターマークを表します。</span><span class="sxs-lookup"><span data-stu-id="5539f-104">The **PreviousWatermark** element represents the watermark of the latest event that was successfully communicated to the client for the subscription.</span></span> 
  
```xml
<PreviousWatermark/>
```

 <span data-ttu-id="5539f-105">**WatermarkType**</span><span class="sxs-lookup"><span data-stu-id="5539f-105">**WatermarkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5539f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5539f-106">Attributes and elements</span></span>

<span data-ttu-id="5539f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5539f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5539f-108">属性</span><span class="sxs-lookup"><span data-stu-id="5539f-108">Attributes</span></span>

<span data-ttu-id="5539f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5539f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5539f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5539f-110">Child elements</span></span>

<span data-ttu-id="5539f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5539f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5539f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5539f-112">Parent elements</span></span>

|<span data-ttu-id="5539f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5539f-113">**Element**</span></span>|<span data-ttu-id="5539f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5539f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5539f-115">通知</span><span class="sxs-lookup"><span data-stu-id="5539f-115">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5539f-116">サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5539f-116">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5539f-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5539f-117">Text value</span></span>

<span data-ttu-id="5539f-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="5539f-118">A text value is required.</span></span> <span data-ttu-id="5539f-119">Text 値は、最新のウォーターマークを表します。</span><span class="sxs-lookup"><span data-stu-id="5539f-119">The text value represents the latest watermark.</span></span> <span data-ttu-id="5539f-120">テキスト値を空の文字列にすることはできません。</span><span class="sxs-lookup"><span data-stu-id="5539f-120">The text value cannot be an empty string.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5539f-121">注釈</span><span class="sxs-lookup"><span data-stu-id="5539f-121">Remarks</span></span>

<span data-ttu-id="5539f-122">**PreviousWatermark**プロパティは、最後に成功した通知を判断するためにクライアントに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="5539f-122">The **PreviousWatermark** property is useful to the client in determining the last successful notification.</span></span> <span data-ttu-id="5539f-123">たとえば、サブスクリプションにウォーターマーク1、2、3の3つのイベントがあり、次の通知が**PreviousWatermark**値3で送信される場合、クライアントはこの値を、最後に受信した通知のウォーターマーク値と比較できます。</span><span class="sxs-lookup"><span data-stu-id="5539f-123">For example, if a subscription has three events with watermarks 1, 2, and 3, and the next notification is sent with a **PreviousWatermark** value of 3, the client can compare this value to the Watermark value of the last notification received.</span></span> <span data-ttu-id="5539f-124">これにより、クライアントはイベントの連続性を確保できます。</span><span class="sxs-lookup"><span data-stu-id="5539f-124">This enables the client to ensure the continuity of events.</span></span> 
  
<span data-ttu-id="5539f-125">プッシュクライアントの場合、 **PreviousWatermark**は、ローカルのクライアント側の最後の既知のウォーターマークと比較されます。</span><span class="sxs-lookup"><span data-stu-id="5539f-125">For push clients, the **PreviousWatermark** is compared to the local, client-side last known watermark.</span></span> <span data-ttu-id="5539f-126">値が異なる場合、クライアントはイベント通知を失ったため、最新のローカルウォーターマークを使用してサブスクリプションを再確立する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5539f-126">If the values are different, the client has missed an event notification and should reestablish a subscription by using the latest local watermark.</span></span> <span data-ttu-id="5539f-127">たとえば、プッシュクライアントがウォーターマーク1、2、3を含むサブスクリプションに対して3つのイベントを受信し、次の通知の**PreviousWatermark**値が5である場合、クライアントは少なくとも1つの通知を失ったため、新しいサブスクリプションを作成して3をウォーターマークとして渡す必要があります。</span><span class="sxs-lookup"><span data-stu-id="5539f-127">For example, if a push client receives three events for a subscription with watermarks 1, 2, and 3, and the next notification comes with a **PreviousWatermark** value of 5, the client has missed at least one notification and should create a new subscription, passing a 3 as the watermark.</span></span> 
  
<span data-ttu-id="5539f-128">プルクライアントの場合、 **PreviousWatermark**の値は、GetEvents 呼び出しのクライアントによって含まれる[ウォーターマーク](watermark.md)と同じになります。</span><span class="sxs-lookup"><span data-stu-id="5539f-128">In the case of a pull client, the value of **PreviousWatermark** will be the same as the [Watermark](watermark.md) included by the client in the GetEvents call.</span></span> 
  
<span data-ttu-id="5539f-129">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="5539f-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5539f-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5539f-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5539f-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="5539f-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5539f-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5539f-132">Schema Name</span></span>  <br/> |<span data-ttu-id="5539f-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="5539f-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="5539f-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5539f-134">Validation File</span></span>  <br/> |<span data-ttu-id="5539f-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="5539f-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5539f-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5539f-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="5539f-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="5539f-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5539f-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="5539f-138">See also</span></span>



[<span data-ttu-id="5539f-139">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="5539f-139">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="5539f-140">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="5539f-140">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="5539f-141">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="5539f-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)


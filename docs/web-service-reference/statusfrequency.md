---
title: StatusFrequency
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StatusFrequency
api_type:
- schema
ms.assetid: 917474e2-a426-4166-b825-53783a41dad4
description: StatusFrequency 要素は、サーバーによって再試行が試行される最大タイムアウト時間 (分単位) を表します。
ms.openlocfilehash: db14ecfd54584188b3da16bb369db6c8089c70f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468244"
---
# <a name="statusfrequency"></a><span data-ttu-id="d3cd1-103">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="d3cd1-103">StatusFrequency</span></span>

<span data-ttu-id="d3cd1-104">**Statusfrequency**要素は、サーバーによって再試行が試行される最大タイムアウト時間 (分単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="d3cd1-104">The **StatusFrequency** element represents the maximum timeout value, in minutes, in which retries are attempted by the server.</span></span> 
  
[<span data-ttu-id="d3cd1-105">登録</span><span class="sxs-lookup"><span data-stu-id="d3cd1-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="d3cd1-106">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="d3cd1-106">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
[<span data-ttu-id="d3cd1-107">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="d3cd1-107">StatusFrequency</span></span>](statusfrequency.md)
  
```XML
<StatusFrequency/>
```

 <span data-ttu-id="d3cd1-108">**SubscriptionStatusFrequencyType**</span><span class="sxs-lookup"><span data-stu-id="d3cd1-108">**SubscriptionStatusFrequencyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3cd1-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d3cd1-109">Attributes and elements</span></span>

<span data-ttu-id="d3cd1-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d3cd1-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3cd1-111">属性</span><span class="sxs-lookup"><span data-stu-id="d3cd1-111">Attributes</span></span>

<span data-ttu-id="d3cd1-112">なし。</span><span class="sxs-lookup"><span data-stu-id="d3cd1-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3cd1-113">子要素</span><span class="sxs-lookup"><span data-stu-id="d3cd1-113">Child elements</span></span>

<span data-ttu-id="d3cd1-114">なし。</span><span class="sxs-lookup"><span data-stu-id="d3cd1-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d3cd1-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d3cd1-115">Parent elements</span></span>

|<span data-ttu-id="d3cd1-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="d3cd1-116">**Element**</span></span>|<span data-ttu-id="d3cd1-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="d3cd1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3cd1-118">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="d3cd1-118">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="d3cd1-119">プッシュベースのイベント通知サブスクリプションのサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="d3cd1-119">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d3cd1-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d3cd1-120">Text value</span></span>

<span data-ttu-id="d3cd1-121">この要素を使用する場合は、整数を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="d3cd1-121">A text value that represents an integer is required if this element is used.</span></span> <span data-ttu-id="d3cd1-122">この要素で使用できる値は、1 ~ 1440 の範囲です。</span><span class="sxs-lookup"><span data-stu-id="d3cd1-122">The possible values for this element are 1 to 1440, inclusive.</span></span> <span data-ttu-id="d3cd1-123">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="d3cd1-123">This element is optional.</span></span> <span data-ttu-id="d3cd1-124">既定値は 30 分です。</span><span class="sxs-lookup"><span data-stu-id="d3cd1-124">The default value is 30 minutes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d3cd1-125">注釈</span><span class="sxs-lookup"><span data-stu-id="d3cd1-125">Remarks</span></span>

<span data-ttu-id="d3cd1-126">**Statusfrequency**値は、プッシュ通知またはクライアントからのステータス ping に対する応答が受信されない場合に、プッシュ通知を再試行するためにサーバーによって使用されます。</span><span class="sxs-lookup"><span data-stu-id="d3cd1-126">The **StatusFrequency** value is used by the server to retry a push notification when it does not receive a response to a push notification or status ping from the client.</span></span> <span data-ttu-id="d3cd1-127">サーバーが応答を受信しない場合は、通知の送信を停止する前に、何度か通知の送信を再試行します。</span><span class="sxs-lookup"><span data-stu-id="d3cd1-127">If the server does not receive a response, it retries sending the notification several times before it stops sending the notification.</span></span> <span data-ttu-id="d3cd1-128">EWS では、既定の再試行間隔は30秒で、その後の再試行は常に最後の再試行間隔の2倍の時間になります。</span><span class="sxs-lookup"><span data-stu-id="d3cd1-128">In EWS, the default retry interval is 30 seconds and subsequent retries are always double the time of the last retry interval.</span></span> <span data-ttu-id="d3cd1-129">サーバー上の他の負荷が原因で遅延が発生する可能性があるので、再試行時間は正確ではありません。</span><span class="sxs-lookup"><span data-stu-id="d3cd1-129">Retry times are not exact as they can be delayed due to other loads on the server.</span></span> <span data-ttu-id="d3cd1-130">次の表に、既定の**Statusfrequency**値 (サーバーで遅延が発生しなかった場合) によって割り当てられた30分間の再試行間隔を示します。</span><span class="sxs-lookup"><span data-stu-id="d3cd1-130">The following table shows how the retry intervals occur in the 30 minutes allotted by the default **StatusFrequency** value (assuming the server did not encounter any delays).</span></span> 
  
|<span data-ttu-id="d3cd1-131">**再試行**</span><span class="sxs-lookup"><span data-stu-id="d3cd1-131">**Retry**</span></span>|<span data-ttu-id="d3cd1-132">**秒**</span><span class="sxs-lookup"><span data-stu-id="d3cd1-132">**Seconds**</span></span>|<span data-ttu-id="d3cd1-133">**Time**</span><span class="sxs-lookup"><span data-stu-id="d3cd1-133">**Time**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d3cd1-134">.0</span><span class="sxs-lookup"><span data-stu-id="d3cd1-134">0</span></span>  <br/> |<span data-ttu-id="d3cd1-135">.0</span><span class="sxs-lookup"><span data-stu-id="d3cd1-135">0</span></span>  <br/> |<span data-ttu-id="d3cd1-136">初期同期</span><span class="sxs-lookup"><span data-stu-id="d3cd1-136">Initial sync</span></span>  <br/> |
|<span data-ttu-id="d3cd1-137">1 </span><span class="sxs-lookup"><span data-stu-id="d3cd1-137">1</span></span>  <br/> |<span data-ttu-id="d3cd1-138">31</span><span class="sxs-lookup"><span data-stu-id="d3cd1-138">30</span></span>  <br/> |<span data-ttu-id="d3cd1-139">00:30</span><span class="sxs-lookup"><span data-stu-id="d3cd1-139">00:30</span></span>  <br/> |
|<span data-ttu-id="d3cd1-140">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d3cd1-140">2</span></span>  <br/> |<span data-ttu-id="d3cd1-141">60</span><span class="sxs-lookup"><span data-stu-id="d3cd1-141">60</span></span>  <br/> |<span data-ttu-id="d3cd1-142">01:00</span><span class="sxs-lookup"><span data-stu-id="d3cd1-142">01:00</span></span>  <br/> |
|<span data-ttu-id="d3cd1-143">1/3</span><span class="sxs-lookup"><span data-stu-id="d3cd1-143">3</span></span>  <br/> |<span data-ttu-id="d3cd1-144">120</span><span class="sxs-lookup"><span data-stu-id="d3cd1-144">120</span></span>  <br/> |<span data-ttu-id="d3cd1-145">02:00</span><span class="sxs-lookup"><span data-stu-id="d3cd1-145">02:00</span></span>  <br/> |
|<span data-ttu-id="d3cd1-146">4 </span><span class="sxs-lookup"><span data-stu-id="d3cd1-146">4</span></span>  <br/> |<span data-ttu-id="d3cd1-147">240</span><span class="sxs-lookup"><span data-stu-id="d3cd1-147">240</span></span>  <br/> |<span data-ttu-id="d3cd1-148">04:00</span><span class="sxs-lookup"><span data-stu-id="d3cd1-148">04:00</span></span>  <br/> |
|<span data-ttu-id="d3cd1-149">5 </span><span class="sxs-lookup"><span data-stu-id="d3cd1-149">5</span></span>  <br/> |<span data-ttu-id="d3cd1-150">480</span><span class="sxs-lookup"><span data-stu-id="d3cd1-150">480</span></span>  <br/> |<span data-ttu-id="d3cd1-151">08:00</span><span class="sxs-lookup"><span data-stu-id="d3cd1-151">08:00</span></span>  <br/> |
|<span data-ttu-id="d3cd1-152">6 </span><span class="sxs-lookup"><span data-stu-id="d3cd1-152">6</span></span>  <br/> |<span data-ttu-id="d3cd1-153">960</span><span class="sxs-lookup"><span data-stu-id="d3cd1-153">960</span></span>  <br/> |<span data-ttu-id="d3cd1-154">16:00</span><span class="sxs-lookup"><span data-stu-id="d3cd1-154">16:00</span></span>  <br/> |
|<span data-ttu-id="d3cd1-155">7 </span><span class="sxs-lookup"><span data-stu-id="d3cd1-155">7</span></span>  <br/> |<span data-ttu-id="d3cd1-156">1920</span><span class="sxs-lookup"><span data-stu-id="d3cd1-156">1920</span></span>  <br/> |<span data-ttu-id="d3cd1-157">32:00- **Statusfrequency**の既定値である30を超えたため、再試行を送信しない</span><span class="sxs-lookup"><span data-stu-id="d3cd1-157">32:00 - **StatusFrequency** default value of 30 exceeded, retry not sent</span></span>  <br/> |
   
<span data-ttu-id="d3cd1-158">**Statusfrequency**で指定された時間を超える期間、クライアントがサーバーからの通知メッセージを受信しない場合、クライアントはサブスクリプションの再作成などの操作を実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d3cd1-158">If the client does not receive notification messages from the server for a period of time that exceeds twice the time specified by **StatusFrequency**, the client should take an action such as recreating the subscription.</span></span> 
  
<span data-ttu-id="d3cd1-159">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d3cd1-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3cd1-160">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d3cd1-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3cd1-161">Namespace</span><span class="sxs-lookup"><span data-stu-id="d3cd1-161">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d3cd1-162">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d3cd1-162">Schema name</span></span>  <br/> |<span data-ttu-id="d3cd1-163">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d3cd1-163">Types schema</span></span>  <br/> |
|<span data-ttu-id="d3cd1-164">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d3cd1-164">Validation file</span></span>  <br/> |<span data-ttu-id="d3cd1-165">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d3cd1-165">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d3cd1-166">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d3cd1-166">Can be empty</span></span>  <br/> |<span data-ttu-id="d3cd1-167">正しくない</span><span class="sxs-lookup"><span data-stu-id="d3cd1-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3cd1-168">関連項目</span><span class="sxs-lookup"><span data-stu-id="d3cd1-168">See also</span></span>



[<span data-ttu-id="d3cd1-169">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="d3cd1-169">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="d3cd1-170">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="d3cd1-170">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="d3cd1-171">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="d3cd1-171">Unsubscribe operation</span></span>](unsubscribe-operation.md)
  
[<span data-ttu-id="d3cd1-172">Watermark</span><span class="sxs-lookup"><span data-stu-id="d3cd1-172">Watermark</span></span>](watermark.md)


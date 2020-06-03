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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468244"
---
# <a name="statusfrequency"></a><span data-ttu-id="d610c-103">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="d610c-103">StatusFrequency</span></span>

<span data-ttu-id="d610c-104">**Statusfrequency**要素は、サーバーによって再試行が試行される最大タイムアウト時間 (分単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="d610c-104">The **StatusFrequency** element represents the maximum timeout value, in minutes, in which retries are attempted by the server.</span></span> 
  
[<span data-ttu-id="d610c-105">登録</span><span class="sxs-lookup"><span data-stu-id="d610c-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="d610c-106">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="d610c-106">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
[<span data-ttu-id="d610c-107">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="d610c-107">StatusFrequency</span></span>](statusfrequency.md)
  
```XML
<StatusFrequency/>
```

 <span data-ttu-id="d610c-108">**SubscriptionStatusFrequencyType**</span><span class="sxs-lookup"><span data-stu-id="d610c-108">**SubscriptionStatusFrequencyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d610c-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d610c-109">Attributes and elements</span></span>

<span data-ttu-id="d610c-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d610c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d610c-111">属性</span><span class="sxs-lookup"><span data-stu-id="d610c-111">Attributes</span></span>

<span data-ttu-id="d610c-112">なし。</span><span class="sxs-lookup"><span data-stu-id="d610c-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d610c-113">子要素</span><span class="sxs-lookup"><span data-stu-id="d610c-113">Child elements</span></span>

<span data-ttu-id="d610c-114">なし。</span><span class="sxs-lookup"><span data-stu-id="d610c-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d610c-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d610c-115">Parent elements</span></span>

|<span data-ttu-id="d610c-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="d610c-116">**Element**</span></span>|<span data-ttu-id="d610c-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="d610c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d610c-118">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="d610c-118">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="d610c-119">プッシュベースのイベント通知サブスクリプションのサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="d610c-119">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d610c-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d610c-120">Text value</span></span>

<span data-ttu-id="d610c-121">この要素を使用する場合は、整数を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="d610c-121">A text value that represents an integer is required if this element is used.</span></span> <span data-ttu-id="d610c-122">この要素で使用できる値は、1 ~ 1440 の範囲です。</span><span class="sxs-lookup"><span data-stu-id="d610c-122">The possible values for this element are 1 to 1440, inclusive.</span></span> <span data-ttu-id="d610c-123">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="d610c-123">This element is optional.</span></span> <span data-ttu-id="d610c-124">既定値は 30 分です。</span><span class="sxs-lookup"><span data-stu-id="d610c-124">The default value is 30 minutes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d610c-125">注釈</span><span class="sxs-lookup"><span data-stu-id="d610c-125">Remarks</span></span>

<span data-ttu-id="d610c-126">**Statusfrequency**値は、プッシュ通知またはクライアントからのステータス ping に対する応答が受信されない場合に、プッシュ通知を再試行するためにサーバーによって使用されます。</span><span class="sxs-lookup"><span data-stu-id="d610c-126">The **StatusFrequency** value is used by the server to retry a push notification when it does not receive a response to a push notification or status ping from the client.</span></span> <span data-ttu-id="d610c-127">サーバーが応答を受信しない場合は、通知の送信を停止する前に、何度か通知の送信を再試行します。</span><span class="sxs-lookup"><span data-stu-id="d610c-127">If the server does not receive a response, it retries sending the notification several times before it stops sending the notification.</span></span> <span data-ttu-id="d610c-128">EWS では、既定の再試行間隔は30秒で、その後の再試行は常に最後の再試行間隔の2倍の時間になります。</span><span class="sxs-lookup"><span data-stu-id="d610c-128">In EWS, the default retry interval is 30 seconds and subsequent retries are always double the time of the last retry interval.</span></span> <span data-ttu-id="d610c-129">サーバー上の他の負荷が原因で遅延が発生する可能性があるので、再試行時間は正確ではありません。</span><span class="sxs-lookup"><span data-stu-id="d610c-129">Retry times are not exact as they can be delayed due to other loads on the server.</span></span> <span data-ttu-id="d610c-130">次の表に、既定の**Statusfrequency**値 (サーバーで遅延が発生しなかった場合) によって割り当てられた30分間の再試行間隔を示します。</span><span class="sxs-lookup"><span data-stu-id="d610c-130">The following table shows how the retry intervals occur in the 30 minutes allotted by the default **StatusFrequency** value (assuming the server did not encounter any delays).</span></span> 
  
|<span data-ttu-id="d610c-131">**再試行**</span><span class="sxs-lookup"><span data-stu-id="d610c-131">**Retry**</span></span>|<span data-ttu-id="d610c-132">**秒**</span><span class="sxs-lookup"><span data-stu-id="d610c-132">**Seconds**</span></span>|<span data-ttu-id="d610c-133">**Time**</span><span class="sxs-lookup"><span data-stu-id="d610c-133">**Time**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d610c-134">.0</span><span class="sxs-lookup"><span data-stu-id="d610c-134">0</span></span>  <br/> |<span data-ttu-id="d610c-135">.0</span><span class="sxs-lookup"><span data-stu-id="d610c-135">0</span></span>  <br/> |<span data-ttu-id="d610c-136">初期同期</span><span class="sxs-lookup"><span data-stu-id="d610c-136">Initial sync</span></span>  <br/> |
|<span data-ttu-id="d610c-137">1 </span><span class="sxs-lookup"><span data-stu-id="d610c-137">1</span></span>  <br/> |<span data-ttu-id="d610c-138">31</span><span class="sxs-lookup"><span data-stu-id="d610c-138">30</span></span>  <br/> |<span data-ttu-id="d610c-139">00:30</span><span class="sxs-lookup"><span data-stu-id="d610c-139">00:30</span></span>  <br/> |
|<span data-ttu-id="d610c-140">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d610c-140">2</span></span>  <br/> |<span data-ttu-id="d610c-141">60</span><span class="sxs-lookup"><span data-stu-id="d610c-141">60</span></span>  <br/> |<span data-ttu-id="d610c-142">01:00</span><span class="sxs-lookup"><span data-stu-id="d610c-142">01:00</span></span>  <br/> |
|<span data-ttu-id="d610c-143">1/3</span><span class="sxs-lookup"><span data-stu-id="d610c-143">3</span></span>  <br/> |<span data-ttu-id="d610c-144">120</span><span class="sxs-lookup"><span data-stu-id="d610c-144">120</span></span>  <br/> |<span data-ttu-id="d610c-145">02:00</span><span class="sxs-lookup"><span data-stu-id="d610c-145">02:00</span></span>  <br/> |
|<span data-ttu-id="d610c-146">4 </span><span class="sxs-lookup"><span data-stu-id="d610c-146">4</span></span>  <br/> |<span data-ttu-id="d610c-147">240</span><span class="sxs-lookup"><span data-stu-id="d610c-147">240</span></span>  <br/> |<span data-ttu-id="d610c-148">04:00</span><span class="sxs-lookup"><span data-stu-id="d610c-148">04:00</span></span>  <br/> |
|<span data-ttu-id="d610c-149">5 </span><span class="sxs-lookup"><span data-stu-id="d610c-149">5</span></span>  <br/> |<span data-ttu-id="d610c-150">480</span><span class="sxs-lookup"><span data-stu-id="d610c-150">480</span></span>  <br/> |<span data-ttu-id="d610c-151">08:00</span><span class="sxs-lookup"><span data-stu-id="d610c-151">08:00</span></span>  <br/> |
|<span data-ttu-id="d610c-152">6 </span><span class="sxs-lookup"><span data-stu-id="d610c-152">6</span></span>  <br/> |<span data-ttu-id="d610c-153">960</span><span class="sxs-lookup"><span data-stu-id="d610c-153">960</span></span>  <br/> |<span data-ttu-id="d610c-154">16:00</span><span class="sxs-lookup"><span data-stu-id="d610c-154">16:00</span></span>  <br/> |
|<span data-ttu-id="d610c-155">7 </span><span class="sxs-lookup"><span data-stu-id="d610c-155">7</span></span>  <br/> |<span data-ttu-id="d610c-156">1920</span><span class="sxs-lookup"><span data-stu-id="d610c-156">1920</span></span>  <br/> |<span data-ttu-id="d610c-157">32:00- **Statusfrequency**の既定値である30を超えたため、再試行を送信しない</span><span class="sxs-lookup"><span data-stu-id="d610c-157">32:00 - **StatusFrequency** default value of 30 exceeded, retry not sent</span></span>  <br/> |
   
<span data-ttu-id="d610c-158">**Statusfrequency**で指定された時間を超える期間、クライアントがサーバーからの通知メッセージを受信しない場合、クライアントはサブスクリプションの再作成などの操作を実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d610c-158">If the client does not receive notification messages from the server for a period of time that exceeds twice the time specified by **StatusFrequency**, the client should take an action such as recreating the subscription.</span></span> 
  
<span data-ttu-id="d610c-159">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d610c-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d610c-160">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d610c-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d610c-161">Namespace</span><span class="sxs-lookup"><span data-stu-id="d610c-161">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d610c-162">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d610c-162">Schema name</span></span>  <br/> |<span data-ttu-id="d610c-163">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d610c-163">Types schema</span></span>  <br/> |
|<span data-ttu-id="d610c-164">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d610c-164">Validation file</span></span>  <br/> |<span data-ttu-id="d610c-165">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d610c-165">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d610c-166">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d610c-166">Can be empty</span></span>  <br/> |<span data-ttu-id="d610c-167">正しくない</span><span class="sxs-lookup"><span data-stu-id="d610c-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d610c-168">関連項目</span><span class="sxs-lookup"><span data-stu-id="d610c-168">See also</span></span>



[<span data-ttu-id="d610c-169">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="d610c-169">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="d610c-170">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="d610c-170">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="d610c-171">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="d610c-171">Unsubscribe operation</span></span>](unsubscribe-operation.md)
  
[<span data-ttu-id="d610c-172">Watermark</span><span class="sxs-lookup"><span data-stu-id="d610c-172">Watermark</span></span>](watermark.md)


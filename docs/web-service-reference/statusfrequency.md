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
description: StatusFrequency 要素は、分単位、サーバーの再試行が行わ、タイムアウトの最大値を表します。
ms.openlocfilehash: 402f8978c0ec6b377dfa020f23595c8954509a07
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833589"
---
# <a name="statusfrequency"></a><span data-ttu-id="18ba9-103">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="18ba9-103">StatusFrequency</span></span>

<span data-ttu-id="18ba9-104">**StatusFrequency**要素は、分単位、サーバーの再試行が行わ、タイムアウトの最大値を表します。</span><span class="sxs-lookup"><span data-stu-id="18ba9-104">The **StatusFrequency** element represents the maximum timeout value, in minutes, in which retries are attempted by the server.</span></span> 
  
[<span data-ttu-id="18ba9-105">購読</span><span class="sxs-lookup"><span data-stu-id="18ba9-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="18ba9-106">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="18ba9-106">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
[<span data-ttu-id="18ba9-107">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="18ba9-107">StatusFrequency</span></span>](statusfrequency.md)
  
```XML
<StatusFrequency/>
```

 <span data-ttu-id="18ba9-108">**SubscriptionStatusFrequencyType**</span><span class="sxs-lookup"><span data-stu-id="18ba9-108">**SubscriptionStatusFrequencyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18ba9-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="18ba9-109">Attributes and elements</span></span>

<span data-ttu-id="18ba9-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="18ba9-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18ba9-111">属性</span><span class="sxs-lookup"><span data-stu-id="18ba9-111">Attributes</span></span>

<span data-ttu-id="18ba9-112">なし。</span><span class="sxs-lookup"><span data-stu-id="18ba9-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18ba9-113">子要素</span><span class="sxs-lookup"><span data-stu-id="18ba9-113">Child elements</span></span>

<span data-ttu-id="18ba9-114">なし。</span><span class="sxs-lookup"><span data-stu-id="18ba9-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="18ba9-115">親要素</span><span class="sxs-lookup"><span data-stu-id="18ba9-115">Parent elements</span></span>

|<span data-ttu-id="18ba9-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="18ba9-116">**Element**</span></span>|<span data-ttu-id="18ba9-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="18ba9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18ba9-118">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="18ba9-118">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="18ba9-119">プッシュ ベースのイベント通知サブスクリプションをサブスクリプションを表します。</span><span class="sxs-lookup"><span data-stu-id="18ba9-119">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="18ba9-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="18ba9-120">Text value</span></span>

<span data-ttu-id="18ba9-121">整数値を表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="18ba9-121">A text value that represents an integer is required if this element is used.</span></span> <span data-ttu-id="18ba9-122">この要素の値は、1 から 1440 の範囲です。</span><span class="sxs-lookup"><span data-stu-id="18ba9-122">The possible values for this element are 1 to 1440, inclusive.</span></span> <span data-ttu-id="18ba9-123">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="18ba9-123">This element is optional.</span></span> <span data-ttu-id="18ba9-124">既定値は、30 分です。</span><span class="sxs-lookup"><span data-stu-id="18ba9-124">The default value is 30 minutes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="18ba9-125">備考</span><span class="sxs-lookup"><span data-stu-id="18ba9-125">Remarks</span></span>

<span data-ttu-id="18ba9-126">**StatusFrequency**値は、クライアントからのプッシュ通知やステータスの ping に応答を受信しません、プッシュ通知を再試行するのには、サーバーによって使用されます。</span><span class="sxs-lookup"><span data-stu-id="18ba9-126">The **StatusFrequency** value is used by the server to retry a push notification when it does not receive a response to a push notification or status ping from the client.</span></span> <span data-ttu-id="18ba9-127">サーバーが応答を受信しない場合は、通知の送信を停止する前に、何回か、通知の送信を再試行します。</span><span class="sxs-lookup"><span data-stu-id="18ba9-127">If the server does not receive a response, it retries sending the notification several times before it stops sending the notification.</span></span> <span data-ttu-id="18ba9-128">EWS、既定の再試行間隔は、30 秒でそれ以降の再試行は、常に最後の再試行間隔の時間が 2 倍。</span><span class="sxs-lookup"><span data-stu-id="18ba9-128">In EWS, the default retry interval is 30 seconds and subsequent retries are always double the time of the last retry interval.</span></span> <span data-ttu-id="18ba9-129">サーバー上の他の負荷のための遅延と、再試行の回数は正確ではないです。</span><span class="sxs-lookup"><span data-stu-id="18ba9-129">Retry times are not exact as they can be delayed due to other loads on the server.</span></span> <span data-ttu-id="18ba9-130">(サーバーは、任意の遅延を検出しなかったと仮定した場合)、デフォルトの**StatusFrequency**値に割り当てられている 30 分以内に再試行の間隔が発生する方法を次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="18ba9-130">The following table shows how the retry intervals occur in the 30 minutes allotted by the default **StatusFrequency** value (assuming the server did not encounter any delays).</span></span> 
  
|<span data-ttu-id="18ba9-131">**再試行**</span><span class="sxs-lookup"><span data-stu-id="18ba9-131">**Retry**</span></span>|<span data-ttu-id="18ba9-132">**秒**</span><span class="sxs-lookup"><span data-stu-id="18ba9-132">**Seconds**</span></span>|<span data-ttu-id="18ba9-133">**時間**</span><span class="sxs-lookup"><span data-stu-id="18ba9-133">**Time**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="18ba9-134">0</span><span class="sxs-lookup"><span data-stu-id="18ba9-134">0</span></span>  <br/> |<span data-ttu-id="18ba9-135">0</span><span class="sxs-lookup"><span data-stu-id="18ba9-135">0</span></span>  <br/> |<span data-ttu-id="18ba9-136">初期同期</span><span class="sxs-lookup"><span data-stu-id="18ba9-136">Initial sync</span></span>  <br/> |
|<span data-ttu-id="18ba9-137">1</span><span class="sxs-lookup"><span data-stu-id="18ba9-137">1</span></span>  <br/> |<span data-ttu-id="18ba9-138">30</span><span class="sxs-lookup"><span data-stu-id="18ba9-138">30</span></span>  <br/> |<span data-ttu-id="18ba9-139">00:30</span><span class="sxs-lookup"><span data-stu-id="18ba9-139">00:30</span></span>  <br/> |
|<span data-ttu-id="18ba9-140">2</span><span class="sxs-lookup"><span data-stu-id="18ba9-140">2</span></span>  <br/> |<span data-ttu-id="18ba9-141">60</span><span class="sxs-lookup"><span data-stu-id="18ba9-141">60</span></span>  <br/> |<span data-ttu-id="18ba9-142">01:00</span><span class="sxs-lookup"><span data-stu-id="18ba9-142">01:00</span></span>  <br/> |
|<span data-ttu-id="18ba9-143">3</span><span class="sxs-lookup"><span data-stu-id="18ba9-143">3</span></span>  <br/> |<span data-ttu-id="18ba9-144">120</span><span class="sxs-lookup"><span data-stu-id="18ba9-144">120</span></span>  <br/> |<span data-ttu-id="18ba9-145">02:00</span><span class="sxs-lookup"><span data-stu-id="18ba9-145">02:00</span></span>  <br/> |
|<span data-ttu-id="18ba9-146">4</span><span class="sxs-lookup"><span data-stu-id="18ba9-146">4</span></span>  <br/> |<span data-ttu-id="18ba9-147">240</span><span class="sxs-lookup"><span data-stu-id="18ba9-147">240</span></span>  <br/> |<span data-ttu-id="18ba9-148">04:00</span><span class="sxs-lookup"><span data-stu-id="18ba9-148">04:00</span></span>  <br/> |
|<span data-ttu-id="18ba9-149">5</span><span class="sxs-lookup"><span data-stu-id="18ba9-149">5</span></span>  <br/> |<span data-ttu-id="18ba9-150">480</span><span class="sxs-lookup"><span data-stu-id="18ba9-150">480</span></span>  <br/> |<span data-ttu-id="18ba9-151">08:00</span><span class="sxs-lookup"><span data-stu-id="18ba9-151">08:00</span></span>  <br/> |
|<span data-ttu-id="18ba9-152">6</span><span class="sxs-lookup"><span data-stu-id="18ba9-152">6</span></span>  <br/> |<span data-ttu-id="18ba9-153">960</span><span class="sxs-lookup"><span data-stu-id="18ba9-153">960</span></span>  <br/> |<span data-ttu-id="18ba9-154">16:00</span><span class="sxs-lookup"><span data-stu-id="18ba9-154">16:00</span></span>  <br/> |
|<span data-ttu-id="18ba9-155">7</span><span class="sxs-lookup"><span data-stu-id="18ba9-155">7</span></span>  <br/> |<span data-ttu-id="18ba9-156">1920</span><span class="sxs-lookup"><span data-stu-id="18ba9-156">1920</span></span>  <br/> |<span data-ttu-id="18ba9-157">32:00 - **StatusFrequency**の既定値の 30 を超えると、再試行が送信されません。</span><span class="sxs-lookup"><span data-stu-id="18ba9-157">32:00 - **StatusFrequency** default value of 30 exceeded, retry not sent</span></span>  <br/> |
   
<span data-ttu-id="18ba9-158">クライアントを受信しない場合の通知メッセージ、サーバーから**StatusFrequency**で指定されたタイムの 2 倍を超える時間の期間、クライアントはサブスクリプションを再作成するなどアクションを実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="18ba9-158">If the client does not receive notification messages from the server for a period of time that exceeds twice the time specified by **StatusFrequency**, the client should take an action such as recreating the subscription.</span></span> 
  
<span data-ttu-id="18ba9-159">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="18ba9-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18ba9-160">要素情報</span><span class="sxs-lookup"><span data-stu-id="18ba9-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18ba9-161">名前空間</span><span class="sxs-lookup"><span data-stu-id="18ba9-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18ba9-162">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="18ba9-162">Schema name</span></span>  <br/> |<span data-ttu-id="18ba9-163">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="18ba9-163">Types schema</span></span>  <br/> |
|<span data-ttu-id="18ba9-164">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="18ba9-164">Validation file</span></span>  <br/> |<span data-ttu-id="18ba9-165">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="18ba9-165">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="18ba9-166">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="18ba9-166">Can be empty</span></span>  <br/> |<span data-ttu-id="18ba9-167">False</span><span class="sxs-lookup"><span data-stu-id="18ba9-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18ba9-168">関連項目</span><span class="sxs-lookup"><span data-stu-id="18ba9-168">See also</span></span>



[<span data-ttu-id="18ba9-169">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="18ba9-169">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="18ba9-170">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="18ba9-170">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="18ba9-171">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="18ba9-171">Unsubscribe operation</span></span>](unsubscribe-operation.md)
  
[<span data-ttu-id="18ba9-172">透かし</span><span class="sxs-lookup"><span data-stu-id="18ba9-172">Watermark</span></span>](watermark.md)


---
title: GetEvents 操作
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
ms.assetid: f268efe5-9a1a-41a2-b6a6-51fcde7720a1
description: GetEvents 操作は、クライアント アクセス サーバーから、プル サブスクリプションのクライアントによって、通知を要求する使用されます。 GetEvents 操作の応答では、項目と以降のメールボックスに最後に通知するイベントの配列を返します。
ms.openlocfilehash: 1a23a9d570a4554e54becb7927f25dff89888c74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760705"
---
# <a name="getevents-operation"></a><span data-ttu-id="1857b-104">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="1857b-104">GetEvents operation</span></span>

<span data-ttu-id="1857b-105">**GetEvents**操作は、クライアント アクセス サーバーから、プル サブスクリプションのクライアントによって、通知を要求する使用されます。</span><span class="sxs-lookup"><span data-stu-id="1857b-105">The **GetEvents** operation is used by pull subscription clients to request notifications from the Client Access server.</span></span> <span data-ttu-id="1857b-106">**GetEvents**操作の応答では、項目と以降のメールボックスに最後に通知するイベントの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="1857b-106">The **GetEvents** operation response returns an array of items and events that have occurred in a mailbox since the last the notification.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="1857b-107">**DeleteUserConfiguration**操作は、イベント通知システムの移動イベントをトリガーします。</span><span class="sxs-lookup"><span data-stu-id="1857b-107">The **DeleteUserConfiguration** operation will trigger a move event for the event notification system.</span></span> <span data-ttu-id="1857b-108">ユーザー設定のオブジェクトを移動するが、ごみ箱をあさる。</span><span class="sxs-lookup"><span data-stu-id="1857b-108">The user configuration object will be moved to the dumpster.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1857b-109">備考</span><span class="sxs-lookup"><span data-stu-id="1857b-109">Remarks</span></span>

<span data-ttu-id="1857b-110">予定表アイテムへの変更は、複数のイベントの生成があります。</span><span class="sxs-lookup"><span data-stu-id="1857b-110">Changes to Calendar items may result in the generation of multiple events.</span></span> <span data-ttu-id="1857b-111">これらのイベントは、一時アイテムが作成される、メールボックスでは、通常の予定表の操作、またはその両方の一部として変更される空き時間情報データ記憶域の項目の結果です。</span><span class="sxs-lookup"><span data-stu-id="1857b-111">These events are the result of temporary items being created in the mailbox, free/busy data storage items being changed as part of the normal Calendar operations, or both.</span></span> <span data-ttu-id="1857b-112">項目のイベント クラスの"IPM.SchedulePlus.FreeBusy.BinaryData」は、Web サービス クライアントによって無視されます。</span><span class="sxs-lookup"><span data-stu-id="1857b-112">Events for item class "IPM.SchedulePlus.FreeBusy.BinaryData" should be ignored by Web service clients.</span></span> <span data-ttu-id="1857b-113">一時アイテムを削除して作成されます。したがって、これらの項目を取得しようとすると場合、エラーが返ります、項目が見つからなかったことを示します。</span><span class="sxs-lookup"><span data-stu-id="1857b-113">These temporary items are deleted after they are created; therefore, if an attempt is made to retrieve these items, an error will be returned that states that the item was not found.</span></span>
  
## <a name="getevents-request-example"></a><span data-ttu-id="1857b-114">GetEvents 要求の例</span><span class="sxs-lookup"><span data-stu-id="1857b-114">GetEvents request example</span></span>

### <a name="description"></a><span data-ttu-id="1857b-115">説明</span><span class="sxs-lookup"><span data-stu-id="1857b-115">Description</span></span>

<span data-ttu-id="1857b-116">次の例では、イベントとサブスクリプションの識別子とウォーターマークで識別されるサブスクリプションに関連付けられている項目を要求する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="1857b-116">The following example shows how to request the events and items that are associated with a subscription that is identified by the subscription identifier and watermark.</span></span>
  
### <a name="code"></a><span data-ttu-id="1857b-117">コード</span><span class="sxs-lookup"><span data-stu-id="1857b-117">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetEvents xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <Watermark>AAAAAMAGAAAAAAAAAQ==</Watermark>
    </GetEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getevents-request-elements"></a><span data-ttu-id="1857b-118">GetEvents 要求要素</span><span class="sxs-lookup"><span data-stu-id="1857b-118">GetEvents Request Elements</span></span>

<span data-ttu-id="1857b-119">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="1857b-119">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="1857b-120">GetEvents</span><span class="sxs-lookup"><span data-stu-id="1857b-120">GetEvents</span></span>](getevents.md)
    
- [<span data-ttu-id="1857b-121">サブスクリプション Id (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="1857b-121">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="1857b-122">透かし</span><span class="sxs-lookup"><span data-stu-id="1857b-122">Watermark</span></span>](watermark.md)
    
## <a name="successful-getevents-response-example"></a><span data-ttu-id="1857b-123">GetEvents 応答の成功の例</span><span class="sxs-lookup"><span data-stu-id="1857b-123">Successful GetEvents response example</span></span>

### <a name="description"></a><span data-ttu-id="1857b-124">説明</span><span class="sxs-lookup"><span data-stu-id="1857b-124">Description</span></span>

<span data-ttu-id="1857b-125">最後の通知要求がサーバーに送信された後、次の応答の例は 2 つの新しいメール メッセージの存在を通知を示します。</span><span class="sxs-lookup"><span data-stu-id="1857b-125">The following example of a response shows a notification of the existence of two new mail messages since the last notification request was sent to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="1857b-126">コード</span><span class="sxs-lookup"><span data-stu-id="1857b-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetEventsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Notification>
            <t:SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</t:SubscriptionId>
            <t:PreviousWatermark>AAAAAMAGAAAAAAAAAQ==</t:PreviousWatermark>
            <t:MoreEvents>false</t:MoreEvents>
            <t:NewMailEvent>
              <t:Watermark>AAAAAM4GAAAAAAAAAQ==</t:Watermark>
              <t:TimeStamp>2006-08-22T00:36:29Z</t:TimeStamp>
              <t:ItemId Id="AQApAHR" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQApAH" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
            <t:NewMailEvent>
              <t:Watermark>AAAAAOQGAAAAAAAAAQ==</t:Watermark>
              <t:TimeStamp>2006-08-22T01:00:50Z</t:TimeStamp>
              <t:ItemId Id="AQApAHRw" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQApAH" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
          </m:Notification>
        </m:GetEventsResponseMessage>
      </m:ResponseMessages>
    </GetEventsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="1857b-127">コメント</span><span class="sxs-lookup"><span data-stu-id="1857b-127">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="1857b-128">アイテムおよびフォルダーの識別子は、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="1857b-128">The item and folder identifiers have been shortened to preserve readability.</span></span> 
  
### <a name="getevents-response-elements"></a><span data-ttu-id="1857b-129">GetEvents 応答の要素</span><span class="sxs-lookup"><span data-stu-id="1857b-129">GetEvents response elements</span></span>

<span data-ttu-id="1857b-130">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="1857b-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="1857b-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="1857b-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="1857b-132">GetEventsResponse</span><span class="sxs-lookup"><span data-stu-id="1857b-132">GetEventsResponse</span></span>](geteventsresponse.md)
    
- [<span data-ttu-id="1857b-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1857b-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="1857b-134">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1857b-134">GetEventsResponseMessage</span></span>](geteventsresponsemessage.md)
    
- [<span data-ttu-id="1857b-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1857b-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1857b-136">通知</span><span class="sxs-lookup"><span data-stu-id="1857b-136">Notification</span></span>](notification-ex15websvcsotherref.md)
    
- [<span data-ttu-id="1857b-137">サブスクリプション Id (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="1857b-137">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="1857b-138">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="1857b-138">PreviousWatermark</span></span>](previouswatermark.md)
    
- [<span data-ttu-id="1857b-139">イベント</span><span class="sxs-lookup"><span data-stu-id="1857b-139">MoreEvents</span></span>](moreevents.md)
    
- [<span data-ttu-id="1857b-140">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="1857b-140">NewMailEvent</span></span>](newmailevent.md)
    
- [<span data-ttu-id="1857b-141">透かし</span><span class="sxs-lookup"><span data-stu-id="1857b-141">Watermark</span></span>](watermark.md)
    
- [<span data-ttu-id="1857b-142">タイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="1857b-142">TimeStamp</span></span>](timestamp.md)
    
- [<span data-ttu-id="1857b-143">ItemId</span><span class="sxs-lookup"><span data-stu-id="1857b-143">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="1857b-144">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="1857b-144">ParentFolderId</span></span>](parentfolderid.md)
    
<span data-ttu-id="1857b-145">**GetEvents**操作の応答メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="1857b-145">To find other options for the response message of the **GetEvents** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="1857b-146">[通知](notification-ex15websvcsotherref.md)の要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="1857b-146">Start at the [Notification](notification-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="getevents-error-response-example"></a><span data-ttu-id="1857b-147">GetEvents エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="1857b-147">GetEvents Error response example</span></span>

### <a name="description"></a><span data-ttu-id="1857b-148">説明</span><span class="sxs-lookup"><span data-stu-id="1857b-148">Description</span></span>

<span data-ttu-id="1857b-149">**GetEvents**要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1857b-149">The following example shows an error response to a **GetEvents** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="1857b-150">コード</span><span class="sxs-lookup"><span data-stu-id="1857b-150">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetEventsResponseMessage ResponseClass="Error">
          <m:MessageText>Access is denied. Only the subscription owner may access the subscription.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionAccessDenied</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:GetEventsResponseMessage>
      </m:ResponseMessages>
    </GetEventsResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="remarks"></a><span data-ttu-id="1857b-151">備考</span><span class="sxs-lookup"><span data-stu-id="1857b-151">Remarks</span></span>

<span data-ttu-id="1857b-152">**GetEvents**要求を処理するときにクライアント アクセス サーバーは、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="1857b-152">When processing a **GetEvents** request, the Client Access server performs the following steps:</span></span> 
  
1. <span data-ttu-id="1857b-153">要求のサブスクリプション Id が、クライアント アクセス サーバーでホストされている有効なサブスクリプションを使用することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1857b-153">The SubscriptionID of the request is confirmed to be a valid subscription that is hosted on the Client Access server.</span></span> <span data-ttu-id="1857b-154">そうでない場合、 **GetEvents**呼び出しは失敗します。</span><span class="sxs-lookup"><span data-stu-id="1857b-154">If it is not, the **GetEvents** call fails.</span></span> 
    
2. <span data-ttu-id="1857b-155">要求の認証済みユーザーの SMTP アドレスは、サブスクリプションを作成したユーザーの SMTP アドレスと比較されます。</span><span class="sxs-lookup"><span data-stu-id="1857b-155">The SMTP address of the authenticated user for the request is compared to the SMTP address of the user who created the subscription.</span></span> <span data-ttu-id="1857b-156">それらが一致しない場合は、 **GetEvents**要求が失敗します。</span><span class="sxs-lookup"><span data-stu-id="1857b-156">If they do not match, the **GetEvents** request fails.</span></span> 
    
3. <span data-ttu-id="1857b-157">サブスクリプションのキューでは、クライアントに送信されるを待機しているイベントが照会されます。</span><span class="sxs-lookup"><span data-stu-id="1857b-157">The subscription queue is queried for events that are waiting to be sent to the client.</span></span> <span data-ttu-id="1857b-158">キューが空でない場合は、キューから最初の 50 のイベントがキューから取得し、通知にエンコードされました。</span><span class="sxs-lookup"><span data-stu-id="1857b-158">If the queue is not empty, the first 50 events from the queue are pulled from the queue and encoded into a notification.</span></span>
    
4. <span data-ttu-id="1857b-159">キュー内のイベントが見つからない場合、StatusEvent が生成され、通知の応答にエンコードします。</span><span class="sxs-lookup"><span data-stu-id="1857b-159">If no events are found in the queue, a StatusEvent is generated and encoded into a notification response.</span></span>
    
5. <span data-ttu-id="1857b-160">通知の応答がクライアントに返されます。</span><span class="sxs-lookup"><span data-stu-id="1857b-160">The notification response is returned to the client.</span></span>
    
6. <span data-ttu-id="1857b-161">サブスクリプションのキューからの通知に含まれているイベントを削除し、クライアント アクセス サーバー ローカル最新のウォーターマークのサブスクリプションが返される最後のイベントのウォーターマークを設定します。</span><span class="sxs-lookup"><span data-stu-id="1857b-161">The events that are included in the notification are removed from the subscription queue and the Client Access server local last watermark for the subscription is set to the watermark of the last event that is returned.</span></span>
    
7. <span data-ttu-id="1857b-162">サブスクリプションのタイムアウト タイマーがリセットされます。</span><span class="sxs-lookup"><span data-stu-id="1857b-162">The timeout timer for the subscription is reset.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="1857b-163">関連項目</span><span class="sxs-lookup"><span data-stu-id="1857b-163">See also</span></span>



[<span data-ttu-id="1857b-164">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="1857b-164">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="1857b-165">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="1857b-165">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="1857b-166">プル サブスクリプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="1857b-166">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)


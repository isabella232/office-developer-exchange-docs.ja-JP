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
description: GetEvents 操作は、プルサブスクリプションクライアントがクライアントアクセスサーバーからの通知を要求するために使用されます。 GetEvents 操作の応答は、最後の通知以降にメールボックスで発生したアイテムとイベントの配列を返します。
ms.openlocfilehash: 9258fd003c242911866aa7abbca5eba2b9582223
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462515"
---
# <a name="getevents-operation"></a><span data-ttu-id="09784-104">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="09784-104">GetEvents operation</span></span>

<span data-ttu-id="09784-105">**GetEvents**操作は、プルサブスクリプションクライアントがクライアントアクセスサーバーからの通知を要求するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="09784-105">The **GetEvents** operation is used by pull subscription clients to request notifications from the Client Access server.</span></span> <span data-ttu-id="09784-106">**GetEvents**操作の応答は、最後の通知以降にメールボックスで発生したアイテムとイベントの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="09784-106">The **GetEvents** operation response returns an array of items and events that have occurred in a mailbox since the last the notification.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="09784-107">**Deleteuserconfiguration**操作は、イベント通知システムの移動イベントをトリガーします。</span><span class="sxs-lookup"><span data-stu-id="09784-107">The **DeleteUserConfiguration** operation will trigger a move event for the event notification system.</span></span> <span data-ttu-id="09784-108">ユーザー構成オブジェクトは、収集に移動されます。</span><span class="sxs-lookup"><span data-stu-id="09784-108">The user configuration object will be moved to the dumpster.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="09784-109">注釈</span><span class="sxs-lookup"><span data-stu-id="09784-109">Remarks</span></span>

<span data-ttu-id="09784-110">予定表アイテムの変更によって、複数のイベントが生成されることがあります。</span><span class="sxs-lookup"><span data-stu-id="09784-110">Changes to Calendar items may result in the generation of multiple events.</span></span> <span data-ttu-id="09784-111">これらのイベントは、メールボックス内に作成された一時アイテム、空き時間情報データストレージアイテムが通常の予定表の操作の一部として変更された結果、またはその両方で発生します。</span><span class="sxs-lookup"><span data-stu-id="09784-111">These events are the result of temporary items being created in the mailbox, free/busy data storage items being changed as part of the normal Calendar operations, or both.</span></span> <span data-ttu-id="09784-112">アイテムクラス "IPM.Web サービスクライアントでは、SchedulePlus データ "を無視する必要があります。</span><span class="sxs-lookup"><span data-stu-id="09784-112">Events for item class "IPM.SchedulePlus.FreeBusy.BinaryData" should be ignored by Web service clients.</span></span> <span data-ttu-id="09784-113">これらの一時アイテムは、作成後に削除されます。そのため、これらのアイテムを取得しようとすると、アイテムが見つからなかったことを示すエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="09784-113">These temporary items are deleted after they are created; therefore, if an attempt is made to retrieve these items, an error will be returned that states that the item was not found.</span></span>
  
## <a name="getevents-request-example"></a><span data-ttu-id="09784-114">GetEvents 要求の例</span><span class="sxs-lookup"><span data-stu-id="09784-114">GetEvents request example</span></span>

### <a name="description"></a><span data-ttu-id="09784-115">説明</span><span class="sxs-lookup"><span data-stu-id="09784-115">Description</span></span>

<span data-ttu-id="09784-116">次の例は、サブスクリプション識別子とウォーターマークで識別されるサブスクリプションに関連付けられたイベントとアイテムを要求する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="09784-116">The following example shows how to request the events and items that are associated with a subscription that is identified by the subscription identifier and watermark.</span></span>
  
### <a name="code"></a><span data-ttu-id="09784-117">コード</span><span class="sxs-lookup"><span data-stu-id="09784-117">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetEvents xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <Watermark>AAAAAMAGAAAAAAAAAQ==</Watermark>
    </GetEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getevents-request-elements"></a><span data-ttu-id="09784-118">GetEvents Request 要素</span><span class="sxs-lookup"><span data-stu-id="09784-118">GetEvents Request Elements</span></span>

<span data-ttu-id="09784-119">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="09784-119">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="09784-120">GetEvents</span><span class="sxs-lookup"><span data-stu-id="09784-120">GetEvents</span></span>](getevents.md)
    
- [<span data-ttu-id="09784-121">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="09784-121">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="09784-122">Watermark</span><span class="sxs-lookup"><span data-stu-id="09784-122">Watermark</span></span>](watermark.md)
    
## <a name="successful-getevents-response-example"></a><span data-ttu-id="09784-123">Successful GetEvents response の例</span><span class="sxs-lookup"><span data-stu-id="09784-123">Successful GetEvents response example</span></span>

### <a name="description"></a><span data-ttu-id="09784-124">説明</span><span class="sxs-lookup"><span data-stu-id="09784-124">Description</span></span>

<span data-ttu-id="09784-125">次の応答の例は、前回の通知要求がサーバーに送信されてから、2つの新しいメールメッセージが存在するという通知を示しています。</span><span class="sxs-lookup"><span data-stu-id="09784-125">The following example of a response shows a notification of the existence of two new mail messages since the last notification request was sent to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="09784-126">コード</span><span class="sxs-lookup"><span data-stu-id="09784-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="09784-127">コメント</span><span class="sxs-lookup"><span data-stu-id="09784-127">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="09784-128">読みやすくするために、アイテムとフォルダーの識別子が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="09784-128">The item and folder identifiers have been shortened to preserve readability.</span></span> 
  
### <a name="getevents-response-elements"></a><span data-ttu-id="09784-129">GetEvents response 要素</span><span class="sxs-lookup"><span data-stu-id="09784-129">GetEvents response elements</span></span>

<span data-ttu-id="09784-130">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="09784-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="09784-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="09784-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="09784-132">Getイベント応答</span><span class="sxs-lookup"><span data-stu-id="09784-132">GetEventsResponse</span></span>](geteventsresponse.md)
    
- [<span data-ttu-id="09784-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="09784-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="09784-134">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="09784-134">GetEventsResponseMessage</span></span>](geteventsresponsemessage.md)
    
- [<span data-ttu-id="09784-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="09784-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="09784-136">通知</span><span class="sxs-lookup"><span data-stu-id="09784-136">Notification</span></span>](notification-ex15websvcsotherref.md)
    
- [<span data-ttu-id="09784-137">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="09784-137">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="09784-138">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="09784-138">PreviousWatermark</span></span>](previouswatermark.md)
    
- [<span data-ttu-id="09784-139">その他のイベント</span><span class="sxs-lookup"><span data-stu-id="09784-139">MoreEvents</span></span>](moreevents.md)
    
- [<span data-ttu-id="09784-140">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="09784-140">NewMailEvent</span></span>](newmailevent.md)
    
- [<span data-ttu-id="09784-141">Watermark</span><span class="sxs-lookup"><span data-stu-id="09784-141">Watermark</span></span>](watermark.md)
    
- [<span data-ttu-id="09784-142">示</span><span class="sxs-lookup"><span data-stu-id="09784-142">TimeStamp</span></span>](timestamp.md)
    
- [<span data-ttu-id="09784-143">ItemId</span><span class="sxs-lookup"><span data-stu-id="09784-143">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="09784-144">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="09784-144">ParentFolderId</span></span>](parentfolderid.md)
    
<span data-ttu-id="09784-145">**GetEvents**操作の応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09784-145">To find other options for the response message of the **GetEvents** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="09784-146">[通知](notification-ex15websvcsotherref.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="09784-146">Start at the [Notification](notification-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="getevents-error-response-example"></a><span data-ttu-id="09784-147">GetEvents エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="09784-147">GetEvents Error response example</span></span>

### <a name="description"></a><span data-ttu-id="09784-148">説明</span><span class="sxs-lookup"><span data-stu-id="09784-148">Description</span></span>

<span data-ttu-id="09784-149">次の例は、 **GetEvents**要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="09784-149">The following example shows an error response to a **GetEvents** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="09784-150">コード</span><span class="sxs-lookup"><span data-stu-id="09784-150">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="remarks"></a><span data-ttu-id="09784-151">注釈</span><span class="sxs-lookup"><span data-stu-id="09784-151">Remarks</span></span>

<span data-ttu-id="09784-152">**GetEvents**要求を処理する場合、クライアントアクセスサーバーは次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="09784-152">When processing a **GetEvents** request, the Client Access server performs the following steps:</span></span> 
  
1. <span data-ttu-id="09784-153">要求の SubscriptionID は、クライアントアクセスサーバーでホストされている有効なサブスクリプションであることが確認されます。</span><span class="sxs-lookup"><span data-stu-id="09784-153">The SubscriptionID of the request is confirmed to be a valid subscription that is hosted on the Client Access server.</span></span> <span data-ttu-id="09784-154">そうでない場合、 **GetEvents**呼び出しは失敗します。</span><span class="sxs-lookup"><span data-stu-id="09784-154">If it is not, the **GetEvents** call fails.</span></span> 
    
2. <span data-ttu-id="09784-155">要求に対する認証済みユーザーの SMTP アドレスは、サブスクリプションを作成したユーザーの SMTP アドレスと比較されます。</span><span class="sxs-lookup"><span data-stu-id="09784-155">The SMTP address of the authenticated user for the request is compared to the SMTP address of the user who created the subscription.</span></span> <span data-ttu-id="09784-156">一致しない場合、 **GetEvents**要求は失敗します。</span><span class="sxs-lookup"><span data-stu-id="09784-156">If they do not match, the **GetEvents** request fails.</span></span> 
    
3. <span data-ttu-id="09784-157">サブスクリプションキューは、クライアントへの送信を待機しているイベントに対して照会されます。</span><span class="sxs-lookup"><span data-stu-id="09784-157">The subscription queue is queried for events that are waiting to be sent to the client.</span></span> <span data-ttu-id="09784-158">キューが空でない場合、キューから最初の50イベントがプルされ、通知にエンコードされます。</span><span class="sxs-lookup"><span data-stu-id="09784-158">If the queue is not empty, the first 50 events from the queue are pulled from the queue and encoded into a notification.</span></span>
    
4. <span data-ttu-id="09784-159">キューにイベントが見つからない場合は、StatusEvent が生成され、通知応答にエンコードされます。</span><span class="sxs-lookup"><span data-stu-id="09784-159">If no events are found in the queue, a StatusEvent is generated and encoded into a notification response.</span></span>
    
5. <span data-ttu-id="09784-160">通知応答がクライアントに返されます。</span><span class="sxs-lookup"><span data-stu-id="09784-160">The notification response is returned to the client.</span></span>
    
6. <span data-ttu-id="09784-161">通知に含まれるイベントは、サブスクリプションキューから削除され、サブスクリプションのクライアントアクセスサーバーのローカルの最後のウォーターマークは、返される最後のイベントのウォーターマークに設定されます。</span><span class="sxs-lookup"><span data-stu-id="09784-161">The events that are included in the notification are removed from the subscription queue and the Client Access server local last watermark for the subscription is set to the watermark of the last event that is returned.</span></span>
    
7. <span data-ttu-id="09784-162">サブスクリプションのタイムアウトタイマーはリセットされます。</span><span class="sxs-lookup"><span data-stu-id="09784-162">The timeout timer for the subscription is reset.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="09784-163">関連項目</span><span class="sxs-lookup"><span data-stu-id="09784-163">See also</span></span>



[<span data-ttu-id="09784-164">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="09784-164">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="09784-165">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="09784-165">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="09784-166">プルサブスクリプションの使用</span><span class="sxs-lookup"><span data-stu-id="09784-166">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)


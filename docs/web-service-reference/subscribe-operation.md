---
title: サブスクライブ操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subscribe
api_type:
- schema
ms.assetid: f17c3d08-c79e-41f1-ba31-6e41e7aafd87
description: サブスクライブ操作は、クライアントアプリケーションに対して、プッシュまたはプル通知のどちらかをサブスクライブするために使用されます。 要求メッセージと応答の構造は、イベント通知の種類によって異なることに注意することが重要です。
ms.openlocfilehash: c40e0e434f698c6535ff5d03fd4d45a453959dd6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467047"
---
# <a name="subscribe-operation"></a><span data-ttu-id="455df-104">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="455df-104">Subscribe operation</span></span>

<span data-ttu-id="455df-105">サブスクライブ操作は、クライアントアプリケーションに対して、プッシュまたはプル通知のどちらかをサブスクライブするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="455df-105">The Subscribe operation is used to subscribe client applications to either push or pull notifications.</span></span> <span data-ttu-id="455df-106">要求メッセージと応答の構造は、イベント通知の種類によって異なることに注意することが重要です。</span><span class="sxs-lookup"><span data-stu-id="455df-106">It is important to be aware that the structure of the request messages and responses is different depending on the type of event notification.</span></span> 
  
## <a name="pull-subscription-subscribe-request-example"></a><span data-ttu-id="455df-107">プルサブスクリプションのサブスクライブ要求の例</span><span class="sxs-lookup"><span data-stu-id="455df-107">Pull Subscription Subscribe request example</span></span>

### <a name="description"></a><span data-ttu-id="455df-108">Description</span><span class="sxs-lookup"><span data-stu-id="455df-108">Description</span></span>

<span data-ttu-id="455df-109">次のコード例は、プルイベント通知サブスクリプションをサブスクライブする方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="455df-109">The following code example shows how to subscribe to a pull event notification subscription.</span></span> <span data-ttu-id="455df-110">新しいメールが受信トレイに追加された場合、および受信トレイからアイテムが削除された場合、サブスクリプションはクライアントアプリケーションに通知します。</span><span class="sxs-lookup"><span data-stu-id="455df-110">The subscription informs the client application if new mail is added to the Inbox and if an item is deleted from the Inbox.</span></span> <span data-ttu-id="455df-111">クライアントが10分以内にイベントに関する情報を要求しない場合、サブスクリプションはタイムアウトになります。</span><span class="sxs-lookup"><span data-stu-id="455df-111">The subscription will time out if the client does not request information about events within ten minutes.</span></span> <span data-ttu-id="455df-112">サブスクリプションの有効期限が切れた場合は、通知を引き続き要求するために、新しいサブスクリプションを確立する必要があります。</span><span class="sxs-lookup"><span data-stu-id="455df-112">If the subscription expires, a new subscription must be established to continue to request notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="455df-113">コード</span><span class="sxs-lookup"><span data-stu-id="455df-113">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <PullSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox"/>
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
          <t:EventType>DeletedEvent</t:EventType>
        </t:EventTypes>
        <t:Timeout>10</t:Timeout>
      </PullSubscriptionRequest>
    </Subscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-subscribe-request-elements"></a><span data-ttu-id="455df-114">プルサブスクリプションサブスクライブ要求要素</span><span class="sxs-lookup"><span data-stu-id="455df-114">Pull Subscription Subscribe Request Elements</span></span>

<span data-ttu-id="455df-115">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="455df-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="455df-116">登録</span><span class="sxs-lookup"><span data-stu-id="455df-116">Subscribe</span></span>](subscribe.md)
    
- [<span data-ttu-id="455df-117">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="455df-117">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
    
- [<span data-ttu-id="455df-118">FolderIds</span><span class="sxs-lookup"><span data-stu-id="455df-118">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="455df-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="455df-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="455df-120">EventTypes</span><span class="sxs-lookup"><span data-stu-id="455df-120">EventTypes</span></span>](eventtypes.md)
    
- [<span data-ttu-id="455df-121">EventType</span><span class="sxs-lookup"><span data-stu-id="455df-121">EventType</span></span>](eventtype.md)
    
- [<span data-ttu-id="455df-122">Timeout</span><span class="sxs-lookup"><span data-stu-id="455df-122">Timeout</span></span>](timeout.md)
    
<span data-ttu-id="455df-123">Subscribe 操作の要求メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="455df-123">To find other options for the request message of the Subscribe operation, explore the schema hierarchy.</span></span> <span data-ttu-id="455df-124">[PullSubscriptionRequest](pullsubscriptionrequest.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="455df-124">Start at the [PullSubscriptionRequest](pullsubscriptionrequest.md) element.</span></span> 
  
## <a name="successful-pull-subscription-subscribe-response-example"></a><span data-ttu-id="455df-125">成功したプルサブスクリプションサブスクライブ応答の例</span><span class="sxs-lookup"><span data-stu-id="455df-125">Successful Pull Subscription Subscribe response example</span></span>

### <a name="description"></a><span data-ttu-id="455df-126">Description</span><span class="sxs-lookup"><span data-stu-id="455df-126">Description</span></span>

<span data-ttu-id="455df-127">次の例は、成功したプルサブスクリプション応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="455df-127">The following example shows a successful pull subscription response.</span></span> <span data-ttu-id="455df-128">応答には、サブスクリプションに関連付けられているイベントの配列を取得するために使用されるサブスクリプション識別子とウォーターマークが含まれています。</span><span class="sxs-lookup"><span data-stu-id="455df-128">The response contains the subscription identifier and watermark that is used to get the array of events that are associated with a subscription.</span></span> <span data-ttu-id="455df-129">サブスクリプション識別子は、サブスクリプションからクライアントの登録を解除するためにも使用されます。</span><span class="sxs-lookup"><span data-stu-id="455df-129">The subscription identifier is also used to unsubscribe a client from a subscription.</span></span>
  
### <a name="code"></a><span data-ttu-id="455df-130">コード</span><span class="sxs-lookup"><span data-stu-id="455df-130">Code</span></span>

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
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>39ea5d0f-f062-455e-a1e9-89c0304390f4</m:SubscriptionId>
          <m:Watermark>AAAAAHgGAAAAAAAAAQ==</m:Watermark>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-subscribe-response-elements"></a><span data-ttu-id="455df-131">プルサブスクリプションのサブスクライブ応答要素</span><span class="sxs-lookup"><span data-stu-id="455df-131">Pull Subscription Subscribe response elements</span></span>

<span data-ttu-id="455df-132">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="455df-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="455df-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="455df-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="455df-134">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="455df-134">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="455df-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="455df-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="455df-136">メッセージの表示</span><span class="sxs-lookup"><span data-stu-id="455df-136">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="455df-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="455df-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="455df-138">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="455df-138">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="455df-139">Watermark</span><span class="sxs-lookup"><span data-stu-id="455df-139">Watermark</span></span>](watermark.md)
    
## <a name="pull-subscription-subscribe-error-response-example"></a><span data-ttu-id="455df-140">プルサブスクリプションサブスクライブエラー応答の例</span><span class="sxs-lookup"><span data-stu-id="455df-140">Pull Subscription Subscribe Error response example</span></span>

### <a name="description"></a><span data-ttu-id="455df-141">Description</span><span class="sxs-lookup"><span data-stu-id="455df-141">Description</span></span>

<span data-ttu-id="455df-142">次の例は、Subscribe 要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="455df-142">The following example shows an error response to a Subscribe request.</span></span> <span data-ttu-id="455df-143">このエラーは、代理人アクセスを使用して通知をサブスクライブしようとした場合に発生します。</span><span class="sxs-lookup"><span data-stu-id="455df-143">The error is caused by an attempt to subscribe to notifications by using delegate access.</span></span>
  
### <a name="code"></a><span data-ttu-id="455df-144">コード</span><span class="sxs-lookup"><span data-stu-id="455df-144">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Error">
          <m:MessageText>Subscriptions are not supported for delegate user access.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionDelegateAccessNotSupported</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-error-response-elements"></a><span data-ttu-id="455df-145">プルサブスクリプションエラー応答要素</span><span class="sxs-lookup"><span data-stu-id="455df-145">Pull Subscription Error response elements</span></span>

<span data-ttu-id="455df-146">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="455df-146">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="455df-147">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="455df-147">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="455df-148">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="455df-148">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="455df-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="455df-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="455df-150">メッセージの表示</span><span class="sxs-lookup"><span data-stu-id="455df-150">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="455df-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="455df-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="455df-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="455df-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="455df-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="455df-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="push-subscription-request-example"></a><span data-ttu-id="455df-154">プッシュサブスクリプション要求の例</span><span class="sxs-lookup"><span data-stu-id="455df-154">Push Subscription request example</span></span>

### <a name="description"></a><span data-ttu-id="455df-155">Description</span><span class="sxs-lookup"><span data-stu-id="455df-155">Description</span></span>

<span data-ttu-id="455df-156">次のコード例は、プッシュイベント通知サブスクリプションをサブスクライブする方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="455df-156">The following code example shows how to subscribe to a push event notification subscription.</span></span> <span data-ttu-id="455df-157">要求は、監視するフォルダー、監視するイベントの種類、状態通知の頻度、およびプッシュ通知を待機するクライアント Web サービスの URL を識別します。</span><span class="sxs-lookup"><span data-stu-id="455df-157">The request identifies the folders to monitor, the types of events to monitor, the frequency of status notifications, and the URL of the client Web service that listens for the push notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="455df-158">コード</span><span class="sxs-lookup"><span data-stu-id="455df-158">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <PushSubscriptionRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <FolderIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <DistinguishedFolderId Id="inbox" />
        </FolderIds>
        <EventTypes xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <EventType>NewMailEvent</EventType>
          <EventType>CopiedEvent</EventType>
          <EventType>CreatedEvent</EventType>
          <EventType>DeletedEvent</EventType>
          <EventType>ModifiedEvent</EventType>
          <EventType>MovedEvent</EventType>
        </EventTypes>
        <StatusFrequency xmlns="https://schemas.microsoft.com/exchange/services/2006/types">1</StatusFrequency>
        <URL xmlns="https://schemas.microsoft.com/exchange/services/2006/types">http://clientWebService/Service.asmx</URL>
      </PushSubscriptionRequest>
    </Subscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="455df-159">コメント</span><span class="sxs-lookup"><span data-stu-id="455df-159">Comments</span></span>

<span data-ttu-id="455df-160">プッシュ通知サブスクライブ要求が送信される前に、クライアント Web サービスがセットアップされている必要があります。それ以外の場合、最初の通知は有効なエンドポイントに送信されず、プッシュ通知は失敗します。</span><span class="sxs-lookup"><span data-stu-id="455df-160">The client Web service must be set up before the push notification subscribe request is sent; otherwise, the first notification will not be sent to a valid endpoint and the push notification will fail.</span></span> <span data-ttu-id="455df-161">詳細については、「[プッシュ通知のサンプルアプリケーション](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="455df-161">For more information, see [Push Notification Sample Application](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="455df-162">再度サブスクライブすると、新しい[SubscriptionId (GetEvents)](subscriptionid-getevents.md)が作成されます。</span><span class="sxs-lookup"><span data-stu-id="455df-162">A new [SubscriptionId (GetEvents)](subscriptionid-getevents.md) is created when you resubscribe.</span></span> <span data-ttu-id="455df-163">以前のサブスクリプションのウォーターマークを使用して、前のサブスクリプションが終了した時点でサブスクライブを再度行います。</span><span class="sxs-lookup"><span data-stu-id="455df-163">Use the watermark of a previous subscription to resubscribe at the point where the previous subscription ended.</span></span> 
  
### <a name="push-subscription-request-elements"></a><span data-ttu-id="455df-164">プッシュサブスクリプションの要求要素</span><span class="sxs-lookup"><span data-stu-id="455df-164">Push Subscription Request Elements</span></span>

<span data-ttu-id="455df-165">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="455df-165">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="455df-166">登録</span><span class="sxs-lookup"><span data-stu-id="455df-166">Subscribe</span></span>](subscribe.md)
    
- [<span data-ttu-id="455df-167">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="455df-167">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
    
- [<span data-ttu-id="455df-168">FolderIds</span><span class="sxs-lookup"><span data-stu-id="455df-168">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="455df-169">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="455df-169">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="455df-170">EventTypes</span><span class="sxs-lookup"><span data-stu-id="455df-170">EventTypes</span></span>](eventtypes.md)
    
- [<span data-ttu-id="455df-171">EventType</span><span class="sxs-lookup"><span data-stu-id="455df-171">EventType</span></span>](eventtype.md)
    
- [<span data-ttu-id="455df-172">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="455df-172">StatusFrequency</span></span>](statusfrequency.md)
    
- [<span data-ttu-id="455df-173">.Url</span><span class="sxs-lookup"><span data-stu-id="455df-173">Url </span></span>](url-ex15websvcsotherref.md)
    
## <a name="successful-push-subscription-response-example"></a><span data-ttu-id="455df-174">成功したプッシュサブスクリプション応答の例</span><span class="sxs-lookup"><span data-stu-id="455df-174">Successful Push Subscription response example</span></span>

### <a name="description"></a><span data-ttu-id="455df-175">Description</span><span class="sxs-lookup"><span data-stu-id="455df-175">Description</span></span>

<span data-ttu-id="455df-176">次の例は、成功したプッシュサブスクリプション応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="455df-176">The following example shows a successful push subscription response.</span></span> 
  
### <a name="code"></a><span data-ttu-id="455df-177">コード</span><span class="sxs-lookup"><span data-stu-id="455df-177">Code</span></span>

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
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <SubscribeResponseMessage ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <SubscriptionId>83826921-afdf-48be-b469-628cc02b5f49</SubscriptionId>
          <Watermark>AQAAAOpvG0LURVdOhQkPOWZLPcI8EgAAAAAAAAE=</Watermark>
        </SubscribeResponseMessage>
      </ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="push-subscription-response-elements"></a><span data-ttu-id="455df-178">プッシュサブスクリプション応答要素</span><span class="sxs-lookup"><span data-stu-id="455df-178">Push Subscription response elements</span></span>

<span data-ttu-id="455df-179">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="455df-179">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="455df-180">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="455df-180">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="455df-181">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="455df-181">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="455df-182">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="455df-182">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="455df-183">メッセージの表示</span><span class="sxs-lookup"><span data-stu-id="455df-183">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="455df-184">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="455df-184">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="455df-185">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="455df-185">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="455df-186">Watermark</span><span class="sxs-lookup"><span data-stu-id="455df-186">Watermark</span></span>](watermark.md)
    
## <a name="see-also"></a><span data-ttu-id="455df-187">関連項目</span><span class="sxs-lookup"><span data-stu-id="455df-187">See also</span></span>



[<span data-ttu-id="455df-188">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="455df-188">Unsubscribe operation</span></span>](unsubscribe-operation.md)
  
[<span data-ttu-id="455df-189">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="455df-189">GetEvents operation</span></span>](getevents-operation.md)


[<span data-ttu-id="455df-190">プルサブスクリプションの使用</span><span class="sxs-lookup"><span data-stu-id="455df-190">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="455df-191">プッシュ通知のサンプル アプリケーション</span><span class="sxs-lookup"><span data-stu-id="455df-191">Push Notification Sample Application</span></span>](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)


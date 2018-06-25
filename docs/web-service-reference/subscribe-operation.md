---
title: 操作を購読します。
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
description: 購読操作を使用して、クライアント アプリケーションがプッシュまたはプルのいずれかの通知をサブスクライブします。 要求メッセージと応答の構造は、イベント通知の種類によって異なることに注意する必要があります。
ms.openlocfilehash: f6cacab80c8ca2e505ab63a162a161fcf5de8585
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833619"
---
# <a name="subscribe-operation"></a><span data-ttu-id="c8939-104">操作を購読します。</span><span class="sxs-lookup"><span data-stu-id="c8939-104">Subscribe operation</span></span>

<span data-ttu-id="c8939-105">購読操作を使用して、クライアント アプリケーションがプッシュまたはプルのいずれかの通知をサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="c8939-105">The Subscribe operation is used to subscribe client applications to either push or pull notifications.</span></span> <span data-ttu-id="c8939-106">要求メッセージと応答の構造は、イベント通知の種類によって異なることに注意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8939-106">It is important to be aware that the structure of the request messages and responses is different depending on the type of event notification.</span></span> 
  
## <a name="pull-subscription-subscribe-request-example"></a><span data-ttu-id="c8939-107">プル サブスクリプションがサブスクライブ要求の例</span><span class="sxs-lookup"><span data-stu-id="c8939-107">Pull Subscription Subscribe request example</span></span>

### <a name="description"></a><span data-ttu-id="c8939-108">説明</span><span class="sxs-lookup"><span data-stu-id="c8939-108">Description</span></span>

<span data-ttu-id="c8939-109">次のコード例では、プル サブスクリプションのイベント通知にサブスクライブする方法を示します。</span><span class="sxs-lookup"><span data-stu-id="c8939-109">The following code example shows how to subscribe to a pull event notification subscription.</span></span> <span data-ttu-id="c8939-110">サブスクリプションは、新しいメールが受信トレイに追加された場合、受信トレイからアイテムが削除される場合、クライアント アプリケーションを通知します。</span><span class="sxs-lookup"><span data-stu-id="c8939-110">The subscription informs the client application if new mail is added to the Inbox and if an item is deleted from the Inbox.</span></span> <span data-ttu-id="c8939-111">クライアントが 10 分以内のイベントに関する情報を要求しない場合、サブスクリプションがタイムアウトします。</span><span class="sxs-lookup"><span data-stu-id="c8939-111">The subscription will time out if the client does not request information about events within ten minutes.</span></span> <span data-ttu-id="c8939-112">サブスクリプションが期限切れになった場合は、引き続き通知を要求する新しいサブスクリプションを確立する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8939-112">If the subscription expires, a new subscription must be established to continue to request notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="c8939-113">コード</span><span class="sxs-lookup"><span data-stu-id="c8939-113">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="pull-subscription-subscribe-request-elements"></a><span data-ttu-id="c8939-114">プル サブスクリプション要求の要素を購読します。</span><span class="sxs-lookup"><span data-stu-id="c8939-114">Pull Subscription Subscribe Request Elements</span></span>

<span data-ttu-id="c8939-115">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="c8939-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="c8939-116">購読</span><span class="sxs-lookup"><span data-stu-id="c8939-116">Subscribe</span></span>](subscribe.md)
    
- [<span data-ttu-id="c8939-117">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="c8939-117">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
    
- [<span data-ttu-id="c8939-118">FolderIds</span><span class="sxs-lookup"><span data-stu-id="c8939-118">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="c8939-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="c8939-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="c8939-120">EventTypes</span><span class="sxs-lookup"><span data-stu-id="c8939-120">EventTypes</span></span>](eventtypes.md)
    
- [<span data-ttu-id="c8939-121">EventType</span><span class="sxs-lookup"><span data-stu-id="c8939-121">EventType</span></span>](eventtype.md)
    
- [<span data-ttu-id="c8939-122">Timeout</span><span class="sxs-lookup"><span data-stu-id="c8939-122">Timeout</span></span>](timeout.md)
    
<span data-ttu-id="c8939-123">Subscribe 操作の要求メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="c8939-123">To find other options for the request message of the Subscribe operation, explore the schema hierarchy.</span></span> <span data-ttu-id="c8939-124">[PullSubscriptionRequest](pullsubscriptionrequest.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="c8939-124">Start at the [PullSubscriptionRequest](pullsubscriptionrequest.md) element.</span></span> 
  
## <a name="successful-pull-subscription-subscribe-response-example"></a><span data-ttu-id="c8939-125">正常な応答例のプル サブスクリプションを購読</span><span class="sxs-lookup"><span data-stu-id="c8939-125">Successful Pull Subscription Subscribe response example</span></span>

### <a name="description"></a><span data-ttu-id="c8939-126">説明</span><span class="sxs-lookup"><span data-stu-id="c8939-126">Description</span></span>

<span data-ttu-id="c8939-127">成功したプル サブスクリプション応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8939-127">The following example shows a successful pull subscription response.</span></span> <span data-ttu-id="c8939-128">応答には、サブスクリプション id、サブスクリプションに関連付けられているイベントの配列を取得するために使用されるウォーターマークが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c8939-128">The response contains the subscription identifier and watermark that is used to get the array of events that are associated with a subscription.</span></span> <span data-ttu-id="c8939-129">サブスクリプションの識別子はクライアント サブスクリプション購読を中止するも使用されます。</span><span class="sxs-lookup"><span data-stu-id="c8939-129">The subscription identifier is also used to unsubscribe a client from a subscription.</span></span>
  
### <a name="code"></a><span data-ttu-id="c8939-130">コード</span><span class="sxs-lookup"><span data-stu-id="c8939-130">Code</span></span>

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
    <SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="pull-subscription-subscribe-response-elements"></a><span data-ttu-id="c8939-131">プル サブスクリプションがサブスクライブの応答の要素</span><span class="sxs-lookup"><span data-stu-id="c8939-131">Pull Subscription Subscribe response elements</span></span>

<span data-ttu-id="c8939-132">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="c8939-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="c8939-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c8939-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c8939-134">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="c8939-134">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="c8939-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c8939-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c8939-136">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c8939-136">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="c8939-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c8939-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c8939-138">サブスクリプション Id (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="c8939-138">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="c8939-139">透かし</span><span class="sxs-lookup"><span data-stu-id="c8939-139">Watermark</span></span>](watermark.md)
    
## <a name="pull-subscription-subscribe-error-response-example"></a><span data-ttu-id="c8939-140">プル サブスクリプションの購読エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="c8939-140">Pull Subscription Subscribe Error response example</span></span>

### <a name="description"></a><span data-ttu-id="c8939-141">説明</span><span class="sxs-lookup"><span data-stu-id="c8939-141">Description</span></span>

<span data-ttu-id="c8939-142">Subscribe 要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8939-142">The following example shows an error response to a Subscribe request.</span></span> <span data-ttu-id="c8939-143">代理人アクセスを使用して通知をサブスクライブしようとしてエラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="c8939-143">The error is caused by an attempt to subscribe to notifications by using delegate access.</span></span>
  
### <a name="code"></a><span data-ttu-id="c8939-144">コード</span><span class="sxs-lookup"><span data-stu-id="c8939-144">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="pull-subscription-error-response-elements"></a><span data-ttu-id="c8939-145">プル サブスクリプションのエラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="c8939-145">Pull Subscription Error response elements</span></span>

<span data-ttu-id="c8939-146">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="c8939-146">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="c8939-147">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c8939-147">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c8939-148">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="c8939-148">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="c8939-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c8939-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c8939-150">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c8939-150">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="c8939-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="c8939-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c8939-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c8939-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c8939-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c8939-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="push-subscription-request-example"></a><span data-ttu-id="c8939-154">プッシュ サブスクリプション要求の例</span><span class="sxs-lookup"><span data-stu-id="c8939-154">Push Subscription request example</span></span>

### <a name="description"></a><span data-ttu-id="c8939-155">説明</span><span class="sxs-lookup"><span data-stu-id="c8939-155">Description</span></span>

<span data-ttu-id="c8939-156">次のコード例では、プッシュ サブスクリプションのイベント通知にサブスクライブする方法を示します。</span><span class="sxs-lookup"><span data-stu-id="c8939-156">The following code example shows how to subscribe to a push event notification subscription.</span></span> <span data-ttu-id="c8939-157">要求は、フォルダーを監視するため、イベントを監視するのには、状態通知の頻度およびクライアントのプッシュ通知をリッスンする Web サービスの URL の種類を識別します。</span><span class="sxs-lookup"><span data-stu-id="c8939-157">The request identifies the folders to monitor, the types of events to monitor, the frequency of status notifications, and the URL of the client Web service that listens for the push notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="c8939-158">コード</span><span class="sxs-lookup"><span data-stu-id="c8939-158">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <PushSubscriptionRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <FolderIds xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <DistinguishedFolderId Id="inbox" />
        </FolderIds>
        <EventTypes xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <EventType>NewMailEvent</EventType>
          <EventType>CopiedEvent</EventType>
          <EventType>CreatedEvent</EventType>
          <EventType>DeletedEvent</EventType>
          <EventType>ModifiedEvent</EventType>
          <EventType>MovedEvent</EventType>
        </EventTypes>
        <StatusFrequency xmlns="http://schemas.microsoft.com/exchange/services/2006/types">1</StatusFrequency>
        <URL xmlns="http://schemas.microsoft.com/exchange/services/2006/types">http://clientWebService/Service.asmx</URL>
      </PushSubscriptionRequest>
    </Subscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="c8939-159">コメント</span><span class="sxs-lookup"><span data-stu-id="c8939-159">Comments</span></span>

<span data-ttu-id="c8939-160">クライアント Web サービスは、プッシュ通知要求をサブスクライブする前に設定する必要がありますが送信されます。それ以外の場合、最初の通知は有効なエンドポイントに送信して、プッシュ通知は失敗します。</span><span class="sxs-lookup"><span data-stu-id="c8939-160">The client Web service must be set up before the push notification subscribe request is sent; otherwise, the first notification will not be sent to a valid endpoint and the push notification will fail.</span></span> <span data-ttu-id="c8939-161">詳細については、[プッシュ通知のサンプル アプリケーション](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8939-161">For more information, see [Push Notification Sample Application](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="c8939-162">新しい[サブスクリプション Id (GetEvents)](subscriptionid-getevents.md)は、サブスクライブするときに作成されます。</span><span class="sxs-lookup"><span data-stu-id="c8939-162">A new [SubscriptionId (GetEvents)](subscriptionid-getevents.md) is created when you resubscribe.</span></span> <span data-ttu-id="c8939-163">以前のサブスクリプションの透かしを使用して、以前のサブスクリプションが終了した時点で再度のサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="c8939-163">Use the watermark of a previous subscription to resubscribe at the point where the previous subscription ended.</span></span> 
  
### <a name="push-subscription-request-elements"></a><span data-ttu-id="c8939-164">プッシュ サブスクリプション要求の要素</span><span class="sxs-lookup"><span data-stu-id="c8939-164">Push Subscription Request Elements</span></span>

<span data-ttu-id="c8939-165">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="c8939-165">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="c8939-166">購読</span><span class="sxs-lookup"><span data-stu-id="c8939-166">Subscribe</span></span>](subscribe.md)
    
- [<span data-ttu-id="c8939-167">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="c8939-167">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
    
- [<span data-ttu-id="c8939-168">FolderIds</span><span class="sxs-lookup"><span data-stu-id="c8939-168">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="c8939-169">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="c8939-169">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="c8939-170">EventTypes</span><span class="sxs-lookup"><span data-stu-id="c8939-170">EventTypes</span></span>](eventtypes.md)
    
- [<span data-ttu-id="c8939-171">EventType</span><span class="sxs-lookup"><span data-stu-id="c8939-171">EventType</span></span>](eventtype.md)
    
- [<span data-ttu-id="c8939-172">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="c8939-172">StatusFrequency</span></span>](statusfrequency.md)
    
- [<span data-ttu-id="c8939-173">Url</span><span class="sxs-lookup"><span data-stu-id="c8939-173">Url </span></span>](url-ex15websvcsotherref.md)
    
## <a name="successful-push-subscription-response-example"></a><span data-ttu-id="c8939-174">成功したプッシュ サブスクリプション応答の例</span><span class="sxs-lookup"><span data-stu-id="c8939-174">Successful Push Subscription response example</span></span>

### <a name="description"></a><span data-ttu-id="c8939-175">説明</span><span class="sxs-lookup"><span data-stu-id="c8939-175">Description</span></span>

<span data-ttu-id="c8939-176">成功したプッシュ サブスクリプション応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8939-176">The following example shows a successful push subscription response.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c8939-177">コード</span><span class="sxs-lookup"><span data-stu-id="c8939-177">Code</span></span>

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
    <SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="push-subscription-response-elements"></a><span data-ttu-id="c8939-178">プッシュ サブスクリプション応答の要素</span><span class="sxs-lookup"><span data-stu-id="c8939-178">Push Subscription response elements</span></span>

<span data-ttu-id="c8939-179">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="c8939-179">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="c8939-180">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c8939-180">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c8939-181">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="c8939-181">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="c8939-182">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c8939-182">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c8939-183">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c8939-183">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="c8939-184">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c8939-184">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c8939-185">サブスクリプション Id (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="c8939-185">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="c8939-186">透かし</span><span class="sxs-lookup"><span data-stu-id="c8939-186">Watermark</span></span>](watermark.md)
    
## <a name="see-also"></a><span data-ttu-id="c8939-187">関連項目</span><span class="sxs-lookup"><span data-stu-id="c8939-187">See also</span></span>



[<span data-ttu-id="c8939-188">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="c8939-188">Unsubscribe operation</span></span>](unsubscribe-operation.md)
  
[<span data-ttu-id="c8939-189">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="c8939-189">GetEvents operation</span></span>](getevents-operation.md)


[<span data-ttu-id="c8939-190">プル サブスクリプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="c8939-190">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="c8939-191">プッシュ通知のサンプル アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8939-191">Push Notification Sample Application</span></span>](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)


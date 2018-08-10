---
title: Exchange の EWS を使用してメールボックス イベントに関する通知を取得する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: eb25cbd1-2244-4c3f-a71a-5ee20f81c41f
description: EWS マネージ API または EWS を使用してプル通知の受信を登録し、イベントを取得する方法について説明します。
ms.openlocfilehash: 6a04aaf0102c149691a30c2bd2f499e03265bce8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759043"
---
# <a name="pull-notifications-about-mailbox-events-by-using-ews-in-exchange"></a><span data-ttu-id="7e00a-103">Exchange の EWS を使用してメールボックス イベントに関する通知を取得する</span><span class="sxs-lookup"><span data-stu-id="7e00a-103">How to: Pull notifications about mailbox events by using EWS in Exchange</span></span>

<span data-ttu-id="7e00a-104">EWS マネージ API または EWS を使用してプル通知の受信を登録し、イベントを取得する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="7e00a-104">Find out how to use the EWS Managed API or EWS to subscribe to pull notifications and get events.</span></span>
  
<span data-ttu-id="7e00a-105">Exchange の EWS では、サーバーからクライアントへのメールボックスの変更内容に関する通知をクライアントが要求 (プル) できるようにするためにプル通知を使用します。</span><span class="sxs-lookup"><span data-stu-id="7e00a-105">EWS in Exchange uses pull notifications to enable clients to request (or pull) notifications about changes to the mailbox from the server to the client.</span></span>
  
<span data-ttu-id="7e00a-106">EWS マネージ API を使用してプル通知の受信を登録する場合は、[SubscribeToPullNotifications](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) メソッドを使用して[プル通知の登録と取得](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma)を実施します。</span><span class="sxs-lookup"><span data-stu-id="7e00a-106">If you're subscribing to pull notifications by using the EWS Managed API, you [subscribe to and get pull notifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) by using the [SubscribeToPullNotifications](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="7e00a-107">その後で、[GetEvents](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) メソッドを使用して、サーバーからイベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="7e00a-107">You then get events from the server by using the [GetEvents](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="7e00a-108">EWS を使用してプル通知にサブスクライブする場合は、[Subscribe 操作](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx)を使用して[サブスクリプションを作成](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews)し、応答を解析して、[GetEvents s 操作](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx)を使用して[通知を取得](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull)します。</span><span class="sxs-lookup"><span data-stu-id="7e00a-108">To subscribe to pull notifications by using EWS, you [create a subscription](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) by using the [Subscribe operation](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), parse the response, and then [get the notifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) by using the [GetEvents operation](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="7e00a-109">サーバー上で変更または作成されたアイテムについての通知をクライアントで受信したら、[変更内容を同期](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps)します。</span><span class="sxs-lookup"><span data-stu-id="7e00a-109">After the client receives notifications of items that are changed or created on the server, it can then [synchronize the changes](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span></span>
  
## <a name="subscribe-to-and-get-pull-notifications-by-using-the-ews-managed-api"></a><span data-ttu-id="7e00a-110">EWS マネージ API を使用したプル通知の受信の登録と取得</span><span class="sxs-lookup"><span data-stu-id="7e00a-110">Subscribe to and get pull notifications by using the EWS Managed API</span></span>
<span data-ttu-id="7e00a-111"><a name="bk_cepullewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="7e00a-111"></span></span>

<span data-ttu-id="7e00a-112">次のコード例は、[SubscribeToPullNotifications](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) メソッドを使用して、受信トレイ フォルダー内のすべてのイベントに対応したプル通知の受信を登録する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="7e00a-112">The following code example shows how to use the [SubscribeToPullNotifications](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method to subscribe to pull notifications for all events in the Inbox folder.</span></span> <span data-ttu-id="7e00a-113">さらに、この例では [GetEvents](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) メソッドを使用して、サーバーからイベントを取得しています。</span><span class="sxs-lookup"><span data-stu-id="7e00a-113">The example then uses the [GetEvents](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) method to retrieve events from the server.</span></span> <span data-ttu-id="7e00a-114">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) バインディングであることを想定しています。</span><span class="sxs-lookup"><span data-stu-id="7e00a-114">In this example, we assume that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) binding.</span></span> 
  
```cs
// Subscribe to pull notifications in the Inbox.
PullSubscription subscription = service.SubscribeToPullNotifications( 
    new FolderId[] { WellKnownFolderName.Inbox }, 30, null, 
    EventType.NewMail, EventType.Created, EventType.Deleted,
    EventType.Modified, EventType.Moved, EventType.Copied, EventType.FreeBusyChanged); 
 
// Call GetEvents to retrieve events from the server. 
GetEventsResults events = subscription.GetEvents(); 
```

<span data-ttu-id="7e00a-115">サーバーからイベントを受信したら、[該当する変更内容をサーバーと同期](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps)できます。</span><span class="sxs-lookup"><span data-stu-id="7e00a-115">After you receive an event from the server, you can [synchronize those changes with the server](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span></span> <span data-ttu-id="7e00a-116">サブスクリプションが不要になったら、「[通知の受信の登録を解除する方法](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe)」に示した登録解除メソッドのいずれかを使用してサーバーとのサブスクリプションを終了します。</span><span class="sxs-lookup"><span data-stu-id="7e00a-116">Use one of the unsubscribe methods specified in [How do I unsubscribe to notifications?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) to end the subscription with the server when the subscription is no longer needed.</span></span> 
  
## <a name="subscribe-to-pull-notifications-by-using-ews"></a><span data-ttu-id="7e00a-117">EWS を使用したプル通知の受信の登録</span><span class="sxs-lookup"><span data-stu-id="7e00a-117">Subscribe to pull notifications by using EWS</span></span>
<span data-ttu-id="7e00a-118"><a name="bk_cepullews"> </a></span><span class="sxs-lookup"><span data-stu-id="7e00a-118"></span></span>

<span data-ttu-id="7e00a-119">次の例は、[Subscribe 操作](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx)を使用して受信トレイ フォルダー内のすべての [EventTypes](http://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) にサブスクライブするために、サーバーに送信される XML 要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="7e00a-119">The following example shows the XML request to send to the server to subscribe to all EventTypes in the Inbox folder by using the Subscribe operation. This is also the XML request that the EWS Managed API sends when subscribing to pull notifications by using the  SubscribeToPullNotifications http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications(v=exchg.80).aspx  method.</span></span> <span data-ttu-id="7e00a-120">これは、[SubscribeToPullNotifications](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) メソッドを使用してプル通知にサブスクライブするときに EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="7e00a-120">This is also the XML request that the EWS Managed API sends when subscribing to pull notifications by using the [SubscribeToPullNotifications](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <PullSubscriptionRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <FolderIds xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
      <DistinguishedFolderId Id="inbox" />
    </FolderIds>
    <EventTypes xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
            <EventType>NewMailEvent</EventType>
            <EventType>CreatedEvent</EventType>
            <EventType>DeletedEvent</EventType>
            <EventType>ModifiedEvent</EventType>
            <EventType>MovedEvent</EventType>
            <EventType>CopiedEvent</EventType>
            <EventType>FreeBusyChangedEvent</EventType>
    </EventTypes>
    <Timeout xmlns="http://schemas.microsoft.com/exchange/services/2006/types">30</Timeout>
  </PullSubscriptionRequest>
</Subscribe>
```

<span data-ttu-id="7e00a-121">次の XML の例は、**Subscribe 操作**要求に対する応答として、サーバーからクライアントに送信される [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) メッセージを示しています。</span><span class="sxs-lookup"><span data-stu-id="7e00a-121">The following XML example shows the [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message that is sent from the server to the client in response to the **Subscribe** operation request.</span></span> <span data-ttu-id="7e00a-122">[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素には、サブスクリプションの作成が成功したことを意味する NoError の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e00a-122">The inclusion of the NoError value for the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element means that the subscription was created successfully.</span></span> <span data-ttu-id="7e00a-123">[SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) 要素により、サーバー上のプル通知サブスクリプションが一意に特定されます。</span><span class="sxs-lookup"><span data-stu-id="7e00a-123">The [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) element uniquely identifies the pull notification subscription on the server.</span></span> <span data-ttu-id="7e00a-124">[Watermark](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) 要素は、メールボックス イベント キュー内のブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="7e00a-124">The [Watermark](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) element represents a bookmark in the mailbox event queue.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<SubscribeResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                   xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <SubscribeResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <SubscriptionId>d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
      <Watermark>AAAAAGUhAAAAAAAAAQ==</Watermark>
    </SubscribeResponseMessage>
  </ResponseMessages>
</SubscribeResponse>
```

<span data-ttu-id="7e00a-125">サブスクリプションを作成すると、**SubscribeResponse** メッセージで返される**SubscriptionId** を使用して、ストリーミングされたイベントを取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="7e00a-125">After creating the subscription, you can now get events by using the **SubscriptionId** that is returned in the **SubscribeResponse** message.</span></span> 
  
## <a name="get-pull-notifications-by-using-ews"></a><span data-ttu-id="7e00a-126">EWS を使用したプル通知の取得</span><span class="sxs-lookup"><span data-stu-id="7e00a-126">Get pull notifications by using EWS</span></span>
<span data-ttu-id="7e00a-127"><a name="bk_getpull"> </a></span><span class="sxs-lookup"><span data-stu-id="7e00a-127"></span></span>

<span data-ttu-id="7e00a-128">次の XML の例は、[SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) メッセージで返された [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) についての通知を取得するために、クライアントからサーバーに送信される [GetEvents 操作](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx)要求のメッセージを示しています。</span><span class="sxs-lookup"><span data-stu-id="7e00a-128">The following XML example shows the [GetEvents operation](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) request message that is sent from the client to the server to get notifications for the [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) that is returned in the [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message. For the first GetEvents request, use the Watermark returned in the Subscribe response. For subsequent GetEvents requests, use the last Watermark that was returned in the previous GetEvents request.</span></span> <span data-ttu-id="7e00a-129">最初の **GetEvents** 要求には、**Subscribe** 応答で返された [Watermark](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) を使用します。</span><span class="sxs-lookup"><span data-stu-id="7e00a-129">For the first **GetEvents** request, use the [Watermark](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) returned in the **Subscribe** response.</span></span> <span data-ttu-id="7e00a-130">その後の **GetEvents** 要求には、前の **GetEvents** 要求で返された最新の **Watermark** を使用します。</span><span class="sxs-lookup"><span data-stu-id="7e00a-130">For subsequent **GetEvents** requests, use the last **Watermark** that was returned in the previous **GetEvents** request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEvents xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <SubscriptionId xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
  <Watermark xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">AAAAAGUhAAAAAAAAAQ==</Watermark>
</GetEvents>
```

<span data-ttu-id="7e00a-131">次の XML の例は、サーバーからクライアントに送信される **GetEvents** 応答メッセージを示しています。</span><span class="sxs-lookup"><span data-stu-id="7e00a-131">The following example shows the XML response message that is sent from the server to the client. Notice that both mailboxes and universal distribution groups are returned.</span></span> <span data-ttu-id="7e00a-132">それぞれの **GetEvents** 応答には、1 つ以上のイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e00a-132">Each **GetEvents** response includes information about one or more events.</span></span> <span data-ttu-id="7e00a-133">**Watermark** は、イベントごとに返されます。</span><span class="sxs-lookup"><span data-stu-id="7e00a-133">A **Watermark** is returned for each event.</span></span> <span data-ttu-id="7e00a-134">最新の **Watermark** は保存しておいて、次回の **GetEvents** 要求で使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7e00a-134">The last **Watermark** must be saved and used in the next **GetEvents** request.</span></span> <span data-ttu-id="7e00a-135">最後の **GetEvents** 要求以降にストア イベントが発生していない場合は、状態イベントが返されます。</span><span class="sxs-lookup"><span data-stu-id="7e00a-135">If no store events have occurred since the last **GetEvents** request, a status event is returned.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEventsResponseType xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <GetEventsResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <Notification>
        <SubscriptionId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
        <PreviousWatermark xmlns="http://schemas.microsoft.com/exchange/services/2006/types">AAAAAGUhAAAAAAAAAQ==</PreviousWatermark>
        <MoreEvents xmlns="http://schemas.microsoft.com/exchange/services/2006/types">false</MoreEvents>
        <NewMailEvent xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Watermark>AAAAAHMhAAAAAAAAAQ==</Watermark>
          <TimeStamp>2013-09-15T21:37:01Z</TimeStamp>
          <ItemId Id="AAAtA=" ChangeKey="CQAAAA==" />
          <ParentFolderId Id="AQAtAEFkbWA==" ChangeKey="AQAAAA==" />
        </NewMailEvent>
      </Notification>
    </GetEventsResponseMessage>
  </ResponseMessages>
</GetEventsResponse>
```

サーバーからイベントを受信したら、[変更内容をクライアントに同期します](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps)。 <span data-ttu-id="7e00a-137">サブスクリプションが不要になったら、[Unsubscribe 操作](http://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx)を使用してサーバーとのサブスクリプションを終了します。</span><span class="sxs-lookup"><span data-stu-id="7e00a-137">After you receive an event from the server, synchronize the changes to the client. Use the [Unsubscribe operation](http://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) to end the subscription with the server when the subscription is no longer needed.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="7e00a-138">次の手順</span><span class="sxs-lookup"><span data-stu-id="7e00a-138">Next steps</span></span>
<span data-ttu-id="7e00a-139"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="7e00a-139"></span></span>

<span data-ttu-id="7e00a-140">通知を受信したら、[フォルダー階層の同期](how-to-synchronize-folders-by-using-ews-in-exchange.md)や[変更されたフォルダーの内容の同期](how-to-synchronize-items-by-using-ews-in-exchange.md)を実行します。</span><span class="sxs-lookup"><span data-stu-id="7e00a-140">After you’re received notifications, you can [sync the folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md) or [sync the contents of the folder that changed](how-to-synchronize-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="7e00a-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="7e00a-141">See also</span></span>


- [<span data-ttu-id="7e00a-142">Exchange の通知サブスクリプション、メールボックス イベント、および EWS</span><span class="sxs-lookup"><span data-stu-id="7e00a-142">Notification subscriptions, mailbox events, and EWS in Exchange</span></span>](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [<span data-ttu-id="7e00a-143">Exchange での EWS を使用したメールボックス イベントに関するストリーム通知</span><span class="sxs-lookup"><span data-stu-id="7e00a-143">How to: Stream notifications about mailbox events by using EWS in Exchange</span></span>](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="7e00a-144">サブスクリプション グループと Exchange のメールボックス サーバー間のアフィニティを維持する</span><span class="sxs-lookup"><span data-stu-id="7e00a-144">How to: Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [<span data-ttu-id="7e00a-145">Exchange の EWS における、通知関連エラーの処理</span><span class="sxs-lookup"><span data-stu-id="7e00a-145">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="7e00a-146">Exchange のメールボックス同期と EWS</span><span class="sxs-lookup"><span data-stu-id="7e00a-146">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    


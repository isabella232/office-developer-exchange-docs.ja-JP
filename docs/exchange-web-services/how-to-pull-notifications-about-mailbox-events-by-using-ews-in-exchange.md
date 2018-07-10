---
title: EWS を使用して Exchange でメールボックスのイベントに関する通知をプルします。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: eb25cbd1-2244-4c3f-a71a-5ee20f81c41f
description: EWS マネージ API または EWS を使用してプル通知の受信を登録し、イベントを取得する方法について説明します。
ms.openlocfilehash: 6a04aaf0102c149691a30c2bd2f499e03265bce8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759043"
---
# <a name="pull-notifications-about-mailbox-events-by-using-ews-in-exchange"></a><span data-ttu-id="d4403-103">EWS を使用して Exchange でメールボックスのイベントに関する通知をプルします。</span><span class="sxs-lookup"><span data-stu-id="d4403-103">Pull notifications about mailbox events by using EWS in Exchange</span></span>

<span data-ttu-id="d4403-104">EWS マネージ API または EWS を使用してプル通知の受信を登録し、イベントを取得する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="d4403-104">Find out how to use the EWS Managed API or EWS to subscribe to pull notifications and get events.</span></span>
  
<span data-ttu-id="d4403-105">Exchange の EWS では、サーバーからクライアントへのメールボックスの変更内容に関する通知をクライアントが要求 (プル) できるようにするためにプル通知を使用します。</span><span class="sxs-lookup"><span data-stu-id="d4403-105">EWS in Exchange uses pull notifications to enable clients to request (or pull) notifications about changes to the mailbox from the server to the client.</span></span>
  
<span data-ttu-id="d4403-106">EWS マネージ API を使用して[サブスクリプションし、プル通知を取得する](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) [SubscribeToPullNotifications](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx)メソッドを使用して、プル通知のサブスクライブしている場合。</span><span class="sxs-lookup"><span data-stu-id="d4403-106">If you're subscribing to pull notifications by using the EWS Managed API, you [subscribe to and get pull notifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) by using the [SubscribeToPullNotifications](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="d4403-107">[GetEvents](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx)メソッドを使用してサーバーからイベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="d4403-107">You then get events from the server by using the [GetEvents](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="d4403-108">プルの通知を購読するには、EWS を使用して、[購読の操作](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx)を使用して[サブスクリプションを作成](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews)をする解析、応答し、[通知を取得する](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) [GetEvents 操作](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx)を使用しています。</span><span class="sxs-lookup"><span data-stu-id="d4403-108">To subscribe to pull notifications by using EWS, you [create a subscription](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) by using the [Subscribe operation](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), parse the response, and then [get the notifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) by using the [GetEvents operation](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="d4403-109">クライアントの変更またはサーバー上に作成されるアイテムの通知を受け取ると後に、ことができますし、[変更の同期します](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps)。</span><span class="sxs-lookup"><span data-stu-id="d4403-109">After the client receives notifications of items that are changed or created on the server, it can then [synchronize the changes](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span></span>
  
## <a name="subscribe-to-and-get-pull-notifications-by-using-the-ews-managed-api"></a><span data-ttu-id="d4403-110">EWS マネージ API を使用したプル通知のサブスクライブと取得</span><span class="sxs-lookup"><span data-stu-id="d4403-110">Subscribe to and get pull notifications by using the EWS Managed API</span></span>
<span data-ttu-id="d4403-111"><a name="bk_cepullewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="d4403-111"></span></span>

<span data-ttu-id="d4403-112">次のコード例では、プルの受信トレイ フォルダー内のすべてのイベント通知をサブスクライブする[SubscribeToPullNotifications](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx)メソッドを使用する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="d4403-112">The following code example shows how to use the [SubscribeToPullNotifications](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method to subscribe to pull notifications for all events in the Inbox folder.</span></span> <span data-ttu-id="d4403-113">例は、 [GetEvents](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx)メソッドを使用してサーバーからイベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="d4403-113">The example then uses the [GetEvents](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) method to retrieve events from the server.</span></span> <span data-ttu-id="d4403-114">この例では、その**サービス**は、有効な[ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)バインドと仮定します。</span><span class="sxs-lookup"><span data-stu-id="d4403-114">In this example, we assume that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) binding.</span></span> 
  
```cs
// Subscribe to pull notifications in the Inbox.
PullSubscription subscription = service.SubscribeToPullNotifications( 
    new FolderId[] { WellKnownFolderName.Inbox }, 30, null, 
    EventType.NewMail, EventType.Created, EventType.Deleted,
    EventType.Modified, EventType.Moved, EventType.Copied, EventType.FreeBusyChanged); 
 
// Call GetEvents to retrieve events from the server. 
GetEventsResults events = subscription.GetEvents(); 
```

<span data-ttu-id="d4403-115">サーバーからイベントを受信したら、[サーバーを使用して変更を同期](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps)することができます。</span><span class="sxs-lookup"><span data-stu-id="d4403-115">After you receive an event from the server, you can [synchronize those changes with the server](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span></span> <span data-ttu-id="d4403-116">指定されている登録解除の方法のいずれかを使用して、[の通知を購読する方法ですか?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe)サブスクリプションは、不要になったときに、サーバーでサブスクリプションを終了します。</span><span class="sxs-lookup"><span data-stu-id="d4403-116">Use one of the unsubscribe methods specified in [How do I unsubscribe to notifications?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) to end the subscription with the server when the subscription is no longer needed.</span></span> 
  
## <a name="subscribe-to-pull-notifications-by-using-ews"></a><span data-ttu-id="d4403-117">EWS を使用したプル通知のサブスクライブ</span><span class="sxs-lookup"><span data-stu-id="d4403-117">Subscribe to pull notifications by using EWS</span></span>
<span data-ttu-id="d4403-118"><a name="bk_cepullews"> </a></span><span class="sxs-lookup"><span data-stu-id="d4403-118"></span></span>

<span data-ttu-id="d4403-119">[購読操作](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx)を使用して、[受信トレイ] フォルダー内のすべての[EventTypes](http://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx)にサブスクライブするサーバーに送信する XML 要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d4403-119">The following example shows the XML request to send to the server to subscribe to all [EventTypes](http://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) in the Inbox folder by using the [Subscribe operation](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx).</span></span> <span data-ttu-id="d4403-120">EWS のマネージ API が、 [SubscribeToPullNotifications](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx)メソッドを使用してプル通知にサブスクライブしているときに送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="d4403-120">This is also the XML request that the EWS Managed API sends when subscribing to pull notifications by using the [SubscribeToPullNotifications](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method.</span></span> 
  
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

<span data-ttu-id="d4403-121">**Subscribe**操作の要求への応答としてクライアントにサーバーから送信される[SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx)メッセージを次の XML 例に示します。</span><span class="sxs-lookup"><span data-stu-id="d4403-121">The following XML example shows the [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message that is sent from the server to the client in response to the **Subscribe** operation request.</span></span> <span data-ttu-id="d4403-122">NoError、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)の要素の値を含めることは、サブスクリプションが正常に作成されたことを意味します。</span><span class="sxs-lookup"><span data-stu-id="d4403-122">The inclusion of the NoError value for the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element means that the subscription was created successfully.</span></span> <span data-ttu-id="d4403-123">[サブスクリプション Id](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx)要素は、サーバー上でプル通知サブスクリプションを一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="d4403-123">The [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) element uniquely identifies the pull notification subscription on the server.</span></span> <span data-ttu-id="d4403-124">[透かし](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx)の要素は、メールボックス イベント キュー内のブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="d4403-124">The [Watermark](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) element represents a bookmark in the mailbox event queue.</span></span> 
  
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

<span data-ttu-id="d4403-125">サブスクリプションを作成した後には、 **SubscribeResponse**メッセージで返される**サブスクリプション Id**を使用してイベントを今すぐ取得できます。</span><span class="sxs-lookup"><span data-stu-id="d4403-125">After creating the subscription, you can now get events by using the **SubscriptionId** that is returned in the **SubscribeResponse** message.</span></span> 
  
## <a name="get-pull-notifications-by-using-ews"></a><span data-ttu-id="d4403-126">EWS を使用したプル通知の取得</span><span class="sxs-lookup"><span data-stu-id="d4403-126">Get pull notifications by using EWS</span></span>
<span data-ttu-id="d4403-127"><a name="bk_getpull"> </a></span><span class="sxs-lookup"><span data-stu-id="d4403-127"></span></span>

<span data-ttu-id="d4403-128">次の XML の例は、 [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx)メッセージで返される[サブスクリプション Id](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx)の通知を取得するクライアントからサーバーに送信される[GetEvents 操作](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx)の要求メッセージを示しています。</span><span class="sxs-lookup"><span data-stu-id="d4403-128">The following XML example shows the [GetEvents operation](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) request message that is sent from the client to the server to get notifications for the [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) that is returned in the [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message.</span></span> <span data-ttu-id="d4403-129">最初の**GetEvents**要求では、**購読**の応答で返される[ウォーターマーク](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx)を使用します。</span><span class="sxs-lookup"><span data-stu-id="d4403-129">For the first **GetEvents** request, use the [Watermark](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) returned in the **Subscribe** response.</span></span> <span data-ttu-id="d4403-130">**GetEvents**の後続の要求の前の**GetEvents**要求で返された最新の**ウォーターマーク**を使用します。</span><span class="sxs-lookup"><span data-stu-id="d4403-130">For subsequent **GetEvents** requests, use the last **Watermark** that was returned in the previous **GetEvents** request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEvents xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <SubscriptionId xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
  <Watermark xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">AAAAAGUhAAAAAAAAAQ==</Watermark>
</GetEvents>
```

<span data-ttu-id="d4403-131">次の XML の例は、サーバーからクライアントに送信される**GetEvents**応答メッセージを示しています。</span><span class="sxs-lookup"><span data-stu-id="d4403-131">The following XML example shows the **GetEvents** response message that is sent from the server to the client.</span></span> <span data-ttu-id="d4403-132">**GetEvents**応答ごとに 1 つまたは複数のイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d4403-132">Each **GetEvents** response includes information about one or more events.</span></span> <span data-ttu-id="d4403-133">**ウォーターマーク**がイベントごとに返されます。</span><span class="sxs-lookup"><span data-stu-id="d4403-133">A **Watermark** is returned for each event.</span></span> <span data-ttu-id="d4403-134">最新の**ウォーターマーク**は保存され、次の**GetEvents**要求で使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d4403-134">The last **Watermark** must be saved and used in the next **GetEvents** request.</span></span> <span data-ttu-id="d4403-135">最後の**GetEvents**要求からストアのイベントが発生していない、状態イベントが返されます。</span><span class="sxs-lookup"><span data-stu-id="d4403-135">If no store events have occurred since the last **GetEvents** request, a status event is returned.</span></span> 
  
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

した後[、クライアントへの変更を同期化](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps)、サーバーからイベントが表示されます。 <span data-ttu-id="d4403-137">サブスクリプションは、不要になったときに、サーバーでサブスクリプションを終了するには、[購読の取り消し操作](http://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx)を使用します。</span><span class="sxs-lookup"><span data-stu-id="d4403-137">Use the [Unsubscribe operation](http://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) to end the subscription with the server when the subscription is no longer needed.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="d4403-138">次の手順</span><span class="sxs-lookup"><span data-stu-id="d4403-138">Next steps</span></span>
<span data-ttu-id="d4403-139"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="d4403-139"></span></span>

<span data-ttu-id="d4403-140">受信した後の通知、[フォルダー階層の同期](how-to-synchronize-folders-by-using-ews-in-exchange.md)または[変更するフォルダーの内容を同期](how-to-synchronize-items-by-using-ews-in-exchange.md)することができます。</span><span class="sxs-lookup"><span data-stu-id="d4403-140">After you're received notifications, you can [sync the folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md) or [sync the contents of the folder that changed](how-to-synchronize-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="d4403-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="d4403-141">See also</span></span>


- [<span data-ttu-id="d4403-142">Notification subscriptions, mailbox events, and EWS in Exchange</span><span class="sxs-lookup"><span data-stu-id="d4403-142">Notification subscriptions, mailbox events, and EWS in Exchange</span></span>](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [<span data-ttu-id="d4403-143">Exchange の EWS を使用してメールボックスのイベントに関する通知をストリーム</span><span class="sxs-lookup"><span data-stu-id="d4403-143">Stream notifications about mailbox events by using EWS in Exchange</span></span>](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="d4403-144">Exchange の購読グループとメールボックス サーバー間のアフィニティを維持します。</span><span class="sxs-lookup"><span data-stu-id="d4403-144">Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [<span data-ttu-id="d4403-145">Exchange における EWS での通知関連エラーの処理</span><span class="sxs-lookup"><span data-stu-id="d4403-145">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="d4403-146">Exchange のメールボックス同期と EWS</span><span class="sxs-lookup"><span data-stu-id="d4403-146">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    


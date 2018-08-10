---
title: Exchange での EWS を使用したメールボックス イベントに関するストリーム通知
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fe9bde1e-da0e-413c-a109-077f399f67a3
description: EWS マネージ API または EWS を使用してストリーミング通知の受信を登録し、イベントを取得する方法について説明します。
ms.openlocfilehash: aad7604511687d1482914183979e954f79572af9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759054"
---
# <a name="stream-notifications-about-mailbox-events-by-using-ews-in-exchange"></a><span data-ttu-id="19e81-103">Exchange での EWS を使用したメールボックス イベントに関するストリーム通知</span><span class="sxs-lookup"><span data-stu-id="19e81-103">How to: Stream notifications about mailbox events by using EWS in Exchange</span></span>

<span data-ttu-id="19e81-104">EWS マネージ API または EWS を使用してストリーミング通知の受信を登録し、イベントを取得する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="19e81-104">Find out how to use the EWS Managed API or EWS to subscribe to streaming notifications and get events.</span></span>
  
<span data-ttu-id="19e81-105">Exchange の EWS はストリーミング通知を使用して、サーバーから送信された通知を受け取ります。これは、特定の期間開いた状態が維持される接続を通じて行われます。</span><span class="sxs-lookup"><span data-stu-id="19e81-105">EWS in Exchange uses streaming notifications to receive notifications that are sent by the server through a connection that remains open for a specified period of time.</span></span>
  
<span data-ttu-id="19e81-106">EWS マネージ API を使用してストリーミング通知にサブスクライブする場合は、[SubscribeToStreamingNotifications](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.subscribetostreamingnotifications%28v=exchg.80%29.aspx) メソッドを使用して[ストリーミング通知のサブスクライブと取得](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cestreamewsma)を実施します。</span><span class="sxs-lookup"><span data-stu-id="19e81-106">If you're subscribing to streaming notifications by using the EWS Managed API, you [subscribe and get streaming notifications](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cestreamewsma) by using the [SubscribeToStreamingNotifications](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.subscribetostreamingnotifications%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="19e81-107">その後で、[StreamingSubscriptionConnection](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.streamingsubscriptionconnection%28v=exchg.80%29.aspx) オブジェクトを使用して、サブスクリプションへの接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="19e81-107">You then create a connection to the subscription by using the [StreamingSubscriptionConnection](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.streamingsubscriptionconnection%28v=exchg.80%29.aspx) object.</span></span> 
  
<span data-ttu-id="19e81-108">EWS を使用してストリーミング通知にサブスクライブする場合は、[Subscribe 操作](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx)を使用して[サブスクリプションを作成](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cestreamews)し、応答を解析して、[GetStreamingEvents 操作](http://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx)を使用して[ストリーミング通知を取得](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cegetnotifsews)します。</span><span class="sxs-lookup"><span data-stu-id="19e81-108">To subscribe to streaming notifications by using EWS, you [create a subscription](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cestreamews) by using the [Subscribe operation](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), parse the response, and then [get the streaming notifications](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cegetnotifsews) by using the [GetStreamingEvents operation](http://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) request.</span></span> 
  
<span data-ttu-id="19e81-109">サーバー上で変更または作成されたアイテムについての通知をクライアントが受信したら、[次の手順](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps)は変更の同期です。</span><span class="sxs-lookup"><span data-stu-id="19e81-109">After the client receives notifications of items changed or created on the server, the [next step](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps) is to synchronize the changes.</span></span> 
  
## <a name="subscribe-to-and-get-streaming-notifications-by-using-the-ews-managed-api"></a><span data-ttu-id="19e81-110">EWS マネージ API を使用したストリーミング通知のサブスクライブと取得</span><span class="sxs-lookup"><span data-stu-id="19e81-110">Subscribe to and get streaming notifications by using the EWS Managed API</span></span>
<span data-ttu-id="19e81-111"><a name="bk_cestreamewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="19e81-111"></span></span>

<span data-ttu-id="19e81-112">次のコード例は、[SubscribeToStreamingNotifications](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.endsubscribetostreamingnotifications%28v=exchg.80%29.aspx) メソッドを使用して、受信トレイ フォルダー内のすべてのイベントのストリーミング通知にサブスクライブする方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="19e81-112">The following code example shows how to use the [SubscribeToStreamingNotifications](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.endsubscribetostreamingnotifications%28v=exchg.80%29.aspx) method to subscribe to streaming notifications for all events in the Inbox folder.</span></span> <span data-ttu-id="19e81-113">その後で、[StreamingSubscriptionConnection](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.streamingsubscriptionconnection%28v=exchg.80%29.aspx) オブジェクトを作成することで、サブスクリプション用の接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="19e81-113">It then creates a connection for the subscription by creating a [StreamingSubscriptionConnection](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.streamingsubscriptionconnection%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="19e81-114">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) バインディングであることを想定しています。</span><span class="sxs-lookup"><span data-stu-id="19e81-114">In this example, we assume that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) binding.</span></span> 
  
```cs
// Subscribe to streaming notifications in the Inbox. 
StreamingSubscription = service.SubscribeToStreamingNotifications(
    new FolderId[] { WellKnownFolderName.Inbox },
    EventType.NewMail,
    EventType.Created,
    EventType.Deleted,
    EventType.Modified,
    EventType.Moved,
    EventType.Copied,
    EventType.FreeBusyChanged);
// Create a streaming connection to the service object, over which events are returned to the client.
// Keep the streaming connection open for 30 minutes.
StreamingSubscriptionConnection connection = new StreamingSubscriptionConnection(service, 30);
connection.AddSubscription(StreamingSubscription);
connection.OnNotificationEvent += OnNotificationEvent;
connection.OnDisconnect += OnDisconnect;
connection.Open();
```

<span data-ttu-id="19e81-115">サーバーからイベントを受信したら、[次の手順](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps)では、該当する変更内容をサーバーと同期します。</span><span class="sxs-lookup"><span data-stu-id="19e81-115">After you have received events from the server, the [next step](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps) is to synchronize those changes with the server. Use the Unsubscribe operation to end the subscription with the server when the subscription is no longer needed.</span></span> <span data-ttu-id="19e81-116">サブスクリプションが不要になったら、「[表 4](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe)」に示した登録解除メソッドのいずれかを使用してサーバーとのサブスクリプションを終了します。</span><span class="sxs-lookup"><span data-stu-id="19e81-116">After you have received events from the server, the next step is to synchronize those changes with the server. Use one of the unsubscribe methods listed in [Table 4](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) to end the subscription with the server when the subscription is no longer needed.</span></span> 
  
## <a name="subscribe-to-streaming-notifications-by-using-ews"></a><span data-ttu-id="19e81-117">EWS を使用したストリーミング通知のサブスクライブ</span><span class="sxs-lookup"><span data-stu-id="19e81-117">Subscribe to streaming notifications by using EWS</span></span>
<span data-ttu-id="19e81-118"><a name="bk_cestreamews"> </a></span><span class="sxs-lookup"><span data-stu-id="19e81-118"></span></span>

<span data-ttu-id="19e81-119">次の例は、受信トレイ フォルダー内のすべての [EventTypes](http://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) にサブスクライブするために、クライアントが [Subscribe 操作](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx)を呼び出すときに、クライアントからサーバーに送信される XML 要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="19e81-119">The following example shows an XML request that is sent by the client to the server when the client calls the [Subscribe operation](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) to subscribe to all [EventTypes](http://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) in the Inbox folder. This is also the XML request that the EWS Managed API sends when you use the SubscribeToStreamingNotificationshttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.endsubscribetostreamingnotifications(v=exchg.80).aspx method to subscribe to streaming notifications.</span></span> <span data-ttu-id="19e81-120">これは、[SubscribeToStreamingNotifications](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.endsubscribetostreamingnotifications%28v=exchg.80%29.aspx) メソッドを使用してストリーミング通知にサブスクライブするときに、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="19e81-120">This is also the XML request that the EWS Managed API sends when you use the AddDelegates method to add delegates.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:Subscribe>
      <m:StreamingSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox" />
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
          <t:EventType>CreatedEvent</t:EventType>
          <t:EventType>DeletedEvent</t:EventType>
          <t:EventType>ModifiedEvent</t:EventType>
          <t:EventType>MovedEvent</t:EventType>
          <t:EventType>CopiedEvent</t:EventType>
          <t:EventType>FreeBusyChangedEvent</t:EventType>
        </t:EventTypes>
      </m:StreamingSubscriptionRequest>
    </m:Subscribe>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="19e81-121">次の XML の例は、[Subscribe 操作](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx)要求に対する応答として、サーバーからクライアントに送信される [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) メッセージを示しています。</span><span class="sxs-lookup"><span data-stu-id="19e81-121">The following XML example shows the [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message that is sent from the server to the client in response to the [Subscribe operation](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) request.</span></span> <span data-ttu-id="19e81-122">[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素には、サブスクリプションの作成が成功したことを意味する NoError の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="19e81-122">The inclusion of the NoError value for the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element means that the subscription was created successfully.</span></span> <span data-ttu-id="19e81-123">[SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) 要素により、サーバー上のストリーミング通知サブスクリプションが一意に特定されます。</span><span class="sxs-lookup"><span data-stu-id="19e81-123">The [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) element uniquely identifies the streaming notification subscription on the server.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="785"
                         MinorBuildNumber="6"
                         Version="V2_6"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
          <m:SubscribeResponseMessage ResponseClass="Success">
            <m:ResponseCode>NoError</m:ResponseCode>
            <m:SubscriptionId>JgBibjFwcjAzbWIyMDIubmFtcHJkMDMucHJvZC5vdXRsb29rLmNvbRAAAADwXxVesOnHS5BxUHKwAW88SHjwd1iB0Ag=</m:SubscriptionId>
          </m:SubscribeResponseMessage>
        </m:ResponseMessages>
      </m:SubscribeResponse>
    </s:Body>
  </s:Envelope>
```

<span data-ttu-id="19e81-124">サブスクリプションを作成すると、[SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) メッセージで返される [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) を使用して、[ストリーミングされたイベントを取得](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cegetnotifsews)できるようになります。</span><span class="sxs-lookup"><span data-stu-id="19e81-124">After creating the subscription, you can now [get the streamed events](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cegetnotifsews) by using the [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) returned in the [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message.</span></span> 
  
## <a name="get-streaming-events-by-using-ews"></a><span data-ttu-id="19e81-125">EWS を使用したストリーミング イベントの取得</span><span class="sxs-lookup"><span data-stu-id="19e81-125">Get streaming events by using EWS</span></span>
<span data-ttu-id="19e81-126"><a name="bk_cegetnotifsews"> </a></span><span class="sxs-lookup"><span data-stu-id="19e81-126"></span></span>

<span data-ttu-id="19e81-127">次の XML の例は、[SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) メッセージで返された [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) についての通知を取得するために、クライアントからサーバーに送信される [GetStreamingEvents 操作](http://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx)要求のメッセージを示しています。 </span><span class="sxs-lookup"><span data-stu-id="19e81-127">The following XML example shows the [GetStreamingEvents operation](http://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) request message that the client sends to the server to get notifications for the [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) returned in the [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message. The GetStreamingEvents operation request indicates that the length of the connection is 30 minutes long.</span></span> <span data-ttu-id="19e81-128">[GetStreamingEvents 操作](http://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx)要求は、接続時間の長さが 30 分であることを示しています。</span><span class="sxs-lookup"><span data-stu-id="19e81-128">The [GetStreamingEvents operation](http://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) request indicates that the length of the connection is 30 minutes long.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:GetStreamingEvents>
      <m:SubscriptionIds>
        <t:SubscriptionId>JgBibjFwcjAzbWIyMDIubmFtcHJkMDMucHJvZC5vdXRsb29rLmNvbRAAAADwXxVesOnHS5BxUHKwAW88SHjwd1iB0Ag=</t:SubscriptionId>
      </m:SubscriptionIds>
      <m:ConnectionTimeout>30</m:ConnectionTimeout>
    </m:GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="19e81-129">次の XML の例は、[GetStreamingEvents 操作](http://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx)要求に対する応答として、サーバーからクライアントに送信される [GetStreamingEventsResponse](http://msdn.microsoft.com/library/ea1e7e7e-1b19-4e07-ba42-5dbd888c6db2%28Office.15%29.aspx) メッセージを示しています。</span><span class="sxs-lookup"><span data-stu-id="19e81-129">The following XML example shows the [GetStreamingEventsResponse](http://msdn.microsoft.com/library/ea1e7e7e-1b19-4e07-ba42-5dbd888c6db2%28Office.15%29.aspx) message that is sent from the server to the client in response to the [GetStreamingEvents operation](http://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) request. It contains a CreatedEvent and a NewMailEvent for the item, and a ModifiedEvent for the folder, all of which occur when a new message is received.</span></span> <span data-ttu-id="19e81-130">これには、アイテムに対する CreatedEvent および NewMailEvent とフォルダーに対する ModifiedEvent が含まれています。これらすべては、新しいメッセージが受信されたときに発生します。</span><span class="sxs-lookup"><span data-stu-id="19e81-130">The following XML example shows the GetStreamingEventsResponse message that is sent from the server to the client in response to the GetStreamingEvents operation request. It contains a CreatedEvent and a NewMailEvent for the item, and a ModifiedEvent for the folder, all of which occur when a new message is received.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="785"
                         MinorBuildNumber="6"
                         Version="V2_6"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <soap:Body xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <m:GetStreamingEventsResponse xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
    <m:ResponseMessages>
      <m:GetStreamingEventsResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Notifications>
          <m:Notification>
            <t:SubscriptionId>JgBibjFwcjAzbWIyMDIubmFtcHJkMDMucHJvZC5vdXRsb29rLmNvbRAAAADwXxVesOnHS5BxUHKwAW88SHjwd1iB0Ag=</t:SubscriptionId>
            <t:CreatedEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:ItemId Id="AAMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwBGAAAAAABSSWVKrmGUTJE+MVIvofglBwDZGACZQpSgSpyNkexYe2b7AAAAAAENAADZGACZQpSgSpyNkexYe2b7AAANGFYwAAA=" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
            </t:CreatedEvent>
            <t:NewMailEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:ItemId Id="AAMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwBGAAAAAABSSWVKrmGUTJE+MVIvofglBwDZGACZQpSgSpyNkexYe2b7AAAAAAENAADZGACZQpSgSpyNkexYe2b7AAANGFYwAAA=" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
            <t:ModifiedEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:FolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgEJAAAA" ChangeKey="AQAAAA==" />
              <t:UnreadCount>1</t:UnreadCount>
            </t:ModifiedEvent>
          </m:Notification>
        </m:Notifications>
      </m:GetStreamingEventsResponseMessage>
    </m:ResponseMessages>
  </m:GetStreamingEventsResponse>
</soap:Body>
```

サーバーからイベントを受信したら、[次の手順](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps)では、該当する変更内容をサーバーと同期します。 <span data-ttu-id="19e81-132">サブスクリプションが不要になったら、[Unsubscribe 操作](http://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx)を使用してサーバーとのサブスクリプションを終了します。</span><span class="sxs-lookup"><span data-stu-id="19e81-132">After you receive an event from the server, synchronize the changes to the client. Use the [Unsubscribe operation](http://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) to end the subscription with the server when the subscription is no longer needed.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="19e81-133">次の手順</span><span class="sxs-lookup"><span data-stu-id="19e81-133">Next steps</span></span>
<span data-ttu-id="19e81-134"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="19e81-134"></span></span>

<span data-ttu-id="19e81-135">通知を受信したら、[フォルダー階層の同期](how-to-synchronize-folders-by-using-ews-in-exchange.md)や[変更されたフォルダーの内容の同期](how-to-synchronize-items-by-using-ews-in-exchange.md)を実行します。</span><span class="sxs-lookup"><span data-stu-id="19e81-135">After you’ve received notifications, you can [sync the folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md) or [sync the contents of the folder that changed](how-to-synchronize-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="19e81-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="19e81-136">See also</span></span>


- [<span data-ttu-id="19e81-137">Exchange の通知サブスクリプション、メールボックス イベント、および EWS</span><span class="sxs-lookup"><span data-stu-id="19e81-137">Notification subscriptions, mailbox events, and EWS in Exchange</span></span>](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [<span data-ttu-id="19e81-138">Exchange の EWS を使用してメールボックス イベントに関する通知を取得する</span><span class="sxs-lookup"><span data-stu-id="19e81-138">How to: Pull notifications about mailbox events by using EWS in Exchange</span></span>](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="19e81-139">サブスクリプション グループと Exchange のメールボックス サーバー間のアフィニティを維持する</span><span class="sxs-lookup"><span data-stu-id="19e81-139">How to: Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [<span data-ttu-id="19e81-140">Exchange の EWS における、通知関連エラーの処理</span><span class="sxs-lookup"><span data-stu-id="19e81-140">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="19e81-141">Exchange のメールボックス同期と EWS</span><span class="sxs-lookup"><span data-stu-id="19e81-141">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    


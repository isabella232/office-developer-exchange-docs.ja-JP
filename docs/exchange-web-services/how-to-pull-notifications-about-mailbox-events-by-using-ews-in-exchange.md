---
title: Exchange の EWS を使用してメールボックス イベントに関する通知を取得する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: eb25cbd1-2244-4c3f-a71a-5ee20f81c41f
description: EWS マネージ API または EWS を使用してプル通知の受信を登録し、イベントを取得する方法について説明します。
ms.openlocfilehash: 3d77c0d4efb8fc853eea64ff2429af5c3dbead27
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456742"
---
# <a name="pull-notifications-about-mailbox-events-by-using-ews-in-exchange"></a>Exchange の EWS を使用してメールボックス イベントに関する通知を取得する

EWS マネージ API または EWS を使用してプル通知の受信を登録し、イベントを取得する方法について説明します。
  
Exchange の EWS では、サーバーからクライアントへのメールボックスの変更内容に関する通知をクライアントが要求 (プル) できるようにするためにプル通知を使用します。
  
EWS マネージ API を使用してプル通知の受信を登録する場合は、[SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) メソッドを使用して[プル通知の登録と取得](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma)を実施します。 その後で、[GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) メソッドを使用して、サーバーからイベントを取得します。 
  
EWS を使用してプル通知にサブスクライブする場合は、[Subscribe 操作](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx)を使用して[サブスクリプションを作成](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews)し、応答を解析して、[GetEvents s 操作](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx)を使用して[通知を取得](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull)します。
  
サーバー上で変更または作成されたアイテムについての通知をクライアントで受信したら、[変更内容を同期](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps)します。
  
## <a name="subscribe-to-and-get-pull-notifications-by-using-the-ews-managed-api"></a>EWS マネージ API を使用したプル通知の受信の登録と取得
<a name="bk_cepullewsma"> </a>

次のコード例は、[SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) メソッドを使用して、受信トレイ フォルダー内のすべてのイベントに対応したプル通知の受信を登録する方法を示しています。 さらに、この例では [GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) メソッドを使用して、サーバーからイベントを取得しています。 この例では、**service** が有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) バインディングであることを想定しています。 
  
```cs
// Subscribe to pull notifications in the Inbox.
PullSubscription subscription = service.SubscribeToPullNotifications( 
    new FolderId[] { WellKnownFolderName.Inbox }, 30, null, 
    EventType.NewMail, EventType.Created, EventType.Deleted,
    EventType.Modified, EventType.Moved, EventType.Copied, EventType.FreeBusyChanged); 
 
// Call GetEvents to retrieve events from the server. 
GetEventsResults events = subscription.GetEvents(); 
```

サーバーからイベントを受信したら、[該当する変更内容をサーバーと同期](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps)できます。 サブスクリプションが不要になったら、「[通知の受信の登録を解除する方法](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe)」に示した登録解除メソッドのいずれかを使用してサーバーとのサブスクリプションを終了します。 
  
## <a name="subscribe-to-pull-notifications-by-using-ews"></a>EWS を使用したプル通知の受信の登録
<a name="bk_cepullews"> </a>

次の例は、[Subscribe 操作](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx)を使用して受信トレイ フォルダー内のすべての [EventTypes](https://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) にサブスクライブするために、サーバーに送信される XML 要求を示しています。 これは、[SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) メソッドを使用してプル通知にサブスクライブするときに EWS マネージ API が送信する XML 要求でもあります。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <PullSubscriptionRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <FolderIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
      <DistinguishedFolderId Id="inbox" />
    </FolderIds>
    <EventTypes xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
            <EventType>NewMailEvent</EventType>
            <EventType>CreatedEvent</EventType>
            <EventType>DeletedEvent</EventType>
            <EventType>ModifiedEvent</EventType>
            <EventType>MovedEvent</EventType>
            <EventType>CopiedEvent</EventType>
            <EventType>FreeBusyChangedEvent</EventType>
    </EventTypes>
    <Timeout xmlns="https://schemas.microsoft.com/exchange/services/2006/types">30</Timeout>
  </PullSubscriptionRequest>
</Subscribe>
```

次の XML の例は、**Subscribe 操作**要求に対する応答として、サーバーからクライアントに送信される [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) メッセージを示しています。 [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素には、サブスクリプションの作成が成功したことを意味する NoError の値が含まれています。 [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) 要素により、サーバー上のプル通知サブスクリプションが一意に特定されます。 [Watermark](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) 要素は、メールボックス イベント キュー内のブックマークを表します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<SubscribeResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                   xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <SubscribeResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <SubscriptionId>d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
      <Watermark>AAAAAGUhAAAAAAAAAQ==</Watermark>
    </SubscribeResponseMessage>
  </ResponseMessages>
</SubscribeResponse>
```

サブスクリプションを作成すると、**SubscribeResponse** メッセージで返される**SubscriptionId** を使用して、ストリーミングされたイベントを取得できるようになります。 
  
## <a name="get-pull-notifications-by-using-ews"></a>EWS を使用したプル通知の取得
<a name="bk_getpull"> </a>

次の XML の例は、[SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) メッセージで返された [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) についての通知を取得するために、クライアントからサーバーに送信される [GetEvents 操作](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx)要求のメッセージを示しています。 最初の **GetEvents** 要求には、**Subscribe** 応答で返された [Watermark](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) を使用します。 その後の **GetEvents** 要求には、前の **GetEvents** 要求で返された最新の **Watermark** を使用します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEvents xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <SubscriptionId xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
  <Watermark xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">AAAAAGUhAAAAAAAAAQ==</Watermark>
</GetEvents>
```

次の XML の例は、サーバーからクライアントに送信される **GetEvents** 応答メッセージを示しています。 それぞれの **GetEvents** 応答には、1 つ以上のイベントに関する情報が含まれています。 **Watermark** は、イベントごとに返されます。 最新の **Watermark** は保存しておいて、次回の **GetEvents** 要求で使用する必要があります。 最後の **GetEvents** 要求以降にストア イベントが発生していない場合は、状態イベントが返されます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEventsResponseType xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <GetEventsResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <Notification>
        <SubscriptionId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
        <PreviousWatermark xmlns="https://schemas.microsoft.com/exchange/services/2006/types">AAAAAGUhAAAAAAAAAQ==</PreviousWatermark>
        <MoreEvents xmlns="https://schemas.microsoft.com/exchange/services/2006/types">false</MoreEvents>
        <NewMailEvent xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

サーバーからイベントを受信したら、[変更内容をクライアントに同期します](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps)。 サブスクリプションが不要になったら、[Unsubscribe 操作](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx)を使用してサーバーとのサブスクリプションを終了します。 
  
## <a name="next-steps"></a>次の手順
<a name="bk_nextsteps"> </a>

通知を受信したら、[フォルダー階層の同期](how-to-synchronize-folders-by-using-ews-in-exchange.md)や[変更されたフォルダーの内容の同期](how-to-synchronize-items-by-using-ews-in-exchange.md)を実行します。
  
## <a name="see-also"></a>関連項目


- [Exchange の通知サブスクリプション、メールボックス イベント、および EWS](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Exchange での EWS を使用したメールボックス イベントに関するストリーム通知](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Exchange の購読グループとメールボックス サーバー間のアフィニティを維持する](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [Exchange における EWS での通知関連エラーの処理](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Exchange のメールボックス同期と EWS](mailbox-synchronization-and-ews-in-exchange.md)
    


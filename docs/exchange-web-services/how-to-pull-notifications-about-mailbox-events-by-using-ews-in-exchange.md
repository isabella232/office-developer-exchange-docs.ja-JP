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
# <a name="pull-notifications-about-mailbox-events-by-using-ews-in-exchange"></a>EWS を使用して Exchange でメールボックスのイベントに関する通知をプルします。

EWS マネージ API または EWS を使用してプル通知の受信を登録し、イベントを取得する方法について説明します。
  
Exchange の EWS では、サーバーからクライアントへのメールボックスの変更内容に関する通知をクライアントが要求 (プル) できるようにするためにプル通知を使用します。
  
EWS マネージ API を使用して[サブスクリプションし、プル通知を取得する](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) [SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx)メソッドを使用して、プル通知のサブスクライブしている場合。 [GetEvents](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx)メソッドを使用してサーバーからイベントを取得します。 
  
プルの通知を購読するには、EWS を使用して、[購読の操作](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx)を使用して[サブスクリプションを作成](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews)をする解析、応答し、[通知を取得する](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) [GetEvents 操作](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx)を使用しています。
  
クライアントの変更またはサーバー上に作成されるアイテムの通知を受け取ると後に、ことができますし、[変更の同期します](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps)。
  
## <a name="subscribe-to-and-get-pull-notifications-by-using-the-ews-managed-api"></a>EWS マネージ API を使用したプル通知のサブスクライブと取得
<a name="bk_cepullewsma"> </a>

次のコード例では、プルの受信トレイ フォルダー内のすべてのイベント通知をサブスクライブする[SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx)メソッドを使用する方法を示します。 例は、 [GetEvents](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx)メソッドを使用してサーバーからイベントを取得します。 この例では、その**サービス**は、有効な[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)バインドと仮定します。 
  
```cs
// Subscribe to pull notifications in the Inbox.
PullSubscription subscription = service.SubscribeToPullNotifications( 
    new FolderId[] { WellKnownFolderName.Inbox }, 30, null, 
    EventType.NewMail, EventType.Created, EventType.Deleted,
    EventType.Modified, EventType.Moved, EventType.Copied, EventType.FreeBusyChanged); 
 
// Call GetEvents to retrieve events from the server. 
GetEventsResults events = subscription.GetEvents(); 
```

サーバーからイベントを受信したら、[サーバーを使用して変更を同期](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps)することができます。 指定されている登録解除の方法のいずれかを使用して、[の通知を購読する方法ですか?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe)サブスクリプションは、不要になったときに、サーバーでサブスクリプションを終了します。 
  
## <a name="subscribe-to-pull-notifications-by-using-ews"></a>EWS を使用したプル通知のサブスクライブ
<a name="bk_cepullews"> </a>

[購読操作](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx)を使用して、[受信トレイ] フォルダー内のすべての[EventTypes](http://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx)にサブスクライブするサーバーに送信する XML 要求の例を次に示します。 EWS のマネージ API が、 [SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx)メソッドを使用してプル通知にサブスクライブしているときに送信する XML 要求にもです。 
  
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

**Subscribe**操作の要求への応答としてクライアントにサーバーから送信される[SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx)メッセージを次の XML 例に示します。 NoError、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)の要素の値を含めることは、サブスクリプションが正常に作成されたことを意味します。 [サブスクリプション Id](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx)要素は、サーバー上でプル通知サブスクリプションを一意に識別します。 [透かし](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx)の要素は、メールボックス イベント キュー内のブックマークを表します。 
  
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

サブスクリプションを作成した後には、 **SubscribeResponse**メッセージで返される**サブスクリプション Id**を使用してイベントを今すぐ取得できます。 
  
## <a name="get-pull-notifications-by-using-ews"></a>EWS を使用したプル通知の取得
<a name="bk_getpull"> </a>

次の XML の例は、 [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx)メッセージで返される[サブスクリプション Id](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx)の通知を取得するクライアントからサーバーに送信される[GetEvents 操作](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx)の要求メッセージを示しています。 最初の**GetEvents**要求では、**購読**の応答で返される[ウォーターマーク](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx)を使用します。 **GetEvents**の後続の要求の前の**GetEvents**要求で返された最新の**ウォーターマーク**を使用します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEvents xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <SubscriptionId xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
  <Watermark xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">AAAAAGUhAAAAAAAAAQ==</Watermark>
</GetEvents>
```

次の XML の例は、サーバーからクライアントに送信される**GetEvents**応答メッセージを示しています。 **GetEvents**応答ごとに 1 つまたは複数のイベントに関する情報が含まれています。 **ウォーターマーク**がイベントごとに返されます。 最新の**ウォーターマーク**は保存され、次の**GetEvents**要求で使用する必要があります。 最後の**GetEvents**要求からストアのイベントが発生していない、状態イベントが返されます。 
  
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

した後[、クライアントへの変更を同期化](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps)、サーバーからイベントが表示されます。 サブスクリプションは、不要になったときに、サーバーでサブスクリプションを終了するには、[購読の取り消し操作](http://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx)を使用します。 
  
## <a name="next-steps"></a>次の手順
<a name="bk_nextsteps"> </a>

受信した後の通知、[フォルダー階層の同期](how-to-synchronize-folders-by-using-ews-in-exchange.md)または[変更するフォルダーの内容を同期](how-to-synchronize-items-by-using-ews-in-exchange.md)することができます。
  
## <a name="see-also"></a>関連項目


- [Notification subscriptions, mailbox events, and EWS in Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Exchange の EWS を使用してメールボックスのイベントに関する通知をストリーム](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Exchange の購読グループとメールボックス サーバー間のアフィニティを維持します。](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [Exchange における EWS での通知関連エラーの処理](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Exchange のメールボックス同期と EWS](mailbox-synchronization-and-ews-in-exchange.md)
    


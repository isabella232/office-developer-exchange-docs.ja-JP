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
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467047"
---
# <a name="subscribe-operation"></a>サブスクライブ操作

サブスクライブ操作は、クライアントアプリケーションに対して、プッシュまたはプル通知のどちらかをサブスクライブするために使用されます。 要求メッセージと応答の構造は、イベント通知の種類によって異なることに注意することが重要です。 
  
## <a name="pull-subscription-subscribe-request-example"></a>プルサブスクリプションのサブスクライブ要求の例

### <a name="description"></a>説明

次のコード例は、プルイベント通知サブスクリプションをサブスクライブする方法を示しています。 新しいメールが受信トレイに追加された場合、および受信トレイからアイテムが削除された場合、サブスクリプションはクライアントアプリケーションに通知します。 クライアントが10分以内にイベントに関する情報を要求しない場合、サブスクリプションはタイムアウトになります。 サブスクリプションの有効期限が切れた場合は、通知を引き続き要求するために、新しいサブスクリプションを確立する必要があります。
  
### <a name="code"></a>コード

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

### <a name="pull-subscription-subscribe-request-elements"></a>プルサブスクリプションサブスクライブ要求要素

要求では、次の要素が使用されます。
  
- [登録](subscribe.md)
    
- [PullSubscriptionRequest](pullsubscriptionrequest.md)
    
- [FolderIds](folderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [EventTypes](eventtypes.md)
    
- [EventType](eventtype.md)
    
- [Timeout](timeout.md)
    
Subscribe 操作の要求メッセージに関するその他のオプションについては、スキーマ階層を参照してください。 [PullSubscriptionRequest](pullsubscriptionrequest.md)要素から開始します。 
  
## <a name="successful-pull-subscription-subscribe-response-example"></a>成功したプルサブスクリプションサブスクライブ応答の例

### <a name="description"></a>説明

次の例は、成功したプルサブスクリプション応答を示しています。 応答には、サブスクリプションに関連付けられているイベントの配列を取得するために使用されるサブスクリプション識別子とウォーターマークが含まれています。 サブスクリプション識別子は、サブスクリプションからクライアントの登録を解除するためにも使用されます。
  
### <a name="code"></a>コード

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

### <a name="pull-subscription-subscribe-response-elements"></a>プルサブスクリプションのサブスクライブ応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SubscribeResponse](subscriberesponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [メッセージの表示](subscriberesponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [Watermark](watermark.md)
    
## <a name="pull-subscription-subscribe-error-response-example"></a>プルサブスクリプションサブスクライブエラー応答の例

### <a name="description"></a>説明

次の例は、Subscribe 要求に対するエラー応答を示しています。 このエラーは、代理人アクセスを使用して通知をサブスクライブしようとした場合に発生します。
  
### <a name="code"></a>コード

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

### <a name="pull-subscription-error-response-elements"></a>プルサブスクリプションエラー応答要素

エラー応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SubscribeResponse](subscriberesponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [メッセージの表示](subscriberesponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="push-subscription-request-example"></a>プッシュサブスクリプション要求の例

### <a name="description"></a>説明

次のコード例は、プッシュイベント通知サブスクリプションをサブスクライブする方法を示しています。 要求は、監視するフォルダー、監視するイベントの種類、状態通知の頻度、およびプッシュ通知を待機するクライアント Web サービスの URL を識別します。
  
### <a name="code"></a>コード

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

### <a name="comments"></a>コメント

プッシュ通知サブスクライブ要求が送信される前に、クライアント Web サービスがセットアップされている必要があります。それ以外の場合、最初の通知は有効なエンドポイントに送信されず、プッシュ通知は失敗します。 詳細については、「[プッシュ通知のサンプルアプリケーション](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)」を参照してください。
  
再度サブスクライブすると、新しい[SubscriptionId (GetEvents)](subscriptionid-getevents.md)が作成されます。 以前のサブスクリプションのウォーターマークを使用して、前のサブスクリプションが終了した時点でサブスクライブを再度行います。 
  
### <a name="push-subscription-request-elements"></a>プッシュサブスクリプションの要求要素

要求では、次の要素が使用されます。
  
- [登録](subscribe.md)
    
- [PushSubscriptionRequest](pushsubscriptionrequest.md)
    
- [FolderIds](folderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [EventTypes](eventtypes.md)
    
- [EventType](eventtype.md)
    
- [StatusFrequency](statusfrequency.md)
    
- [.Url](url-ex15websvcsotherref.md)
    
## <a name="successful-push-subscription-response-example"></a>成功したプッシュサブスクリプション応答の例

### <a name="description"></a>説明

次の例は、成功したプッシュサブスクリプション応答を示しています。 
  
### <a name="code"></a>コード

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

### <a name="push-subscription-response-elements"></a>プッシュサブスクリプション応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SubscribeResponse](subscriberesponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [メッセージの表示](subscriberesponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [Watermark](watermark.md)
    
## <a name="see-also"></a>関連項目



[Unsubscribe 操作](unsubscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)


[プルサブスクリプションの使用](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[プッシュ通知のサンプル アプリケーション](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)


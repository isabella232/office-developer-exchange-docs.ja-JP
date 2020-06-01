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
# <a name="getevents-operation"></a>GetEvents 操作

**GetEvents**操作は、プルサブスクリプションクライアントがクライアントアクセスサーバーからの通知を要求するために使用されます。 **GetEvents**操作の応答は、最後の通知以降にメールボックスで発生したアイテムとイベントの配列を返します。 
  
> [!IMPORTANT]
> **Deleteuserconfiguration**操作は、イベント通知システムの移動イベントをトリガーします。 ユーザー構成オブジェクトは、収集に移動されます。 
  
## <a name="remarks"></a>注釈

予定表アイテムの変更によって、複数のイベントが生成されることがあります。 これらのイベントは、メールボックス内に作成された一時アイテム、空き時間情報データストレージアイテムが通常の予定表の操作の一部として変更された結果、またはその両方で発生します。 アイテムクラス "IPM.Web サービスクライアントでは、SchedulePlus データ "を無視する必要があります。 これらの一時アイテムは、作成後に削除されます。そのため、これらのアイテムを取得しようとすると、アイテムが見つからなかったことを示すエラーが返されます。
  
## <a name="getevents-request-example"></a>GetEvents 要求の例

### <a name="description"></a>説明

次の例は、サブスクリプション識別子とウォーターマークで識別されるサブスクリプションに関連付けられたイベントとアイテムを要求する方法を示しています。
  
### <a name="code"></a>コード

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

### <a name="getevents-request-elements"></a>GetEvents Request 要素

要求では、次の要素が使用されます。
  
- [GetEvents](getevents.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [Watermark](watermark.md)
    
## <a name="successful-getevents-response-example"></a>Successful GetEvents response の例

### <a name="description"></a>説明

次の応答の例は、前回の通知要求がサーバーに送信されてから、2つの新しいメールメッセージが存在するという通知を示しています。
  
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

### <a name="comments"></a>コメント

> [!NOTE]
> 読みやすくするために、アイテムとフォルダーの識別子が短縮されています。 
  
### <a name="getevents-response-elements"></a>GetEvents response 要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [Getイベント応答](geteventsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetEventsResponseMessage](geteventsresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [通知](notification-ex15websvcsotherref.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [PreviousWatermark](previouswatermark.md)
    
- [その他のイベント](moreevents.md)
    
- [NewMailEvent](newmailevent.md)
    
- [Watermark](watermark.md)
    
- [示](timestamp.md)
    
- [ItemId](itemid.md)
    
- [ParentFolderId](parentfolderid.md)
    
**GetEvents**操作の応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。 [通知](notification-ex15websvcsotherref.md)要素から開始します。 
  
## <a name="getevents-error-response-example"></a>GetEvents エラー応答の例

### <a name="description"></a>説明

次の例は、 **GetEvents**要求に対するエラー応答を示しています。 
  
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

## <a name="remarks"></a>注釈

**GetEvents**要求を処理する場合、クライアントアクセスサーバーは次の手順を実行します。 
  
1. 要求の SubscriptionID は、クライアントアクセスサーバーでホストされている有効なサブスクリプションであることが確認されます。 そうでない場合、 **GetEvents**呼び出しは失敗します。 
    
2. 要求に対する認証済みユーザーの SMTP アドレスは、サブスクリプションを作成したユーザーの SMTP アドレスと比較されます。 一致しない場合、 **GetEvents**要求は失敗します。 
    
3. サブスクリプションキューは、クライアントへの送信を待機しているイベントに対して照会されます。 キューが空でない場合、キューから最初の50イベントがプルされ、通知にエンコードされます。
    
4. キューにイベントが見つからない場合は、StatusEvent が生成され、通知応答にエンコードされます。
    
5. 通知応答がクライアントに返されます。
    
6. 通知に含まれるイベントは、サブスクリプションキューから削除され、サブスクリプションのクライアントアクセスサーバーのローカルの最後のウォーターマークは、返される最後のイベントのウォーターマークに設定されます。
    
7. サブスクリプションのタイムアウトタイマーはリセットされます。
    
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)


[プルサブスクリプションの使用](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)


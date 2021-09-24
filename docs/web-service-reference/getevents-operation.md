---
title: GetEvents 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetEvents
api_type:
- schema
ms.assetid: f268efe5-9a1a-41a2-b6a6-51fcde7720a1
description: GetEvents 操作は、プル サブスクリプション クライアントがクライアント アクセス サーバーから通知を要求するために使用します。 GetEvents 操作応答は、最後の通知以降にメールボックスで発生したアイテムとイベントの配列を返します。
ms.openlocfilehash: 72d99a654921794115d56d28327a39a21c9ea378
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511601"
---
# <a name="getevents-operation"></a>GetEvents 操作

**GetEvents 操作は**、プル サブスクリプション クライアントがクライアント アクセス サーバーから通知を要求するために使用します。 **GetEvents 操作** 応答は、最後の通知以降にメールボックスで発生したアイテムとイベントの配列を返します。 
  
> [!IMPORTANT]
> **DeleteUserConfiguration 操作は**、イベント通知システムの移動イベントをトリガーします。 ユーザー構成オブジェクトは、ゴミ箱に移動されます。 
  
## <a name="notes"></a>メモ

予定表アイテムを変更すると、複数のイベントが生成される場合があります。 これらのイベントは、メールボックス内に一時的なアイテムが作成された結果、空き時間情報データストレージ アイテムが通常の予定表操作の一部として変更された結果、または両方です。 アイテム クラス "IPM" のイベント。SchedulePlus.FreeBusy.BinaryData" は、Web サービス クライアントでは無視する必要があります。 これらの一時アイテムは、作成後に削除されます。したがって、これらのアイテムを取得しようとすると、アイテムが見つからなかったというエラーが返されます。
  
## <a name="getevents-request-example"></a>GetEvents 要求の例

### <a name="description"></a>説明

次の例は、サブスクリプション識別子と透かしによって識別されるサブスクリプションに関連付けられているイベントとアイテムを要求する方法を示しています。
  
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

### <a name="getevents-request-elements"></a>GetEvents 要求要素

要求では、次の要素が使用されます。
  
- [GetEvents](getevents.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [Watermark](watermark.md)
    
## <a name="successful-getevents-response-example"></a>GetEvents 応答の成功例

### <a name="description"></a>説明

次の応答例は、最後の通知要求がサーバーに送信された後、2 つの新しいメール メッセージが存在する通知を示しています。
  
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
> アイテムとフォルダーの識別子は、読みやすさを維持するために短縮されました。 
  
### <a name="getevents-response-elements"></a>GetEvents 応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetEventsResponse](geteventsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetEventsResponseMessage](geteventsresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [通知](notification-ex15websvcsotherref.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [PreviousWatermark](previouswatermark.md)
    
- [MoreEvents](moreevents.md)
    
- [NewMailEvent](newmailevent.md)
    
- [Watermark](watermark.md)
    
- [TimeStamp](timestamp.md)
    
- [ItemId](itemid.md)
    
- [ParentFolderId](parentfolderid.md)
    
**GetEvents** 操作の応答メッセージに関するその他のオプションを見つけるには、スキーマ階層を確認します。 Notification 要素 [から開始](notification-ex15websvcsotherref.md) します。 
  
## <a name="getevents-error-response-example"></a>GetEvents エラー応答の例

### <a name="description"></a>説明

次の例は、GetEvents 要求に対する **エラー応答を示** しています。 
  
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

**GetEvents 要求を処理する** 場合、クライアント アクセス サーバーは次の手順を実行します。 
  
1. 要求の SubscriptionID が、クライアント アクセス サーバーでホストされている有効なサブスクリプションである確認されます。 それではない場合 **、GetEvents 呼び出しは** 失敗します。 
    
2. 要求の認証されたユーザーの SMTP アドレスは、サブスクリプションを作成したユーザーの SMTP アドレスと比較されます。 一致しない場合 **、GetEvents 要求は** 失敗します。 
    
3. サブスクリプション キューは、クライアントへの送信を待機しているイベントに対して照会されます。 キューが空ではない場合、キューの最初の 50 イベントがキューからプルされ、通知にエンコードされます。
    
4. キューにイベントが見つからない場合、StatusEvent が生成され、通知応答にエンコードされます。
    
5. 通知応答がクライアントに返されます。
    
6. 通知に含まれるイベントはサブスクリプション キューから削除され、サブスクリプションのクライアント アクセス サーバーのローカルの最後の透かしは、返される最後のイベントの透かしに設定されます。
    
7. サブスクリプションのタイムアウト タイマーがリセットされます。
    
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)


[プル サブスクリプションの使用](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)


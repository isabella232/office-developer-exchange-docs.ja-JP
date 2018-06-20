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
description: GetEvents 操作は、クライアント アクセス サーバーから、プル サブスクリプションのクライアントによって、通知を要求する使用されます。 GetEvents 操作の応答では、項目と以降のメールボックスに最後に通知するイベントの配列を返します。
ms.openlocfilehash: 1a23a9d570a4554e54becb7927f25dff89888c74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760705"
---
# <a name="getevents-operation"></a>GetEvents 操作

**GetEvents**操作は、クライアント アクセス サーバーから、プル サブスクリプションのクライアントによって、通知を要求する使用されます。 **GetEvents**操作の応答では、項目と以降のメールボックスに最後に通知するイベントの配列を返します。 
  
> [!IMPORTANT]
> **DeleteUserConfiguration**操作は、イベント通知システムの移動イベントをトリガーします。 ユーザー設定のオブジェクトを移動するが、ごみ箱をあさる。 
  
## <a name="remarks"></a>備考

予定表アイテムへの変更は、複数のイベントの生成があります。 これらのイベントは、一時アイテムが作成される、メールボックスでは、通常の予定表の操作、またはその両方の一部として変更される空き時間情報データ記憶域の項目の結果です。 項目のイベント クラスの"IPM.SchedulePlus.FreeBusy.BinaryData」は、Web サービス クライアントによって無視されます。 一時アイテムを削除して作成されます。したがって、これらの項目を取得しようとすると場合、エラーが返ります、項目が見つからなかったことを示します。
  
## <a name="getevents-request-example"></a>GetEvents 要求の例

### <a name="description"></a>説明

次の例では、イベントとサブスクリプションの識別子とウォーターマークで識別されるサブスクリプションに関連付けられている項目を要求する方法を示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetEvents xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <Watermark>AAAAAMAGAAAAAAAAAQ==</Watermark>
    </GetEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getevents-request-elements"></a>GetEvents 要求要素

次の要素は、要求で使用されます。
  
- [GetEvents](getevents.md)
    
- [サブスクリプション Id (GetEvents)](subscriptionid-getevents.md)
    
- [透かし](watermark.md)
    
## <a name="successful-getevents-response-example"></a>GetEvents 応答の成功の例

### <a name="description"></a>説明

最後の通知要求がサーバーに送信された後、次の応答の例は 2 つの新しいメール メッセージの存在を通知を示します。
  
### <a name="code"></a>コード

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
    <GetEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
> アイテムおよびフォルダーの識別子は、読みやすさを保持するために短縮されています。 
  
### <a name="getevents-response-elements"></a>GetEvents 応答の要素

次の要素は、応答で使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetEventsResponse](geteventsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetEventsResponseMessage](geteventsresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [通知](notification-ex15websvcsotherref.md)
    
- [サブスクリプション Id (GetEvents)](subscriptionid-getevents.md)
    
- [PreviousWatermark](previouswatermark.md)
    
- [イベント](moreevents.md)
    
- [NewMailEvent](newmailevent.md)
    
- [透かし](watermark.md)
    
- [タイムスタンプ](timestamp.md)
    
- [ItemId](itemid.md)
    
- [ParentFolderId](parentfolderid.md)
    
**GetEvents**操作の応答メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。 [通知](notification-ex15websvcsotherref.md)の要素から開始します。 
  
## <a name="getevents-error-response-example"></a>GetEvents エラー応答の例

### <a name="description"></a>説明

**GetEvents**要求に対してエラー応答の例を次に示します。 
  
### <a name="code"></a>コード

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
    <GetEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="remarks"></a>備考

**GetEvents**要求を処理するときにクライアント アクセス サーバーは、次の手順を実行します。 
  
1. 要求のサブスクリプション Id が、クライアント アクセス サーバーでホストされている有効なサブスクリプションを使用することを確認します。 そうでない場合、 **GetEvents**呼び出しは失敗します。 
    
2. 要求の認証済みユーザーの SMTP アドレスは、サブスクリプションを作成したユーザーの SMTP アドレスと比較されます。 それらが一致しない場合は、 **GetEvents**要求が失敗します。 
    
3. サブスクリプションのキューでは、クライアントに送信されるを待機しているイベントが照会されます。 キューが空でない場合は、キューから最初の 50 のイベントがキューから取得し、通知にエンコードされました。
    
4. キュー内のイベントが見つからない場合、StatusEvent が生成され、通知の応答にエンコードします。
    
5. 通知の応答がクライアントに返されます。
    
6. サブスクリプションのキューからの通知に含まれているイベントを削除し、クライアント アクセス サーバー ローカル最新のウォーターマークのサブスクリプションが返される最後のイベントのウォーターマークを設定します。
    
7. サブスクリプションのタイムアウト タイマーがリセットされます。
    
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)


[プル サブスクリプションを使用します。](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)


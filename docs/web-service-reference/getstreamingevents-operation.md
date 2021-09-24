---
title: GetStreamingEvents 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetStreamingEvents
api_type:
- schema
ms.assetid: 8da95423-72bc-4034-90a8-162eedcd059b
description: GetStreamingEvents EWS 操作に関する情報を検索します。
ms.openlocfilehash: 794407c2224e606be4f32cc610eff9f95e65a83b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523063"
---
# <a name="getstreamingevents-operation"></a>GetStreamingEvents 操作

**GetStreamingEvents** EWS 操作に関する情報を検索します。 
  
**GetStreamingEvents** 操作は、サブスクリプション クライアントをストリーミングしてクライアント アクセス サーバーから通知を要求するために使用されます。 **GetStreamingEvents** 応答は、最後の通知以降にメールボックスで発生したアイテムとイベントの配列を返します。 
  
## <a name="getstreamingevents-request-example"></a>GetStreamingEvents 要求の例

### <a name="description"></a>説明

**GetStreamingEvents** 操作の次の例は、サブスクリプション識別子によって識別されるサブスクリプションに関連付けられているイベントとアイテムを要求する方法を示しています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
  xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Body>
    <GetStreamingEvents xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <ConnectionTimeout>30</ConnectionTimeout>
    </GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getstreamingevents-request-elements"></a>GetStreamingEvents 要求要素

要求では、次の要素が使用されます。
  
- [GetStreamingEvents](getstreamingevents.md)
    
- [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md)
    
- [ConnectionTimeout](connectiontimeout.md)
    
## <a name="successful-getstreamingevents-response-example"></a>GetStreamingEvents 応答の成功例

### <a name="description"></a>説明

**GetStreamingEvents 応答の次** の例は、新しい電子メール メッセージを受信するときにクライアントに送信される通知を示しています。 これには、CreatedEvent、NewMail、および ModifiedEvent のイベントに関する通知が含まれます。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Header xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <ServerVersionInfo xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
</soap:Header>
<soap:Body xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <m:GetStreamingEventsResponse xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
    <m:ResponseMessages>
      <m:GetStreamingEventsResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Notifications>
          <m:Notification>
            <t:SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</t:SubscriptionId>
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

### <a name="getstreamingevents-response-elements"></a>GetStreamingEvents 応答要素

応答では、次の要素が使用されます。
  
- [GetStreamingEventsResponse](getstreamingeventsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md)
    
- [NotesFolderPermissionLevel](notesfolderpermissionlevel.md)
    
- [通知](notification-ex15websvcsotherref.md)
    
- [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md)
    
**GetStreamingEvents** 操作の応答メッセージに関するその他のオプションを見つけるには、スキーマ階層を参照してください。 Notification 要素 [から開始](notification-ex15websvcsotherref.md) します。 
  
## <a name="getstreamingevents-error-response-example"></a>GetStreamingEvents エラー応答の例

### <a name="description"></a>説明

次の例は **、GetStreamingEvents 要求** に対するエラー応答を示しています。 
  
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
    <GetStreamingEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetStreamingEventsResponseMessage ResponseClass="Error">
        <m:MessageText></m:MessageText>
        <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        <m:ResponseCode>ErrorInvalidSubscription</m:ResponseCode>
        <m:ConnectionStatus>Closed</m:ConnectionStatus>
      </m:ResponseMessages>
    </GetStreamingEventsResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="remarks"></a>注釈

**GetStreamingEvents 要求を処理する** 場合、クライアント アクセス サーバーは次の手順を実行します。 
  
1. 要求 [の SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md) が、クライアント アクセス サーバーでホストされている有効なサブスクリプションとして確認されます。 それではない場合 **、GetStreamingEvents 呼び出しは失敗** します。 
    
2. 要求の認証されたユーザーの SMTP アドレスが偽装権限を持っている検証されます。 そうしない場合 **、GetStreamingEvents 要求は失敗** します。 
    
3. サブスクリプション キューは、クライアントへの送信を待機しているイベントに対して照会されます。 キューが空ではない場合、キューの最初の 50 イベントがキューからプルされ、通知にエンコードされます。
    
4. キューにイベントが見つからない場合 [、StatusEvent](statusevent.md) が生成され、通知応答にエンコードされます。 
    
5. 通知応答がクライアントに返されます。
    
6. 通知に含まれるイベントはサブスクリプション キューから削除され、サブスクリプションのクライアント アクセス サーバーローカルの最後の透かしは、返される最後のイベントの透かしに設定されます。
    
7. サブスクリプションのタイムアウト タイマーがリセットされます。
    
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)


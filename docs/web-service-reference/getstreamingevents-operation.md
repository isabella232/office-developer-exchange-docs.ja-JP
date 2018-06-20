---
title: GetStreamingEvents 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEvents
api_type:
- schema
ms.assetid: 8da95423-72bc-4034-90a8-162eedcd059b
description: 操作 GetStreamingEvents EWS についての情報を検索します。
ms.openlocfilehash: 0e93be7b14cb1ca6a2a9821b016f7bdc0e8d7772
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831673"
---
# <a name="getstreamingevents-operation"></a>GetStreamingEvents 操作

**GetStreamingEvents** EWS の操作に関する情報を検索します。 
  
**GetStreamingEvents**操作は、クライアント アクセス サーバーからの通知を要求するのには、ストリーミング サブスクリプション クライアントによって使用されます。 **GetStreamingEvents**の応答は、アイテムおよび以降のメールボックスに最後に通知するイベントの配列を返します。 
  
## <a name="getstreamingevents-request-example"></a>GetStreamingEvents 要求の例

### <a name="description"></a>説明

**GetStreamingEvents**操作の次の例では、イベントとサブスクリプションの識別子によって識別されるサブスクリプションに関連付けられている項目を要求する方法を示します。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
  xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Body>
    <GetStreamingEvents xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <ConnectionTimeout>30</ConnectionTimeout>
    </GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getstreamingevents-request-elements"></a>GetStreamingEvents 要求の要素

次の要素は、要求で使用されます。
  
- [GetStreamingEvents](getstreamingevents.md)
    
- [サブスクリプション Id (GetStreamingEvents)](subscriptionid-getstreamingevents.md)
    
- [タイムアウト](connectiontimeout.md)
    
## <a name="successful-getstreamingevents-response-example"></a>成功した GetStreamingEvents の応答の例

### <a name="description"></a>説明

**GetStreamingEvents**応答の次の使用例は、新しい電子メール メッセージを受信したときにクライアントに送信される通知を示しています。 次のイベントの通知が含まれています: CreatedEvent、NewMail、および ModifiedEvent。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Header xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <ServerVersionInfo xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
</soap:Header>
<soap:Body xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <m:GetStreamingEventsResponse xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="getstreamingevents-response-elements"></a>GetStreamingEvents の応答の要素

次の要素は、応答で使用されます。
  
- [GetStreamingEventsResponse](getstreamingeventsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md)
    
- [NotesFolderPermissionLevel](notesfolderpermissionlevel.md)
    
- [通知](notification-ex15websvcsotherref.md)
    
- [サブスクリプション Id (GetStreamingEvents)](subscriptionid-getstreamingevents.md)
    
**GetStreamingEvents**操作の応答メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。 [通知](notification-ex15websvcsotherref.md)の要素から開始します。 
  
## <a name="getstreamingevents-error-response-example"></a>GetStreamingEvents エラー応答の例

### <a name="description"></a>説明

**GetStreamingEvents**要求に対してエラー応答の例を次に示します。 
  
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
    <GetStreamingEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="remarks"></a>備考

**GetStreamingEvents**要求を処理するときにクライアント アクセス サーバーは次の手順を実行します。 
  
1. 要求の[サブスクリプション Id (GetStreamingEvents)](subscriptionid-getstreamingevents.md)は、クライアント アクセス サーバーでホストされている有効なサブスクリプションを使用することを確認します。 そうでない場合、 **GetStreamingEvents**呼び出しが失敗します。 
    
2. 偽装権限を持っている要求の認証済みユーザーの SMTP アドレスが検証されます。 署名がない場合、 **GetStreamingEvents**要求が失敗します。 
    
3. サブスクリプションのキューでは、クライアントに送信されるを待機しているイベントが照会されます。 キューが空でない場合は、キューから最初の 50 のイベントがキューから取得し、通知にエンコードされました。
    
4. キュー内のイベントが見つからない場合、 [StatusEvent](statusevent.md)が生成され、通知の応答にエンコードされました。 
    
5. 通知の応答がクライアントに返されます。
    
6. 通知に含まれるイベントをサブスクリプションのキューから削除し、サブスクリプションのクライアント アクセス サーバーのローカルの最新のウォーターマークが返される最後のイベントのウォーターマークを設定します。
    
7. サブスクリプションのタイムアウト タイマーがリセットされます。
    
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)


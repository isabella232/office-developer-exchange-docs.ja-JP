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
# <a name="getstreamingevents-operation"></a><span data-ttu-id="74e53-103">GetStreamingEvents 操作</span><span class="sxs-lookup"><span data-stu-id="74e53-103">GetStreamingEvents operation</span></span>

<span data-ttu-id="74e53-104">**GetStreamingEvents** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="74e53-104">Find information about the **GetStreamingEvents** EWS operation.</span></span> 
  
<span data-ttu-id="74e53-105">**GetStreamingEvents**操作は、クライアント アクセス サーバーからの通知を要求するのには、ストリーミング サブスクリプション クライアントによって使用されます。</span><span class="sxs-lookup"><span data-stu-id="74e53-105">The **GetStreamingEvents** operation is used by streaming subscription clients to request notifications from the Client Access server.</span></span> <span data-ttu-id="74e53-106">**GetStreamingEvents**の応答は、アイテムおよび以降のメールボックスに最後に通知するイベントの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="74e53-106">The **GetStreamingEvents** response returns an array of items and events that have occurred in a mailbox since the last the notification.</span></span> 
  
## <a name="getstreamingevents-request-example"></a><span data-ttu-id="74e53-107">GetStreamingEvents 要求の例</span><span class="sxs-lookup"><span data-stu-id="74e53-107">GetStreamingEvents request example</span></span>

### <a name="description"></a><span data-ttu-id="74e53-108">説明</span><span class="sxs-lookup"><span data-stu-id="74e53-108">Description</span></span>

<span data-ttu-id="74e53-109">**GetStreamingEvents**操作の次の例では、イベントとサブスクリプションの識別子によって識別されるサブスクリプションに関連付けられている項目を要求する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="74e53-109">The following example of a **GetStreamingEvents** operation shows how to request the events and items that are associated with a subscription that is identified by the subscription identifier.</span></span> 
  
### <a name="code"></a><span data-ttu-id="74e53-110">コード</span><span class="sxs-lookup"><span data-stu-id="74e53-110">Code</span></span>

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

### <a name="getstreamingevents-request-elements"></a><span data-ttu-id="74e53-111">GetStreamingEvents 要求の要素</span><span class="sxs-lookup"><span data-stu-id="74e53-111">GetStreamingEvents request elements</span></span>

<span data-ttu-id="74e53-112">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="74e53-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="74e53-113">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="74e53-113">GetStreamingEvents</span></span>](getstreamingevents.md)
    
- [<span data-ttu-id="74e53-114">サブスクリプション Id (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="74e53-114">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md)
    
- [<span data-ttu-id="74e53-115">タイムアウト</span><span class="sxs-lookup"><span data-stu-id="74e53-115">ConnectionTimeout</span></span>](connectiontimeout.md)
    
## <a name="successful-getstreamingevents-response-example"></a><span data-ttu-id="74e53-116">成功した GetStreamingEvents の応答の例</span><span class="sxs-lookup"><span data-stu-id="74e53-116">Successful GetStreamingEvents response example</span></span>

### <a name="description"></a><span data-ttu-id="74e53-117">説明</span><span class="sxs-lookup"><span data-stu-id="74e53-117">Description</span></span>

<span data-ttu-id="74e53-118">**GetStreamingEvents**応答の次の使用例は、新しい電子メール メッセージを受信したときにクライアントに送信される通知を示しています。</span><span class="sxs-lookup"><span data-stu-id="74e53-118">The following example of a **GetStreamingEvents** response shows the notifications that are sent to the client when a new email message is received.</span></span> <span data-ttu-id="74e53-119">次のイベントの通知が含まれています: CreatedEvent、NewMail、および ModifiedEvent。</span><span class="sxs-lookup"><span data-stu-id="74e53-119">It includes notifications for the following events: CreatedEvent, NewMail, and ModifiedEvent.</span></span> 
  
### <a name="code"></a><span data-ttu-id="74e53-120">コード</span><span class="sxs-lookup"><span data-stu-id="74e53-120">Code</span></span>

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

### <a name="getstreamingevents-response-elements"></a><span data-ttu-id="74e53-121">GetStreamingEvents の応答の要素</span><span class="sxs-lookup"><span data-stu-id="74e53-121">GetStreamingEvents response elements</span></span>

<span data-ttu-id="74e53-122">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="74e53-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="74e53-123">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="74e53-123">GetStreamingEventsResponse</span></span>](getstreamingeventsresponse.md)
    
- [<span data-ttu-id="74e53-124">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="74e53-124">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="74e53-125">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="74e53-125">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md)
    
- [<span data-ttu-id="74e53-126">NotesFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="74e53-126">NotesFolderPermissionLevel</span></span>](notesfolderpermissionlevel.md)
    
- [<span data-ttu-id="74e53-127">通知</span><span class="sxs-lookup"><span data-stu-id="74e53-127">Notification</span></span>](notification-ex15websvcsotherref.md)
    
- [<span data-ttu-id="74e53-128">サブスクリプション Id (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="74e53-128">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md)
    
<span data-ttu-id="74e53-129">**GetStreamingEvents**操作の応答メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="74e53-129">To find other options for the response message of the **GetStreamingEvents** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="74e53-130">[通知](notification-ex15websvcsotherref.md)の要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="74e53-130">Start at the [Notification](notification-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="getstreamingevents-error-response-example"></a><span data-ttu-id="74e53-131">GetStreamingEvents エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="74e53-131">GetStreamingEvents error response example</span></span>

### <a name="description"></a><span data-ttu-id="74e53-132">説明</span><span class="sxs-lookup"><span data-stu-id="74e53-132">Description</span></span>

<span data-ttu-id="74e53-133">**GetStreamingEvents**要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74e53-133">The following example shows an error response to a **GetStreamingEvents** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="74e53-134">コード</span><span class="sxs-lookup"><span data-stu-id="74e53-134">Code</span></span>

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

## <a name="remarks"></a><span data-ttu-id="74e53-135">備考</span><span class="sxs-lookup"><span data-stu-id="74e53-135">Remarks</span></span>

<span data-ttu-id="74e53-136">**GetStreamingEvents**要求を処理するときにクライアント アクセス サーバーは次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="74e53-136">When processing a **GetStreamingEvents** request, the Client Access server performs the following steps:</span></span> 
  
1. <span data-ttu-id="74e53-137">要求の[サブスクリプション Id (GetStreamingEvents)](subscriptionid-getstreamingevents.md)は、クライアント アクセス サーバーでホストされている有効なサブスクリプションを使用することを確認します。</span><span class="sxs-lookup"><span data-stu-id="74e53-137">The [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md) of the request is confirmed to be a valid subscription that is hosted on the Client Access server.</span></span> <span data-ttu-id="74e53-138">そうでない場合、 **GetStreamingEvents**呼び出しが失敗します。</span><span class="sxs-lookup"><span data-stu-id="74e53-138">If it is not, the **GetStreamingEvents** call fails.</span></span> 
    
2. <span data-ttu-id="74e53-139">偽装権限を持っている要求の認証済みユーザーの SMTP アドレスが検証されます。</span><span class="sxs-lookup"><span data-stu-id="74e53-139">The SMTP address of the authenticated user for the request is validated to have impersonation rights.</span></span> <span data-ttu-id="74e53-140">署名がない場合、 **GetStreamingEvents**要求が失敗します。</span><span class="sxs-lookup"><span data-stu-id="74e53-140">If they do not, the **GetStreamingEvents** request fails.</span></span> 
    
3. <span data-ttu-id="74e53-141">サブスクリプションのキューでは、クライアントに送信されるを待機しているイベントが照会されます。</span><span class="sxs-lookup"><span data-stu-id="74e53-141">The subscription queue is queried for events that are waiting to be sent to the client.</span></span> <span data-ttu-id="74e53-142">キューが空でない場合は、キューから最初の 50 のイベントがキューから取得し、通知にエンコードされました。</span><span class="sxs-lookup"><span data-stu-id="74e53-142">If the queue is not empty, the first 50 events from the queue are pulled from the queue and encoded into a notification.</span></span>
    
4. <span data-ttu-id="74e53-143">キュー内のイベントが見つからない場合、 [StatusEvent](statusevent.md)が生成され、通知の応答にエンコードされました。</span><span class="sxs-lookup"><span data-stu-id="74e53-143">If no events are found in the queue, a [StatusEvent](statusevent.md) is generated and encoded into a notification response.</span></span> 
    
5. <span data-ttu-id="74e53-144">通知の応答がクライアントに返されます。</span><span class="sxs-lookup"><span data-stu-id="74e53-144">The notification response is returned to the client.</span></span>
    
6. <span data-ttu-id="74e53-145">通知に含まれるイベントをサブスクリプションのキューから削除し、サブスクリプションのクライアント アクセス サーバーのローカルの最新のウォーターマークが返される最後のイベントのウォーターマークを設定します。</span><span class="sxs-lookup"><span data-stu-id="74e53-145">The events that are included in the notification are removed from the subscription queue and the Client Access server-local last watermark for the subscription is set to the watermark of the last event that is returned.</span></span>
    
7. <span data-ttu-id="74e53-146">サブスクリプションのタイムアウト タイマーがリセットされます。</span><span class="sxs-lookup"><span data-stu-id="74e53-146">The timeout timer for the subscription is reset.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="74e53-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="74e53-147">See also</span></span>



[<span data-ttu-id="74e53-148">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="74e53-148">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="74e53-149">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="74e53-149">Unsubscribe operation</span></span>](unsubscribe-operation.md)


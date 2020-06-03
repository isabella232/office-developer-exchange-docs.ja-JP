---
title: GetStreamingEvents の操作
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
description: GetStreamingEvents EWS 操作に関する情報を検索します。
ms.openlocfilehash: 27744ec40d7c7cb551f35ed5f6fcb726f23d4865
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530170"
---
# <a name="getstreamingevents-operation"></a><span data-ttu-id="6018b-103">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="6018b-103">GetStreamingEvents operation</span></span>

<span data-ttu-id="6018b-104">**Getstreamingevents** EWS 操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="6018b-104">Find information about the **GetStreamingEvents** EWS operation.</span></span> 
  
<span data-ttu-id="6018b-105">**Getstreamingevents**操作は、ストリーミングサブスクリプションクライアントがクライアントアクセスサーバーからの通知を要求するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="6018b-105">The **GetStreamingEvents** operation is used by streaming subscription clients to request notifications from the Client Access server.</span></span> <span data-ttu-id="6018b-106">**Getstreamingevents**応答は、最後の通知以降にメールボックスで発生したアイテムとイベントの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="6018b-106">The **GetStreamingEvents** response returns an array of items and events that have occurred in a mailbox since the last the notification.</span></span> 
  
## <a name="getstreamingevents-request-example"></a><span data-ttu-id="6018b-107">GetStreamingEvents 要求の例</span><span class="sxs-lookup"><span data-stu-id="6018b-107">GetStreamingEvents request example</span></span>

### <a name="description"></a><span data-ttu-id="6018b-108">Description</span><span class="sxs-lookup"><span data-stu-id="6018b-108">Description</span></span>

<span data-ttu-id="6018b-109">次の**Getstreamingevents**操作の例は、サブスクリプション識別子によって識別されるサブスクリプションに関連付けられているイベントとアイテムを要求する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="6018b-109">The following example of a **GetStreamingEvents** operation shows how to request the events and items that are associated with a subscription that is identified by the subscription identifier.</span></span> 
  
### <a name="code"></a><span data-ttu-id="6018b-110">コード</span><span class="sxs-lookup"><span data-stu-id="6018b-110">Code</span></span>

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

### <a name="getstreamingevents-request-elements"></a><span data-ttu-id="6018b-111">GetStreamingEvents 要求要素</span><span class="sxs-lookup"><span data-stu-id="6018b-111">GetStreamingEvents request elements</span></span>

<span data-ttu-id="6018b-112">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="6018b-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="6018b-113">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="6018b-113">GetStreamingEvents</span></span>](getstreamingevents.md)
    
- [<span data-ttu-id="6018b-114">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="6018b-114">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md)
    
- [<span data-ttu-id="6018b-115">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="6018b-115">ConnectionTimeout</span></span>](connectiontimeout.md)
    
## <a name="successful-getstreamingevents-response-example"></a><span data-ttu-id="6018b-116">Successful GetStreamingEvents 応答の例</span><span class="sxs-lookup"><span data-stu-id="6018b-116">Successful GetStreamingEvents response example</span></span>

### <a name="description"></a><span data-ttu-id="6018b-117">Description</span><span class="sxs-lookup"><span data-stu-id="6018b-117">Description</span></span>

<span data-ttu-id="6018b-118">次の**Getstreamingevents**応答の例は、新しい電子メールメッセージの受信時にクライアントに送信される通知を示しています。</span><span class="sxs-lookup"><span data-stu-id="6018b-118">The following example of a **GetStreamingEvents** response shows the notifications that are sent to the client when a new email message is received.</span></span> <span data-ttu-id="6018b-119">CreatedEvent、NewMail、および、次のイベントの通知が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6018b-119">It includes notifications for the following events: CreatedEvent, NewMail, and ModifiedEvent.</span></span> 
  
### <a name="code"></a><span data-ttu-id="6018b-120">コード</span><span class="sxs-lookup"><span data-stu-id="6018b-120">Code</span></span>

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

### <a name="getstreamingevents-response-elements"></a><span data-ttu-id="6018b-121">GetStreamingEvents 応答要素</span><span class="sxs-lookup"><span data-stu-id="6018b-121">GetStreamingEvents response elements</span></span>

<span data-ttu-id="6018b-122">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="6018b-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="6018b-123">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="6018b-123">GetStreamingEventsResponse</span></span>](getstreamingeventsresponse.md)
    
- [<span data-ttu-id="6018b-124">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6018b-124">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="6018b-125">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6018b-125">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md)
    
- [<span data-ttu-id="6018b-126">注釈 Folderpermissionlevel</span><span class="sxs-lookup"><span data-stu-id="6018b-126">NotesFolderPermissionLevel</span></span>](notesfolderpermissionlevel.md)
    
- [<span data-ttu-id="6018b-127">通知</span><span class="sxs-lookup"><span data-stu-id="6018b-127">Notification</span></span>](notification-ex15websvcsotherref.md)
    
- [<span data-ttu-id="6018b-128">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="6018b-128">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md)
    
<span data-ttu-id="6018b-129">**Getstreamingevents**操作の応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6018b-129">To find other options for the response message of the **GetStreamingEvents** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="6018b-130">[通知](notification-ex15websvcsotherref.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="6018b-130">Start at the [Notification](notification-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="getstreamingevents-error-response-example"></a><span data-ttu-id="6018b-131">GetStreamingEvents エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="6018b-131">GetStreamingEvents error response example</span></span>

### <a name="description"></a><span data-ttu-id="6018b-132">Description</span><span class="sxs-lookup"><span data-stu-id="6018b-132">Description</span></span>

<span data-ttu-id="6018b-133">次の例は、 **Getstreamingevents**要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="6018b-133">The following example shows an error response to a **GetStreamingEvents** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="6018b-134">コード</span><span class="sxs-lookup"><span data-stu-id="6018b-134">Code</span></span>

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

## <a name="remarks"></a><span data-ttu-id="6018b-135">注釈</span><span class="sxs-lookup"><span data-stu-id="6018b-135">Remarks</span></span>

<span data-ttu-id="6018b-136">**Getstreamingevents**要求を処理する場合、クライアントアクセスサーバーは次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="6018b-136">When processing a **GetStreamingEvents** request, the Client Access server performs the following steps:</span></span> 
  
1. <span data-ttu-id="6018b-137">要求の[SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md)は、クライアントアクセスサーバーでホストされている有効なサブスクリプションであることが確認されます。</span><span class="sxs-lookup"><span data-stu-id="6018b-137">The [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md) of the request is confirmed to be a valid subscription that is hosted on the Client Access server.</span></span> <span data-ttu-id="6018b-138">そうでない場合、 **Getstreamingevents**呼び出しは失敗します。</span><span class="sxs-lookup"><span data-stu-id="6018b-138">If it is not, the **GetStreamingEvents** call fails.</span></span> 
    
2. <span data-ttu-id="6018b-139">要求の認証済みユーザーの SMTP アドレスは、偽装権限を持っていることが検証されます。</span><span class="sxs-lookup"><span data-stu-id="6018b-139">The SMTP address of the authenticated user for the request is validated to have impersonation rights.</span></span> <span data-ttu-id="6018b-140">そうでない場合、 **Getstreamingevents**要求は失敗します。</span><span class="sxs-lookup"><span data-stu-id="6018b-140">If they do not, the **GetStreamingEvents** request fails.</span></span> 
    
3. <span data-ttu-id="6018b-141">サブスクリプションキューは、クライアントへの送信を待機しているイベントに対して照会されます。</span><span class="sxs-lookup"><span data-stu-id="6018b-141">The subscription queue is queried for events that are waiting to be sent to the client.</span></span> <span data-ttu-id="6018b-142">キューが空でない場合、キューから最初の50イベントがプルされ、通知にエンコードされます。</span><span class="sxs-lookup"><span data-stu-id="6018b-142">If the queue is not empty, the first 50 events from the queue are pulled from the queue and encoded into a notification.</span></span>
    
4. <span data-ttu-id="6018b-143">キューにイベントが見つからない場合は、 [Statusevent](statusevent.md)が生成され、通知応答にエンコードされます。</span><span class="sxs-lookup"><span data-stu-id="6018b-143">If no events are found in the queue, a [StatusEvent](statusevent.md) is generated and encoded into a notification response.</span></span> 
    
5. <span data-ttu-id="6018b-144">通知応答がクライアントに返されます。</span><span class="sxs-lookup"><span data-stu-id="6018b-144">The notification response is returned to the client.</span></span>
    
6. <span data-ttu-id="6018b-145">通知に含まれるイベントは、サブスクリプションキューから削除され、サブスクリプションのクライアントアクセスサーバーの最後のウォーターマークは、返される最後のイベントのウォーターマークに設定されます。</span><span class="sxs-lookup"><span data-stu-id="6018b-145">The events that are included in the notification are removed from the subscription queue and the Client Access server-local last watermark for the subscription is set to the watermark of the last event that is returned.</span></span>
    
7. <span data-ttu-id="6018b-146">サブスクリプションのタイムアウトタイマーはリセットされます。</span><span class="sxs-lookup"><span data-stu-id="6018b-146">The timeout timer for the subscription is reset.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="6018b-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="6018b-147">See also</span></span>



[<span data-ttu-id="6018b-148">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="6018b-148">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="6018b-149">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="6018b-149">Unsubscribe operation</span></span>](unsubscribe-operation.md)


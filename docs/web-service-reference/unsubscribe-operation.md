---
title: Unsubscribe 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Unsubscribe
api_type:
- schema
ms.assetid: 994a9d2b-1501-4804-90f0-12bd914496ec
description: 登録解除操作を使用して、プル通知サブスクリプションを終了します。 サブスクリプションのタイムアウトを使用するのではなく、この操作を使用します。 この操作は、プル通知に対してのみ有効です。
ms.openlocfilehash: 054f89af1ba5c780c7de5016a6dfe34086c97f02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468027"
---
# <a name="unsubscribe-operation"></a><span data-ttu-id="7db27-105">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="7db27-105">Unsubscribe operation</span></span>

<span data-ttu-id="7db27-106">登録解除操作を使用して、プル通知サブスクリプションを終了します。</span><span class="sxs-lookup"><span data-stu-id="7db27-106">The Unsubscribe operation is used to end a pull notification subscription.</span></span> <span data-ttu-id="7db27-107">サブスクリプションのタイムアウトを使用するのではなく、この操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="7db27-107">Use this operation rather than letting a subscription timeout.</span></span> <span data-ttu-id="7db27-108">この操作は、プル通知に対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="7db27-108">This operation is only valid for pull notifications.</span></span>
  
## <a name="unsubscribe-request-example"></a><span data-ttu-id="7db27-109">登録解除要求の例</span><span class="sxs-lookup"><span data-stu-id="7db27-109">Unsubscribe request example</span></span>

### <a name="description"></a><span data-ttu-id="7db27-110">説明</span><span class="sxs-lookup"><span data-stu-id="7db27-110">Description</span></span>

<span data-ttu-id="7db27-111">次の例は、通知サービスからクライアントの登録を解除するために送信される SOAP XML メッセージを示しています。</span><span class="sxs-lookup"><span data-stu-id="7db27-111">The following example shows the SOAP XML message that is sent to unsubscribe a client from the Notification service.</span></span>
  
### <a name="code"></a><span data-ttu-id="7db27-112">コード</span><span class="sxs-lookup"><span data-stu-id="7db27-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Unsubscribe xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>e6fbf5c1-7e26-4bc6-a5f2-882063d5e34e</SubscriptionId>  
    </Unsubscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-request-elements"></a><span data-ttu-id="7db27-113">登録解除の要求要素</span><span class="sxs-lookup"><span data-stu-id="7db27-113">Unsubscribe request elements</span></span>

<span data-ttu-id="7db27-114">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="7db27-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="7db27-115">登録を解除する</span><span class="sxs-lookup"><span data-stu-id="7db27-115">Unsubscribe</span></span>](unsubscribe.md)
    
- [<span data-ttu-id="7db27-116">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="7db27-116">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
## <a name="successful-unsubscribe-response-example"></a><span data-ttu-id="7db27-117">正常な登録解除の応答の例</span><span class="sxs-lookup"><span data-stu-id="7db27-117">Successful Unsubscribe response example</span></span>

### <a name="description"></a><span data-ttu-id="7db27-118">説明</span><span class="sxs-lookup"><span data-stu-id="7db27-118">Description</span></span>

<span data-ttu-id="7db27-119">次の例は、購読中止要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="7db27-119">The following example shows a successful response to an Unsubscribe request.</span></span>
  
### <a name="code"></a><span data-ttu-id="7db27-120">コード</span><span class="sxs-lookup"><span data-stu-id="7db27-120">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-response-elements"></a><span data-ttu-id="7db27-121">応答の取り消し要素</span><span class="sxs-lookup"><span data-stu-id="7db27-121">Unsubscribe response elements</span></span>

<span data-ttu-id="7db27-122">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="7db27-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="7db27-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7db27-123">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7db27-124">登録を解除する</span><span class="sxs-lookup"><span data-stu-id="7db27-124">Unsubscribe</span></span>](unsubscribe.md)
    
- [<span data-ttu-id="7db27-125">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7db27-125">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7db27-126">非表示の表示/非表示のメッセージ</span><span class="sxs-lookup"><span data-stu-id="7db27-126">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
    
- [<span data-ttu-id="7db27-127">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7db27-127">ResponseCode</span></span>](responsecode.md)
    
## <a name="unsubscribe-error-response-example"></a><span data-ttu-id="7db27-128">登録解除エラーの応答の例</span><span class="sxs-lookup"><span data-stu-id="7db27-128">Unsubscribe Error response example</span></span>

### <a name="description"></a><span data-ttu-id="7db27-129">説明</span><span class="sxs-lookup"><span data-stu-id="7db27-129">Description</span></span>

<span data-ttu-id="7db27-130">次のサブスクライブ解除エラー応答の例は、Exchange ストアに配置できないサブスクリプション識別子を使用してサブスクライブを中止しようとした場合に発生します。</span><span class="sxs-lookup"><span data-stu-id="7db27-130">The following example of an Unsubscribe error response occurs in response to an attempt to unsubscribe by using a subscription identifier that cannot be located in the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="7db27-131">コード</span><span class="sxs-lookup"><span data-stu-id="7db27-131">Code</span></span>

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
    <UnsubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Error">
          <m:MessageText>The specified subscription was not found.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-error-response-elements"></a><span data-ttu-id="7db27-132">登録解除エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="7db27-132">Unsubscribe Error response elements</span></span>

<span data-ttu-id="7db27-133">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="7db27-133">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="7db27-134">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7db27-134">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7db27-135">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="7db27-135">UnsubscribeResponse</span></span>](unsubscriberesponse.md)
    
- [<span data-ttu-id="7db27-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7db27-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7db27-137">非表示の表示/非表示のメッセージ</span><span class="sxs-lookup"><span data-stu-id="7db27-137">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
    
- [<span data-ttu-id="7db27-138">MessageText</span><span class="sxs-lookup"><span data-stu-id="7db27-138">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="7db27-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7db27-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7db27-140">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7db27-140">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="7db27-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="7db27-141">See also</span></span>

- [<span data-ttu-id="7db27-142">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="7db27-142">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="7db27-143">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="7db27-143">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="7db27-144">プルサブスクリプションの使用</span><span class="sxs-lookup"><span data-stu-id="7db27-144">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)


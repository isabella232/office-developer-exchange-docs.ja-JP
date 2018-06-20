---
title: 操作の購読を解除します。
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
description: 購読の取り消し操作を使用して、プル サブスクリプションの通知を終了します。 サブスクリプションのタイムアウトを通知するのではなく、この操作を使用します。 この操作の通知をプルのみです。
ms.openlocfilehash: 64514a718d473f0fd7d0320bd1ccecddb1940ac8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839821"
---
# <a name="unsubscribe-operation"></a><span data-ttu-id="e9c31-105">操作の購読を解除します。</span><span class="sxs-lookup"><span data-stu-id="e9c31-105">Unsubscribe operation</span></span>

<span data-ttu-id="e9c31-106">購読の取り消し操作を使用して、プル サブスクリプションの通知を終了します。</span><span class="sxs-lookup"><span data-stu-id="e9c31-106">The Unsubscribe operation is used to end a pull notification subscription.</span></span> <span data-ttu-id="e9c31-107">サブスクリプションのタイムアウトを通知するのではなく、この操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="e9c31-107">Use this operation rather than letting a subscription timeout.</span></span> <span data-ttu-id="e9c31-108">この操作の通知をプルのみです。</span><span class="sxs-lookup"><span data-stu-id="e9c31-108">This operation is only valid for pull notifications.</span></span>
  
## <a name="unsubscribe-request-example"></a><span data-ttu-id="e9c31-109">購読の取り消しの要求の例</span><span class="sxs-lookup"><span data-stu-id="e9c31-109">Unsubscribe request example</span></span>

### <a name="description"></a><span data-ttu-id="e9c31-110">説明</span><span class="sxs-lookup"><span data-stu-id="e9c31-110">Description</span></span>

<span data-ttu-id="e9c31-111">購読を解除するクライアントの通知サービスに送信される SOAP XML メッセージの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e9c31-111">The following example shows the SOAP XML message that is sent to unsubscribe a client from the Notification service.</span></span>
  
### <a name="code"></a><span data-ttu-id="e9c31-112">コード</span><span class="sxs-lookup"><span data-stu-id="e9c31-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Unsubscribe xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>e6fbf5c1-7e26-4bc6-a5f2-882063d5e34e</SubscriptionId>  
    </Unsubscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-request-elements"></a><span data-ttu-id="e9c31-113">要求要素の購読を解除します。</span><span class="sxs-lookup"><span data-stu-id="e9c31-113">Unsubscribe request elements</span></span>

<span data-ttu-id="e9c31-114">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="e9c31-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="e9c31-115">購読の取り消し</span><span class="sxs-lookup"><span data-stu-id="e9c31-115">Unsubscribe</span></span>](unsubscribe.md)
    
- [<span data-ttu-id="e9c31-116">サブスクリプション Id (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="e9c31-116">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
## <a name="successful-unsubscribe-response-example"></a><span data-ttu-id="e9c31-117">成功した購読取り消しの応答の例</span><span class="sxs-lookup"><span data-stu-id="e9c31-117">Successful Unsubscribe response example</span></span>

### <a name="description"></a><span data-ttu-id="e9c31-118">説明</span><span class="sxs-lookup"><span data-stu-id="e9c31-118">Description</span></span>

<span data-ttu-id="e9c31-119">購読の取り消しの要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e9c31-119">The following example shows a successful response to an Unsubscribe request.</span></span>
  
### <a name="code"></a><span data-ttu-id="e9c31-120">コード</span><span class="sxs-lookup"><span data-stu-id="e9c31-120">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-response-elements"></a><span data-ttu-id="e9c31-121">応答要素の購読を解除します。</span><span class="sxs-lookup"><span data-stu-id="e9c31-121">Unsubscribe response elements</span></span>

<span data-ttu-id="e9c31-122">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="e9c31-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="e9c31-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e9c31-123">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="e9c31-124">購読の取り消し</span><span class="sxs-lookup"><span data-stu-id="e9c31-124">Unsubscribe</span></span>](unsubscribe.md)
    
- [<span data-ttu-id="e9c31-125">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e9c31-125">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e9c31-126">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e9c31-126">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
    
- [<span data-ttu-id="e9c31-127">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e9c31-127">ResponseCode</span></span>](responsecode.md)
    
## <a name="unsubscribe-error-response-example"></a><span data-ttu-id="e9c31-128">エラー応答の例の購読を解除します。</span><span class="sxs-lookup"><span data-stu-id="e9c31-128">Unsubscribe Error response example</span></span>

### <a name="description"></a><span data-ttu-id="e9c31-129">説明</span><span class="sxs-lookup"><span data-stu-id="e9c31-129">Description</span></span>

<span data-ttu-id="e9c31-130">見つからない場合、サブスクリプションの識別子を使用して、購読を解除しようとするへの応答としての登録解除エラー応答は、次の例が発生した Exchange ストアにします。</span><span class="sxs-lookup"><span data-stu-id="e9c31-130">The following example of an Unsubscribe error response occurs in response to an attempt to unsubscribe by using a subscription identifier that cannot be located in the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="e9c31-131">コード</span><span class="sxs-lookup"><span data-stu-id="e9c31-131">Code</span></span>

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
    <UnsubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="unsubscribe-error-response-elements"></a><span data-ttu-id="e9c31-132">エラー応答の要素の購読を解除します。</span><span class="sxs-lookup"><span data-stu-id="e9c31-132">Unsubscribe Error response elements</span></span>

<span data-ttu-id="e9c31-133">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="e9c31-133">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="e9c31-134">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e9c31-134">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="e9c31-135">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="e9c31-135">UnsubscribeResponse</span></span>](unsubscriberesponse.md)
    
- [<span data-ttu-id="e9c31-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e9c31-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e9c31-137">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e9c31-137">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
    
- [<span data-ttu-id="e9c31-138">MessageText</span><span class="sxs-lookup"><span data-stu-id="e9c31-138">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="e9c31-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e9c31-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e9c31-140">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e9c31-140">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="e9c31-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="e9c31-141">See also</span></span>

- [<span data-ttu-id="e9c31-142">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="e9c31-142">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="e9c31-143">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="e9c31-143">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="e9c31-144">プル サブスクリプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="e9c31-144">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)


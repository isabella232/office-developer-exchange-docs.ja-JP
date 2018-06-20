---
title: GetCallInfo 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfo
api_type:
- schema
ms.assetid: 6bccd418-caf7-4eb9-8a6f-410e56a635c3
description: GetCallInfo 操作では、CallId (UM web サービス) で指定されている送信呼び出しのステータスを返します。
ms.openlocfilehash: 36f9cba3690520ebb457a4cb2bfbcde3fea4b8dc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760649"
---
# <a name="getcallinfo-operation-um-web-service"></a><span data-ttu-id="83d22-103">GetCallInfo 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="83d22-103">GetCallInfo operation (UM web service)</span></span>

<span data-ttu-id="83d22-104">GetCallInfo 操作では、 [CallId (UM web サービス)](callid-um-web-service.md)で指定されている送信呼び出しのステータスを返します。</span><span class="sxs-lookup"><span data-stu-id="83d22-104">The GetCallInfo operation returns the status of the outbound call that is specified by [CallId (UM web service)](callid-um-web-service.md).</span></span>
  
## <a name="getcallinfo-request-example"></a><span data-ttu-id="83d22-105">GetCallInfo 要求の例</span><span class="sxs-lookup"><span data-stu-id="83d22-105">GetCallInfo request example</span></span>

### <a name="description"></a><span data-ttu-id="83d22-106">説明</span><span class="sxs-lookup"><span data-stu-id="83d22-106">Description</span></span>

<span data-ttu-id="83d22-107">GetCallInfo 要求の次の例では、指定した発信呼び出しについての情報を取得する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="83d22-107">The following example of a GetCallInfo request shows how to form a request to get information about a specified outbound call.</span></span>
  
### <a name="code"></a><span data-ttu-id="83d22-108">コード</span><span class="sxs-lookup"><span data-stu-id="83d22-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetCallInfo xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </GetCallInfo>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getcallinfo-response-example"></a><span data-ttu-id="83d22-109">成功した GetCallInfo の応答の例</span><span class="sxs-lookup"><span data-stu-id="83d22-109">Successful GetCallInfo response example</span></span>

### <a name="description"></a><span data-ttu-id="83d22-110">説明</span><span class="sxs-lookup"><span data-stu-id="83d22-110">Description</span></span>

<span data-ttu-id="83d22-111">GetCallInfo 要求への応答を GetCallInfo の応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="83d22-111">The following example of a GetCallInfo response shows a response to a GetCallInfo request.</span></span>
  
### <a name="code"></a><span data-ttu-id="83d22-112">コード</span><span class="sxs-lookup"><span data-stu-id="83d22-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetCallInfoResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetCallInfoResponse>
        <CallState>Connected</CallState> 
        <EventCause>None</EventCause> 
      </GetCallInfoResponse>
    </GetCallInfoResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="83d22-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="83d22-113">See also</span></span>



[<span data-ttu-id="83d22-114">GetCallInfo (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="83d22-114">GetCallInfo (UM web service)</span></span>](getcallinfo-um-web-service.md)
  
[<span data-ttu-id="83d22-115">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="83d22-115">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="83d22-116">CallId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="83d22-116">CallId (UM web service)</span></span>](callid-um-web-service.md)
  
[<span data-ttu-id="83d22-117">CallState (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="83d22-117">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
[<span data-ttu-id="83d22-118">EventCause (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="83d22-118">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)


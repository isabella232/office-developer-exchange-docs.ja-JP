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
description: GetCallInfo 操作は、CallId (UM web サービス) によって指定された発信呼び出しの状態を返します。
ms.openlocfilehash: 6b5664dfe16f9c74cc7175098145141b815a6355
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461241"
---
# <a name="getcallinfo-operation-um-web-service"></a><span data-ttu-id="81988-103">GetCallInfo 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="81988-103">GetCallInfo operation (UM web service)</span></span>

<span data-ttu-id="81988-104">GetCallInfo 操作は、 [Callid (UM web サービス)](callid-um-web-service.md)によって指定された発信呼び出しの状態を返します。</span><span class="sxs-lookup"><span data-stu-id="81988-104">The GetCallInfo operation returns the status of the outbound call that is specified by [CallId (UM web service)](callid-um-web-service.md).</span></span>
  
## <a name="getcallinfo-request-example"></a><span data-ttu-id="81988-105">GetCallInfo 要求の例</span><span class="sxs-lookup"><span data-stu-id="81988-105">GetCallInfo request example</span></span>

### <a name="description"></a><span data-ttu-id="81988-106">Description</span><span class="sxs-lookup"><span data-stu-id="81988-106">Description</span></span>

<span data-ttu-id="81988-107">次の GetCallInfo 要求の例は、指定された発信呼び出しに関する情報を取得するための要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="81988-107">The following example of a GetCallInfo request shows how to form a request to get information about a specified outbound call.</span></span>
  
### <a name="code"></a><span data-ttu-id="81988-108">コード</span><span class="sxs-lookup"><span data-stu-id="81988-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetCallInfo xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </GetCallInfo>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getcallinfo-response-example"></a><span data-ttu-id="81988-109">Successful GetCallInfo response の例</span><span class="sxs-lookup"><span data-stu-id="81988-109">Successful GetCallInfo response example</span></span>

### <a name="description"></a><span data-ttu-id="81988-110">Description</span><span class="sxs-lookup"><span data-stu-id="81988-110">Description</span></span>

<span data-ttu-id="81988-111">GetCallInfo 応答の次の例は、GetCallInfo 要求に対する応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="81988-111">The following example of a GetCallInfo response shows a response to a GetCallInfo request.</span></span>
  
### <a name="code"></a><span data-ttu-id="81988-112">コード</span><span class="sxs-lookup"><span data-stu-id="81988-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetCallInfoResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GetCallInfoResponse>
        <CallState>Connected</CallState> 
        <EventCause>None</EventCause> 
      </GetCallInfoResponse>
    </GetCallInfoResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="81988-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="81988-113">See also</span></span>



[<span data-ttu-id="81988-114">GetCallInfo (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="81988-114">GetCallInfo (UM web service)</span></span>](getcallinfo-um-web-service.md)
  
[<span data-ttu-id="81988-115">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="81988-115">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="81988-116">CallId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="81988-116">CallId (UM web service)</span></span>](callid-um-web-service.md)
  
[<span data-ttu-id="81988-117">CallState (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="81988-117">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
[<span data-ttu-id="81988-118">EventCause (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="81988-118">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)


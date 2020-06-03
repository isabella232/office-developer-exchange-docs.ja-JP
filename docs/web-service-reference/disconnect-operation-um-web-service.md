---
title: Disconnect 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Disconnect
api_type:
- schema
ms.assetid: a987000b-d6e6-49d7-944c-e9c278d0236f
description: 切断操作は、指定した CallId (UM web サービス) によって識別される呼び出しを終了します。
ms.openlocfilehash: a1268f9ea3d879f472e019bf1847fc13d65d1819
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529071"
---
# <a name="disconnect-operation-um-web-service"></a><span data-ttu-id="651dc-103">Disconnect 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="651dc-103">Disconnect operation (UM web service)</span></span>

<span data-ttu-id="651dc-104">切断操作は、指定した[Callid (UM web サービス)](callid-um-web-service.md)によって識別される呼び出しを終了します。</span><span class="sxs-lookup"><span data-stu-id="651dc-104">The Disconnect operation terminates the call that is identified by the specified [CallId (UM web service)](callid-um-web-service.md).</span></span>
  
## <a name="disconnect-request-example"></a><span data-ttu-id="651dc-105">切断要求の例</span><span class="sxs-lookup"><span data-stu-id="651dc-105">Disconnect request example</span></span>

### <a name="description"></a><span data-ttu-id="651dc-106">Description</span><span class="sxs-lookup"><span data-stu-id="651dc-106">Description</span></span>

<span data-ttu-id="651dc-107">次の切断要求の例は、呼び出しを切断する要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="651dc-107">The following example of a Disconnect request shows how to form a request to disconnect a call.</span></span>
  
### <a name="code"></a><span data-ttu-id="651dc-108">コード</span><span class="sxs-lookup"><span data-stu-id="651dc-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <Disconnect xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </Disconnect>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-disconnect-response-example"></a><span data-ttu-id="651dc-109">成功した切断応答の例</span><span class="sxs-lookup"><span data-stu-id="651dc-109">Successful Disconnect response example</span></span>

### <a name="description"></a><span data-ttu-id="651dc-110">Description</span><span class="sxs-lookup"><span data-stu-id="651dc-110">Description</span></span>

<span data-ttu-id="651dc-111">次の切断応答の例は、切断要求に対する応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="651dc-111">The following example of a Disconnect response shows a response to the Disconnect request.</span></span>
  
### <a name="code"></a><span data-ttu-id="651dc-112">コード</span><span class="sxs-lookup"><span data-stu-id="651dc-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <DisconnectResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="651dc-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="651dc-113">See also</span></span>

- [<span data-ttu-id="651dc-114">Disconnect (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="651dc-114">Disconnect (UM web service)</span></span>](disconnect-um-web-service.md) 
- <span data-ttu-id="651dc-115">[[切断] 応答 (UM web サービス)](disconnectresponse-um-web-service.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-115">[DisconnectResponse (UM web service)](disconnectresponse-um-web-service.md)</span></span> 
- [<span data-ttu-id="651dc-116">CallId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="651dc-116">CallId (UM web service)</span></span>](callid-um-web-service.md)


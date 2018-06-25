---
title: 操作 (UM web サービス) に接続を切断します。
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
description: 切断操作は、指定した CallId (UM web サービス) によって識別されるコールを終了します。
ms.openlocfilehash: 1e04e65fa1951a6aa46e2c8b6dd5fe524c84a8fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760076"
---
# <a name="disconnect-operation-um-web-service"></a><span data-ttu-id="b973d-103">操作 (UM web サービス) に接続を切断します。</span><span class="sxs-lookup"><span data-stu-id="b973d-103">Disconnect operation (UM web service)</span></span>

<span data-ttu-id="b973d-104">切断操作は、指定した[CallId (UM web サービス)](callid-um-web-service.md)によって識別されるコールを終了します。</span><span class="sxs-lookup"><span data-stu-id="b973d-104">The Disconnect operation terminates the call that is identified by the specified [CallId (UM web service)](callid-um-web-service.md).</span></span>
  
## <a name="disconnect-request-example"></a><span data-ttu-id="b973d-105">切断要求の例</span><span class="sxs-lookup"><span data-stu-id="b973d-105">Disconnect request example</span></span>

### <a name="description"></a><span data-ttu-id="b973d-106">説明</span><span class="sxs-lookup"><span data-stu-id="b973d-106">Description</span></span>

<span data-ttu-id="b973d-107">切断要求の次の例では、呼び出しの切断要求を形成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="b973d-107">The following example of a Disconnect request shows how to form a request to disconnect a call.</span></span>
  
### <a name="code"></a><span data-ttu-id="b973d-108">コード</span><span class="sxs-lookup"><span data-stu-id="b973d-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <Disconnect xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </Disconnect>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-disconnect-response-example"></a><span data-ttu-id="b973d-109">切断応答の成功の例</span><span class="sxs-lookup"><span data-stu-id="b973d-109">Successful Disconnect response example</span></span>

### <a name="description"></a><span data-ttu-id="b973d-110">説明</span><span class="sxs-lookup"><span data-stu-id="b973d-110">Description</span></span>

<span data-ttu-id="b973d-111">切断応答の次の例では、切断要求への応答を示します。</span><span class="sxs-lookup"><span data-stu-id="b973d-111">The following example of a Disconnect response shows a response to the Disconnect request.</span></span>
  
### <a name="code"></a><span data-ttu-id="b973d-112">コード</span><span class="sxs-lookup"><span data-stu-id="b973d-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <DisconnectResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="b973d-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="b973d-113">See also</span></span>

- [<span data-ttu-id="b973d-114">(UM web サービス) に接続を切断します。</span><span class="sxs-lookup"><span data-stu-id="b973d-114">Disconnect (UM web service)</span></span>](disconnect-um-web-service.md) 
- [<span data-ttu-id="b973d-115">DisconnectResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="b973d-115">DisconnectResponse (UM web service)</span></span>](disconnectresponse-um-web-service.md) 
- [<span data-ttu-id="b973d-116">CallId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="b973d-116">CallId (UM web service)</span></span>](callid-um-web-service.md)


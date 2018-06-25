---
title: SetOofStatus 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetOofStatus
api_type:
- schema
ms.assetid: 97c271e9-506e-43eb-89cd-46803fc47ee5
description: SetOofStatus 操作は、要求したユーザーの Office (OOF) の案内応答を再生するかどうかを示す値を設定します。
ms.openlocfilehash: 2bb1deeec8ddb5be56979bfb2fae3396672298a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833445"
---
# <a name="setoofstatus-operation-um-web-service"></a><span data-ttu-id="d6a55-103">SetOofStatus 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="d6a55-103">SetOofStatus operation (UM web service)</span></span>

<span data-ttu-id="d6a55-104">SetOofStatus 操作は、要求したユーザーの Office (OOF) の案内応答を再生するかどうかを示す値を設定します。</span><span class="sxs-lookup"><span data-stu-id="d6a55-104">The SetOofStatus operation sets a value that indicates whether the Out of Office (OOF) greeting should be played for the user who makes the request.</span></span>
  
## <a name="setoofstatus-request-example"></a><span data-ttu-id="d6a55-105">SetOofStatus 要求の例</span><span class="sxs-lookup"><span data-stu-id="d6a55-105">SetOofStatus request example</span></span>

### <a name="description"></a><span data-ttu-id="d6a55-106">説明</span><span class="sxs-lookup"><span data-stu-id="d6a55-106">Description</span></span>

<span data-ttu-id="d6a55-107">SetOofStatus 要求の次の例では、メールボックスの不在時の Office の案内応答を有効にする要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="d6a55-107">The following example of a SetOofStatus request shows how to form a request to enable the Out of Office greeting for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="d6a55-108">コード</span><span class="sxs-lookup"><span data-stu-id="d6a55-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetOofStatus xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetOofStatus>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setoofstatus-response-example"></a><span data-ttu-id="d6a55-109">成功した SetOofStatus の応答の例</span><span class="sxs-lookup"><span data-stu-id="d6a55-109">Successful SetOofStatus response example</span></span>

### <a name="description"></a><span data-ttu-id="d6a55-110">説明</span><span class="sxs-lookup"><span data-stu-id="d6a55-110">Description</span></span>

<span data-ttu-id="d6a55-111">SetOofStatus 要求への応答を SetOofStatus の応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d6a55-111">The following example of a SetOofStatus response shows a response to the SetOofStatus request.</span></span>
  
### <a name="code"></a><span data-ttu-id="d6a55-112">コード</span><span class="sxs-lookup"><span data-stu-id="d6a55-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetOofStatusResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="d6a55-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="d6a55-113">See also</span></span>



[<span data-ttu-id="d6a55-114">SetOofStatus (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="d6a55-114">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
[<span data-ttu-id="d6a55-115">SetOofStatusResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="d6a55-115">SetOofStatusResponse (UM web service)</span></span>](setoofstatusresponse-um-web-service.md)
  
[<span data-ttu-id="d6a55-116">状態 (UM web サービス - SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="d6a55-116">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)


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
description: SetOofStatus 操作は、要求を行うユーザーに対して不在時 (OOF) の案内応答を再生するかどうかを示す値を設定します。
ms.openlocfilehash: 2311b6137ac25d15ad3d06668450c1d0f7ec1fad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467355"
---
# <a name="setoofstatus-operation-um-web-service"></a><span data-ttu-id="bd3f7-103">SetOofStatus 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="bd3f7-103">SetOofStatus operation (UM web service)</span></span>

<span data-ttu-id="bd3f7-104">SetOofStatus 操作は、要求を行うユーザーに対して不在時 (OOF) の案内応答を再生するかどうかを示す値を設定します。</span><span class="sxs-lookup"><span data-stu-id="bd3f7-104">The SetOofStatus operation sets a value that indicates whether the Out of Office (OOF) greeting should be played for the user who makes the request.</span></span>
  
## <a name="setoofstatus-request-example"></a><span data-ttu-id="bd3f7-105">SetOofStatus 要求の例</span><span class="sxs-lookup"><span data-stu-id="bd3f7-105">SetOofStatus request example</span></span>

### <a name="description"></a><span data-ttu-id="bd3f7-106">説明</span><span class="sxs-lookup"><span data-stu-id="bd3f7-106">Description</span></span>

<span data-ttu-id="bd3f7-107">次の SetOofStatus 要求の例は、メールボックスの不在時の応答メッセージを有効にする要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="bd3f7-107">The following example of a SetOofStatus request shows how to form a request to enable the Out of Office greeting for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="bd3f7-108">コード</span><span class="sxs-lookup"><span data-stu-id="bd3f7-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetOofStatus xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetOofStatus>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setoofstatus-response-example"></a><span data-ttu-id="bd3f7-109">成功した SetOofStatus response の例</span><span class="sxs-lookup"><span data-stu-id="bd3f7-109">Successful SetOofStatus response example</span></span>

### <a name="description"></a><span data-ttu-id="bd3f7-110">説明</span><span class="sxs-lookup"><span data-stu-id="bd3f7-110">Description</span></span>

<span data-ttu-id="bd3f7-111">次の SetOofStatus 応答の例は、SetOofStatus 要求に対する応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="bd3f7-111">The following example of a SetOofStatus response shows a response to the SetOofStatus request.</span></span>
  
### <a name="code"></a><span data-ttu-id="bd3f7-112">コード</span><span class="sxs-lookup"><span data-stu-id="bd3f7-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetOofStatusResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="bd3f7-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="bd3f7-113">See also</span></span>



[<span data-ttu-id="bd3f7-114">SetOofStatus (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="bd3f7-114">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
[<span data-ttu-id="bd3f7-115">SetOofStatusResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="bd3f7-115">SetOofStatusResponse (UM web service)</span></span>](setoofstatusresponse-um-web-service.md)
  
[<span data-ttu-id="bd3f7-116">状態 (UM web サービス-SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="bd3f7-116">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)


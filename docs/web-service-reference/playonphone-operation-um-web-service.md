---
title: PlayOnPhone 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 7d55be55-f8b6-4e96-a61e-26fa190217fd
description: PlayOnPhone 操作では、発信呼び出しし、DialString 要素で指定されている電話で指定されたメッセージを再生します。
ms.openlocfilehash: b55bb45d6654f57503879f33e1cd5013ddb69a2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832818"
---
# <a name="playonphone-operation-um-web-service"></a><span data-ttu-id="c9d37-103">PlayOnPhone 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="c9d37-103">PlayOnPhone operation (UM web service)</span></span>

<span data-ttu-id="c9d37-104">PlayOnPhone 操作では、発信呼び出しし、 **DialString**要素で指定されている電話で指定されたメッセージを再生します。</span><span class="sxs-lookup"><span data-stu-id="c9d37-104">The PlayOnPhone operation makes an outbound call and plays a specified message over the telephone that is specified by the **DialString** element.</span></span> 
  
## <a name="playonphone-request-example"></a><span data-ttu-id="c9d37-105">PlayOnPhone 要求の例</span><span class="sxs-lookup"><span data-stu-id="c9d37-105">PlayOnPhone request example</span></span>

### <a name="description"></a><span data-ttu-id="c9d37-106">説明</span><span class="sxs-lookup"><span data-stu-id="c9d37-106">Description</span></span>

<span data-ttu-id="c9d37-107">PlayOnPhone 要求の次の例では、発信呼び出しを行い、メッセージを再生する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="c9d37-107">The following example of a PlayOnPhone request shows how to form a request to make an outbound call and play a message.</span></span>
  
### <a name="code"></a><span data-ttu-id="c9d37-108">コード</span><span class="sxs-lookup"><span data-stu-id="c9d37-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhone xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <entryId>AAAAAGsd2rbQLVtLobUGbrq/9IUHAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAACxVpEl+KVVLl957wp//x6UAGAetcDUAAA==</entryId>
      <DialString>12345</DialString>
    </PlayOnPhone>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphone-response-example"></a><span data-ttu-id="c9d37-109">成功した PlayOnPhone の応答の例</span><span class="sxs-lookup"><span data-stu-id="c9d37-109">Successful PlayOnPhone response example</span></span>

### <a name="description"></a><span data-ttu-id="c9d37-110">説明</span><span class="sxs-lookup"><span data-stu-id="c9d37-110">Description</span></span>

<span data-ttu-id="c9d37-111">PlayOnPhone 要求への応答を PlayOnPhone の応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c9d37-111">The following example of a PlayOnPhone response shows a response to the PlayOnPhone request.</span></span>
  
### <a name="code"></a><span data-ttu-id="c9d37-112">コード</span><span class="sxs-lookup"><span data-stu-id="c9d37-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <PlayOnPhoneResponse>NDEzYjEzNmMtZTE2Zi00NTJlLWI3YzctNDhkMTE3MDE3YjlmQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneResponse> 
    </PlayOnPhoneResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="c9d37-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="c9d37-113">See also</span></span>



[<span data-ttu-id="c9d37-114">PlayOnPhone (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="c9d37-114">PlayOnPhone (UM web service)</span></span>](playonphone-um-web-service.md)
  
[<span data-ttu-id="c9d37-115">PlayOnPhoneResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="c9d37-115">PlayOnPhoneResponse (UM web service)</span></span>](playonphoneresponse-um-web-service.md)
  
[<span data-ttu-id="c9d37-116">PlayOnPhoneGreeting 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="c9d37-116">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)


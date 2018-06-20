---
title: PlayOnPhoneGreeting 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 6deafc40-290b-4bce-9914-b6bcc529f38a
description: PlayOnPhoneGreeting 操作では、発信呼び出しし、2 つの応答メッセージのメッセージのいずれかを電話で再生します。
ms.openlocfilehash: 85ba76c7638911678c1ef1aef88f47fdab2c6a4e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832828"
---
# <a name="playonphonegreeting-operation-um-web-service"></a><span data-ttu-id="78b8f-103">PlayOnPhoneGreeting 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="78b8f-103">PlayOnPhoneGreeting operation (UM web service)</span></span>

<span data-ttu-id="78b8f-104">PlayOnPhoneGreeting 操作では、発信呼び出しし、2 つの応答メッセージのメッセージのいずれかを電話で再生します。</span><span class="sxs-lookup"><span data-stu-id="78b8f-104">The PlayOnPhoneGreeting operation makes an outbound call and plays one of the two greeting messages on the telephone.</span></span>
  
## <a name="playonphonegreeting-request-example"></a><span data-ttu-id="78b8f-105">PlayOnPhoneGreeting 要求の例</span><span class="sxs-lookup"><span data-stu-id="78b8f-105">PlayOnPhoneGreeting request example</span></span>

### <a name="description"></a><span data-ttu-id="78b8f-106">説明</span><span class="sxs-lookup"><span data-stu-id="78b8f-106">Description</span></span>

<span data-ttu-id="78b8f-107">PlayOnPhoneGreeting 要求の次の例では、発信呼び出しを行い、通常のグリーティング メッセージを電話で再生する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="78b8f-107">The following example of a PlayOnPhoneGreeting request shows how to form a request to make an outbound call and play the normal greeting message on a telephone.</span></span>
  
### <a name="code"></a><span data-ttu-id="78b8f-108">コード</span><span class="sxs-lookup"><span data-stu-id="78b8f-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhoneGreeting xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GreetingType>NormalCustom</GreetingType>
      <DialString>12345</DialString>
    </PlayOnPhoneGreeting>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphonegreeting-response-example"></a><span data-ttu-id="78b8f-109">成功した PlayOnPhoneGreeting の応答の例</span><span class="sxs-lookup"><span data-stu-id="78b8f-109">Successful PlayOnPhoneGreeting response example</span></span>

### <a name="description"></a><span data-ttu-id="78b8f-110">説明</span><span class="sxs-lookup"><span data-stu-id="78b8f-110">Description</span></span>

<span data-ttu-id="78b8f-111">PlayOnPhoneGreeting 要求への応答を PlayOnPhoneGreeting の応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="78b8f-111">The following example of a PlayOnPhoneGreeting response shows a response to the PlayOnPhoneGreeting request.</span></span>
  
### <a name="code"></a><span data-ttu-id="78b8f-112">コード</span><span class="sxs-lookup"><span data-stu-id="78b8f-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneGreetingResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <PlayOnPhoneGreetingResponse>MjA4MTQ5MmItMTBmZC00ZGFmLThiMzEtNDllNDJjM2Y3MjIxQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneGreetingResponse> 
    </PlayOnPhoneGreetingResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="78b8f-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="78b8f-113">See also</span></span>



[<span data-ttu-id="78b8f-114">PlayOnPhoneGreeting (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="78b8f-114">PlayOnPhoneGreeting (UM web service)</span></span>](playonphonegreeting-um-web-service.md)
  
[<span data-ttu-id="78b8f-115">PlayOnPhoneGreetingResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="78b8f-115">PlayOnPhoneGreetingResponse (UM web service)</span></span>](playonphonegreetingresponse-um-web-service.md)
  
[<span data-ttu-id="78b8f-116">GreetingType (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="78b8f-116">GreetingType (UM web service)</span></span>](greetingtype-um-web-service.md)
  
[<span data-ttu-id="78b8f-117">dialString (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="78b8f-117">dialString (UM web service)</span></span>](dialstring-um-web-service.md)


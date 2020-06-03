---
title: Playon電話案内応答操作 (UM web サービス)
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
description: Playon電話案内応答操作は、発信通話を行い、電話で2つの案内応答メッセージの1つを再生します。
ms.openlocfilehash: 3af120b9ac8d7a368742fad2850c924228488662
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528896"
---
# <a name="playonphonegreeting-operation-um-web-service"></a><span data-ttu-id="6f85c-103">Playon電話案内応答操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="6f85c-103">PlayOnPhoneGreeting operation (UM web service)</span></span>

<span data-ttu-id="6f85c-104">Playon電話案内応答操作は、発信通話を行い、電話で2つの案内応答メッセージの1つを再生します。</span><span class="sxs-lookup"><span data-stu-id="6f85c-104">The PlayOnPhoneGreeting operation makes an outbound call and plays one of the two greeting messages on the telephone.</span></span>
  
## <a name="playonphonegreeting-request-example"></a><span data-ttu-id="6f85c-105">Playon電話案内応答要求の例</span><span class="sxs-lookup"><span data-stu-id="6f85c-105">PlayOnPhoneGreeting request example</span></span>

### <a name="description"></a><span data-ttu-id="6f85c-106">Description</span><span class="sxs-lookup"><span data-stu-id="6f85c-106">Description</span></span>

<span data-ttu-id="6f85c-107">次に示す Playon電話案内応答要求の例は、発信通話を行い、電話で通常の案内応答メッセージを再生する要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="6f85c-107">The following example of a PlayOnPhoneGreeting request shows how to form a request to make an outbound call and play the normal greeting message on a telephone.</span></span>
  
### <a name="code"></a><span data-ttu-id="6f85c-108">コード</span><span class="sxs-lookup"><span data-stu-id="6f85c-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhoneGreeting xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GreetingType>NormalCustom</GreetingType>
      <DialString>12345</DialString>
    </PlayOnPhoneGreeting>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphonegreeting-response-example"></a><span data-ttu-id="6f85c-109">成功した Playon電話案内応答の例</span><span class="sxs-lookup"><span data-stu-id="6f85c-109">Successful PlayOnPhoneGreeting response example</span></span>

### <a name="description"></a><span data-ttu-id="6f85c-110">Description</span><span class="sxs-lookup"><span data-stu-id="6f85c-110">Description</span></span>

<span data-ttu-id="6f85c-111">次の Playon電話案内応答の例は、Playonphone 案内応答要求に対する応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="6f85c-111">The following example of a PlayOnPhoneGreeting response shows a response to the PlayOnPhoneGreeting request.</span></span>
  
### <a name="code"></a><span data-ttu-id="6f85c-112">コード</span><span class="sxs-lookup"><span data-stu-id="6f85c-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneGreetingResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <PlayOnPhoneGreetingResponse>MjA4MTQ5MmItMTBmZC00ZGFmLThiMzEtNDllNDJjM2Y3MjIxQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneGreetingResponse> 
    </PlayOnPhoneGreetingResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="6f85c-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="6f85c-113">See also</span></span>



[<span data-ttu-id="6f85c-114">Playon電話応答メッセージ (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="6f85c-114">PlayOnPhoneGreeting (UM web service)</span></span>](playonphonegreeting-um-web-service.md)
  
[<span data-ttu-id="6f85c-115">PlayOnPhoneGreetingResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="6f85c-115">PlayOnPhoneGreetingResponse (UM web service)</span></span>](playonphonegreetingresponse-um-web-service.md)
  
[<span data-ttu-id="6f85c-116">GreetingType (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="6f85c-116">GreetingType (UM web service)</span></span>](greetingtype-um-web-service.md)
  
<span data-ttu-id="6f85c-117">[[] (UM web サービス)](dialstring-um-web-service.md)</span><span class="sxs-lookup"><span data-stu-id="6f85c-117">[dialString (UM web service)](dialstring-um-web-service.md)</span></span>


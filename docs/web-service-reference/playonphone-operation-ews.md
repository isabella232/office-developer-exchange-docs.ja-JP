---
title: PlayOnPhone 操作 (EWS)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 70e6ef33-2046-4eb8-9987-e106009be04b
description: PlayOnPhone 操作は、発信通話を開始し、電話でメッセージを再生します。
ms.openlocfilehash: 18af810160e72856599f296c4faa83cf9c73c393
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467957"
---
# <a name="playonphone-operation-ews"></a><span data-ttu-id="525e9-103">PlayOnPhone 操作 (EWS)</span><span class="sxs-lookup"><span data-stu-id="525e9-103">PlayOnPhone operation (EWS)</span></span>

<span data-ttu-id="525e9-104">**Playonphone**操作は、発信通話を開始し、電話でメッセージを再生します。</span><span class="sxs-lookup"><span data-stu-id="525e9-104">The **PlayOnPhone** operation initiates an outbound call and plays a message over the telephone.</span></span> 
  
## <a name="playonphone-request-example"></a><span data-ttu-id="525e9-105">PlayOnPhone 要求の例</span><span class="sxs-lookup"><span data-stu-id="525e9-105">PlayOnPhone request example</span></span>

### <a name="description"></a><span data-ttu-id="525e9-106">説明</span><span class="sxs-lookup"><span data-stu-id="525e9-106">Description</span></span>

<span data-ttu-id="525e9-107">次の**Playonphone**要求の例は、電話でメッセージを再生するための要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="525e9-107">The following example of a **PlayOnPhone** request shows how to form a request to play a message on a phone.</span></span> 
  
### <a name="code"></a><span data-ttu-id="525e9-108">コード</span><span class="sxs-lookup"><span data-stu-id="525e9-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:PlayOnPhone>
      <m:ItemId Id="AkAjzQTbY/i="/>
      <m:DialString>5555551212</m:DialString>
    </m:PlayOnPhone>
  </soap:Body>
</soap:Envelope>
```

## <a name="playonphone-response-example"></a><span data-ttu-id="525e9-109">PlayOnPhone 応答の例</span><span class="sxs-lookup"><span data-stu-id="525e9-109">PlayOnPhone response example</span></span>

### <a name="description"></a><span data-ttu-id="525e9-110">説明</span><span class="sxs-lookup"><span data-stu-id="525e9-110">Description</span></span>

<span data-ttu-id="525e9-111">次の例は、 **Playonphone**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="525e9-111">The following example shows a successful response to the **PlayOnPhone** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="525e9-112">コード</span><span class="sxs-lookup"><span data-stu-id="525e9-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PlayOnPhoneResponse ResponseClass="Success" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <PhoneCallId Id="ZWMtWYtMY29t"/>
    </PlayOnPhoneResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="525e9-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="525e9-113">See also</span></span>

- [<span data-ttu-id="525e9-114">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="525e9-114">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="525e9-115">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="525e9-115">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


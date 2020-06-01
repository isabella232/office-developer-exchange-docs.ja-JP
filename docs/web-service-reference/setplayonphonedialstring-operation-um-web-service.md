---
title: SetPlayOnPhoneDialString 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: a68479f2-d900-4dd8-a5ce-dbea8247e841
description: SetPlayOnPhoneDialString 操作では、PlayOnPhone 操作 (UM web サービス) および Playonphone 案内応答操作 (UM web サービス) の既定として使用するダイヤル文字列を設定します。
ms.openlocfilehash: 7df806eedc2d6d037394f31ec4ccbfe28aaf3372
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458643"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a><span data-ttu-id="5b899-103">SetPlayOnPhoneDialString 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="5b899-103">SetPlayOnPhoneDialString operation (UM web service)</span></span>

<span data-ttu-id="5b899-104">SetPlayOnPhoneDialString 操作では、 [Playonphone 操作 (um web サービス)](playonphone-operation-um-web-service.md)および[Playonphone 案内応答操作 (um web サービス)](playonphonegreeting-operation-um-web-service.md)の既定として使用するダイヤル文字列を設定します。</span><span class="sxs-lookup"><span data-stu-id="5b899-104">The SetPlayOnPhoneDialString operation sets the dial string to use as the default for the [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and the [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md).</span></span>
  
## <a name="setplayonphonedialstring-request-example"></a><span data-ttu-id="5b899-105">SetPlayOnPhoneDialString 要求の例</span><span class="sxs-lookup"><span data-stu-id="5b899-105">SetPlayOnPhoneDialString request example</span></span>

### <a name="description"></a><span data-ttu-id="5b899-106">説明</span><span class="sxs-lookup"><span data-stu-id="5b899-106">Description</span></span>

<span data-ttu-id="5b899-107">次の SetPlayOnPhoneDialString 要求の例は、メールボックスの既定のダイヤル文字列を設定する要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5b899-107">The following example of a SetPlayOnPhoneDialString request shows how to form a request to set the default dial string for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="5b899-108">コード</span><span class="sxs-lookup"><span data-stu-id="5b899-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetPlayOnPhoneDialString xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <dialString>12345</dialString>
    </SetPlayOnPhoneDialString>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setplayonphonedialstring-response-example"></a><span data-ttu-id="5b899-109">Successful SetPlayOnPhoneDialString response の例</span><span class="sxs-lookup"><span data-stu-id="5b899-109">Successful SetPlayOnPhoneDialString response example</span></span>

### <a name="description"></a><span data-ttu-id="5b899-110">説明</span><span class="sxs-lookup"><span data-stu-id="5b899-110">Description</span></span>

<span data-ttu-id="5b899-111">SetPlayOnePhoneDialString response の次の例は、SetPlayOnPhoneDialString 要求に対する応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="5b899-111">The following example of a SetPlayOnePhoneDialString response shows a response to the SetPlayOnPhoneDialString request.</span></span>
  
### <a name="code"></a><span data-ttu-id="5b899-112">コード</span><span class="sxs-lookup"><span data-stu-id="5b899-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetPlayOnPhoneDialStringResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="5b899-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="5b899-113">See also</span></span>



[<span data-ttu-id="5b899-114">SetPlayOnPhoneDialString (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="5b899-114">SetPlayOnPhoneDialString (UM web service)</span></span>](setplayonphonedialstring-um-web-service.md)
  
[<span data-ttu-id="5b899-115">SetPlayOnPhoneDialStringResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="5b899-115">SetPlayOnPhoneDialStringResponse (UM web service)</span></span>](setplayonphonedialstringresponse-um-web-service.md)
  
<span data-ttu-id="5b899-116">[[] (UM web サービス)](dialstring-um-web-service.md)</span><span class="sxs-lookup"><span data-stu-id="5b899-116">[dialString (UM web service)](dialstring-um-web-service.md)</span></span>


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
description: SetPlayOnPhoneDialString 操作では、PlayOnPhone 操作 (UM web サービス)、および PlayOnPhoneGreeting 操作 (UM web サービス) の既定値として使用するダイヤル文字列を設定します。
ms.openlocfilehash: 0d1a879784740777e5eab0cbd5f85e59a6479461
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833446"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a><span data-ttu-id="a4373-103">SetPlayOnPhoneDialString 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="a4373-103">SetPlayOnPhoneDialString operation (UM web service)</span></span>

<span data-ttu-id="a4373-104">SetPlayOnPhoneDialString 操作では、 [PlayOnPhone 操作 (UM web サービス)](playonphone-operation-um-web-service.md) 、および[PlayOnPhoneGreeting 操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)の既定値として使用するダイヤル文字列を設定します。</span><span class="sxs-lookup"><span data-stu-id="a4373-104">The SetPlayOnPhoneDialString operation sets the dial string to use as the default for the [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and the [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md).</span></span>
  
## <a name="setplayonphonedialstring-request-example"></a><span data-ttu-id="a4373-105">SetPlayOnPhoneDialString 要求の例</span><span class="sxs-lookup"><span data-stu-id="a4373-105">SetPlayOnPhoneDialString request example</span></span>

### <a name="description"></a><span data-ttu-id="a4373-106">説明</span><span class="sxs-lookup"><span data-stu-id="a4373-106">Description</span></span>

<span data-ttu-id="a4373-107">SetPlayOnPhoneDialString 要求の次の例では、メールボックスの既定のダイヤル文字列を設定する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="a4373-107">The following example of a SetPlayOnPhoneDialString request shows how to form a request to set the default dial string for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="a4373-108">コード</span><span class="sxs-lookup"><span data-stu-id="a4373-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetPlayOnPhoneDialString xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <dialString>12345</dialString>
    </SetPlayOnPhoneDialString>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setplayonphonedialstring-response-example"></a><span data-ttu-id="a4373-109">成功した SetPlayOnPhoneDialString の応答の例</span><span class="sxs-lookup"><span data-stu-id="a4373-109">Successful SetPlayOnPhoneDialString response example</span></span>

### <a name="description"></a><span data-ttu-id="a4373-110">説明</span><span class="sxs-lookup"><span data-stu-id="a4373-110">Description</span></span>

<span data-ttu-id="a4373-111">SetPlayOnPhoneDialString 要求への応答を SetPlayOnePhoneDialString の応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a4373-111">The following example of a SetPlayOnePhoneDialString response shows a response to the SetPlayOnPhoneDialString request.</span></span>
  
### <a name="code"></a><span data-ttu-id="a4373-112">コード</span><span class="sxs-lookup"><span data-stu-id="a4373-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetPlayOnPhoneDialStringResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="a4373-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="a4373-113">See also</span></span>



[<span data-ttu-id="a4373-114">SetPlayOnPhoneDialString (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="a4373-114">SetPlayOnPhoneDialString (UM web service)</span></span>](setplayonphonedialstring-um-web-service.md)
  
[<span data-ttu-id="a4373-115">SetPlayOnPhoneDialStringResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="a4373-115">SetPlayOnPhoneDialStringResponse (UM web service)</span></span>](setplayonphonedialstringresponse-um-web-service.md)
  
[<span data-ttu-id="a4373-116">dialString (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="a4373-116">dialString (UM web service)</span></span>](dialstring-um-web-service.md)


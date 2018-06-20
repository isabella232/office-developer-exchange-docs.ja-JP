---
title: IsUMEnabled 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: fbe6cd95-f7a5-42b9-8a9d-b6159a269d55
description: IsUMEnabled 操作では、ユニファイド メッセージングのメールボックスが有効になっているかどうかを決定します。
ms.openlocfilehash: 9d94a359d6b11e41762d21aa2fe5501bd9f7b577
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832107"
---
# <a name="isumenabled-operation-um-web-service"></a><span data-ttu-id="1b457-103">IsUMEnabled 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="1b457-103">IsUMEnabled operation (UM web service)</span></span>

<span data-ttu-id="1b457-104">IsUMEnabled 操作では、ユニファイド メッセージングのメールボックスが有効になっているかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="1b457-104">The IsUMEnabled operation determines whether a mailbox is enabled for Unified Messaging.</span></span>
  
## <a name="isumenabled-request-example"></a><span data-ttu-id="1b457-105">IsUMEnabled 要求の例</span><span class="sxs-lookup"><span data-stu-id="1b457-105">IsUMEnabled request example</span></span>

### <a name="description"></a><span data-ttu-id="1b457-106">説明</span><span class="sxs-lookup"><span data-stu-id="1b457-106">Description</span></span>

<span data-ttu-id="1b457-107">IsUMEnabled 要求の次の例では、ユニファイド メッセージングのメールボックスが有効になっているかどうかを判断するための要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="1b457-107">The following example of an IsUMEnabled request shows how to form a request to determine whether a mailbox is enabled for Unified Messaging.</span></span>
  
### <a name="code"></a><span data-ttu-id="1b457-108">コード</span><span class="sxs-lookup"><span data-stu-id="1b457-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <IsUMEnabled xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-isumenabled-response-example"></a><span data-ttu-id="1b457-109">成功した IsUMEnabled の応答の例</span><span class="sxs-lookup"><span data-stu-id="1b457-109">Successful IsUMEnabled response example</span></span>

### <a name="description"></a><span data-ttu-id="1b457-110">説明</span><span class="sxs-lookup"><span data-stu-id="1b457-110">Description</span></span>

<span data-ttu-id="1b457-111">IsUMEnabled 要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1b457-111">The following example shows a successful response to an IsUMEnabled request.</span></span>
  
### <a name="code"></a><span data-ttu-id="1b457-112">コード</span><span class="sxs-lookup"><span data-stu-id="1b457-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <IsUMEnabledResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <IsUMEnabledResponse>true</IsUMEnabledResponse> 
    </IsUMEnabledResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="1b457-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="1b457-113">See also</span></span>



[<span data-ttu-id="1b457-114">IsUMEnabled (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="1b457-114">IsUMEnabled (UM web service)</span></span>](isumenabled-um-web-service.md)
  
[<span data-ttu-id="1b457-115">IsUMEnabledResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="1b457-115">IsUMEnabledResponse (UM web service)</span></span>](isumenabledresponse-um-web-service.md)


[<span data-ttu-id="1b457-116">ユニファイド メッセージング web サービスの XML 要素の交換</span><span class="sxs-lookup"><span data-stu-id="1b457-116">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)


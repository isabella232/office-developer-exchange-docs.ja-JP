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
description: IsUMEnabled 操作は、メールボックスがユニファイドメッセージングに対して有効になっているかどうかを判断します。
ms.openlocfilehash: b1478f5a113059251fe1b036ac7d77e5a4ab4f50
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458237"
---
# <a name="isumenabled-operation-um-web-service"></a><span data-ttu-id="ca442-103">IsUMEnabled 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="ca442-103">IsUMEnabled operation (UM web service)</span></span>

<span data-ttu-id="ca442-104">IsUMEnabled 操作は、メールボックスがユニファイドメッセージングに対して有効になっているかどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="ca442-104">The IsUMEnabled operation determines whether a mailbox is enabled for Unified Messaging.</span></span>
  
## <a name="isumenabled-request-example"></a><span data-ttu-id="ca442-105">IsUMEnabled 要求の例</span><span class="sxs-lookup"><span data-stu-id="ca442-105">IsUMEnabled request example</span></span>

### <a name="description"></a><span data-ttu-id="ca442-106">説明</span><span class="sxs-lookup"><span data-stu-id="ca442-106">Description</span></span>

<span data-ttu-id="ca442-107">次の IsUMEnabled 要求の例は、メールボックスがユニファイドメッセージングに対して有効になっているかどうかを判断する要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="ca442-107">The following example of an IsUMEnabled request shows how to form a request to determine whether a mailbox is enabled for Unified Messaging.</span></span>
  
### <a name="code"></a><span data-ttu-id="ca442-108">コード</span><span class="sxs-lookup"><span data-stu-id="ca442-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <IsUMEnabled xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-isumenabled-response-example"></a><span data-ttu-id="ca442-109">Successful IsUMEnabled response の例</span><span class="sxs-lookup"><span data-stu-id="ca442-109">Successful IsUMEnabled response example</span></span>

### <a name="description"></a><span data-ttu-id="ca442-110">説明</span><span class="sxs-lookup"><span data-stu-id="ca442-110">Description</span></span>

<span data-ttu-id="ca442-111">次の例は、IsUMEnabled 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="ca442-111">The following example shows a successful response to an IsUMEnabled request.</span></span>
  
### <a name="code"></a><span data-ttu-id="ca442-112">コード</span><span class="sxs-lookup"><span data-stu-id="ca442-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <IsUMEnabledResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <IsUMEnabledResponse>true</IsUMEnabledResponse> 
    </IsUMEnabledResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="ca442-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="ca442-113">See also</span></span>



[<span data-ttu-id="ca442-114">IsUMEnabled (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="ca442-114">IsUMEnabled (UM web service)</span></span>](isumenabled-um-web-service.md)
  
[<span data-ttu-id="ca442-115">IsUMEnabledResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="ca442-115">IsUMEnabledResponse (UM web service)</span></span>](isumenabledresponse-um-web-service.md)


[<span data-ttu-id="ca442-116">Exchange 用のユニファイドメッセージング web サービスの XML 要素</span><span class="sxs-lookup"><span data-stu-id="ca442-116">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)


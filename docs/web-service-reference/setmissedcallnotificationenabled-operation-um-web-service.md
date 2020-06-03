---
title: SetMissedCallNotificationEnabled 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetMissedCallNotificationEnabled
api_type:
- schema
ms.assetid: 6693b5db-ac6b-43bc-af83-a9c94fc425bf
description: SetMissedCallNotificationEnabled 操作は、不在着信通知を有効または無効にします。
ms.openlocfilehash: ca4942942a81bc187e8e18a5e6f003f8587f79d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467397"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a><span data-ttu-id="39bd9-103">SetMissedCallNotificationEnabled 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="39bd9-103">SetMissedCallNotificationEnabled operation (UM web service)</span></span>

<span data-ttu-id="39bd9-104">SetMissedCallNotificationEnabled 操作は、不在着信通知を有効または無効にします。</span><span class="sxs-lookup"><span data-stu-id="39bd9-104">The SetMissedCallNotificationEnabled operation enables or disables missed call notifications.</span></span>
  
## <a name="setmissedcallnotificationenabled-request-example"></a><span data-ttu-id="39bd9-105">SetMissedCallNotificationEnabled 要求の例</span><span class="sxs-lookup"><span data-stu-id="39bd9-105">SetMissedCallNotificationEnabled request example</span></span>

### <a name="description"></a><span data-ttu-id="39bd9-106">Description</span><span class="sxs-lookup"><span data-stu-id="39bd9-106">Description</span></span>

<span data-ttu-id="39bd9-107">次の SetMissedCallNotificationEnabled 要求の例は、不在着信通知を有効にする要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="39bd9-107">The following example of a SetMissedCallNotificationEnabled request shows how to form a request to enable missed call notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="39bd9-108">コード</span><span class="sxs-lookup"><span data-stu-id="39bd9-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetMissedCallNotificationEnabled xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetMissedCallNotificationEnabled>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setmissedcallnotificationenabled-response-example"></a><span data-ttu-id="39bd9-109">Successful SetMissedCallNotificationEnabled response の例</span><span class="sxs-lookup"><span data-stu-id="39bd9-109">Successful SetMissedCallNotificationEnabled response example</span></span>

### <a name="description"></a><span data-ttu-id="39bd9-110">Description</span><span class="sxs-lookup"><span data-stu-id="39bd9-110">Description</span></span>

<span data-ttu-id="39bd9-111">次の Playon電話案内応答の例は、SetMissedCallNotificationEnabled 要求に対する応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="39bd9-111">The following example of a PlayOnPhoneGreeting response shows a response to the SetMissedCallNotificationEnabled request.</span></span>
  
### <a name="code"></a><span data-ttu-id="39bd9-112">コード</span><span class="sxs-lookup"><span data-stu-id="39bd9-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetMissedCallNotificationEnabledResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="39bd9-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="39bd9-113">See also</span></span>



[<span data-ttu-id="39bd9-114">SetMissedCallNotificationEnabled (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="39bd9-114">SetMissedCallNotificationEnabled (UM web service)</span></span>](setmissedcallnotificationenabled-um-web-service.md)
  
[<span data-ttu-id="39bd9-115">SetMissedCallNotificationEnabledResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="39bd9-115">SetMissedCallNotificationEnabledResponse (UM web service)</span></span>](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[<span data-ttu-id="39bd9-116">状態 (UM web サービス-SetMissedCallNotificationEnabled)</span><span class="sxs-lookup"><span data-stu-id="39bd9-116">Status (UM web service - SetMissedCallNotificationEnabled)</span></span>](status-um-web-servicesetmissedcallnotificationenabled.md)


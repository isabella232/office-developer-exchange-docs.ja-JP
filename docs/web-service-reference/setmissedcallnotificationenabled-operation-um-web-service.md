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
description: SetMissedCallNotificationEnabled 操作は、有効または、不在着信通知を無効にします。
ms.openlocfilehash: be9479d6ed2c5238ed19c3d22e028fca62b8deed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833434"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a><span data-ttu-id="550e8-103">SetMissedCallNotificationEnabled 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="550e8-103">SetMissedCallNotificationEnabled operation (UM web service)</span></span>

<span data-ttu-id="550e8-104">SetMissedCallNotificationEnabled 操作は、有効または、不在着信通知を無効にします。</span><span class="sxs-lookup"><span data-stu-id="550e8-104">The SetMissedCallNotificationEnabled operation enables or disables missed call notifications.</span></span>
  
## <a name="setmissedcallnotificationenabled-request-example"></a><span data-ttu-id="550e8-105">SetMissedCallNotificationEnabled 要求の例</span><span class="sxs-lookup"><span data-stu-id="550e8-105">SetMissedCallNotificationEnabled request example</span></span>

### <a name="description"></a><span data-ttu-id="550e8-106">説明</span><span class="sxs-lookup"><span data-stu-id="550e8-106">Description</span></span>

<span data-ttu-id="550e8-107">SetMissedCallNotificationEnabled 要求の次の例では、不在着信通知を有効にする要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="550e8-107">The following example of a SetMissedCallNotificationEnabled request shows how to form a request to enable missed call notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="550e8-108">コード</span><span class="sxs-lookup"><span data-stu-id="550e8-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetMissedCallNotificationEnabled xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetMissedCallNotificationEnabled>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setmissedcallnotificationenabled-response-example"></a><span data-ttu-id="550e8-109">成功した SetMissedCallNotificationEnabled の応答の例</span><span class="sxs-lookup"><span data-stu-id="550e8-109">Successful SetMissedCallNotificationEnabled response example</span></span>

### <a name="description"></a><span data-ttu-id="550e8-110">説明</span><span class="sxs-lookup"><span data-stu-id="550e8-110">Description</span></span>

<span data-ttu-id="550e8-111">SetMissedCallNotificationEnabled 要求への応答を PlayOnPhoneGreeting の応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="550e8-111">The following example of a PlayOnPhoneGreeting response shows a response to the SetMissedCallNotificationEnabled request.</span></span>
  
### <a name="code"></a><span data-ttu-id="550e8-112">コード</span><span class="sxs-lookup"><span data-stu-id="550e8-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetMissedCallNotificationEnabledResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="550e8-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="550e8-113">See also</span></span>



[<span data-ttu-id="550e8-114">SetMissedCallNotificationEnabled (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="550e8-114">SetMissedCallNotificationEnabled (UM web service)</span></span>](setmissedcallnotificationenabled-um-web-service.md)
  
[<span data-ttu-id="550e8-115">SetMissedCallNotificationEnabledResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="550e8-115">SetMissedCallNotificationEnabledResponse (UM web service)</span></span>](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[<span data-ttu-id="550e8-116">状態 (UM web サービス - SetMissedCallNotificationEnabled)</span><span class="sxs-lookup"><span data-stu-id="550e8-116">Status (UM web service - SetMissedCallNotificationEnabled)</span></span>](status-um-web-servicesetmissedcallnotificationenabled.md)


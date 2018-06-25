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
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a>SetMissedCallNotificationEnabled 操作 (UM web サービス)

SetMissedCallNotificationEnabled 操作は、有効または、不在着信通知を無効にします。
  
## <a name="setmissedcallnotificationenabled-request-example"></a>SetMissedCallNotificationEnabled 要求の例

### <a name="description"></a>説明

SetMissedCallNotificationEnabled 要求の次の例では、不在着信通知を有効にする要求を作成する方法を示します。
  
### <a name="code"></a>コード

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

## <a name="successful-setmissedcallnotificationenabled-response-example"></a>成功した SetMissedCallNotificationEnabled の応答の例

### <a name="description"></a>説明

SetMissedCallNotificationEnabled 要求への応答を PlayOnPhoneGreeting の応答の例を次に示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetMissedCallNotificationEnabledResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[SetMissedCallNotificationEnabled (UM web サービス)](setmissedcallnotificationenabled-um-web-service.md)
  
[SetMissedCallNotificationEnabledResponse (UM web サービス)](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[状態 (UM web サービス - SetMissedCallNotificationEnabled)](status-um-web-servicesetmissedcallnotificationenabled.md)


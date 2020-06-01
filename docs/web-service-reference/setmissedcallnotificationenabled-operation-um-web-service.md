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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467397"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a>SetMissedCallNotificationEnabled 操作 (UM web サービス)

SetMissedCallNotificationEnabled 操作は、不在着信通知を有効または無効にします。
  
## <a name="setmissedcallnotificationenabled-request-example"></a>SetMissedCallNotificationEnabled 要求の例

### <a name="description"></a>説明

次の SetMissedCallNotificationEnabled 要求の例は、不在着信通知を有効にする要求を形成する方法を示しています。
  
### <a name="code"></a>コード

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

## <a name="successful-setmissedcallnotificationenabled-response-example"></a>Successful SetMissedCallNotificationEnabled response の例

### <a name="description"></a>説明

次の Playon電話案内応答の例は、SetMissedCallNotificationEnabled 要求に対する応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetMissedCallNotificationEnabledResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[SetMissedCallNotificationEnabled (UM web サービス)](setmissedcallnotificationenabled-um-web-service.md)
  
[SetMissedCallNotificationEnabledResponse (UM web サービス)](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[状態 (UM web サービス-SetMissedCallNotificationEnabled)](status-um-web-servicesetmissedcallnotificationenabled.md)


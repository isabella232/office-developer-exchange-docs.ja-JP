---
title: SetMissedCallNotificationEnabled 操作 (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- SetMissedCallNotificationEnabled
api_type:
- schema
ms.assetid: 6693b5db-ac6b-43bc-af83-a9c94fc425bf
description: SetMissedCallNotificationEnabled 操作は、欠けている通話通知を有効または無効にします。
ms.openlocfilehash: 31f59887041aac02e5876b596931902373870203
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521418"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a>SetMissedCallNotificationEnabled 操作 (UM Web サービス)

SetMissedCallNotificationEnabled 操作は、欠けている通話通知を有効または無効にします。
  
## <a name="setmissedcallnotificationenabled-request-example"></a>SetMissedCallNotificationEnabled 要求の例

### <a name="description"></a>説明

SetMissedCallNotificationEnabled 要求の次の例は、欠けている通話通知を有効にする要求を形成する方法を示しています。
  
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

## <a name="successful-setmissedcallnotificationenabled-response-example"></a>成功した SetMissedCallNotificationEnabled 応答の例

### <a name="description"></a>説明

PlayOnPhoneGreeting 応答の次の例は、SetMissedCallNotificationEnabled 要求に対する応答を示しています。
  
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



[SetMissedCallNotificationEnabled (UM Web サービス)](setmissedcallnotificationenabled-um-web-service.md)
  
[SetMissedCallNotificationEnabledResponse (UM Web サービス)](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[状態 (UM Web サービス - SetMissedCallNotificationEnabled)](status-um-web-servicesetmissedcallnotificationenabled.md)


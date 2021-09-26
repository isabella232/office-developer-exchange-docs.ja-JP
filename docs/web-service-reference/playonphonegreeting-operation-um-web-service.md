---
title: PlayOnPhoneGreeting 操作 (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 6deafc40-290b-4bce-9914-b6bcc529f38a
description: PlayOnPhoneGreeting 操作は、発信呼び出しを行い、電話で 2 つの案内応答メッセージの 1 つを再生します。
ms.openlocfilehash: 540cd44d35e70e2588446996aec19aeab17f83e9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543136"
---
# <a name="playonphonegreeting-operation-um-web-service"></a>PlayOnPhoneGreeting 操作 (UM Web サービス)

PlayOnPhoneGreeting 操作は、発信呼び出しを行い、電話で 2 つの案内応答メッセージの 1 つを再生します。
  
## <a name="playonphonegreeting-request-example"></a>PlayOnPhoneGreeting 要求の例

### <a name="description"></a>説明

PlayOnPhoneGreeting 要求の次の例は、発信呼び出しを行い、電話で通常の案内応答メッセージを再生する要求を形成する方法を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhoneGreeting xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GreetingType>NormalCustom</GreetingType>
      <DialString>12345</DialString>
    </PlayOnPhoneGreeting>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphonegreeting-response-example"></a>PlayOnPhoneGreeting 応答の成功例

### <a name="description"></a>説明

PlayOnPhoneGreeting 応答の次の例は、PlayOnPhoneGreeting 要求に対する応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneGreetingResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <PlayOnPhoneGreetingResponse>MjA4MTQ5MmItMTBmZC00ZGFmLThiMzEtNDllNDJjM2Y3MjIxQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneGreetingResponse> 
    </PlayOnPhoneGreetingResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[PlayOnPhoneGreeting (UM Web サービス)](playonphonegreeting-um-web-service.md)
  
[PlayOnPhoneGreetingResponse (UM Web サービス)](playonphonegreetingresponse-um-web-service.md)
  
[GreetingType (UM Web サービス)](greetingtype-um-web-service.md)
  
[dialString (UM Web サービス)](dialstring-um-web-service.md)


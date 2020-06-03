---
title: Playon電話案内応答操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 6deafc40-290b-4bce-9914-b6bcc529f38a
description: Playon電話案内応答操作は、発信通話を行い、電話で2つの案内応答メッセージの1つを再生します。
ms.openlocfilehash: 3af120b9ac8d7a368742fad2850c924228488662
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528896"
---
# <a name="playonphonegreeting-operation-um-web-service"></a>Playon電話案内応答操作 (UM web サービス)

Playon電話案内応答操作は、発信通話を行い、電話で2つの案内応答メッセージの1つを再生します。
  
## <a name="playonphonegreeting-request-example"></a>Playon電話案内応答要求の例

### <a name="description"></a>Description

次に示す Playon電話案内応答要求の例は、発信通話を行い、電話で通常の案内応答メッセージを再生する要求を形成する方法を示しています。
  
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

## <a name="successful-playonphonegreeting-response-example"></a>成功した Playon電話案内応答の例

### <a name="description"></a>Description

次の Playon電話案内応答の例は、Playonphone 案内応答要求に対する応答を示しています。
  
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



[Playon電話応答メッセージ (UM web サービス)](playonphonegreeting-um-web-service.md)
  
[PlayOnPhoneGreetingResponse (UM web サービス)](playonphonegreetingresponse-um-web-service.md)
  
[GreetingType (UM web サービス)](greetingtype-um-web-service.md)
  
[[] (UM web サービス)](dialstring-um-web-service.md)


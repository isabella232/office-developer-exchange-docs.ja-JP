---
title: PlayOnPhoneGreeting 操作 (UM web サービス)
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
description: PlayOnPhoneGreeting 操作では、発信呼び出しし、2 つの応答メッセージのメッセージのいずれかを電話で再生します。
ms.openlocfilehash: 85ba76c7638911678c1ef1aef88f47fdab2c6a4e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832828"
---
# <a name="playonphonegreeting-operation-um-web-service"></a>PlayOnPhoneGreeting 操作 (UM web サービス)

PlayOnPhoneGreeting 操作では、発信呼び出しし、2 つの応答メッセージのメッセージのいずれかを電話で再生します。
  
## <a name="playonphonegreeting-request-example"></a>PlayOnPhoneGreeting 要求の例

### <a name="description"></a>説明

PlayOnPhoneGreeting 要求の次の例では、発信呼び出しを行い、通常のグリーティング メッセージを電話で再生する要求を作成する方法を示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhoneGreeting xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GreetingType>NormalCustom</GreetingType>
      <DialString>12345</DialString>
    </PlayOnPhoneGreeting>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphonegreeting-response-example"></a>成功した PlayOnPhoneGreeting の応答の例

### <a name="description"></a>説明

PlayOnPhoneGreeting 要求への応答を PlayOnPhoneGreeting の応答の例を次に示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneGreetingResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <PlayOnPhoneGreetingResponse>MjA4MTQ5MmItMTBmZC00ZGFmLThiMzEtNDllNDJjM2Y3MjIxQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneGreetingResponse> 
    </PlayOnPhoneGreetingResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[PlayOnPhoneGreeting (UM web サービス)](playonphonegreeting-um-web-service.md)
  
[PlayOnPhoneGreetingResponse (UM web サービス)](playonphonegreetingresponse-um-web-service.md)
  
[GreetingType (UM web サービス)](greetingtype-um-web-service.md)
  
[dialString (UM web サービス)](dialstring-um-web-service.md)


---
title: PlayOnPhone 操作 (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 7d55be55-f8b6-4e96-a61e-26fa190217fd
description: PlayOnPhone 操作は、発信呼び出しを行い、DialString 要素で指定された電話で指定されたメッセージを再生します。
ms.openlocfilehash: 4d18727da18c36e6410c3cc6ab3bbf873993be72
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516566"
---
# <a name="playonphone-operation-um-web-service"></a>PlayOnPhone 操作 (UM Web サービス)

PlayOnPhone 操作は、発信呼び出しを行い **、DialString** 要素で指定された電話で指定されたメッセージを再生します。 
  
## <a name="playonphone-request-example"></a>PlayOnPhone 要求の例

### <a name="description"></a>説明

PlayOnPhone 要求の次の例は、送信呼び出しを行い、メッセージを再生する要求を形成する方法を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhone xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <entryId>AAAAAGsd2rbQLVtLobUGbrq/9IUHAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAACxVpEl+KVVLl957wp//x6UAGAetcDUAAA==</entryId>
      <DialString>12345</DialString>
    </PlayOnPhone>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphone-response-example"></a>PlayOnPhone 応答の成功例

### <a name="description"></a>説明

PlayOnPhone 応答の次の例は、PlayOnPhone 要求に対する応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <PlayOnPhoneResponse>NDEzYjEzNmMtZTE2Zi00NTJlLWI3YzctNDhkMTE3MDE3YjlmQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneResponse> 
    </PlayOnPhoneResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[PlayOnPhone (UM Web サービス)](playonphone-um-web-service.md)
  
[PlayOnPhoneResponse (UM Web サービス)](playonphoneresponse-um-web-service.md)
  
[PlayOnPhoneGreeting 操作 (UM Web サービス)](playonphonegreeting-operation-um-web-service.md)


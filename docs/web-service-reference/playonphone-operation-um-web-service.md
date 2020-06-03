---
title: PlayOnPhone 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 7d55be55-f8b6-4e96-a61e-26fa190217fd
description: PlayOnPhone 操作は、発信呼び出しを行い、ダイヤル文字列要素で指定されている電話で指定されたメッセージを再生します。
ms.openlocfilehash: c5ff82bcd822aa2c659d1782ea4a1349d198bc80
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466235"
---
# <a name="playonphone-operation-um-web-service"></a>PlayOnPhone 操作 (UM web サービス)

PlayOnPhone 操作は、発信呼び出しを行い、ダイヤル**文字列**要素で指定されている電話で指定されたメッセージを再生します。 
  
## <a name="playonphone-request-example"></a>PlayOnPhone 要求の例

### <a name="description"></a>Description

次の PlayOnPhone 要求の例は、発信通話を行い、メッセージを再生するための要求を形成する方法を示しています。
  
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

## <a name="successful-playonphone-response-example"></a>成功した PlayOnPhone 応答の例

### <a name="description"></a>Description

次の PlayOnPhone 応答の例は、PlayOnPhone 要求に対する応答を示しています。
  
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



[PlayOnPhone (UM web サービス)](playonphone-um-web-service.md)
  
[PlayOnPhoneResponse (UM web サービス)](playonphoneresponse-um-web-service.md)
  
[Playon電話案内応答操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)


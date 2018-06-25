---
title: 操作 (UM web サービス) に接続を切断します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Disconnect
api_type:
- schema
ms.assetid: a987000b-d6e6-49d7-944c-e9c278d0236f
description: 切断操作は、指定した CallId (UM web サービス) によって識別されるコールを終了します。
ms.openlocfilehash: 1e04e65fa1951a6aa46e2c8b6dd5fe524c84a8fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760076"
---
# <a name="disconnect-operation-um-web-service"></a>操作 (UM web サービス) に接続を切断します。

切断操作は、指定した[CallId (UM web サービス)](callid-um-web-service.md)によって識別されるコールを終了します。
  
## <a name="disconnect-request-example"></a>切断要求の例

### <a name="description"></a>説明

切断要求の次の例では、呼び出しの切断要求を形成する方法を示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <Disconnect xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </Disconnect>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-disconnect-response-example"></a>切断応答の成功の例

### <a name="description"></a>説明

切断応答の次の例では、切断要求への応答を示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <DisconnectResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目

- [(UM web サービス) に接続を切断します。](disconnect-um-web-service.md) 
- [DisconnectResponse (UM web サービス)](disconnectresponse-um-web-service.md) 
- [CallId (UM web サービス)](callid-um-web-service.md)


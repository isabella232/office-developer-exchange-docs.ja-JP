---
title: GetCallInfo 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfo
api_type:
- schema
ms.assetid: 6bccd418-caf7-4eb9-8a6f-410e56a635c3
description: GetCallInfo 操作では、CallId (UM web サービス) で指定されている送信呼び出しのステータスを返します。
ms.openlocfilehash: 36f9cba3690520ebb457a4cb2bfbcde3fea4b8dc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760649"
---
# <a name="getcallinfo-operation-um-web-service"></a>GetCallInfo 操作 (UM web サービス)

GetCallInfo 操作では、 [CallId (UM web サービス)](callid-um-web-service.md)で指定されている送信呼び出しのステータスを返します。
  
## <a name="getcallinfo-request-example"></a>GetCallInfo 要求の例

### <a name="description"></a>説明

GetCallInfo 要求の次の例では、指定した発信呼び出しについての情報を取得する要求を作成する方法を示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetCallInfo xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </GetCallInfo>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getcallinfo-response-example"></a>成功した GetCallInfo の応答の例

### <a name="description"></a>説明

GetCallInfo 要求への応答を GetCallInfo の応答の例を次に示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetCallInfoResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetCallInfoResponse>
        <CallState>Connected</CallState> 
        <EventCause>None</EventCause> 
      </GetCallInfoResponse>
    </GetCallInfoResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[GetCallInfo (UM web サービス)](getcallinfo-um-web-service.md)
  
[GetCallInfoResponse (UM web サービス)](getcallinforesponse-um-web-service.md)
  
[CallId (UM web サービス)](callid-um-web-service.md)
  
[CallState (UM web サービス)](callstate-um-web-service.md)
  
[EventCause (UM web サービス)](eventcause-um-web-service.md)


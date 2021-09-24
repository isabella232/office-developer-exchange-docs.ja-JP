---
title: GetCallInfo 操作 (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- GetCallInfo
api_type:
- schema
ms.assetid: 6bccd418-caf7-4eb9-8a6f-410e56a635c3
description: GetCallInfo 操作は、CallId (UM Web サービス) で指定された発信呼び出しの状態を返します。
ms.openlocfilehash: 0563190ab267b3a48d7ccacbdb1e136c6e3da0b4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509945"
---
# <a name="getcallinfo-operation-um-web-service"></a>GetCallInfo 操作 (UM Web サービス)

GetCallInfo 操作は [、CallId (UM Web サービス)](callid-um-web-service.md)で指定された発信呼び出しの状態を返します。
  
## <a name="getcallinfo-request-example"></a>GetCallInfo 要求の例

### <a name="description"></a>説明

GetCallInfo 要求の次の例は、指定された発信呼び出しに関する情報を取得する要求を形成する方法を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetCallInfo xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </GetCallInfo>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getcallinfo-response-example"></a>GetCallInfo 応答の成功例

### <a name="description"></a>説明

GetCallInfo 応答の次の例は、GetCallInfo 要求に対する応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetCallInfoResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GetCallInfoResponse>
        <CallState>Connected</CallState> 
        <EventCause>None</EventCause> 
      </GetCallInfoResponse>
    </GetCallInfoResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[GetCallInfo (UM Web サービス)](getcallinfo-um-web-service.md)
  
[GetCallInfoResponse (UM Web サービス)](getcallinforesponse-um-web-service.md)
  
[CallId (UM Web サービス)](callid-um-web-service.md)
  
[CallState (UM Web サービス)](callstate-um-web-service.md)
  
[EventCause (UM Web サービス)](eventcause-um-web-service.md)


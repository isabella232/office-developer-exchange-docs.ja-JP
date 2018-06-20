---
title: SetOofStatus 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetOofStatus
api_type:
- schema
ms.assetid: 97c271e9-506e-43eb-89cd-46803fc47ee5
description: SetOofStatus 操作は、要求したユーザーの Office (OOF) の案内応答を再生するかどうかを示す値を設定します。
ms.openlocfilehash: 2bb1deeec8ddb5be56979bfb2fae3396672298a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833445"
---
# <a name="setoofstatus-operation-um-web-service"></a>SetOofStatus 操作 (UM web サービス)

SetOofStatus 操作は、要求したユーザーの Office (OOF) の案内応答を再生するかどうかを示す値を設定します。
  
## <a name="setoofstatus-request-example"></a>SetOofStatus 要求の例

### <a name="description"></a>説明

SetOofStatus 要求の次の例では、メールボックスの不在時の Office の案内応答を有効にする要求を作成する方法を示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetOofStatus xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetOofStatus>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setoofstatus-response-example"></a>成功した SetOofStatus の応答の例

### <a name="description"></a>説明

SetOofStatus 要求への応答を SetOofStatus の応答の例を次に示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetOofStatusResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[SetOofStatus (UM web サービス)](setoofstatus-um-web-service.md)
  
[SetOofStatusResponse (UM web サービス)](setoofstatusresponse-um-web-service.md)
  
[状態 (UM web サービス - SetOofStatus)](status-um-web-servicesetoofstatus.md)


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
description: SetOofStatus 操作は、要求を行うユーザーに対して不在時 (OOF) の案内応答を再生するかどうかを示す値を設定します。
ms.openlocfilehash: 2311b6137ac25d15ad3d06668450c1d0f7ec1fad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467355"
---
# <a name="setoofstatus-operation-um-web-service"></a>SetOofStatus 操作 (UM web サービス)

SetOofStatus 操作は、要求を行うユーザーに対して不在時 (OOF) の案内応答を再生するかどうかを示す値を設定します。
  
## <a name="setoofstatus-request-example"></a>SetOofStatus 要求の例

### <a name="description"></a>説明

次の SetOofStatus 要求の例は、メールボックスの不在時の応答メッセージを有効にする要求を形成する方法を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetOofStatus xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetOofStatus>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setoofstatus-response-example"></a>成功した SetOofStatus response の例

### <a name="description"></a>説明

次の SetOofStatus 応答の例は、SetOofStatus 要求に対する応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetOofStatusResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[SetOofStatus (UM web サービス)](setoofstatus-um-web-service.md)
  
[SetOofStatusResponse (UM web サービス)](setoofstatusresponse-um-web-service.md)
  
[状態 (UM web サービス-SetOofStatus)](status-um-web-servicesetoofstatus.md)


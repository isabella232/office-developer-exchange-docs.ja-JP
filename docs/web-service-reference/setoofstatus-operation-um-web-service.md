---
title: SetOofStatus 操作 (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- SetOofStatus
api_type:
- schema
ms.assetid: 97c271e9-506e-43eb-89cd-46803fc47ee5
description: SetOofStatus 操作は、要求を行うユーザーに対して、Office (OOF) の出力案内応答を再生するかどうかを示す値を設定します。
ms.openlocfilehash: ce736e7d7bea39f65843923187af3ae616ae1c86
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544753"
---
# <a name="setoofstatus-operation-um-web-service"></a>SetOofStatus 操作 (UM Web サービス)

SetOofStatus 操作は、要求を行うユーザーに対して、Office (OOF) の出力案内応答を再生するかどうかを示す値を設定します。
  
## <a name="setoofstatus-request-example"></a>SetOofStatus 要求の例

### <a name="description"></a>説明

SetOofStatus 要求の次の例は、メールボックスのアウト オブ Officeを有効にする要求を形成する方法を示しています。
  
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

## <a name="successful-setoofstatus-response-example"></a>成功した SetOofStatus 応答の例

### <a name="description"></a>説明

SetOofStatus 応答の次の例は、SetOofStatus 要求に対する応答を示しています。
  
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



[SetOofStatus (UM Web サービス)](setoofstatus-um-web-service.md)
  
[SetOofStatusResponse (UM Web サービス)](setoofstatusresponse-um-web-service.md)
  
[状態 (UM Web サービス - SetOofStatus)](status-um-web-servicesetoofstatus.md)


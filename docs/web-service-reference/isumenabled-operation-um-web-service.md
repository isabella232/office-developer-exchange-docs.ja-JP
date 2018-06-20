---
title: IsUMEnabled 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: fbe6cd95-f7a5-42b9-8a9d-b6159a269d55
description: IsUMEnabled 操作では、ユニファイド メッセージングのメールボックスが有効になっているかどうかを決定します。
ms.openlocfilehash: 9d94a359d6b11e41762d21aa2fe5501bd9f7b577
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832107"
---
# <a name="isumenabled-operation-um-web-service"></a>IsUMEnabled 操作 (UM web サービス)

IsUMEnabled 操作では、ユニファイド メッセージングのメールボックスが有効になっているかどうかを決定します。
  
## <a name="isumenabled-request-example"></a>IsUMEnabled 要求の例

### <a name="description"></a>説明

IsUMEnabled 要求の次の例では、ユニファイド メッセージングのメールボックスが有効になっているかどうかを判断するための要求を作成する方法を示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <IsUMEnabled xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-isumenabled-response-example"></a>成功した IsUMEnabled の応答の例

### <a name="description"></a>説明

IsUMEnabled 要求に正常な応答の例を次に示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <IsUMEnabledResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <IsUMEnabledResponse>true</IsUMEnabledResponse> 
    </IsUMEnabledResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[IsUMEnabled (UM web サービス)](isumenabled-um-web-service.md)
  
[IsUMEnabledResponse (UM web サービス)](isumenabledresponse-um-web-service.md)


[ユニファイド メッセージング web サービスの XML 要素の交換](unified-messaging-web-service-xml-elements-for-exchange.md)


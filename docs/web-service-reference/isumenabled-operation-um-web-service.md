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
description: IsUMEnabled 操作は、メールボックスがユニファイドメッセージングに対して有効になっているかどうかを判断します。
ms.openlocfilehash: b1478f5a113059251fe1b036ac7d77e5a4ab4f50
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458237"
---
# <a name="isumenabled-operation-um-web-service"></a>IsUMEnabled 操作 (UM web サービス)

IsUMEnabled 操作は、メールボックスがユニファイドメッセージングに対して有効になっているかどうかを判断します。
  
## <a name="isumenabled-request-example"></a>IsUMEnabled 要求の例

### <a name="description"></a>説明

次の IsUMEnabled 要求の例は、メールボックスがユニファイドメッセージングに対して有効になっているかどうかを判断する要求を形成する方法を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <IsUMEnabled xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-isumenabled-response-example"></a>Successful IsUMEnabled response の例

### <a name="description"></a>説明

次の例は、IsUMEnabled 要求に対する正常な応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <IsUMEnabledResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <IsUMEnabledResponse>true</IsUMEnabledResponse> 
    </IsUMEnabledResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[IsUMEnabled (UM web サービス)](isumenabled-um-web-service.md)
  
[IsUMEnabledResponse (UM web サービス)](isumenabledresponse-um-web-service.md)


[Exchange 用のユニファイドメッセージング web サービスの XML 要素](unified-messaging-web-service-xml-elements-for-exchange.md)


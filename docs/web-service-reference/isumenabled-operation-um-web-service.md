---
title: IsUMEnabled 操作 (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: fbe6cd95-f7a5-42b9-8a9d-b6159a269d55
description: IsUMEnabled 操作は、メールボックスがユニファイド メッセージングに対して有効になっているかどうかを決定します。
ms.openlocfilehash: 2c637711fc34a1d1ccc484b14be3199632aaaaa3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514460"
---
# <a name="isumenabled-operation-um-web-service"></a>IsUMEnabled 操作 (UM Web サービス)

IsUMEnabled 操作は、メールボックスがユニファイド メッセージングに対して有効になっているかどうかを決定します。
  
## <a name="isumenabled-request-example"></a>IsUMEnabled 要求の例

### <a name="description"></a>説明

IsUMEnabled 要求の次の例は、ユニファイド メッセージングでメールボックスが有効かどうかを判断する要求を形成する方法を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <IsUMEnabled xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-isumenabled-response-example"></a>成功した IsUMEnabled 応答の例

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



[IsUMEnabled (UM Web サービス)](isumenabled-um-web-service.md)
  
[IsUMEnabledResponse (UM Web サービス)](isumenabledresponse-um-web-service.md)


[ユニファイド メッセージング Web サービスの XML 要素 (Exchange](unified-messaging-web-service-xml-elements-for-exchange.md)


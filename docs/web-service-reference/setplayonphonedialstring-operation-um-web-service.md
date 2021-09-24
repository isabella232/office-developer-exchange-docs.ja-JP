---
title: SetPlayOnPhoneDialString 操作 (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: a68479f2-d900-4dd8-a5ce-dbea8247e841
description: SetPlayOnPhoneDialString 操作は、PlayOnPhone 操作 (UM Web サービス) および PlayOnPhoneGreeting 操作 (UM Web サービス) の既定として使用するダイヤル文字列を設定します。
ms.openlocfilehash: 89f83d7b0a1d56cb0adeccbf4fa0bb67f1197253
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531910"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a>SetPlayOnPhoneDialString 操作 (UM Web サービス)

SetPlayOnPhoneDialString 操作では、ダイヤル文字列を [PlayOnPhone](playonphone-operation-um-web-service.md) 操作 (UM Web サービス) および [PlayOnPhoneGreeting](playonphonegreeting-operation-um-web-service.md)操作 (UM Web サービス) の既定値として設定します。
  
## <a name="setplayonphonedialstring-request-example"></a>SetPlayOnPhoneDialString 要求の例

### <a name="description"></a>説明

SetPlayOnPhoneDialString 要求の次の例は、メールボックスの既定のダイヤル文字列を設定する要求を形成する方法を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetPlayOnPhoneDialString xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <dialString>12345</dialString>
    </SetPlayOnPhoneDialString>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setplayonphonedialstring-response-example"></a>成功した SetPlayOnPhoneDialString 応答の例

### <a name="description"></a>説明

SetPlayOnePhoneDialString 応答の次の例は、SetPlayOnPhoneDialString 要求に対する応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetPlayOnPhoneDialStringResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[SetPlayOnPhoneDialString (UM Web サービス)](setplayonphonedialstring-um-web-service.md)
  
[SetPlayOnPhoneDialStringResponse (UM Web サービス)](setplayonphonedialstringresponse-um-web-service.md)
  
[dialString (UM Web サービス)](dialstring-um-web-service.md)


---
title: SetPlayOnPhoneDialString 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: a68479f2-d900-4dd8-a5ce-dbea8247e841
description: SetPlayOnPhoneDialString 操作では、PlayOnPhone 操作 (UM web サービス) および Playonphone 案内応答操作 (UM web サービス) の既定として使用するダイヤル文字列を設定します。
ms.openlocfilehash: 7df806eedc2d6d037394f31ec4ccbfe28aaf3372
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458643"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a>SetPlayOnPhoneDialString 操作 (UM web サービス)

SetPlayOnPhoneDialString 操作では、 [Playonphone 操作 (um web サービス)](playonphone-operation-um-web-service.md)および[Playonphone 案内応答操作 (um web サービス)](playonphonegreeting-operation-um-web-service.md)の既定として使用するダイヤル文字列を設定します。
  
## <a name="setplayonphonedialstring-request-example"></a>SetPlayOnPhoneDialString 要求の例

### <a name="description"></a>説明

次の SetPlayOnPhoneDialString 要求の例は、メールボックスの既定のダイヤル文字列を設定する要求を形成する方法を示しています。
  
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

## <a name="successful-setplayonphonedialstring-response-example"></a>Successful SetPlayOnPhoneDialString response の例

### <a name="description"></a>説明

SetPlayOnePhoneDialString response の次の例は、SetPlayOnPhoneDialString 要求に対する応答を示しています。
  
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



[SetPlayOnPhoneDialString (UM web サービス)](setplayonphonedialstring-um-web-service.md)
  
[SetPlayOnPhoneDialStringResponse (UM web サービス)](setplayonphonedialstringresponse-um-web-service.md)
  
[[] (UM web サービス)](dialstring-um-web-service.md)


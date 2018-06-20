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
description: SetPlayOnPhoneDialString 操作では、PlayOnPhone 操作 (UM web サービス)、および PlayOnPhoneGreeting 操作 (UM web サービス) の既定値として使用するダイヤル文字列を設定します。
ms.openlocfilehash: 0d1a879784740777e5eab0cbd5f85e59a6479461
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833446"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a>SetPlayOnPhoneDialString 操作 (UM web サービス)

SetPlayOnPhoneDialString 操作では、 [PlayOnPhone 操作 (UM web サービス)](playonphone-operation-um-web-service.md) 、および[PlayOnPhoneGreeting 操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)の既定値として使用するダイヤル文字列を設定します。
  
## <a name="setplayonphonedialstring-request-example"></a>SetPlayOnPhoneDialString 要求の例

### <a name="description"></a>説明

SetPlayOnPhoneDialString 要求の次の例では、メールボックスの既定のダイヤル文字列を設定する要求を作成する方法を示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetPlayOnPhoneDialString xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <dialString>12345</dialString>
    </SetPlayOnPhoneDialString>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setplayonphonedialstring-response-example"></a>成功した SetPlayOnPhoneDialString の応答の例

### <a name="description"></a>説明

SetPlayOnPhoneDialString 要求への応答を SetPlayOnePhoneDialString の応答の例を次に示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetPlayOnPhoneDialStringResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[SetPlayOnPhoneDialString (UM web サービス)](setplayonphonedialstring-um-web-service.md)
  
[SetPlayOnPhoneDialStringResponse (UM web サービス)](setplayonphonedialstringresponse-um-web-service.md)
  
[dialString (UM web サービス)](dialstring-um-web-service.md)


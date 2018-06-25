---
title: ResetPIN 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- ResetPIN
api_type:
- schema
ms.assetid: c0f14a15-3389-4311-8bac-f87930c5f5d4
description: ResetPIN 操作では、暗証番号 (pin) (TUI パスワード) を新しいランダムな値に変更します。
ms.openlocfilehash: e6417b86ce17c0d34fe857cf1209a18972cbef63
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833146"
---
# <a name="resetpin-operation-um-web-service"></a>ResetPIN 操作 (UM web サービス)

ResetPIN 操作では、暗証番号 (pin) (TUI パスワード) を新しいランダムな値に変更します。
  
## <a name="remarks"></a>備考

ResetPIN 操作では、暗証番号 (pin) のポリシーに基づき、新しい PIN を作成します。 操作が成功した場合、新しい暗証番号 (pin) を含む電子メール メッセージがユーザーのメールボックスに送信されます。 操作が失敗した場合、エラーに関する情報が含まれている例外がスローされます。
  
## <a name="resetpin-request-example"></a>ResetPIN 要求の例

### <a name="description"></a>説明

ResetPIN 要求の次の例では、メールボックスの PIN をリセットする要求を作成する方法を示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a>ResetPIN 応答の成功の例

### <a name="description"></a>説明

ResetPIN 要求への応答を ResetPIN 応答の例を次に示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResetPINResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[ResetPIN (UM web サービス)](resetpin-um-web-service.md)
  
[ResetPINResponse (UM web サービス)](resetpinresponse-um-web-service.md)


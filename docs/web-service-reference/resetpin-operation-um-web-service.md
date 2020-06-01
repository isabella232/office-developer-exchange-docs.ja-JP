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
description: ResetPIN 操作は、PIN (TUI パスワード) を新しいランダムな値に変更します。
ms.openlocfilehash: 8de64ce7a47e9c426f8eb9298e1ca00508fb616c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44465493"
---
# <a name="resetpin-operation-um-web-service"></a>ResetPIN 操作 (UM web サービス)

ResetPIN 操作は、PIN (TUI パスワード) を新しいランダムな値に変更します。
  
## <a name="remarks"></a>注釈

ResetPIN 操作は、PIN ポリシーに基づいて新しい PIN を作成します。 操作が成功した場合は、新しい PIN を含む電子メールメッセージがユーザーのメールボックスに送信されます。 操作が失敗した場合は、エラーに関する情報を含む例外がスローされます。
  
## <a name="resetpin-request-example"></a>ResetPIN 要求の例

### <a name="description"></a>説明

次の ResetPIN 要求の例は、メールボックスの PIN をリセットする要求を形成する方法を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a>正常な ResetPIN 応答の例

### <a name="description"></a>説明

次の ResetPIN 応答の例は、ResetPIN 要求に対する応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResetPINResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[ResetPIN (UM web サービス)](resetpin-um-web-service.md)
  
[ResetPINResponse (UM web サービス)](resetpinresponse-um-web-service.md)


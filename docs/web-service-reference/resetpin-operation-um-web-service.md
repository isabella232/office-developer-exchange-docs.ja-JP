---
title: ResetPIN 操作 (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- ResetPIN
api_type:
- schema
ms.assetid: c0f14a15-3389-4311-8bac-f87930c5f5d4
description: ResetPIN 操作では、PIN (TUI パスワード) が新しいランダム値に変更されます。
ms.openlocfilehash: 12f1e5719184df84f6c29ab3d02cc362f87abc76
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539109"
---
# <a name="resetpin-operation-um-web-service"></a>ResetPIN 操作 (UM Web サービス)

ResetPIN 操作では、PIN (TUI パスワード) が新しいランダム値に変更されます。
  
## <a name="remarks"></a>注釈

ResetPIN 操作は、PIN ポリシーに基づいて新しい PIN を作成します。 操作が成功すると、新しい PIN を含む電子メール メッセージがユーザーのメールボックスに送信されます。 操作が失敗した場合、エラーに関する情報を含む例外がスローされます。
  
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

## <a name="successful-resetpin-response-example"></a>ResetPIN 応答の成功例

### <a name="description"></a>説明

ResetPIN 応答の次の例は、ResetPIN 要求に対する応答を示しています。
  
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



[ResetPIN (UM Web サービス)](resetpin-um-web-service.md)
  
[ResetPINResponse (UM Web サービス)](resetpinresponse-um-web-service.md)


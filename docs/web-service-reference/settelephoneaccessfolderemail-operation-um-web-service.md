---
title: SetTelephoneAccessFolderEmail 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetTelephoneAccessFolderEmail
api_type:
- schema
ms.assetid: 2c92d914-bdee-4337-b3ea-0655fdb658e9
description: SetTelephoneAccessFolderEmail 操作では、ユニファイド メッセージングはの読み取り元メッセージのユーザーに電話でフォルダーを設定します。
ms.openlocfilehash: 9497e58f66b8efcf7e358aa529223942298a3bed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833459"
---
# <a name="settelephoneaccessfolderemail-operation-um-web-service"></a>SetTelephoneAccessFolderEmail 操作 (UM web サービス)

SetTelephoneAccessFolderEmail 操作では、ユニファイド メッセージングはの読み取り元メッセージのユーザーに電話でフォルダーを設定します。
  
## <a name="settelephoneaccessfolderemail-request-example"></a>SetTelephoneAccessFolderEmail 要求の例

### <a name="description"></a>説明

SetTelephoneAccessFolderEmail 要求の次の例では、ユニファイド メッセージングはの読み取り元のユーザーに電話でフォルダーを設定する要求を作成する方法を示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetTelephoneAccessFolderEmail xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <base64FolderID>AAAAAGsd2rbQLVtLobUGbrq/9IUBAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAAA==</base64FolderID>
    </SetTelephoneAccessFolderEmail>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-settelephoneaccessfolderemail-response-example"></a>成功した SetTelephoneAccessFolderEmail の応答の例

### <a name="description"></a>説明

SetTelephoneAccessFolderEmail 要求への応答を SetTelephoneAccessFolderEmail の応答の例を次に示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetTelephoneAccessFolderEmailResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[SetTelephoneAccessFolderEmail (UM web サービス)](settelephoneaccessfolderemail-um-web-service.md)
  
[SetTelephoneAccessFolderEmailResponse (UM web サービス)](settelephoneaccessfolderemailresponse-um-web-service.md)
  
[base64FolderId (UM web サービス)](base64folderid-um-web-service.md)


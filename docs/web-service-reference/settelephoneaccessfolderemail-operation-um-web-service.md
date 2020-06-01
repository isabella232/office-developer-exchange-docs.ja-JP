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
description: SetTelephoneAccessFolderEmail 操作は、ユニファイドメッセージングが電話でユーザーにメッセージを読み取るためのフォルダーを設定します。
ms.openlocfilehash: a2bb630f812ca811b4cbe68db1308dc18e5d3ba0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467334"
---
# <a name="settelephoneaccessfolderemail-operation-um-web-service"></a>SetTelephoneAccessFolderEmail 操作 (UM web サービス)

SetTelephoneAccessFolderEmail 操作は、ユニファイドメッセージングが電話でユーザーにメッセージを読み取るためのフォルダーを設定します。
  
## <a name="settelephoneaccessfolderemail-request-example"></a>SetTelephoneAccessFolderEmail 要求の例

### <a name="description"></a>説明

次の SetTelephoneAccessFolderEmail 要求の例は、ユニファイドメッセージングが電話でユーザーに返信するフォルダーを設定する要求を形成する方法を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetTelephoneAccessFolderEmail xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <base64FolderID>AAAAAGsd2rbQLVtLobUGbrq/9IUBAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAAA==</base64FolderID>
    </SetTelephoneAccessFolderEmail>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-settelephoneaccessfolderemail-response-example"></a>Successful SetTelephoneAccessFolderEmail response の例

### <a name="description"></a>説明

SetTelephoneAccessFolderEmail response の次の例は、SetTelephoneAccessFolderEmail 要求に対する応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetTelephoneAccessFolderEmailResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[SetTelephoneAccessFolderEmail (UM web サービス)](settelephoneaccessfolderemail-um-web-service.md)
  
[SetTelephoneAccessFolderEmailResponse (UM web サービス)](settelephoneaccessfolderemailresponse-um-web-service.md)
  
[base64FolderId (UM web サービス)](base64folderid-um-web-service.md)


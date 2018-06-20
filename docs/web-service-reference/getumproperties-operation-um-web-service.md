---
title: GetUMProperties 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetUMProperties
api_type:
- schema
ms.assetid: 301fb9a3-67df-44c4-8ffe-0600237fc344
description: GetUMProperties 操作は、要求を行っているユーザーのメールボックスのすべてのユニファイド メッセージング プロパティを取得します。
ms.openlocfilehash: 8878099bbd907fe0648f7d64dde3cd9600c2c45f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831678"
---
# <a name="getumproperties-operation-um-web-service"></a>GetUMProperties 操作 (UM web サービス)

GetUMProperties 操作は、要求を行っているユーザーのメールボックスのすべてのユニファイド メッセージング プロパティを取得します。
  
## <a name="getumproperties-request-example"></a>GetUMProperties 要求の例

### <a name="description"></a>説明

GetUMProperties 要求の次の例では、メールボックスのユニファイド メッセージング プロパティを取得する要求を作成する方法を示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUMProperties xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getumproperties-response-example"></a>成功した GetUMProperties の応答の例

### <a name="description"></a>説明

GetUMProperties 要求への応答を GetUMProperties の応答の例を次に示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetUMPropertiesResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetUMPropertiesResponse>
        <OofStatus>false</OofStatus> 
        <MissedCallNotificationEnabled>true</MissedCallNotificationEnabled> 
        <PlayOnPhoneDialString>12345</PlayOnPhoneDialString> 
        <TelephoneAccessNumbers>54321</TelephoneAccessNumbers> 
        <TelephoneAccessFolderEmail>AAAAAGsd2rbQLVtLobUGbrq/9IUBAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAAA==</TelephoneAccessFolderEmail> 
      </GetUMPropertiesResponse>
    </GetUMPropertiesResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[GetUMProperties (UM web サービス)](getumproperties-um-web-service.md)
  
[GetUMPropertiesResponse (UM web サービス)](getumpropertiesresponse-um-web-service.md)


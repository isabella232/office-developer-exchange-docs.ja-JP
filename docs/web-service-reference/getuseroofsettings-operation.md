---
title: GetUserOofSettings 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetUserOofSettings
api_type:
- schema
ms.assetid: 153e4440-495b-4972-9811-2fbea740142a
description: GetUserOofSettings 操作は、メールボックス ユーザーの [無効] (OOF) Officeメッセージを取得します。
ms.openlocfilehash: 9298681bff1cce5be37e8bee978ddeb0431bacdc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533411"
---
# <a name="getuseroofsettings-operation"></a>GetUserOofSettings 操作

**GetUserOofSettings** 操作は、メールボックス ユーザーの [無効] (OOF) Officeメッセージを取得します。 
  
## <a name="soap-headers"></a>SOAP ヘッダー

**GetUserOofSettings** 操作では、次の表に示す SOAP ヘッダーを使用できます。 
  
|**Header**|**Element**|**説明**|
|:-----|:-----|:-----|
|偽装  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装しているユーザーを識別します。  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。  <br/> |
   
## <a name="using-the-getuseroofsettings-operation"></a>GetUserOofSettings 操作の使用

**GetUserOofSettings** 操作では、ユーザーの OOF 設定にアクセスできます。 ユーザーは、ユーザーの電子メール アドレスによって識別されます。 OOF メッセージが null で、OOF が有効になっている場合、OOF メッセージは送信されません。 
  
> [!IMPORTANT]
> OOF メッセージが MicrosoftOfficeOutlook によって設定されている場合、この操作は OOF メッセージを HTML 形式で返します。 
  
## <a name="getuseroofsettings-request-example"></a>GetUserOofSettings 要求の例

### <a name="description"></a>説明

次の例は、1 人のユーザーの OOF 情報を取得する **GetUserOofSettings** 要求を示しています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns ="https://schemas.microsoft.com/exchange/services/2006/types">
        <Address>User1@example.com</Address>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>要求要素

要求では、次の要素が使用されます。
  
- [GetUserOofSettingsRequest](getuseroofsettingsrequest.md)
    
- [Mailbox (Availability)](mailbox-availability.md)
    
- [Address (string)](address-string.md)
    
## <a name="successful-getuseroofsettings-response-example"></a>GetUserOofSettings 応答の成功例

### <a name="description"></a>説明

次の使用例は、OOF メッセージを含む無効な OOF 状態を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetUserOofSettingsResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessage ResponseClass="Success">
        <ResponseCode>NoError</ResponseCode>
      </ResponseMessage>
      <OofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Disabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2006-11-03T23:00:00</StartTime>
          <EndTime>2006-11-04T23:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office. This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </OofSettings>
      <AllowExternalOof>All</AllowExternalOof>
    </GetUserOofSettingsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-getuseroofsettings-response-elements"></a>GetUserOofSettings 応答要素の成功

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetUserOofSettingsResponse](getuseroofsettingsresponse.md)
    
- [ResponseMessage](responsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [OofSettings](oofsettings.md)
    
- [OofState](oofstate.md)
    
- [ExternalAudience](externalaudience.md)
    
- [Duration (UserOofSettings)](duration-useroofsettings.md)
    
- [StartTime](starttime.md)
    
- [EndTime](endtime.md)
    
- [InternalReply](internalreply.md)
    
- [ExternalReply](externalreply.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [AllowExternalOof](allowexternaloof.md)
    
## <a name="getuseroofsettings-error-response-example"></a>GetUserOofSettings エラー応答の例

### <a name="description"></a>説明

次の例は、別のユーザーの OOF 情報にアクセスしようとして発生したエラー応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <soap:Fault>
      <faultcode>soap:Client</faultcode>
      <faultstring>Microsoft.Exchange.Data.Storage.AccessDeniedException: User is not mailbox owner. User = S-1-5-21-3642464542-282065186-3871681729-1155, MailboxGuid = S-1-5-21-3642464542-282065186-3871681729-1156 ---> User is not mailbox owner. </faultstring>
      <faultactor>https://CAS01.example.com/EWS/Exchange.asmx</faultactor>
      <detail>
        <ErrorCode xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">-2146233088</ErrorCode>
      </detail>
    </soap:Fault>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


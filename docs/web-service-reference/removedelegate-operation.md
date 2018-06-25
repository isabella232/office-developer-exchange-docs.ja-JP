---
title: RemoveDelegate 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveDelegate
api_type:
- schema
ms.assetid: 1d42d5ff-8fde-4f8a-b18d-57b1ef7a946a
description: RemoveDelegate 操作は、ユーザーのメールボックスから、1 つまたは複数のデリゲートを削除します。
ms.openlocfilehash: 6f3371d19bd8a7fd967d4959d85037ae6b51f6aa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833088"
---
# <a name="removedelegate-operation"></a>RemoveDelegate 操作

**RemoveDelegate**操作は、ユーザーのメールボックスから、1 つまたは複数のデリゲートを削除します。 
  
## <a name="soap-headers"></a>SOAP ヘッダー

**RemoveDelegate**操作が一覧表示され、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**Header**|**要素**|**説明**|
|:-----|:-----|:-----|
|偽装  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装するユーザーを識別します。  <br/> |
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC3066 カルチャを使用してメールボックスへのアクセスを識別します。  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。  <br/> |
   
## <a name="removedelegate-request-example"></a>RemoveDelegate 要求の例

### <a name="description"></a>説明

次のコード例は、user1 のメールボックスからの 2 つのデリゲートを削除する方法を示しています。 この例では、代理人のプライマリ SMTP アドレスを使用して 1 つのデリゲートが削除され、代理人のセキュリティ識別子 (SID) を使用して、もう 1 つが削除されます。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <RemoveDelegate xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>user1@example.com</t:EmailAddress>
      </Mailbox>
      <UserIds>
        <t:UserId>
          <t:PrimarySmtpAddress>user2@example.com</t:PrimarySmtpAddress>
        </t:UserId>
        <t:UserId>
          <t:SID>S-1-5-21-1333220396-2200287332-232816053-1118</t:SID>
        </t:UserId>
      </UserIds>
    </RemoveDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

**RemoveDelegate**操作では、指定した代理ユーザーのメールボックスを持つまたは Active Directory ディレクトリ サービスに存在するは必要はありません。 代理エントリが孤立した場合は、 **RemoveDelegate**操作が成功します。 
  
## <a name="removedelegate-response-example"></a>RemoveDelegate の応答の例

### <a name="description"></a>説明

**RemoveDelegate**要求に正常な応答を**RemoveDelegate**の応答の例を次に示します。 応答には、各メールボックスから削除されるデリゲートの**DelegateUserResponseMessageType**要素が含まれています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" 
                         MinorVersion="1" 
                         MajorBuildNumber="206" 
                         MinorBuildNumber="0" 
                         Version="Exchange2007_SP1" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:RemoveDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              ResponseClass="Success" 
                              xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      </m:RemoveDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="removedelegate-error-response-example"></a>RemoveDelegate エラー応答の例

### <a name="description"></a>説明

**RemoveDelegate**エラー応答の次の使用例は、存在しないデリゲートを削除する要求の結果を示しています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8"
                         MinorVersion="1"
                         MajorBuildNumber="206"
                         MinorBuildNumber="0"
                         Version="Exchange2007_SP1"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:RemoveDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                              ResponseClass="Success"
                              xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Error">
          <m:MessageText>The user is not a delegate for the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorNotDelegate</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:RemoveDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


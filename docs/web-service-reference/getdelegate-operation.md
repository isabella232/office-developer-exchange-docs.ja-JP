---
title: GetDelegate 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegate
api_type:
- schema
ms.assetid: 849b2c9e-4685-4bd1-9adb-aba0fcc52650
description: GetDelegate 操作は、指定されたメールボックスの代理人の設定を取得します。
ms.openlocfilehash: bd1a0add54ee5fd1c23b4ba09a921a9061afa394
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760684"
---
# <a name="getdelegate-operation"></a>GetDelegate 操作

**GetDelegate**操作は、指定されたメールボックスの代理人の設定を取得します。 
  
## <a name="soap-headers"></a>SOAP ヘッダー

**GetDelegate**操作が一覧表示され、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**Header**|**要素**|**説明**|
|:-----|:-----|:-----|
|偽装  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装するユーザーを識別します。  <br/> |
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC3066 カルチャを使用してメールボックスへのアクセスを識別します。  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。  <br/> |
   
## <a name="getdelegate-request-example"></a>GetDelegate 要求の例

### <a name="description"></a>説明

User3 のメールボックスに設定されているすべての代理人の代理人の設定を取得する方法を次のコード例に示します。 ユーザーごとにすべてのアクセス許可は、応答で返されます。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <GetDelegate xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                 IncludePermissions="true">
      <Mailbox>
        <t:EmailAddress>user3@example.com</t:EmailAddress>
      </Mailbox>
    </GetDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

[ユーザー Id](userid.md)要素を使用するには、メールボックスの代理人アクセス権限を持っているすべてのユーザーを返すのではなく個々 のユーザーを指定します。 
  
> [!NOTE]
> Exchange Web サービス (EWS) は、管理グループの代理人をサポートしていません。 セキュリティ グループの代理人がいる主体の**GetDelegate**操作が呼び出された場合、EWS はエラーを返します。 
  
## <a name="getdelegate-response-example"></a>GetDelegate の応答の例

### <a name="description"></a>説明

**GetDelegate**要求に正常な応答を**GetDelegate**の応答の例を次に示します。 応答には、代理人アクセスのアクセス許可に関する情報が含まれている、要求が配信されたか、代理人が代理人にコピーし、メッセージ、会議の出席の会議の対象にするかどうか、プライベートなアイテムを表示できます。 
  
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
    <m:GetDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                           ResponseClass="Success" 
                           xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
              <t:UserId>
                <t:SID>S-1-5-21-1333220396-2200287332-232816053-1116</t:SID>
                <t:PrimarySmtpAddress>User1@example.com</t:PrimarySmtpAddress>
                <t:DisplayName>User1</t:DisplayName>
              </t:UserId>
              <t:DelegatePermissions>
                <t:CalendarFolderPermissionLevel>Author</t:CalendarFolderPermissionLevel>
                <t:ContactsFolderPermissionLevel>Reviewer</t:ContactsFolderPermissionLevel>
              </t:DelegatePermissions>
              <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
            </m:DelegateUser>
          </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      <m:DeliverMeetingRequests>DelegatesAndMe</m:DeliverMeetingRequests>
      </m:GetDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


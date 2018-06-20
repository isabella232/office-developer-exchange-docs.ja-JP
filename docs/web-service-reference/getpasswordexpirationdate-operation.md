---
title: GetPasswordExpirationDate 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0297458-58fb-4e5d-bb47-0cd17155e106
description: GetPasswordExpirationDate 操作では、現在のユーザーの電子メール アカウントのパスワード有効期限の日付を提供します。
ms.openlocfilehash: c57942c88b09a910e2d529a12ea279bb2da5d693
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760816"
---
# <a name="getpasswordexpirationdate-operation"></a>GetPasswordExpirationDate 操作

**GetPasswordExpirationDate**操作では、現在のユーザーの電子メール アカウントのパスワード有効期限の日付を提供します。 
  
この操作は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="getpasswordexpirationdate-operation-soap-headers"></a>GetPasswordExpirationDate 操作の SOAP ヘッダー

**GetPasswordExpirationDate**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**Header**|**要素**|**説明**|
|:-----|:-----|:-----|
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。 これは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマを識別します。 これは、要求に適用されます。 これは、要求に適用されます。  <br/> |
   
## <a name="getpasswordexpirationdate-operation-request-example"></a>GetPasswordExpirationDate 操作の要求の例

### <a name="description"></a>説明

**GetPasswordExpirationDate**操作要求の次の例では、電子メール アカウントのパスワードの有効期限の日付を取得する方法を示します。 
  
### <a name="code"></a>コード

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
  </soap:Header>
  <soap:Body>
    <tns:GetPasswordExpirationDate>
      <tns:MailboxSmtpAddress>user1@DTZMZX-dom.extest.microsoft.com</tns:MailboxSmtpAddress>
    </tns:GetPasswordExpirationDate>
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a>要素を要求します。

次の要素は、要求で使用されます。
  
- [GetPasswordExpirationDate](getpasswordexpirationdate.md)
    
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
## <a name="successful-getpasswordexpirationdate-operation-response"></a>GetPasswordExpirationDate 操作の成功の応答

次の要素は、応答で使用されます。
  
- [GetPasswordExpirationDateResponse](getpasswordexpirationdateresponse.md)
    
- [PasswordExpirationDate](passwordexpirationdate.md)
    


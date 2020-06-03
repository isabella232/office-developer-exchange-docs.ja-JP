---
title: GetPasswordExpirationDate 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0297458-58fb-4e5d-bb47-0cd17155e106
description: GetPasswordExpirationDate 操作は、現在のユーザーの電子メールアカウントパスワードの有効期限日を提供します。
ms.openlocfilehash: 4184092cf98161e4c2f74446cef5439722ae71a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457894"
---
# <a name="getpasswordexpirationdate-operation"></a>GetPasswordExpirationDate 操作

**GetPasswordExpirationDate**操作は、現在のユーザーの電子メールアカウントパスワードの有効期限日を提供します。 
  
この操作は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="getpasswordexpirationdate-operation-soap-headers"></a>GetPasswordExpirationDate 操作の SOAP ヘッダー

**GetPasswordExpirationDate**操作では、次の表に示す SOAP ヘッダーを使用できます。 
  
|**Header**|**要素**|**説明**|
|:-----|:-----|:-----|
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。 これは要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマを識別します。 これは要求に適用されます。 これは要求に適用されます。  <br/> |
   
## <a name="getpasswordexpirationdate-operation-request-example"></a>GetPasswordExpirationDate 操作要求の例

### <a name="description"></a>Description

次の**GetPasswordExpirationDate**操作要求の例は、電子メールアカウントのパスワードの有効期限を取得する方法を示しています。 
  
### <a name="code"></a>コード

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
  </soap:Header>
  <soap:Body>
    <tns:GetPasswordExpirationDate>
      <tns:MailboxSmtpAddress>user1@DTZMZX-dom.extest.microsoft.com</tns:MailboxSmtpAddress>
    </tns:GetPasswordExpirationDate>
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a>Request 要素

要求では、次の要素が使用されます。
  
- [GetPasswordExpirationDate](getpasswordexpirationdate.md)
    
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
## <a name="successful-getpasswordexpirationdate-operation-response"></a>成功した GetPasswordExpirationDate 操作の応答

応答では、次の要素が使用されます。
  
- [GetPasswordExpirationDateResponse](getpasswordexpirationdateresponse.md)
    
- [PasswordExpirationDate](passwordexpirationdate.md)
    


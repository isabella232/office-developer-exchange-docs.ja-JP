---
title: OAuth を使用して IMAP、POP、SMTP 接続を認証する
description: IMAP、POP、および SMTP アプリケーションで OAuth 認証を使用する方法について説明します。
author: svpsiva
ms.date: 07/08/2021
ms.audience: Developer
ms.openlocfilehash: 4a307a6e329d5320b2b304d17a78a61db6d111bd
ms.sourcegitcommit: 357b882a02e37b380a23b8a45b15f9c006a40b02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/31/2021
ms.locfileid: "58764589"
---
# <a name="authenticate-an-imap-pop-or-smtp-connection-using-oauth"></a>OAuth を使用して IMAP、POP、SMTP 接続を認証する

OAuth 認証を使用して IMAP、POP、SMTP プロトコルに接続し、ユーザーの電子メール データにOffice 365します。

> 以下で説明する IMAP、POP、SMTP プロトコルの OAuth2 サポートは、Microsoft 365 (Office on the web を含む) と Outlook.com ユーザーの両方でサポートされています。

OAuth 2.0 プロトコルについて理解していない場合は、まず、OAuth [2.0](/azure/active-directory/develop/active-directory-v2-protocols)プロトコルの概要をMicrosoft ID プラットフォームしてください。 OAuth 2.0 プロトコルを実装してユーザーを認証し、セキュリティで保護された API にアクセスする Microsoft Authentication Libariers [(MSAL)](/azure/active-directory/develop/msal-overview)の詳細については、「MSAL の概要」を参照してください。

Azure Active Directory によって提供される OAuth 認証サービスを使用して、アプリケーションが IMAP、POP、または SMTP プロトコルに接続して、Exchange OnlineにアクセスOffice 365。 OAuth をアプリケーションで使用するには、次の必要があります。

1. Azure Active Directory に[アプリケーションを登録する](#register-your-application)。
1. [アプリケーションを構成](#configure-your-application)するには、Azure Active Directory。
1. [トークン サーバーからアクセス トークン](#get-an-access-token) を取得します。
1. [アクセス トークンを使用して接続](#authenticate-connection-requests) 要求を認証します。

## <a name="register-your-application"></a>アプリケーションを登録する

OAuth を使用するには、アプリケーションをアプリケーションに登録するAzure Active Directory。

「アプリケーションをアプリケーションに登録する」に記載されている手順に従って[、Microsoft ID プラットフォーム](/azure/active-directory/develop/quickstart-register-app)アプリケーションを作成します。

## <a name="get-an-access-token"></a>アクセス トークンを取得する

MSAL クライアント ライブラリのいずれかを使用 [して](/azure/active-directory/develop/msal-overview) 、クライアント アプリケーションからアクセス トークンを取得できます。

または、次の一覧から適切なフローを選択し、対応する手順に従って基になる ID プラットフォーム REST API を呼び出し、アクセス トークンを取得できます。

1. [OAuth2 承認コード フロー](/azure/active-directory/develop/v2-oauth2-auth-code-flow)
1. [OAuth2 デバイス承認付与フロー](/azure/active-directory/develop/v2-oauth2-device-code)

OAuth2 クライアント資格情報付与フローを介した IMAP、POP、SMTP AUTH プロトコルへの OAuth アクセスはサポートされていません。 アプリケーションで Microsoft 365 組織内のすべてのメールボックスへの永続的なアクセスが必要な場合は、ユーザーなしでアクセスを許可する Microsoft Graph API を使用し、詳細なアクセス許可を有効にし、管理者が特定のメールボックス セットへのアクセスをスコープに設定することをお勧めします。

アプリケーションを承認し、アクセス トークンを要求する場合Outlookリソース URL を含む、完全なスコープを指定してください。

| プロトコル  | アクセス許可スコープの文字列 |
|-----------|-------------------------|
| IMAP      | `https://outlook.office.com/IMAP.AccessAsUser.All` |
| POP       | `https://outlook.office.com/POP.AccessAsUser.All`  |
| SMTP AUTH | `https://outlook.office.com/SMTP.Send`             |

さらに、スコープを [要求offline_accessできます](/azure/active-directory/develop/v2-permissions-and-consent#offline_access) 。 ユーザーがスコープを承認offline_access、アプリはトークン エンドポイントから更新トークンMicrosoft ID プラットフォームできます。 更新トークンは長時間使用されます。 古いアクセス トークンの有効期限が切れると、アプリは新しいアクセス トークンを取得できます。

## <a name="authenticate-connection-requests"></a>接続要求の認証

メール サーバーの IMAP および POP Office 365設定を使用して、メール サーバーへの接続[を](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353)開始Office 365。

### <a name="sasl-xoauth2"></a>SASL XOAUTH2

OAuth との統合では、アプリケーションでアクセス トークンのエンコードと送信に SASL XOAUTH2 形式を使用する必要があります。 SASL XOAUTH2 は、ユーザー名とアクセス トークンを次の形式でエンコードします。

```text
base64("user=" + userName + "^Aauth=Bearer " + accessToken + "^A^A")
```

`^A`コントロール A ( **)**  +  **を表** します `%x01` 。

たとえば、アクセス トークンを使用してアクセスする SASL XOAUTH2 `test@contoso.onmicrosoft.com` 形式は次 `EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA` のようになります。

```text
base64("user=test@contoso.onmicrosoft.com^Aauth=Bearer EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA^A^A")
```

base64 エンコード後、これは次の文字列に変換されます。 読みやすさのために改行が挿入されます。

```text
dXNlcj10ZXN0QGNvbnRvc28ub25taWNyb3NvZnQuY29tAWF1dGg9QmVhcmVy
IEV3QkFBbDNCQUFVRkZwVUFvN0ozVmUwYmpMQldaV0NjbFJDM0VvQUEBAQ==
```

### <a name="sasl-xoauth2-authentication-for-shared-mailboxes-in-office-365"></a>サーバー内の共有メールボックスの SASL XOAUTH2 認証Office 365

OAuth を使用して共有メールボックスにアクセスする場合、アプリケーションはユーザーに代わってアクセス トークンを取得する必要がありますが、SASL XOAUTH2 エンコード文字列の userName フィールドを共有メールボックスの電子メール アドレスに置き換える必要があります。 

### <a name="imap-protocol-exchange"></a>IMAP プロトコル Exchange

IMAP サーバー接続を認証するには、クライアントは次の形式のコマンド `AUTHENTICATE` で応答する必要があります。

```text
AUTHENTICATE XOAUTH2 <base64 string in XOAUTH2 format>
```

認証が成功するクライアントとサーバーのメッセージ交換の例を次に示します。

```text
[connection begins]
C: C01 CAPABILITY
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 OK AUTHENTICATE completed.
```

認証エラーが発生するクライアントとサーバーのメッセージ交換の例を次に示します。

```text
[connection begins]
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 NO AUTHENTICATE failed.
```

### <a name="pop-protocol-exchange"></a>POP プロトコル Exchange

POP サーバー接続を認証するには、クライアントはコマンドを次の形式で 2 行に分割 `AUTH` して応答する必要があります。    

```text 
AUTH XOAUTH2 
<base64 string in XOAUTH2 format>   
``` 

認証が成功するクライアントとサーバーのメッセージ交換の例を次に示します。    

```text 
[connection begins] 
C: AUTH XOAUTH2     
S: +    
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYX   
JlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0  
Q2cBAQ==    
S: +OK User successfully authenticated. 
[connection continues...]   
``` 

認証エラーが発生するクライアントとサーバーのメッセージ交換の例を次に示します。    

```text 
[connection begins] 
C: AUTH XOAUTH2     
S: +    
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY    
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj   
l0Q2cBAQ=   
S: -ERR Authentication failure: unknown user name or bad password.  
```

### <a name="smtp-protocol-exchange"></a>SMTP プロトコル Exchange

SMTP サーバー接続を認証するには、クライアントは次の形式のコマンド `AUTH` で応答する必要があります。

```text
AUTH XOAUTH2 <base64 string in XOAUTH2 format>
```

認証が成功するクライアントとサーバーのメッセージ交換の例を次に示します。

```text
[connection begins]
C: auth xoauth2
S: 334
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj
l0Q2cBAQ==
S: 235 2.7.0 Authentication successful
[connection continues...]
```

認証エラーが発生するクライアントとサーバーのメッセージ交換の例を次に示します。

```text
[connection begins]
C: auth xoauth2
S: 334
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj
l0Q2cBAQ==
S: 535 5.7.3 Authentication unsuccessful [SN2PR00CA0018.namprd00.prod.outlook.com]
```

## <a name="see-also"></a>関連項目

- [Exchange における認証と EWS](../exchange-web-services/authentication-and-ews-in-exchange.md)
- [IMAP、POP 接続の設定](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353)
- [インターネット メッセージ アクセス プロトコル](https://tools.ietf.org/html/rfc3501)
- [Post Office プロトコル](https://tools.ietf.org/html/rfc1081)
- [認証用の SMTP サービス拡張機能](https://tools.ietf.org/html/rfc4954)

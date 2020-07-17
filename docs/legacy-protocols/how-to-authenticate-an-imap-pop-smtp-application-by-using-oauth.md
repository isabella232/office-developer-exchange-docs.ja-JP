---
title: OAuth を使用して IMAP、POP、または SMTP 接続を認証する
description: IMAP、POP、および SMTP アプリケーションで OAuth 認証を使用する方法について説明します。
author: svpsiva
ms.date: 02/19/2020
ms.audience: Developer
ms.openlocfilehash: f83a932790cde558e741ece1e87403103aff18fd
ms.sourcegitcommit: eeda51cb037aa25566adb293f25574674fdb2d9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/01/2020
ms.locfileid: "45012560"
---
# <a name="authenticate-an-imap-pop-or-smtp-connection-using-oauth"></a>OAuth を使用して IMAP、POP、または SMTP 接続を認証する

OAuth 認証を使用して IMAP、POP、または SMTP プロトコルに接続し、Office 365 ユーザーの電子メールデータにアクセスする方法について説明します。

> OAuth2 では、以下に示す IMAP、POP、SMTP プロトコルのサポートは、Outlook.com ユーザーに対してサポートされていません。

OAuth 2.0 に精通していない場合は、まず「 [Microsoft identity platform (v2.0)」の概要](/azure/active-directory/develop/v2-overview)を参照してください。 このドキュメントでは、Sdk を含む Microsoft identity platform のさまざまなコンポーネントについて説明します。

Azure Active Directory によって提供される OAuth 認証サービスを使用して、アプリケーションが IMAP、POP、または SMTP プロトコルを使用して Office 365 で Exchange Online にアクセスできるようにすることができます。 アプリケーションで OAuth を使用するには、次のことを行う必要があります。

1. Azure Active Directory に[アプリケーションを登録する](#register-your-application)。
1. Azure Active Directory で[アプリケーションを構成](#configure-your-application)します。
1. トークンサーバーから[アクセストークンを取得](#get-an-access-token)します。
1. アクセストークンを使用して[接続要求を認証](#authenticate-connection-requests)します。

## <a name="register-your-application"></a>アプリケーションを登録する

OAuth を使用するには、アプリケーションが Azure Active Directory に登録されている必要があります。

「 [Microsoft identity platform を使用してアプリケーションを登録](/azure/active-directory/develop/quickstart-register-app)する」に記載されている手順に従って、新しいアプリケーションを作成します。

## <a name="configure-your-application"></a>アプリケーションを構成する

[「Configure a client application to access Web api](/azure/active-directory/develop/quickstart-configure-app-access-web-apis) 」に記載されている手順に従います。

統合するプロトコルに対応する次の1つ以上のアクセス許可のスコープを追加してください。 **アクセス許可の追加**ウィザードで、[ **Microsoft Graph** ] を選択し、[**アクセス許可の委任**] をクリックして、次のアクセス許可スコープを検索します。

| プロトコル  | アクセス許可の適用範囲        |
|-----------|-------------------------|
| IMAP      | `IMAP.AccessAsUser.All` |
| POP       | `POP.AccessAsUser.All`  |
| SMTP 認証 | `SMTP.Send`             |

## <a name="get-an-access-token"></a>アクセス トークンを取得する

[Msal クライアントライブラリ](/azure/active-directory/develop/msal-overview)のいずれかを使用して、クライアントアプリケーションからアクセストークンを取得することができます。

または、次の一覧から適切なフローを選択し、対応する手順に従って、基になる identity platform REST Api を呼び出し、アクセストークンを取得することもできます。

1. [OAuth2 認証コードフロー](/azure/active-directory/develop/v2-oauth2-auth-code-flow)
1. [OAuth2 デバイス承認の付与フロー](/azure/active-directory/develop/v2-oauth2-device-code)

OAuth2 クライアント資格情報の付与フローを介した IMAP、POP、SMTP 認証プロトコルへの OAuth アクセスはサポートされていません。 アプリケーションが Microsoft 365 組織のすべてのメールボックスに永続的にアクセスする必要がある場合は、Microsoft Graph Api を使用して、ユーザーなしでアクセスを許可し、詳細なアクセス許可を有効にし、管理者が特定のメールボックスのセットへのアクセスを許可されるようにすることをお勧めします。

アプリケーションを承認してアクセストークンを要求するときには、Outlook リソース Url を含む完全な範囲を指定してください。

| プロトコル  | アクセス許可のスコープ文字列 |
|-----------|-------------------------|
| IMAP      | `https://outlook.office.com/IMAP.AccessAsUser.All` |
| POP       | `https://outlook.office.com/POP.AccessAsUser.All`  |
| SMTP 認証 | `https://outlook.office.com/SMTP.Send`             |

また、 [offline_access](/azure/active-directory/develop/v2-permissions-and-consent#offline_access)スコープを要求することもできます。 ユーザーが offline_access スコープを承認すると、アプリは Microsoft identity platform token endpoint から更新トークンを受け取ることができます。 更新トークンは長期間の場合があります。 アプリは、新しいアクセストークンを古いものとして期限切れにすることができます。

## <a name="authenticate-connection-requests"></a>接続要求を認証する

Office 365 メールサーバーへの接続は、 [office 365 の IMAP および POP の電子メール設定](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353)を使用して開始できます。

### <a name="sasl-xoauth2"></a>SASL XOAUTH2

OAuth の統合には、アプリケーションで、アクセストークンのエンコードと送信に SASL XOAUTH2 format を使用する必要があります。 SASL XOAUTH2 は、次の形式でユーザー名とアクセストークンをエンコードします。

```text
base64("user=" + userName + "^Aauth=Bearer " + accessToken + "^A^A")
```

`^A`**コントロール**  +  **a** () を表し `%x01` ます。

たとえば、アクセストークンを使用してアクセスする SASL XOAUTH2 形式は次のように `test@contoso.onmicrosoft.com` `EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA` なります。

```text
base64("user=test@contoso.onmicrosoft.com^Aauth=Bearer EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA^A^A")
```

Base64 エンコード後は、次の文字列に変換されます。 読みやすくするために改行が挿入されることに注意してください。

```text
dXNlcj10ZXN0QGNvbnRvc28ub25taWNyb3NvZnQuY29tAWF1dGg9QmVhcmVy
IEV3QkFBbDNCQUFVRkZwVUFvN0ozVmUwYmpMQldaV0NjbFJDM0VvQUEBAQ==
```

### <a name="sasl-xoauth2-authentication-for-shared-mailboxes-in-office-365"></a>Office 365 の共有メールボックスのための SASL XOAUTH2 認証

OAuth を使用した共有メールボックスアクセスの場合、アプリケーションはユーザーの代わりにアクセストークンを取得する必要がありますが、SASL XOAUTH2 encoded string の userName フィールドを共有メールボックスの電子メールアドレスに置き換えます。 

### <a name="imap-protocol-exchange"></a>IMAP プロトコルの Exchange

IMAP サーバー接続を認証するには、クライアントは次の形式のコマンドで応答する必要があり `AUTHENTICATE` ます。

```text
AUTHENTICATE XOAUTH2 <base64 string in XOAUTH2 format>
```

認証に成功した結果として得られるクライアントとサーバー間のメッセージ交換の例を次に示します。

```text
[connection begins]
C: C01 CAPABILITY
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 OK AUTHENTICATE completed.
```

認証エラーが発生するクライアントサーバーのメッセージ交換の例を次に示します。

```text
[connection begins]
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 NO AUTHENTICATE failed.
```

### <a name="pop-protocol-exchange"></a>POP プロトコルの交換

POP サーバー接続を認証するには、クライアントは `AUTH` コマンドを次の形式で2行に分割して応答する必要があります。    

```text 
AUTH XOAUTH2 
<base64 string in XOAUTH2 format>   
``` 

認証に成功した結果として得られるクライアントとサーバー間のメッセージ交換の例を次に示します。    

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

認証エラーが発生するクライアントサーバーのメッセージ交換の例を次に示します。    

```text 
[connection begins] 
C: AUTH XOAUTH2     
S: +    
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY    
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj   
l0Q2cBAQ=   
S: -ERR Authentication failure: unknown user name or bad password.  
```

### <a name="smtp-protocol-exchange"></a>SMTP プロトコルの Exchange

SMTP サーバー接続を認証するには、クライアントは次の形式のコマンドで応答する必要があり `AUTH` ます。

```text
AUTH XOAUTH2 <base64 string in XOAUTH2 format>
```

認証に成功した結果として得られるクライアントとサーバー間のメッセージ交換の例を次に示します。

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

認証エラーが発生するクライアントサーバーのメッセージ交換の例を次に示します。

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
- [インターネットメッセージアクセスプロトコル](https://tools.ietf.org/html/rfc3501)
- [Post Office Protocol](https://tools.ietf.org/html/rfc1081)
- [認証用の SMTP サービス拡張機能](https://tools.ietf.org/html/rfc4954)

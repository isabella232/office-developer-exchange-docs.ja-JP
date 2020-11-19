---
title: OAuth を使用して IMAP、POP、または SMTP 接続を認証する
description: IMAP、POP、および SMTP アプリケーションで OAuth 認証を使用する方法について説明します。
author: svpsiva
ms.date: 02/19/2020
ms.audience: Developer
ms.openlocfilehash: 4662aa904ed162edcced6c096eac8cf636180f6a
ms.sourcegitcommit: 37d4ecd4f469690ba1de87baad2f2f58c40c96ba
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/18/2020
ms.locfileid: "49348816"
---
# <a name="authenticate-an-imap-pop-or-smtp-connection-using-oauth"></a><span data-ttu-id="77063-103">OAuth を使用して IMAP、POP、または SMTP 接続を認証する</span><span class="sxs-lookup"><span data-stu-id="77063-103">Authenticate an IMAP, POP or SMTP connection using OAuth</span></span>

<span data-ttu-id="77063-104">OAuth 認証を使用して IMAP、POP、または SMTP プロトコルに接続し、Office 365 ユーザーの電子メールデータにアクセスする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="77063-104">Learn how to use OAuth authentication to connect with IMAP, POP or SMTP protocols and access email data for Office 365 users.</span></span>

> <span data-ttu-id="77063-105">以下に示すように、Microsoft 365 (web 上の Office を含む) および Outlook.com ユーザーの両方でサポートされている IMAP、POP、SMTP プロトコルの OAuth2 サポートがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="77063-105">OAuth2 support for IMAP, POP, SMTP protocols as described below is supported for both Microsoft 365 (which includes Office on the web) and Outlook.com users.</span></span>

<span data-ttu-id="77063-106">OAuth 2.0 プロトコルに精通していない場合は、まず「 [Microsoft identity platform の oauth 2.0 プロトコルの概要」](/azure/active-directory/develop/active-directory-v2-protocols)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77063-106">If you're not familiar with the OAuth 2.0 protocol, start by reading the [OAuth 2.0 protocol on Microsoft identity platform overview](/azure/active-directory/develop/active-directory-v2-protocols).</span></span> <span data-ttu-id="77063-107">OAuth 2.0 プロトコルを実装してユーザーを認証し、セキュリティで保護された Api にアクセスする Microsoft Authentication Libariers (MSAL) の詳細については、 [「Msal の概要」](/azure/active-directory/develop/msal-overview)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77063-107">To learn more about the Microsoft Authentication Libariers (MSAL), which implement the OAuth 2.0 protocol to authenticate users and access secure APIs, read the [MSAL overview](/azure/active-directory/develop/msal-overview).</span></span>

<span data-ttu-id="77063-108">Azure Active Directory によって提供される OAuth 認証サービスを使用して、アプリケーションが IMAP、POP、または SMTP プロトコルを使用して Office 365 で Exchange Online にアクセスできるようにすることができます。</span><span class="sxs-lookup"><span data-stu-id="77063-108">You can use the OAuth authentication service provided by Azure Active Directory to enable your application to connect with IMAP, POP or SMTP protocols to access Exchange Online in Office 365.</span></span> <span data-ttu-id="77063-109">アプリケーションで OAuth を使用するには、次のことを行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="77063-109">To use OAuth with your application you need to:</span></span>

1. <span data-ttu-id="77063-110">Azure Active Directory に[アプリケーションを登録する](#register-your-application)。</span><span class="sxs-lookup"><span data-stu-id="77063-110">[Register your application](#register-your-application) with Azure Active Directory.</span></span>
1. <span data-ttu-id="77063-111">Azure Active Directory で[アプリケーションを構成](#configure-your-application)します。</span><span class="sxs-lookup"><span data-stu-id="77063-111">[Configure your application](#configure-your-application) in Azure Active Directory.</span></span>
1. <span data-ttu-id="77063-112">トークンサーバーから[アクセストークンを取得](#get-an-access-token)します。</span><span class="sxs-lookup"><span data-stu-id="77063-112">[Get an access token](#get-an-access-token) from a token server.</span></span>
1. <span data-ttu-id="77063-113">アクセストークンを使用して[接続要求を認証](#authenticate-connection-requests)します。</span><span class="sxs-lookup"><span data-stu-id="77063-113">[Authenticate connection requests](#authenticate-connection-requests) with an access token.</span></span>

## <a name="register-your-application"></a><span data-ttu-id="77063-114">アプリケーションを登録する</span><span class="sxs-lookup"><span data-stu-id="77063-114">Register your application</span></span>

<span data-ttu-id="77063-115">OAuth を使用するには、アプリケーションが Azure Active Directory に登録されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="77063-115">To use OAuth, an application must be registered with Azure Active Directory.</span></span>

<span data-ttu-id="77063-116">「 [Microsoft identity platform を使用してアプリケーションを登録](/azure/active-directory/develop/quickstart-register-app) する」に記載されている手順に従って、新しいアプリケーションを作成します。</span><span class="sxs-lookup"><span data-stu-id="77063-116">Follow the instructions listed in [Register an application with the Microsoft identity platform](/azure/active-directory/develop/quickstart-register-app) to create a new application.</span></span>

## <a name="configure-your-application"></a><span data-ttu-id="77063-117">アプリケーションを構成する</span><span class="sxs-lookup"><span data-stu-id="77063-117">Configure your application</span></span>

<span data-ttu-id="77063-118">[「Configure a client application to access Web api](/azure/active-directory/develop/quickstart-configure-app-access-web-apis) 」に記載されている手順に従います。</span><span class="sxs-lookup"><span data-stu-id="77063-118">Follow the instructions listed in [Configure a client application to access web APIs](/azure/active-directory/develop/quickstart-configure-app-access-web-apis)</span></span>

<span data-ttu-id="77063-119">統合するプロトコルに対応する次の1つ以上のアクセス許可のスコープを追加してください。</span><span class="sxs-lookup"><span data-stu-id="77063-119">Make sure to add one or more of the following permission scopes that correspond to the protocols you would like to integrate with.</span></span> <span data-ttu-id="77063-120">**アクセス許可の追加** ウィザードで、[ **Microsoft Graph** ] を選択し、[**アクセス許可の委任**] をクリックして、次のアクセス許可スコープを検索します。</span><span class="sxs-lookup"><span data-stu-id="77063-120">In the **Add a permission** wizard, select **Microsoft Graph** and then **Delegated permissions** to find the following permission scopes listed.</span></span>

| <span data-ttu-id="77063-121">プロトコル</span><span class="sxs-lookup"><span data-stu-id="77063-121">Protocol</span></span>  | <span data-ttu-id="77063-122">アクセス許可の適用範囲</span><span class="sxs-lookup"><span data-stu-id="77063-122">Permission scope</span></span>        |
|-----------|-------------------------|
| <span data-ttu-id="77063-123">IMAP</span><span class="sxs-lookup"><span data-stu-id="77063-123">IMAP</span></span>      | `IMAP.AccessAsUser.All` |
| <span data-ttu-id="77063-124">POP</span><span class="sxs-lookup"><span data-stu-id="77063-124">POP</span></span>       | `POP.AccessAsUser.All`  |
| <span data-ttu-id="77063-125">SMTP 認証</span><span class="sxs-lookup"><span data-stu-id="77063-125">SMTP AUTH</span></span> | `SMTP.Send`             |

## <a name="get-an-access-token"></a><span data-ttu-id="77063-126">アクセス トークンを取得する</span><span class="sxs-lookup"><span data-stu-id="77063-126">Get an access token</span></span>

<span data-ttu-id="77063-127">[Msal クライアントライブラリ](/azure/active-directory/develop/msal-overview)のいずれかを使用して、クライアントアプリケーションからアクセストークンを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="77063-127">You can use one of our [MSAL client libraries](/azure/active-directory/develop/msal-overview) to fetch an access token from your client application.</span></span>

<span data-ttu-id="77063-128">または、次の一覧から適切なフローを選択し、対応する手順に従って、基になる identity platform REST Api を呼び出し、アクセストークンを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="77063-128">Alternatively, you can select an appropriate flow from the following list and follow the corresponding steps to call the underlying identity platform REST APIs and retrieve an access token.</span></span>

1. [<span data-ttu-id="77063-129">OAuth2 認証コードフロー</span><span class="sxs-lookup"><span data-stu-id="77063-129">OAuth2 authorization code flow</span></span>](/azure/active-directory/develop/v2-oauth2-auth-code-flow)
1. [<span data-ttu-id="77063-130">OAuth2 デバイス承認の付与フロー</span><span class="sxs-lookup"><span data-stu-id="77063-130">OAuth2 Device authorization grant flow</span></span>](/azure/active-directory/develop/v2-oauth2-device-code)

<span data-ttu-id="77063-131">OAuth2 クライアント資格情報の付与フローを介した IMAP、POP、SMTP 認証プロトコルへの OAuth アクセスはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77063-131">OAuth access to IMAP, POP, SMTP AUTH protocols via OAuth2 client credentials grant flow is not supported.</span></span> <span data-ttu-id="77063-132">アプリケーションが Microsoft 365 組織のすべてのメールボックスに永続的にアクセスする必要がある場合は、Microsoft Graph Api を使用して、ユーザーなしでアクセスを許可し、詳細なアクセス許可を有効にし、管理者が特定のメールボックスのセットへのアクセスを許可されるようにすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="77063-132">If your application needs persistent access to all mailboxes in a Microsoft 365 organization, we recommend that you use the Microsoft Graph APIs which allow access without a user, enable granular permissions and let administrators scope such access to a specific set of mailboxes.</span></span>

<span data-ttu-id="77063-133">アプリケーションを承認してアクセストークンを要求するときには、Outlook リソース Url を含む完全な範囲を指定してください。</span><span class="sxs-lookup"><span data-stu-id="77063-133">Make sure to specify the full scopes, including Outlook resource URLs, when authorizing your application and requesting an access token.</span></span>

| <span data-ttu-id="77063-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="77063-134">Protocol</span></span>  | <span data-ttu-id="77063-135">アクセス許可のスコープ文字列</span><span class="sxs-lookup"><span data-stu-id="77063-135">Permission scope string</span></span> |
|-----------|-------------------------|
| <span data-ttu-id="77063-136">IMAP</span><span class="sxs-lookup"><span data-stu-id="77063-136">IMAP</span></span>      | `https://outlook.office.com/IMAP.AccessAsUser.All` |
| <span data-ttu-id="77063-137">POP</span><span class="sxs-lookup"><span data-stu-id="77063-137">POP</span></span>       | `https://outlook.office.com/POP.AccessAsUser.All`  |
| <span data-ttu-id="77063-138">SMTP 認証</span><span class="sxs-lookup"><span data-stu-id="77063-138">SMTP AUTH</span></span> | `https://outlook.office.com/SMTP.Send`             |

<span data-ttu-id="77063-139">また、 [offline_access](/azure/active-directory/develop/v2-permissions-and-consent#offline_access) スコープを要求することもできます。</span><span class="sxs-lookup"><span data-stu-id="77063-139">In addition, you can request for [offline_access](/azure/active-directory/develop/v2-permissions-and-consent#offline_access) scope.</span></span> <span data-ttu-id="77063-140">ユーザーが offline_access スコープを承認すると、アプリは Microsoft identity platform token endpoint から更新トークンを受け取ることができます。</span><span class="sxs-lookup"><span data-stu-id="77063-140">When a user approves the offline_access scope, your app can receive refresh tokens from the Microsoft identity platform token endpoint.</span></span> <span data-ttu-id="77063-141">更新トークンは長期間の場合があります。</span><span class="sxs-lookup"><span data-stu-id="77063-141">Refresh tokens are long-lived.</span></span> <span data-ttu-id="77063-142">アプリは、新しいアクセストークンを古いものとして期限切れにすることができます。</span><span class="sxs-lookup"><span data-stu-id="77063-142">Your app can get new access tokens as older ones expire.</span></span>

## <a name="authenticate-connection-requests"></a><span data-ttu-id="77063-143">接続要求を認証する</span><span class="sxs-lookup"><span data-stu-id="77063-143">Authenticate connection requests</span></span>

<span data-ttu-id="77063-144">Office 365 メールサーバーへの接続は、 [office 365 の IMAP および POP の電子メール設定](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353)を使用して開始できます。</span><span class="sxs-lookup"><span data-stu-id="77063-144">You can initiate a connection to Office 365 mail servers using the [IMAP and POP email settings for Office 365](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353).</span></span>

### <a name="sasl-xoauth2"></a><span data-ttu-id="77063-145">SASL XOAUTH2</span><span class="sxs-lookup"><span data-stu-id="77063-145">SASL XOAUTH2</span></span>

<span data-ttu-id="77063-146">OAuth の統合には、アプリケーションで、アクセストークンのエンコードと送信に SASL XOAUTH2 format を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="77063-146">OAuth integration with requires your application to use SASL XOAUTH2 format for encoding and transmitting the access token.</span></span> <span data-ttu-id="77063-147">SASL XOAUTH2 は、次の形式でユーザー名とアクセストークンをエンコードします。</span><span class="sxs-lookup"><span data-stu-id="77063-147">SASL XOAUTH2 encodes the username, access token together in the following format:</span></span>

```text
base64("user=" + userName + "^Aauth=Bearer " + accessToken + "^A^A")
```

<span data-ttu-id="77063-148">`^A`**コントロール**  +  **a** () を表し `%x01` ます。</span><span class="sxs-lookup"><span data-stu-id="77063-148">`^A` represents a **Control** + **A** (`%x01`).</span></span>

<span data-ttu-id="77063-149">たとえば、アクセストークンを使用してアクセスする SASL XOAUTH2 形式は次のように `test@contoso.onmicrosoft.com` `EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA` なります。</span><span class="sxs-lookup"><span data-stu-id="77063-149">For example, the SASL XOAUTH2 format to access `test@contoso.onmicrosoft.com` with access token `EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA` is:</span></span>

```text
base64("user=test@contoso.onmicrosoft.com^Aauth=Bearer EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA^A^A")
```

<span data-ttu-id="77063-150">Base64 エンコード後は、次の文字列に変換されます。</span><span class="sxs-lookup"><span data-stu-id="77063-150">After base64 encoding, this translates to the following string.</span></span> <span data-ttu-id="77063-151">読みやすくするために改行が挿入されることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="77063-151">Note that line breaks are inserted for readability.</span></span>

```text
dXNlcj10ZXN0QGNvbnRvc28ub25taWNyb3NvZnQuY29tAWF1dGg9QmVhcmVy
IEV3QkFBbDNCQUFVRkZwVUFvN0ozVmUwYmpMQldaV0NjbFJDM0VvQUEBAQ==
```

### <a name="sasl-xoauth2-authentication-for-shared-mailboxes-in-office-365"></a><span data-ttu-id="77063-152">Office 365 の共有メールボックスのための SASL XOAUTH2 認証</span><span class="sxs-lookup"><span data-stu-id="77063-152">SASL XOAUTH2 authentication for shared mailboxes in Office 365</span></span>

<span data-ttu-id="77063-153">OAuth を使用した共有メールボックスアクセスの場合、アプリケーションはユーザーの代わりにアクセストークンを取得する必要がありますが、SASL XOAUTH2 encoded string の userName フィールドを共有メールボックスの電子メールアドレスに置き換えます。</span><span class="sxs-lookup"><span data-stu-id="77063-153">In case of shared mailbox access using OAuth, application needs to obtain the access token on behalf of a user but replace the userName field in the SASL XOAUTH2 encoded string with the email address of the shared mailbox.</span></span> 

### <a name="imap-protocol-exchange"></a><span data-ttu-id="77063-154">IMAP プロトコルの Exchange</span><span class="sxs-lookup"><span data-stu-id="77063-154">IMAP Protocol Exchange</span></span>

<span data-ttu-id="77063-155">IMAP サーバー接続を認証するには、クライアントは次の形式のコマンドで応答する必要があり `AUTHENTICATE` ます。</span><span class="sxs-lookup"><span data-stu-id="77063-155">To authenticate a IMAP server connection, the client will have to respond with an `AUTHENTICATE` command in the following format:</span></span>

```text
AUTHENTICATE XOAUTH2 <base64 string in XOAUTH2 format>
```

<span data-ttu-id="77063-156">認証に成功した結果として得られるクライアントとサーバー間のメッセージ交換の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="77063-156">Sample client-server message exchange that results in an authentication success:</span></span>

```text
[connection begins]
C: C01 CAPABILITY
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 OK AUTHENTICATE completed.
```

<span data-ttu-id="77063-157">認証エラーが発生するクライアントサーバーのメッセージ交換の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="77063-157">Sample client-server message exchange that results in an authentication failure:</span></span>

```text
[connection begins]
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 NO AUTHENTICATE failed.
```

### <a name="pop-protocol-exchange"></a><span data-ttu-id="77063-158">POP プロトコルの交換</span><span class="sxs-lookup"><span data-stu-id="77063-158">POP Protocol Exchange</span></span>

<span data-ttu-id="77063-159">POP サーバー接続を認証するには、クライアントは `AUTH` コマンドを次の形式で2行に分割して応答する必要があります。</span><span class="sxs-lookup"><span data-stu-id="77063-159">To authenticate a POP server connection, the client will have to respond with an `AUTH` command split into two lines in the following format:</span></span>    

```text 
AUTH XOAUTH2 
<base64 string in XOAUTH2 format>   
``` 

<span data-ttu-id="77063-160">認証に成功した結果として得られるクライアントとサーバー間のメッセージ交換の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="77063-160">Sample client-server message exchange that results in an authentication success:</span></span>    

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

<span data-ttu-id="77063-161">認証エラーが発生するクライアントサーバーのメッセージ交換の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="77063-161">Sample client-server message exchange that results in an authentication failure:</span></span>    

```text 
[connection begins] 
C: AUTH XOAUTH2     
S: +    
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY    
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj   
l0Q2cBAQ=   
S: -ERR Authentication failure: unknown user name or bad password.  
```

### <a name="smtp-protocol-exchange"></a><span data-ttu-id="77063-162">SMTP プロトコルの Exchange</span><span class="sxs-lookup"><span data-stu-id="77063-162">SMTP Protocol Exchange</span></span>

<span data-ttu-id="77063-163">SMTP サーバー接続を認証するには、クライアントは次の形式のコマンドで応答する必要があり `AUTH` ます。</span><span class="sxs-lookup"><span data-stu-id="77063-163">To authenticate a SMTP server connection, the client will have to respond with an `AUTH` command in the following format:</span></span>

```text
AUTH XOAUTH2 <base64 string in XOAUTH2 format>
```

<span data-ttu-id="77063-164">認証に成功した結果として得られるクライアントとサーバー間のメッセージ交換の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="77063-164">Sample client-server message exchange that results in an authentication success:</span></span>

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

<span data-ttu-id="77063-165">認証エラーが発生するクライアントサーバーのメッセージ交換の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="77063-165">Sample client-server message exchange that results in an authentication failure:</span></span>

```text
[connection begins]
C: auth xoauth2
S: 334
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj
l0Q2cBAQ==
S: 535 5.7.3 Authentication unsuccessful [SN2PR00CA0018.namprd00.prod.outlook.com]
```

## <a name="see-also"></a><span data-ttu-id="77063-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="77063-166">See also</span></span>

- [<span data-ttu-id="77063-167">Exchange における認証と EWS</span><span class="sxs-lookup"><span data-stu-id="77063-167">Authentication and EWS in Exchange</span></span>](../exchange-web-services/authentication-and-ews-in-exchange.md)
- [<span data-ttu-id="77063-168">IMAP、POP 接続の設定</span><span class="sxs-lookup"><span data-stu-id="77063-168">IMAP, POP Connection settings</span></span>](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353)
- [<span data-ttu-id="77063-169">インターネットメッセージアクセスプロトコル</span><span class="sxs-lookup"><span data-stu-id="77063-169">Internet Message Access Protocol</span></span>](https://tools.ietf.org/html/rfc3501)
- [<span data-ttu-id="77063-170">Post Office Protocol</span><span class="sxs-lookup"><span data-stu-id="77063-170">Post Office Protocol</span></span>](https://tools.ietf.org/html/rfc1081)
- [<span data-ttu-id="77063-171">認証用の SMTP サービス拡張機能</span><span class="sxs-lookup"><span data-stu-id="77063-171">SMTP Service extension for Authentication</span></span>](https://tools.ietf.org/html/rfc4954)

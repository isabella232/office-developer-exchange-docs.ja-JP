---
title: OAuth を使用して EWS アプリケーションを認証する
manager: sethgros
ms.date: 11/25/2020
ms.audience: Developer
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: EWS Managed API アプリケーションで、OAuth 認証を使用する方法について説明します。
localization_priority: Priority
ms.openlocfilehash: a7b1d2a099cf5f3c95f8453605363de12ff33c54
ms.sourcegitcommit: 843a2e030a94b12aec70c553ca4e06e39ac02d82
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/09/2020
ms.locfileid: "49603828"
---
<!-- markdownlint-disable MD025 -->
# <a name="authenticate-an-ews-application-by-using-oauth"></a>OAuth を使用して EWS アプリケーションを認証する
<!-- markdownlint-enable MD025 -->

EWS Managed API アプリケーションで、OAuth 認証を使用する方法について説明します。

Azure Active Directory が提供する OAuth の認証サービスを使用すると、EWS Managed API アプリケーションが Office 365 での Exchange Online にアクセスできるようにすることができます。 OAuth をアプリケーションで使用するには、次のようにする必要があります。

1. Azure Active Directory に[アプリケーションを登録する](#register-your-application)。
1. トークン サーバーから認証トークンを取得するために、[認証トークンを取得するコードを追加する](#add-code-to-get-an-authentication-token)。
1. 送信する [EWS 要求に認証トークンを追加する](#add-an-authentication-token-to-ews-requests)。

> [!NOTE]
> EWS の OAuth 認証は、Microsoft 365 の一部として Exchange Online でのみ利用可能です。 OAuth を使用する EWS アプリケーションは、Azure Active Directory に登録する必要があります。

この記事のコードを使用するには、次に対するアクセス権が必要です。

- Exchange Online メールボックスを使用している Microsoft 365 アカウント。 Microsoft 365 アカウントをお持ちでない場合は、[Microsoft 365 開発者プログラムにサインアップ](https://developer.microsoft.com/microsoft-365/dev-program)して、無料の Microsoft 365 サブスクリプションを取得できます。
- [.NET 用の Microsoft Authentication Library](/dotnet/api/microsoft.identity.client)。
- [EWS マネージ API](https://github.com/officedev/ews-managed-api)。

Exchange Online で EWS API へのアクセスに使用できる OAuth 許可には 2 つの種類があります。 チュートリアルを続行する前に、使用するアクセス許可の具体的な種類を選択する必要があります。

- **委任されたアクセス許可** は、サインインしているユーザーが存在するアプリで使用します。 これに該当するアプリの場合は、ユーザーまたは管理者がアプリの要求するアクセス許可に同意します。アプリは API 呼び出しを行う時に、サインインしているユーザーとして動作できます。
- **アプリケーションのアクセス許可** は、サインインしているユーザーが存在しないアプリで使用します。たとえば、バックグラウンド サービスやデーモンとして実行され、複数のメールボックスにアクセスできるアプリです。

## <a name="register-your-application"></a>アプリケーションを登録する

OAuth を使用するには、アプリケーションに Azure Active Directory が発行したアプリケーション ID が必要です。 このチュートリアルでは、アプリケーションがコンソール アプリケーションであることが前提となるので、アプリケーションを Azure Active Directory にパブリック クライアントとして登録する必要があります。 アプリケーションの登録は、Azure Active Directory 管理センターか、Microsoft Graph を使用して行うことができます。

1. ブラウザーを開き、[Azure Active Directory 管理センター](https://aad.portal.azure.com)へ移動して、**個人用アカウント** (別名: Microsoft アカウント)、または **職場/学校アカウント** を使用してログインします。

1. 左側のナビゲーションで **[Azure Active Directory]** を選択し、それから **[管理]** で **[アプリの登録]** を選択します。

1. **[新規登録]** を選択します。 
            **[アプリケーションを登録]** ページで、次のように値を設定します。

    - **[名前]** をアプリのフレンドリ名に設定します。
    - **[サポートされているアカウントの種類]** をシナリオに合った選択肢に設定します。
    - **リダイレクト URI** については、ドロップダウンを **[パブリック クライアント (モバイルとデスクトップ)]** に変更し、値を `urn:ietf:wg:oauth:2.0:oob` に設定します。

1. **[登録]** を選択します。 次のページで、**アプリケーション (クライアント) ID** と **ディレクトリ (テナント) ID** の値をコピーして保存します。これらの値は、後ほど必要になります。

### <a name="configure-for-delegated-authentication"></a>委任された認証の構成

アプリケーションが委任された認証を使用する場合は、これ以上の構成は必要ありません。 [[Microsoft ID プラットフォーム]](/azure/active-directory/develop/v2-overview) では、アプリが動的にアクセス許可を要求できるようになっているので、アプリの登録時にアクセス許可を事前に構成する必要がありません。 ただし、いくつかのシナリオにおいては ([代理 (On-Behalf-Of) フロー](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) など)、アクセス許可の事前構成が必要です。 EWS のアクセス許可を事前に構成するには、次の手順を実行します。

1. 左側のナビゲーションの **[管理]** で **[マニフェスト]** を選択します。

1. マニフェスト内で `requiredResourceAccess` プロパティを見つけ、角かっこ (`[]`) の中に以下を追加します。

    ```json
    {
        "resourceAppId": "00000002-0000-0ff1-ce00-000000000000",
        "resourceAccess": [
            {
                "id": "3b5f3d61-589b-4a3c-a359-5dd4b5ee5bd5",
                "type": "Scope"
            }
        ]
    }
    ```

1. **[保存]** を選択します。

1. **[管理]** で、**[API のアクセス許可]** を選択します。 **EWS.AccessAsUser.All** アクセス許可が表示されていることを確認します。

### <a name="configure-for-app-only-authentication"></a>アプリ専用の認証の構成

アプリケーションのアクセス許可を使用するには、次の追加の手順を実行します。

1. 左側のナビゲーションの **[管理]** で **[マニフェスト]** を選択します。

1. マニフェスト内で `requiredResourceAccess` プロパティを見つけ、角かっこ (`[]`) の中に以下を追加します。

    ```json
    {
        "resourceAppId": "00000002-0000-0ff1-ce00-000000000000",
        "resourceAccess": [
            {
                "id": "dc890d15-9560-4a4c-9b7f-a736ec74ec40",
                "type": "Role"
            }
        ]
    }
    ```

1. **[保存]** を選択します。

1. **[管理]** で、**[API のアクセス許可]** を選択します。 **full_access_as_app** アクセス許可が表示されていることを確認します。

1. **[組織に対して管理者の同意を与える]** を選択して、同意ダイアログに同意します。

1. 左側のナビゲーション ウィンドウの **[管理]** で、**[証明書とシークレット]** を選択します。

1. **[新しいクライアント シークレット]** を選択して、短い説明を入力して **[追加]** を選択します。

1. 新しく追加したシークレットの **[値]** をコピーして保存します。この値は後で必要になります。

## <a name="add-code-to-get-an-authentication-token"></a>認証トークンを取得するコードを追加する

次のコード スニペットは、Microsoft Authentication Library を使用して、委任されたアクセス許可とアプリケーションのアクセス許可の認証トークンを取得する方法を示しています。 これらのスニペットは、認証要求を行うために必要な情報がアプリケーションの **App.config** ファイルに格納されていると仮定します。 これらの例では、エラー チェックは含まれません。完全なコードについては、[コード サンプル](#code-samples)を参照してください。

### <a name="get-a-token-with-delegated-auth"></a>委任された認証を使用してトークンを取得する

```cs
// Using Microsoft.Identity.Client 4.22.0

// Configure the MSAL client to get tokens
var pcaOptions = new PublicClientApplicationOptions
{
    ClientId = ConfigurationManager.AppSettings["appId"],
    TenantId = ConfigurationManager.AppSettings["tenantId"]
};

var pca = PublicClientApplicationBuilder
    .CreateWithApplicationOptions(pcaOptions).Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "https://outlook.office365.com/EWS.AccessAsUser.All" };

// Make the interactive token request
var authResult = await pca.AcquireTokenInteractive(ewsScopes).ExecuteAsync();
```

### <a name="get-a-token-with-app-only-auth"></a>アプリ専用の認証を使用してトークンを取得する

```cs
// Using Microsoft.Identity.Client 4.22.0
var cca = ConfidentialClientApplicationBuilder
    .Create(ConfigurationManager.AppSettings["appId"])
    .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"])
    .WithTenantId(ConfigurationManager.AppSettings["tenantId"])
    .Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "https://outlook.office365.com/.default" };

//Make the token request
var authResult = await cca.AcquireTokenForClient(ewsScopes).ExecuteAsync();
```

## <a name="add-an-authentication-token-to-ews-requests"></a>EWS 要求に認証トークンを追加します。

**AuthenticationResult** オブジェクトを受信すると、**AccessToken** プロパティを使用して、トークン サービスによって発行されるトークンを取得できます。

```cs
// Configure the ExchangeService with the access token
var ewsClient = new ExchangeService();
ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
```

アプリケーションのアクセス許可を使用するには、アクセスするメールボックスを明示的に偽装する必要もあります。

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a>コード サンプル

### <a name="delegated-authentication"></a>委任された認証

以下は、委任された認証を使用した OAuth 認証された EWS 要求の作成方法を示す完全なコード サンプルです。

```cs
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;
using System;
using System.Configuration;

namespace EwsOAuth
{
    class Program
    {
        static async System.Threading.Tasks.Task Main(string[] args)
        {
            // Using Microsoft.Identity.Client 4.22.0

            // Configure the MSAL client to get tokens
            var pcaOptions = new PublicClientApplicationOptions
            {
                ClientId = ConfigurationManager.AppSettings["appId"],
                TenantId = ConfigurationManager.AppSettings["tenantId"]
            };

            var pca = PublicClientApplicationBuilder
                .CreateWithApplicationOptions(pcaOptions).Build();

            // The permission scope required for EWS access
            var ewsScopes = new string[] { "https://outlook.office365.com/EWS.AccessAsUser.All" };

            try
            {
                // Make the interactive token request
                var authResult = await pca.AcquireTokenInteractive(ewsScopes).ExecuteAsync();

                // Configure the ExchangeService with the access token
                var ewsClient = new ExchangeService();
                ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
                ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);

                // Make an EWS call
                var folders = ewsClient.FindFolders(WellKnownFolderName.MsgFolderRoot, new FolderView(10));
                foreach(var folder in folders)
                {
                    Console.WriteLine($"Folder: {folder.DisplayName}");
                }
            }
            catch (MsalException ex)
            {
                Console.WriteLine($"Error acquiring access token: {ex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex}");
            }

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
            }
        }
    }
}
```

### <a name="app-only-authentication"></a>アプリ専用の認証

以下は、アプリ専用の認証を使用した OAuth 認証された EWS 要求の作成方法を示す完全なコード サンプルです。

> [!NOTE]
> 偽装を使用するときには、必ず X-AnchorMailbox 要求ヘッダーを使用し、偽装メールボックスの SMTP アドレスに設定する必要があります。

```cs
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;
using System;
using System.Configuration;

namespace EwsOAuth
{
    class Program
    {
        static async System.Threading.Tasks.Task Main(string[] args)
        {
            // Using Microsoft.Identity.Client 4.22.0
            var cca = ConfidentialClientApplicationBuilder
                .Create(ConfigurationManager.AppSettings["appId"])
                .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"])
                .WithTenantId(ConfigurationManager.AppSettings["tenantId"])
                .Build();

            var ewsScopes = new string[] { "https://outlook.office365.com/.default" };

            try
            {
                var authResult = await cca.AcquireTokenForClient(ewsScopes)
                    .ExecuteAsync();

                // Configure the ExchangeService with the access token
                var ewsClient = new ExchangeService();
                ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
                ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
                ewsClient.ImpersonatedUserId =
                    new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "meganb@contoso.onmicrosoft.com");

                //Include x-anchormailbox header
                ewsClient.HttpHeaders.Add("X-AnchorMailbox", "meganb@contoso.onmicrosoft.com");

                // Make an EWS call
                var folders = ewsClient.FindFolders(WellKnownFolderName.MsgFolderRoot, new FolderView(10));
                foreach(var folder in folders)
                {
                    Console.WriteLine($"Folder: {folder.DisplayName}");
                }
            }
            catch (MsalException ex)
            {
                Console.WriteLine($"Error acquiring access token: {ex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex}");
            }

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
            }
        }
    }
}
```

どちらの場合も、サンプル コードには次のエントリを持つ **App.config** ファイルが必要です。

```xml
<?xml version="1.0" encoding="utf-8" ?>
<configuration>
  <startup>
    <supportedRuntime version="v4.0" sku=".NETFramework,Version=v4.7.2" />
  </startup>
  <appSettings>
    <!-- The application ID from your app registration -->
    <add key="appId" value="YOUR_APP_ID_HERE" />
    <!-- The tenant ID copied from your app registration -->
    <add key="tenantId" value="YOUR_TENANT_ID_HERE"/>
    <!-- The application's client secret from your app registration. Needed for application permission access -->
    <add key="clientSecret" value="YOUR_CLIENT_SECRET_HERE"/>
  </appSettings>
</configuration>
```

## <a name="see-also"></a>関連項目

- [Exchange における認証と EWS](authentication-and-ews-in-exchange.md)

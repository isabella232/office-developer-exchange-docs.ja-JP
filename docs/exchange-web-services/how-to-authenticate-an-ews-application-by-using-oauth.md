---
title: OAuth を使用して EWS アプリケーションを認証する
manager: sethgros
ms.date: 05/17/2019
ms.audience: Developer
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: EWS Managed API アプリケーションで、OAuth 認証を使用する方法について説明します。
localization_priority: Priority
ms.openlocfilehash: 795cbcc3dd1c895850086ebf0e23da905c1c99b7
ms.sourcegitcommit: 636c05a929279812c6ef87d75b01c166a4a05584
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/26/2020
ms.locfileid: "47254966"
---
<!-- markdownlint-disable MD025 -->
# <a name="authenticate-an-ews-application-by-using-oauth"></a>OAuth を使用して EWS アプリケーションを認証する
<!-- markdownlint-enable MD025 -->

EWS Managed API アプリケーションで、OAuth 認証を使用する方法について説明します。

Azure Active Directory が提供する OAuth の認証サービスを使用すると、EWS Managed API アプリケーションが Office 365 での Exchange Online にアクセスできるようにすることができます。 OAuth をアプリケーションで使用するには、次のようにする必要があります。

1. Azure Active Directory に[アプリケーションを登録する](#register-your-application)。

2. トークン サーバーから認証トークンを取得するために、[認証トークンを取得するコードを追加する](#add-code-to-get-an-authentication-token)。

3. 送信する [EWS 要求に認証トークンを追加する](#add-an-authentication-token-to-ews-requests)。

> [!NOTE]
> EWS の OAuth 認証は、Office 365 の一部として Exchange でのみ利用可能です。 OAuth を使用する EWS アプリケーションは、Azure Active Directory に登録する必要があります。

この記事のコードを使用するには、次に対するアクセス権が必要です。

- Exchange Online メールボックスを使用している Office 365 アカウント。 Office 365 アカウントをお持ちでない場合は、[Office 365 開発者プログラムに新規登録](https://developer.microsoft.com/office/dev-program)して、無料の Office 365 サブスクリプションを取得できます。

- [.NET 用の Microsoft Authentication Library](/dotnet/api/microsoft.identity.client?view=azure-dotnet)。

- [EWS マネージ API](https://github.com/officedev/ews-managed-api)。


Exchange Online で EWS API へのアクセスに使用できる OAuth 許可には 2 つの種類があります。 チュートリアルを続行する前に、使用するアクセス許可の具体的な種類を選択する必要があります。

* **委任されたアクセス許可**は、サインインしているユーザーが存在するアプリで使用します。 これに該当するアプリの場合は、ユーザーまたは管理者がアプリの要求するアクセス許可に同意します。アプリは API 呼び出しを行う時に、サインインしているユーザーとして動作できます。 
* **アプリケーションのアクセス許可**は、サインインしているユーザーが存在しないアプリで使用します。たとえば、バックグラウンド サービスやデーモンとして実行され、複数のメールボックスにアクセスできるアプリです。

## <a name="register-your-application"></a>アプリケーションを登録する

OAuth を使用するには、アプリケーションに Azure Active Directory が発行したアプリケーション ID が必要です。 このチュートリアルでは、アプリケーションがコンソール アプリケーションであることが前提となるので、アプリケーションを Azure Active Directory にパブリック クライアントとして登録する必要があります。

1. ブラウザーを開き、[Azure Active Directory 管理センター](https://aad.portal.azure.com)へ移動して、**個人用アカウント** (別名: Microsoft アカウント)、または**職場/学校アカウント**を使用してログインします。

1. 左側のナビゲーションで **[Azure Active Directory]** を選択し、それから **[管理]** で **[アプリの登録]** を選択します。

1. **[新規登録]** を選択します。 
            **[アプリケーションを登録]** ページで、次のように値を設定します。

    - **[名前]** をアプリのフレンドリ名に設定します。
    - **[サポートされているアカウントの種類]** をシナリオに合った選択肢に設定します。
    - **リダイレクト URI** については、ドロップダウンを **[パブリック クライアント (モバイルとデスクトップ)]** に変更し、値を `urn:ietf:wg:oauth:2.0:oob` に設定します。

1. **[登録]** を選択します。 次のページで、**[アプリケーション (クライアント) ID]** の値をコピーして保存します。この値は後で必要になります。

1. 左側のナビゲーションの **[管理]** で **[API のアクセス許可]** を選択します。 

1. **[アクセス許可を追加]** を選択します。 **[API アクセス許可を要求する]** ページの **[サポートされているレガシ API]** で、**[Exchange]** を選択します。 

1. 委任されたアクセス許可を使用するには、**[委任されたアクセス許可]** を選択して、**[EWS]** で **[EWS.AccessAsUser.All]** を選択します。 **[アクセス許可を追加する]** をクリックします。 

アプリケーションのアクセス許可を使用するには、次の追加の手順を実行します。

1. **[アプリケーションのアクセス許可]** を選択して、次に **[full_access_as_app]** を選択します。 **[アクセス許可を追加する]** をクリックします。

1. **[組織に対して管理者の同意を与える]** を選択して、同意ダイアログに同意します。 

1. 左側のナビゲーション ウィンドウの **[管理]** で、**[証明書とシークレット]** を選択します。 

1. **[新しいクライアント シークレット]** を選択して、短い説明を入力して **[追加]** を選択します。

1. 新しく追加したシークレットの **[値]** をコピーして保存します。この値は後で必要になります。 

## <a name="add-code-to-get-an-authentication-token"></a>認証トークンを取得するコードを追加する

次のコード スニペットは、Microsoft Authentication Library を使用して、委任されたアクセス許可とアプリケーションのアクセス許可の認証トークンを取得する方法を示しています。 これらのスニペットは、認証要求を行うために必要な情報がアプリケーションの **App.config** ファイルに格納されていると仮定します。 これらの例では、エラー チェックは含まれません。完全なコードについては、[コード サンプル](#code-samples)を参照してください。

### <a name="delegated-permissions"></a>委任されたアクセス許可

```cs
// Configure the MSAL client to get tokens
var pcaOptions = new PublicClientApplicationOptions
{
    ClientId = ConfigurationManager.AppSettings["appId"],
    TenantId = ConfigurationManager.AppSettings["tenantId"]
};

var pca = PublicClientApplicationBuilder
    .CreateWithApplicationOptions(pcaOptions).Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "https://outlook.office.com/EWS.AccessAsUser.All" };

// Make the interactive token request
var authResult = await pca.AcquireTokenInteractive(ewsScopes).ExecuteAsync();
```

### <a name="application-permissions"></a>アプリケーションのアクセス許可

```cs
// Configure the MSAL client to get tokens
var app = ConfidentialClientApplicationBuilder
    .Create(ConfigurationManager.AppSettings["appId"])
    .WithAuthority(AzureCloudInstance.AzurePublic, ConfigurationManager.AppSettings["tenantId"])
    .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"]).Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "https://outlook.office.com/.default" };

//Make the token request
AuthenticationResult authResult = await app.AcquireTokenForClient(ewsScopes).ExecuteAsync();

```

## <a name="add-an-authentication-token-to-ews-requests"></a>EWS 要求に認証トークンを追加します。

**AuthenticationResult** オブジェクトを受信すると、**AccessToken** プロパティを使用して、トークン サービスによって発行されるトークンを取得できます。

```cs
// Configure the ExchangeService with the access token
var ewsClient = new ExchangeService();
ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
```

アプリケーションのアクセス許可を使用するには、アクセスしたいメールボックスを明示的に偽装する必要もあります。 

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a>コード サンプル

### <a name="delegated-permissions"></a>委任されたアクセス許可

以下の完全なコード サンプルでは、委任されたアクセス許可を使用して OAuth 認証が行われる EWS 要求を示します。

```cs
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;
using System;
using System.Configuration;

namespace EwsOAuth
{
    class Program
    {
        static void Main(string[] args)
        {
            MainAsync(args).Wait();

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
            }
        }

        static async System.Threading.Tasks.Task MainAsync(string[] args)
        {
            // Configure the MSAL client to get tokens
            var pcaOptions = new PublicClientApplicationOptions
            {
                ClientId = ConfigurationManager.AppSettings["appId"],
                TenantId = ConfigurationManager.AppSettings["tenantId"]
            };

            var pca = PublicClientApplicationBuilder
                .CreateWithApplicationOptions(pcaOptions).Build();

            var ewsScopes = new string[] { "https://outlook.office.com/EWS.AccessAsUser.All" };

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
                Console.WriteLine($"Error acquiring access token: {ex.ToString()}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.ToString()}");
            }
        }
    }
}
```

### <a name="application-permissions"></a>アプリケーションのアクセス許可

以下の完全なコード サンプルでは、アプリケーションのアクセス許可を使用して OAuth 認証が行われる EWS 要求を示します。

> [!NOTE]
> 偽装を使用するとき、必ず X-AnchorMailbox 要求ヘッダーを使用し、偽装メールボックスの SMTP に設定する必要があります。

```cs
using System;
using System.Configuration;
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;

namespace ews_oauth_samples
{
    class Program
    {
        static void Main(string[] args)
        {
            MainAsync(args).Wait();

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
            }
        }
        
        static async System.Threading.Tasks.Task MainAsync(string[] args)
        {
            // Configure the MSAL client to get tokens
            var ewsScopes = new string[] { "https://outlook.office.com/.default" };

            var app = ConfidentialClientApplicationBuilder.Create(ConfigurationManager.AppSettings["appId"])
                .WithAuthority(AzureCloudInstance.AzurePublic, ConfigurationManager.AppSettings["tenantId"])
                .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"])
                .Build();

            AuthenticationResult result = null;

            try
            {
                // Make the interactive token request
                result = await app.AcquireTokenForClient(ewsScopes)
                    .ExecuteAsync();

                // Configure the ExchangeService with the access token
                var ewsClient = new ExchangeService();
                ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
                ewsClient.Credentials = new OAuthCredentials(result.AccessToken);

                //Impersonate the mailbox you'd like to access.
                ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");

                //Include x-anchormailbox header
                ewsClient.HttpHeaders.Add("X-AnchorMailbox", "test@demotenant.onmicrosoft.com");

                // Make an EWS call
                var folders = ewsClient.FindFolders(WellKnownFolderName.MsgFolderRoot, new FolderView(10));
                foreach (var folder in folders)
                {
                    Console.WriteLine($"Folder: {folder.DisplayName}");
                }
            }
            catch (MsalException ex)
            {
                Console.WriteLine($"Error acquiring access token: {ex.ToString()}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.ToString()}");
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
    <!-- If you registered your app to support only users in your organization, change the value
           of this key to your tenant ID -->
    <add key="tenantId" value="common"/>
    <!-- The application's client secret from your app registration. Needed for application permission access -->
    <add key="clientSecret" value="YOUR_CLIENT_SECRET_HERE"/>
  </appSettings>
</configuration>
```

## <a name="see-also"></a>関連項目

- [Exchange における認証と EWS](authentication-and-ews-in-exchange.md)

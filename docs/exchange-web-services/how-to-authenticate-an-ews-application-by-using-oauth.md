---
title: OAuth を使用して EWS アプリケーションを認証する
manager: sethgros
ms.date: 05/17/2019
ms.audience: Developer
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: EWS Managed API アプリケーションで、OAuth 認証を使用する方法について説明します。
localization_priority: Priority
ms.openlocfilehash: e2bcb339ddac51b888660b6f982a8377591b1a29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528252"
---
<!-- markdownlint-disable MD025 -->
# <a name="authenticate-an-ews-application-by-using-oauth"></a>OAuth を使用して EWS アプリケーションを認証する
<!-- markdownlint-enable MD025 -->

EWS Managed API アプリケーションで、OAuth 認証を使用する方法について説明します。

Azure Active Directory によって提供される OAuth 認証サービスを使用して、EWS マネージ API アプリケーションが Office 365 の Exchange Online にアクセスできるようにすることができます。 OAuth をアプリケーションで使用するには、次のようにする必要があります。

1. Azure Active Directory に[アプリケーションを登録する](#register-your-application)。

2. トークン サーバーから認証トークンを取得するために、[認証トークンを取得するコードを追加する](#add-code-to-get-an-authentication-token)。

3. 送信する [EWS 要求に認証トークンを追加する](#add-an-authentication-token-to-ews-requests)。

> [!NOTE]
> EWS の OAuth 認証は、Office 365 の一部として Exchange でのみ利用可能です。 OAuth を使用する EWS アプリケーションは、Azure Active Directory に登録する必要があります。

この記事のコードを使用するには、次に対するアクセス権が必要です。

- Exchange Online メールボックスを含む Office 365 アカウント。 Office 365 アカウントを持っていない場合は、 [office 365 開発者プログラムにサインアップ](https://developer.microsoft.com/office/dev-program)して、無料の office 365 サブスクリプションを取得することができます。

- [.Net 用の Microsoft 認証ライブラリ](/dotnet/api/microsoft.identity.client?view=azure-dotnet)。

- [EWS マネージ API](https://github.com/officedev/ews-managed-api)。


Exchange Online で EWS Api にアクセスするために使用できる OAuth アクセス許可には2種類あります。 チュートリアルを開始する前に、使用する特定のアクセス許可の種類を選択する必要があります。

* **委任されたアクセス許可**は、サインインしているユーザーが存在するアプリで使用します。 これらのアプリの場合、ユーザーまたは管理者は、API 呼び出しを行うときに、アプリが要求するアクセス許可とアプリがサインインしているユーザーとして機能する権限を同意ます。 
* **アプリケーションのアクセス許可**は、サインインしているユーザーが存在しない状態で実行されるアプリで使用されます。たとえば、バックグラウンドサービスまたはデーモンとして実行され、複数のメールボックスにアクセスできるアプリがあります。

## <a name="register-your-application"></a>アプリケーションを登録する

OAuth を使用するには、アプリケーションが Azure Active Directory によって発行されたアプリケーション ID を持っている必要があります。 このチュートリアルでは、アプリケーションがコンソールアプリケーションであることを前提としているため、アプリケーションを Azure Active Directory を使用して公開クライアントとして登録する必要があります。

1. ブラウザーを開き、[Azure Active Directory 管理センター](https://aad.portal.azure.com)へ移動して、**個人用アカウント** (別名: Microsoft アカウント)、または**職場/学校アカウント**を使用してログインします。

1. 左側のナビゲーションで **[Azure Active Directory]** を選択し、それから **[管理]** で **[アプリの登録]** を選択します。

1. **[新規登録]** を選択します。 
            **[アプリケーションを登録]** ページで、次のように値を設定します。

    - **名前**をアプリのフレンドリ名に設定します。
    - **サポートされているアカウントの種類**を、シナリオに適した選択肢に設定します。
    - **リダイレクト URI**の場合は、ドロップダウンを [**パブリッククライアント (モバイル & デスクトップ)** ] に変更し、値をに設定し `urn:ietf:wg:oauth:2.0:oob` ます。

1. **[登録]** を選択します。 次のページで、**アプリケーション (クライアント) ID**の値をコピーして保存します。後で必要になります。

1. 左側のナビゲーションで、[**管理**] の下にある [ **API のアクセス許可**] を選択します。 

1. [**アクセス許可の追加**] を選択します。 [ **API アクセス許可の要求**] ページで、[**サポートされているレガシ api**] の下の [ **Exchange** ] を選択します。 

1. 委任されたアクセス許可を使用するには、[委任された**アクセス許可**] を選択してから、[ **EWS** **EWS**の下に directory.accessasuser.all。 [**アクセス許可の追加**] をクリックします。 

アプリケーションのアクセス許可を使用するには、次の追加の手順に従います。

1. [**アプリケーションの権限**] を選択し、[ **full_access_as_app**] を選択します。 [**アクセス許可の追加**] をクリックします。

1. [**組織に対する管理者の同意を許可**する] を選択し、同意ダイアログを承諾します。 

1. [**管理**] の下にある左側のナビゲーションで、[**証明書 & シークレット**] を選択します。 

1. [**新しいクライアントシークレット**] を選択し、簡単な説明を入力して [**追加**] を選択します。

1. 新しく追加したクライアントシークレットの**値**をコピーして保存し、後で必要になります。 

## <a name="add-code-to-get-an-authentication-token"></a>認証トークンを取得するコードを追加する

次のコードスニペットは、Microsoft 認証ライブラリを使用して、委任されたアクセス許可とアプリケーションのアクセス許可の認証トークンを取得する方法を示しています。 これらのスニペットは、認証要求を行うために必要な情報が、**アプリケーションの app.config**ファイルに格納されていることを前提としています。 これらの例には、エラーチェックは含まれていません。完全なコードについては、[コードサンプル](#code-samples)を参照してください。

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

//Make the toekn request
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

アプリケーションのアクセス許可を使用するには、アクセスするメールボックスを明示的に偽装する必要もあります。 

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a>コード サンプル

### <a name="delegated-permissions"></a>委任されたアクセス許可

次に示す完全なコードサンプルは、委任されたアクセス許可を使用して OAuth 認証された EWS 要求を作成する方法を示しています。

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

以下に、アプリケーションのアクセス許可を使用して OAuth 認証された EWS 要求を作成する方法を示す完全なコードサンプルを示します。

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

どちらの場合も、サンプルコードでは、次のエントリを持つ**app.config**ファイルが必要です。

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

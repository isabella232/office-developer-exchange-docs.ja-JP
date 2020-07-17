---
title: OAuth を使用して EWS アプリケーションを認証する
manager: sethgros
ms.date: 05/17/2019
ms.audience: Developer
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: EWS Managed API アプリケーションで、OAuth 認証を使用する方法について説明します。
localization_priority: Priority
ms.openlocfilehash: 0375095faac918859354da026118ea4ccfd6792b
ms.sourcegitcommit: eeda51cb037aa25566adb293f25574674fdb2d9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/01/2020
ms.locfileid: "45012567"
---
<!-- markdownlint-disable MD025 -->
# <a name="authenticate-an-ews-application-by-using-oauth"></a><span data-ttu-id="e5c78-103">OAuth を使用して EWS アプリケーションを認証する</span><span class="sxs-lookup"><span data-stu-id="e5c78-103">Authenticate an EWS application by using OAuth</span></span>
<!-- markdownlint-enable MD025 -->

<span data-ttu-id="e5c78-104">EWS Managed API アプリケーションで、OAuth 認証を使用する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="e5c78-104">Learn how to use OAuth authentication with your EWS Managed API applications.</span></span>

<span data-ttu-id="e5c78-105">Azure Active Directory によって提供される OAuth 認証サービスを使用して、EWS マネージ API アプリケーションが Office 365 の Exchange Online にアクセスできるようにすることができます。</span><span class="sxs-lookup"><span data-stu-id="e5c78-105">You can use the OAuth authentication service provided by Azure Active Directory to enable your EWS Managed API applications to access Exchange Online in Office 365.</span></span> <span data-ttu-id="e5c78-106">OAuth をアプリケーションで使用するには、次のようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="e5c78-106">To use OAuth with your application you will need to:</span></span>

1. <span data-ttu-id="e5c78-107">Azure Active Directory に[アプリケーションを登録する](#register-your-application)。</span><span class="sxs-lookup"><span data-stu-id="e5c78-107">[Register your application](#register-your-application) with Azure Active Directory.</span></span>

2. <span data-ttu-id="e5c78-108">トークン サーバーから認証トークンを取得するために、[認証トークンを取得するコードを追加する](#add-code-to-get-an-authentication-token)。</span><span class="sxs-lookup"><span data-stu-id="e5c78-108">[Add code to get an authentication token](#add-code-to-get-an-authentication-token) to get an authentication token from a token server.</span></span>

3. <span data-ttu-id="e5c78-109">送信する [EWS 要求に認証トークンを追加する](#add-an-authentication-token-to-ews-requests)。</span><span class="sxs-lookup"><span data-stu-id="e5c78-109">[Add an authentication token to EWS requests](#add-an-authentication-token-to-ews-requests) that you send.</span></span>

> [!NOTE]
> <span data-ttu-id="e5c78-110">EWS の OAuth 認証は、Office 365 の一部として Exchange でのみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="e5c78-110">OAuth authentication for EWS is only available in Exchange as part of Office 365.</span></span> <span data-ttu-id="e5c78-111">OAuth を使用する EWS アプリケーションは、Azure Active Directory に登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e5c78-111">EWS applications that use OAuth must be registered with Azure Active Directory.</span></span>

<span data-ttu-id="e5c78-112">この記事のコードを使用するには、次に対するアクセス権が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5c78-112">To use the code in this article, you will need to have access to the following:</span></span>

- <span data-ttu-id="e5c78-113">Exchange Online メールボックスを含む Office 365 アカウント。</span><span class="sxs-lookup"><span data-stu-id="e5c78-113">An Office 365 account with an Exchange Online mailbox.</span></span> <span data-ttu-id="e5c78-114">Office 365 アカウントを持っていない場合は、 [office 365 開発者プログラムにサインアップ](https://developer.microsoft.com/office/dev-program)して、無料の office 365 サブスクリプションを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="e5c78-114">If you do not have an Office 365 account, you can [sign up for the Office 365 Developer Program](https://developer.microsoft.com/office/dev-program) to get a free Office 365 subscription.</span></span>

- <span data-ttu-id="e5c78-115">[.Net 用の Microsoft 認証ライブラリ](/dotnet/api/microsoft.identity.client?view=azure-dotnet)。</span><span class="sxs-lookup"><span data-stu-id="e5c78-115">The [Microsoft Authentication Library for .NET](/dotnet/api/microsoft.identity.client?view=azure-dotnet).</span></span>

- <span data-ttu-id="e5c78-116">[EWS マネージ API](https://github.com/officedev/ews-managed-api)。</span><span class="sxs-lookup"><span data-stu-id="e5c78-116">The [EWS Managed API](https://github.com/officedev/ews-managed-api).</span></span>


<span data-ttu-id="e5c78-117">Exchange Online で EWS Api にアクセスするために使用できる OAuth アクセス許可には2種類あります。</span><span class="sxs-lookup"><span data-stu-id="e5c78-117">There are two types of OAuth permissions that can be used to access EWS APIs in Exchange Online.</span></span> <span data-ttu-id="e5c78-118">チュートリアルを開始する前に、使用する特定のアクセス許可の種類を選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e5c78-118">Before you proceed with the tutorial, you will need to choose the specific permission type to use.</span></span>

* <span data-ttu-id="e5c78-119">**委任されたアクセス許可**は、サインインしているユーザーが存在するアプリで使用します。</span><span class="sxs-lookup"><span data-stu-id="e5c78-119">**Delegated permissions** are used by apps that have a signed-in user present.</span></span> <span data-ttu-id="e5c78-120">これらのアプリの場合、ユーザーまたは管理者は、API 呼び出しを行うときに、アプリが要求するアクセス許可とアプリがサインインしているユーザーとして機能する権限を同意ます。</span><span class="sxs-lookup"><span data-stu-id="e5c78-120">For these apps, either the user or an administrator consents to the permissions that the app requests and the app can act as the signed-in user when making API calls.</span></span> 
* <span data-ttu-id="e5c78-121">**アプリケーションのアクセス許可**は、サインインしているユーザーが存在しない状態で実行されるアプリで使用されます。たとえば、バックグラウンドサービスまたはデーモンとして実行され、複数のメールボックスにアクセスできるアプリがあります。</span><span class="sxs-lookup"><span data-stu-id="e5c78-121">**Application permissions** are used by apps that run without a signed-in user present; for example, apps that run as background services or daemons and can access multiple mailboxes.</span></span>

## <a name="register-your-application"></a><span data-ttu-id="e5c78-122">アプリケーションを登録する</span><span class="sxs-lookup"><span data-stu-id="e5c78-122">Register your application</span></span>

<span data-ttu-id="e5c78-123">OAuth を使用するには、アプリケーションが Azure Active Directory によって発行されたアプリケーション ID を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e5c78-123">To use OAuth, an application must have an application ID issued by Azure Active Directory.</span></span> <span data-ttu-id="e5c78-124">このチュートリアルでは、アプリケーションがコンソールアプリケーションであることを前提としているため、アプリケーションを Azure Active Directory を使用して公開クライアントとして登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e5c78-124">In this tutorial, it is assumed that the application is a console application, so you need to register your application as a public client with Azure Active Directory.</span></span>

1. <span data-ttu-id="e5c78-125">ブラウザーを開き、[Azure Active Directory 管理センター](https://aad.portal.azure.com)へ移動して、**個人用アカウント** (別名: Microsoft アカウント)、または**職場/学校アカウント**を使用してログインします。</span><span class="sxs-lookup"><span data-stu-id="e5c78-125">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com) and login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="e5c78-126">左側のナビゲーションで **[Azure Active Directory]** を選択し、それから **[管理]** で **[アプリの登録]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e5c78-126">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage**.</span></span>

1. <span data-ttu-id="e5c78-127">**[新規登録]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e5c78-127">Select **New registration**.</span></span> <span data-ttu-id="e5c78-128">
            \**[アプリケーションを登録]\*\* ページで、次のように値を設定します。</span><span class="sxs-lookup"><span data-stu-id="e5c78-128">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="e5c78-129">**名前**をアプリのフレンドリ名に設定します。</span><span class="sxs-lookup"><span data-stu-id="e5c78-129">Set **Name** to a friendly name for your app.</span></span>
    - <span data-ttu-id="e5c78-130">**サポートされているアカウントの種類**を、シナリオに適した選択肢に設定します。</span><span class="sxs-lookup"><span data-stu-id="e5c78-130">Set **Supported account types** to the choice that makes sense for your scenario.</span></span>
    - <span data-ttu-id="e5c78-131">**リダイレクト URI**の場合は、ドロップダウンを [**パブリッククライアント (モバイル & デスクトップ)** ] に変更し、値をに設定し `urn:ietf:wg:oauth:2.0:oob` ます。</span><span class="sxs-lookup"><span data-stu-id="e5c78-131">For **Redirect URI**, change the dropdown to **Public client (mobile & desktop)** and set the value to `urn:ietf:wg:oauth:2.0:oob`.</span></span>

1. <span data-ttu-id="e5c78-132">**[登録]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e5c78-132">Choose **Register**.</span></span> <span data-ttu-id="e5c78-133">次のページで、**アプリケーション (クライアント) ID**の値をコピーして保存します。後で必要になります。</span><span class="sxs-lookup"><span data-stu-id="e5c78-133">On the next page, copy the value of the **Application (client) ID** and save it, you will need it later.</span></span>

1. <span data-ttu-id="e5c78-134">左側のナビゲーションで、[**管理**] の下にある [ **API のアクセス許可**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="e5c78-134">Select **API permissions** in the left-hand navigation under **Manage**.</span></span> 

1. <span data-ttu-id="e5c78-135">[**アクセス許可を追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="e5c78-135">Select **Add a permission**.</span></span> <span data-ttu-id="e5c78-136">[ **API アクセス許可の要求**] ページで、[**サポートされているレガシ api**] の下の [ **Exchange** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="e5c78-136">On the **Request API permissions** page, select **Exchange** under **Supported legacy APIs**.</span></span> 

1. <span data-ttu-id="e5c78-137">委任されたアクセス許可を使用するには、[委任された**アクセス許可**] を選択してから、[ **EWS** **EWS**の下に directory.accessasuser.all。</span><span class="sxs-lookup"><span data-stu-id="e5c78-137">To use Delegated permissions, select **Delegated permissions** and then select **EWS.AccessAsUser.All** under **EWS**.</span></span> <span data-ttu-id="e5c78-138">[**アクセス許可の追加**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="e5c78-138">Click on **Add permissions**.</span></span> 

<span data-ttu-id="e5c78-139">アプリケーションのアクセス許可を使用するには、次の追加の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="e5c78-139">To use Application permissions, follow these additional steps.</span></span>

1. <span data-ttu-id="e5c78-140">[**アプリケーションの権限**] を選択し、[ **full_access_as_app**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="e5c78-140">Select **Application permissions** and then select **full_access_as_app**.</span></span> <span data-ttu-id="e5c78-141">[**アクセス許可の追加**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="e5c78-141">Click on **Add permissions**.</span></span>

1. <span data-ttu-id="e5c78-142">[**組織に対する管理者の同意を許可**する] を選択し、同意ダイアログを承諾します。</span><span class="sxs-lookup"><span data-stu-id="e5c78-142">Select **Grant admin consent for org** and accept the consent dialog.</span></span> 

1. <span data-ttu-id="e5c78-143">[**管理**] の下にある左側のナビゲーションで、[**証明書 & シークレット**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="e5c78-143">Select **Certificates & Secrets** in the left-hand navigation under **Manage**.</span></span> 

1. <span data-ttu-id="e5c78-144">[**新しいクライアントシークレット**] を選択し、簡単な説明を入力して [**追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="e5c78-144">Select **New client secret**, enter a short description and select **Add**.</span></span>

1. <span data-ttu-id="e5c78-145">新しく追加したクライアントシークレットの**値**をコピーして保存し、後で必要になります。</span><span class="sxs-lookup"><span data-stu-id="e5c78-145">Copy the **Value** of the newly added client secret and save it, you will need it later.</span></span> 

## <a name="add-code-to-get-an-authentication-token"></a><span data-ttu-id="e5c78-146">認証トークンを取得するコードを追加する</span><span class="sxs-lookup"><span data-stu-id="e5c78-146">Add code to get an authentication token</span></span>

<span data-ttu-id="e5c78-147">次のコードスニペットは、Microsoft 認証ライブラリを使用して、委任されたアクセス許可とアプリケーションのアクセス許可の認証トークンを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e5c78-147">The following code snippets show how to use the Microsoft Authentication Library to get authentication tokens for delegated permissions and application permissions.</span></span> <span data-ttu-id="e5c78-148">これらのスニペットは、認証要求を行うために必要な情報が、アプリケーションの**App.config**ファイルに格納されていることを前提としています。</span><span class="sxs-lookup"><span data-stu-id="e5c78-148">These snippets assume that the information required to make the authentication request is stored in the application's **App.config** file.</span></span> <span data-ttu-id="e5c78-149">これらの例には、エラーチェックは含まれていません。完全なコードについては、[コードサンプル](#code-samples)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5c78-149">These examples do not include error checking, see the [Code samples](#code-samples) for the complete code.</span></span>

### <a name="delegated-permissions"></a><span data-ttu-id="e5c78-150">委任されたアクセス許可</span><span class="sxs-lookup"><span data-stu-id="e5c78-150">Delegated permissions</span></span>

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

### <a name="application-permissions"></a><span data-ttu-id="e5c78-151">アプリケーションのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="e5c78-151">Application permissions</span></span>

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

## <a name="add-an-authentication-token-to-ews-requests"></a><span data-ttu-id="e5c78-152">EWS 要求に認証トークンを追加します。</span><span class="sxs-lookup"><span data-stu-id="e5c78-152">Add an authentication token to EWS requests</span></span>

<span data-ttu-id="e5c78-153">**AuthenticationResult** オブジェクトを受信すると、**AccessToken** プロパティを使用して、トークン サービスによって発行されるトークンを取得できます。</span><span class="sxs-lookup"><span data-stu-id="e5c78-153">After you've received the **AuthenticationResult** object you can use the **AccessToken** property to get the token issued by the token service.</span></span>

```cs
// Configure the ExchangeService with the access token
var ewsClient = new ExchangeService();
ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
```

<span data-ttu-id="e5c78-154">アプリケーションのアクセス許可を使用するには、アクセスするメールボックスを明示的に偽装する必要もあります。</span><span class="sxs-lookup"><span data-stu-id="e5c78-154">To use Application permissions, you will also need to explictly impersonate a mailbox that you would like to access.</span></span> 

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a><span data-ttu-id="e5c78-155">コード サンプル</span><span class="sxs-lookup"><span data-stu-id="e5c78-155">Code samples</span></span>

### <a name="delegated-permissions"></a><span data-ttu-id="e5c78-156">委任されたアクセス許可</span><span class="sxs-lookup"><span data-stu-id="e5c78-156">Delegated permissions</span></span>

<span data-ttu-id="e5c78-157">次に示す完全なコードサンプルは、委任されたアクセス許可を使用して OAuth 認証された EWS 要求を作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e5c78-157">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using Delegated permissions.</span></span>

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

### <a name="application-permissions"></a><span data-ttu-id="e5c78-158">アプリケーションのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="e5c78-158">Application permissions</span></span>

<span data-ttu-id="e5c78-159">以下に、アプリケーションのアクセス許可を使用して OAuth 認証された EWS 要求を作成する方法を示す完全なコードサンプルを示します。</span><span class="sxs-lookup"><span data-stu-id="e5c78-159">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using Application permissions.</span></span>

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

<span data-ttu-id="e5c78-160">両方のサンプルコードでは、次のエントリを含む**App.config**ファイルが必要です。</span><span class="sxs-lookup"><span data-stu-id="e5c78-160">The sample code in both cases requires an **App.config** file with the following entries:</span></span>

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

## <a name="see-also"></a><span data-ttu-id="e5c78-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="e5c78-161">See also</span></span>

- [<span data-ttu-id="e5c78-162">Exchange における認証と EWS</span><span class="sxs-lookup"><span data-stu-id="e5c78-162">Authentication and EWS in Exchange</span></span>](authentication-and-ews-in-exchange.md)

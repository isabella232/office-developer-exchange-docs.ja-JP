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
# <a name="authenticate-an-ews-application-by-using-oauth"></a><span data-ttu-id="d7913-103">OAuth を使用して EWS アプリケーションを認証する</span><span class="sxs-lookup"><span data-stu-id="d7913-103">Authenticate an EWS application by using OAuth</span></span>
<!-- markdownlint-enable MD025 -->

<span data-ttu-id="d7913-104">EWS Managed API アプリケーションで、OAuth 認証を使用する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="d7913-104">Learn how to use OAuth authentication with your EWS Managed API applications.</span></span>

<span data-ttu-id="d7913-105">Azure Active Directory が提供する OAuth の認証サービスを使用すると、EWS Managed API アプリケーションが Office 365 での Exchange Online にアクセスできるようにすることができます。</span><span class="sxs-lookup"><span data-stu-id="d7913-105">You can use the OAuth authentication service provided by Azure Active Directory to enable your EWS Managed API applications to access Exchange Online in Office 365.</span></span> <span data-ttu-id="d7913-106">OAuth をアプリケーションで使用するには、次のようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7913-106">To use OAuth with your application you will need to:</span></span>

1. <span data-ttu-id="d7913-107">Azure Active Directory に[アプリケーションを登録する](#register-your-application)。</span><span class="sxs-lookup"><span data-stu-id="d7913-107">[Register your application](#register-your-application) with Azure Active Directory.</span></span>
1. <span data-ttu-id="d7913-108">トークン サーバーから認証トークンを取得するために、[認証トークンを取得するコードを追加する](#add-code-to-get-an-authentication-token)。</span><span class="sxs-lookup"><span data-stu-id="d7913-108">[Add code to get an authentication token](#add-code-to-get-an-authentication-token) to get an authentication token from a token server.</span></span>
1. <span data-ttu-id="d7913-109">送信する [EWS 要求に認証トークンを追加する](#add-an-authentication-token-to-ews-requests)。</span><span class="sxs-lookup"><span data-stu-id="d7913-109">[Add an authentication token to EWS requests](#add-an-authentication-token-to-ews-requests) that you send.</span></span>

> [!NOTE]
> <span data-ttu-id="d7913-110">EWS の OAuth 認証は、Microsoft 365 の一部として Exchange Online でのみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="d7913-110">OAuth authentication for EWS is only available in Exchange Online as part of Microsoft 365.</span></span> <span data-ttu-id="d7913-111">OAuth を使用する EWS アプリケーションは、Azure Active Directory に登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7913-111">EWS applications that use OAuth must be registered with Azure Active Directory.</span></span>

<span data-ttu-id="d7913-112">この記事のコードを使用するには、次に対するアクセス権が必要です。</span><span class="sxs-lookup"><span data-stu-id="d7913-112">To use the code in this article, you will need to have access to the following:</span></span>

- <span data-ttu-id="d7913-113">Exchange Online メールボックスを使用している Microsoft 365 アカウント。</span><span class="sxs-lookup"><span data-stu-id="d7913-113">A Microsoft 365 account with an Exchange Online mailbox.</span></span> <span data-ttu-id="d7913-114">Microsoft 365 アカウントをお持ちでない場合は、[Microsoft 365 開発者プログラムにサインアップ](https://developer.microsoft.com/microsoft-365/dev-program)して、無料の Microsoft 365 サブスクリプションを取得できます。</span><span class="sxs-lookup"><span data-stu-id="d7913-114">If you do not have a Microsoft 365 account, you can [sign up for the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program) to get a free Microsoft 365 subscription.</span></span>
- <span data-ttu-id="d7913-115">[.NET 用の Microsoft Authentication Library](/dotnet/api/microsoft.identity.client)。</span><span class="sxs-lookup"><span data-stu-id="d7913-115">The [Microsoft Authentication Library for .NET](/dotnet/api/microsoft.identity.client).</span></span>
- <span data-ttu-id="d7913-116">[EWS マネージ API](https://github.com/officedev/ews-managed-api)。</span><span class="sxs-lookup"><span data-stu-id="d7913-116">The [EWS Managed API](https://github.com/officedev/ews-managed-api).</span></span>

<span data-ttu-id="d7913-117">Exchange Online で EWS API へのアクセスに使用できる OAuth 許可には 2 つの種類があります。</span><span class="sxs-lookup"><span data-stu-id="d7913-117">There are two types of OAuth permissions that can be used to access EWS APIs in Exchange Online.</span></span> <span data-ttu-id="d7913-118">チュートリアルを続行する前に、使用するアクセス許可の具体的な種類を選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7913-118">Before you proceed with the tutorial, you will need to choose the specific permission type to use.</span></span>

- <span data-ttu-id="d7913-119">**委任されたアクセス許可** は、サインインしているユーザーが存在するアプリで使用します。</span><span class="sxs-lookup"><span data-stu-id="d7913-119">**Delegated permissions** are used by apps that have a signed-in user present.</span></span> <span data-ttu-id="d7913-120">これに該当するアプリの場合は、ユーザーまたは管理者がアプリの要求するアクセス許可に同意します。アプリは API 呼び出しを行う時に、サインインしているユーザーとして動作できます。</span><span class="sxs-lookup"><span data-stu-id="d7913-120">For these apps, either the user or an administrator consents to the permissions that the app requests and the app can act as the signed-in user when making API calls.</span></span>
- <span data-ttu-id="d7913-121">**アプリケーションのアクセス許可** は、サインインしているユーザーが存在しないアプリで使用します。たとえば、バックグラウンド サービスやデーモンとして実行され、複数のメールボックスにアクセスできるアプリです。</span><span class="sxs-lookup"><span data-stu-id="d7913-121">**Application permissions** are used by apps that run without a signed-in user present; for example, apps that run as background services or daemons and can access multiple mailboxes.</span></span>

## <a name="register-your-application"></a><span data-ttu-id="d7913-122">アプリケーションを登録する</span><span class="sxs-lookup"><span data-stu-id="d7913-122">Register your application</span></span>

<span data-ttu-id="d7913-123">OAuth を使用するには、アプリケーションに Azure Active Directory が発行したアプリケーション ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="d7913-123">To use OAuth, an application must have an application ID issued by Azure Active Directory.</span></span> <span data-ttu-id="d7913-124">このチュートリアルでは、アプリケーションがコンソール アプリケーションであることが前提となるので、アプリケーションを Azure Active Directory にパブリック クライアントとして登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7913-124">In this tutorial, it is assumed that the application is a console application, so you need to register your application as a public client with Azure Active Directory.</span></span> <span data-ttu-id="d7913-125">アプリケーションの登録は、Azure Active Directory 管理センターか、Microsoft Graph を使用して行うことができます。</span><span class="sxs-lookup"><span data-stu-id="d7913-125">You can register an application in the Azure Active Directory admin center or by using Microsoft Graph.</span></span>

1. <span data-ttu-id="d7913-126">ブラウザーを開き、[Azure Active Directory 管理センター](https://aad.portal.azure.com)へ移動して、**個人用アカウント** (別名: Microsoft アカウント)、または **職場/学校アカウント** を使用してログインします。</span><span class="sxs-lookup"><span data-stu-id="d7913-126">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com) and login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="d7913-127">左側のナビゲーションで **[Azure Active Directory]** を選択し、それから **[管理]** で **[アプリの登録]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d7913-127">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage**.</span></span>

1. <span data-ttu-id="d7913-128">**[新規登録]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d7913-128">Select **New registration**.</span></span> <span data-ttu-id="d7913-129">
            \**[アプリケーションを登録]\*\* ページで、次のように値を設定します。</span><span class="sxs-lookup"><span data-stu-id="d7913-129">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="d7913-130">**[名前]** をアプリのフレンドリ名に設定します。</span><span class="sxs-lookup"><span data-stu-id="d7913-130">Set **Name** to a friendly name for your app.</span></span>
    - <span data-ttu-id="d7913-131">**[サポートされているアカウントの種類]** をシナリオに合った選択肢に設定します。</span><span class="sxs-lookup"><span data-stu-id="d7913-131">Set **Supported account types** to the choice that makes sense for your scenario.</span></span>
    - <span data-ttu-id="d7913-132">**リダイレクト URI** については、ドロップダウンを **[パブリック クライアント (モバイルとデスクトップ)]** に変更し、値を `urn:ietf:wg:oauth:2.0:oob` に設定します。</span><span class="sxs-lookup"><span data-stu-id="d7913-132">For **Redirect URI**, change the dropdown to **Public client (mobile & desktop)** and set the value to `urn:ietf:wg:oauth:2.0:oob`.</span></span>

1. <span data-ttu-id="d7913-133">**[登録]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d7913-133">Choose **Register**.</span></span> <span data-ttu-id="d7913-134">次のページで、**アプリケーション (クライアント) ID** と **ディレクトリ (テナント) ID** の値をコピーして保存します。これらの値は、後ほど必要になります。</span><span class="sxs-lookup"><span data-stu-id="d7913-134">On the next page, copy the values of the **Application (client) ID** and **Directory (tenant) ID** and save them, you will need them later.</span></span>

### <a name="configure-for-delegated-authentication"></a><span data-ttu-id="d7913-135">委任された認証の構成</span><span class="sxs-lookup"><span data-stu-id="d7913-135">Configure for delegated authentication</span></span>

<span data-ttu-id="d7913-136">アプリケーションが委任された認証を使用する場合は、これ以上の構成は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="d7913-136">If your application uses delegated authentication, no further configuration is required.</span></span> <span data-ttu-id="d7913-137">[[Microsoft ID プラットフォーム]](/azure/active-directory/develop/v2-overview) では、アプリが動的にアクセス許可を要求できるようになっているので、アプリの登録時にアクセス許可を事前に構成する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="d7913-137">The [Microsoft identity platform](/azure/active-directory/develop/v2-overview) allows apps to request permissions dynamically, so you do not have to pre-configure permissions on the app registration.</span></span> <span data-ttu-id="d7913-138">ただし、いくつかのシナリオにおいては ([代理 (On-Behalf-Of) フロー](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) など)、アクセス許可の事前構成が必要です。</span><span class="sxs-lookup"><span data-stu-id="d7913-138">However, in some scenarios (like the [on-behalf-of flow](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)) pre-configuring permissions is required.</span></span> <span data-ttu-id="d7913-139">EWS のアクセス許可を事前に構成するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="d7913-139">Use the following steps to pre-configure EWS permissions.</span></span>

1. <span data-ttu-id="d7913-140">左側のナビゲーションの **[管理]** で **[マニフェスト]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d7913-140">Select **Manifest** in the left-hand navigation under **Manage**.</span></span>

1. <span data-ttu-id="d7913-141">マニフェスト内で `requiredResourceAccess` プロパティを見つけ、角かっこ (`[]`) の中に以下を追加します。</span><span class="sxs-lookup"><span data-stu-id="d7913-141">Locate the `requiredResourceAccess` property in the manifest, and add the following inside the square brackets (`[]`):</span></span>

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

1. <span data-ttu-id="d7913-142">**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d7913-142">Select **Save**.</span></span>

1. <span data-ttu-id="d7913-143">**[管理]** で、**[API のアクセス許可]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d7913-143">Select **API permissions** under **Manage**.</span></span> <span data-ttu-id="d7913-144">**EWS.AccessAsUser.All** アクセス許可が表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="d7913-144">Confirm that the **EWS.AccessAsUser.All** permission is listed.</span></span>

### <a name="configure-for-app-only-authentication"></a><span data-ttu-id="d7913-145">アプリ専用の認証の構成</span><span class="sxs-lookup"><span data-stu-id="d7913-145">Configure for app-only authentication</span></span>

<span data-ttu-id="d7913-146">アプリケーションのアクセス許可を使用するには、次の追加の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="d7913-146">To use application permissions, follow these additional steps.</span></span>

1. <span data-ttu-id="d7913-147">左側のナビゲーションの **[管理]** で **[マニフェスト]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d7913-147">Select **Manifest** in the left-hand navigation under **Manage**.</span></span>

1. <span data-ttu-id="d7913-148">マニフェスト内で `requiredResourceAccess` プロパティを見つけ、角かっこ (`[]`) の中に以下を追加します。</span><span class="sxs-lookup"><span data-stu-id="d7913-148">Locate the `requiredResourceAccess` property in the manifest, and add the following inside the square brackets (`[]`):</span></span>

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

1. <span data-ttu-id="d7913-149">**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d7913-149">Select **Save**.</span></span>

1. <span data-ttu-id="d7913-150">**[管理]** で、**[API のアクセス許可]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d7913-150">Select **API permissions** under **Manage**.</span></span> <span data-ttu-id="d7913-151">**full_access_as_app** アクセス許可が表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="d7913-151">Confirm that the **full_access_as_app** permission is listed.</span></span>

1. <span data-ttu-id="d7913-152">**[組織に対して管理者の同意を与える]** を選択して、同意ダイアログに同意します。</span><span class="sxs-lookup"><span data-stu-id="d7913-152">Select **Grant admin consent for org** and accept the consent dialog.</span></span>

1. <span data-ttu-id="d7913-153">左側のナビゲーション ウィンドウの **[管理]** で、**[証明書とシークレット]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d7913-153">Select **Certificates & Secrets** in the left-hand navigation under **Manage**.</span></span>

1. <span data-ttu-id="d7913-154">**[新しいクライアント シークレット]** を選択して、短い説明を入力して **[追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d7913-154">Select **New client secret**, enter a short description and select **Add**.</span></span>

1. <span data-ttu-id="d7913-155">新しく追加したシークレットの **[値]** をコピーして保存します。この値は後で必要になります。</span><span class="sxs-lookup"><span data-stu-id="d7913-155">Copy the **Value** of the newly added client secret and save it, you will need it later.</span></span>

## <a name="add-code-to-get-an-authentication-token"></a><span data-ttu-id="d7913-156">認証トークンを取得するコードを追加する</span><span class="sxs-lookup"><span data-stu-id="d7913-156">Add code to get an authentication token</span></span>

<span data-ttu-id="d7913-157">次のコード スニペットは、Microsoft Authentication Library を使用して、委任されたアクセス許可とアプリケーションのアクセス許可の認証トークンを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="d7913-157">The following code snippets show how to use the Microsoft Authentication Library to get authentication tokens for delegated permissions and application permissions.</span></span> <span data-ttu-id="d7913-158">これらのスニペットは、認証要求を行うために必要な情報がアプリケーションの **App.config** ファイルに格納されていると仮定します。</span><span class="sxs-lookup"><span data-stu-id="d7913-158">These snippets assume that the information required to make the authentication request is stored in the application's **App.config** file.</span></span> <span data-ttu-id="d7913-159">これらの例では、エラー チェックは含まれません。完全なコードについては、[コード サンプル](#code-samples)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7913-159">These examples do not include error checking, see the [Code samples](#code-samples) for the complete code.</span></span>

### <a name="get-a-token-with-delegated-auth"></a><span data-ttu-id="d7913-160">委任された認証を使用してトークンを取得する</span><span class="sxs-lookup"><span data-stu-id="d7913-160">Get a token with delegated auth</span></span>

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

### <a name="get-a-token-with-app-only-auth"></a><span data-ttu-id="d7913-161">アプリ専用の認証を使用してトークンを取得する</span><span class="sxs-lookup"><span data-stu-id="d7913-161">Get a token with app-only auth</span></span>

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

## <a name="add-an-authentication-token-to-ews-requests"></a><span data-ttu-id="d7913-162">EWS 要求に認証トークンを追加します。</span><span class="sxs-lookup"><span data-stu-id="d7913-162">Add an authentication token to EWS requests</span></span>

<span data-ttu-id="d7913-163">**AuthenticationResult** オブジェクトを受信すると、**AccessToken** プロパティを使用して、トークン サービスによって発行されるトークンを取得できます。</span><span class="sxs-lookup"><span data-stu-id="d7913-163">After you've received the **AuthenticationResult** object you can use the **AccessToken** property to get the token issued by the token service.</span></span>

```cs
// Configure the ExchangeService with the access token
var ewsClient = new ExchangeService();
ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
```

<span data-ttu-id="d7913-164">アプリケーションのアクセス許可を使用するには、アクセスするメールボックスを明示的に偽装する必要もあります。</span><span class="sxs-lookup"><span data-stu-id="d7913-164">To use application permissions, you will also need to explicitly impersonate a mailbox that you would like to access.</span></span>

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a><span data-ttu-id="d7913-165">コード サンプル</span><span class="sxs-lookup"><span data-stu-id="d7913-165">Code samples</span></span>

### <a name="delegated-authentication"></a><span data-ttu-id="d7913-166">委任された認証</span><span class="sxs-lookup"><span data-stu-id="d7913-166">Delegated authentication</span></span>

<span data-ttu-id="d7913-167">以下は、委任された認証を使用した OAuth 認証された EWS 要求の作成方法を示す完全なコード サンプルです。</span><span class="sxs-lookup"><span data-stu-id="d7913-167">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using delegated authentication.</span></span>

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

### <a name="app-only-authentication"></a><span data-ttu-id="d7913-168">アプリ専用の認証</span><span class="sxs-lookup"><span data-stu-id="d7913-168">App-only authentication</span></span>

<span data-ttu-id="d7913-169">以下は、アプリ専用の認証を使用した OAuth 認証された EWS 要求の作成方法を示す完全なコード サンプルです。</span><span class="sxs-lookup"><span data-stu-id="d7913-169">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using app-only authentication.</span></span>

> [!NOTE]
> <span data-ttu-id="d7913-170">偽装を使用するときには、必ず X-AnchorMailbox 要求ヘッダーを使用し、偽装メールボックスの SMTP アドレスに設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7913-170">When using impersonation you must always use the X-AnchorMailbox request header, which should be set to the SMTP address of the impersonated mailbox.</span></span>

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

<span data-ttu-id="d7913-171">どちらの場合も、サンプル コードには次のエントリを持つ **App.config** ファイルが必要です。</span><span class="sxs-lookup"><span data-stu-id="d7913-171">The sample code in both cases requires an **App.config** file with the following entries:</span></span>

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

## <a name="see-also"></a><span data-ttu-id="d7913-172">関連項目</span><span class="sxs-lookup"><span data-stu-id="d7913-172">See also</span></span>

- [<span data-ttu-id="d7913-173">Exchange における認証と EWS</span><span class="sxs-lookup"><span data-stu-id="d7913-173">Authentication and EWS in Exchange</span></span>](authentication-and-ews-in-exchange.md)

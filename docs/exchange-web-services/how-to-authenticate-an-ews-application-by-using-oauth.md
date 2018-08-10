---
title: OAuth を使用して EWS アプリケーションを認証する
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: EWS Managed API アプリケーションで、OAuth 認証を使用する方法について説明します。
ms.openlocfilehash: 8b6a3fd72e42a36e31f261205292de28ef341270
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353582"
---
# <a name="authenticate-an-ews-application-by-using-oauth"></a><span data-ttu-id="070a6-103">OAuth を使用して EWS アプリケーションを認証する</span><span class="sxs-lookup"><span data-stu-id="070a6-103">Authenticate an EWS application by using OAuth</span></span>

<span data-ttu-id="070a6-104">EWS Managed API アプリケーションで、OAuth 認証を使用する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="070a6-104">Learn how to use OAuth authentication with your EWS Managed API applications.</span></span>
  
<span data-ttu-id="070a6-105">Azure Active Directory が提供する OAuth の認証サービスを使用すると、Office 365 REST API で使用される同じ認証モデルに EWS Managed API アプリケーションを統合できます。</span><span class="sxs-lookup"><span data-stu-id="070a6-105">You can use the OAuth authentication service provided by Azure Active Directory to integrate your EWS Managed API applications  with the same authentication model used by the Office 365 REST APIs. To use OAuth with your  application you will need to:</span></span> <span data-ttu-id="070a6-106">OAuth をアプリケーションで使用するには、次のようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="070a6-106">To use OAuth with your application you will need to:</span></span>
  
1. <span data-ttu-id="070a6-107">Azure Active Directory に[アプリケーションを登録する](#bk_register)。</span><span class="sxs-lookup"><span data-stu-id="070a6-107">Register your application with Azure Active Directory</span></span> 
    
2. <span data-ttu-id="070a6-108">トークン サーバーから認証トークンを取得するために、[認証トークンを取得するコードを追加する](#bk_getToken)。</span><span class="sxs-lookup"><span data-stu-id="070a6-108">Add code to your application to get an authentication token from a token server.</span></span> 
    
3. <span data-ttu-id="070a6-109">送信する [EWS 要求に認証トークンを追加する](#bk_useToken)。</span><span class="sxs-lookup"><span data-stu-id="070a6-109">[Add the authentication token to the EWS requests](#bk_useToken) that you send.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="070a6-p102">EWS の OAuth 認証は、Office 365 の一部として Exchange でのみ利用可能です。EWS アプリケーションには、「ユーザーのメールボックスへのフル アクセス」権限が必要です。</span><span class="sxs-lookup"><span data-stu-id="070a6-p102">OAuth authentication for EWS is only available in Exchange as part of Office 365. EWS applications require the "Full access to user's mailbox" permission.</span></span> 
  
<span data-ttu-id="070a6-112">この記事のコードを使用するには、次に対するアクセス権が必要です。</span><span class="sxs-lookup"><span data-stu-id="070a6-112">To use the code in this article, you will need to have access to the following:</span></span>
  
- <span data-ttu-id="070a6-113">[Office 365 開発者アカウント](https://docs.microsoft.com/ja-JP/office/developer-program/office-365-developer-program)。</span><span class="sxs-lookup"><span data-stu-id="070a6-113">An [Office 365 developer site](https://docs.microsoft.com/ja-JP/office/developer-program/office-365-developer-program).</span></span> <span data-ttu-id="070a6-114">試用版のアカウントを使用して、アプリケーションをテストできます。</span><span class="sxs-lookup"><span data-stu-id="070a6-114">An Office 365 developer account. You can use a trial account to test your application</span></span>
    
- <span data-ttu-id="070a6-115">[Azure AD Authentication Library for .NET](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-authentication-libraries)。</span><span class="sxs-lookup"><span data-stu-id="070a6-115">The [Azure AD Authentication Library for .NET](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-authentication-libraries).</span></span>
    
- <span data-ttu-id="070a6-116">[EWS マネージ API](https://github.com/officedev/ews-managed-api.aspx)。</span><span class="sxs-lookup"><span data-stu-id="070a6-116">[The EWS Managed API](https://github.com/officedev/ews-managed-api.aspx)</span></span>

<span data-ttu-id="070a6-117"><a name="bk_register"> </a></span><span class="sxs-lookup"><span data-stu-id="070a6-117"></span></span>

## <a name="register-your-application"></a><span data-ttu-id="070a6-118">アプリケーションを登録する</span><span class="sxs-lookup"><span data-stu-id="070a6-118">Register your application</span></span>

<span data-ttu-id="070a6-119">OAuth を使用するには、アプリケーションにクライアントの ID と、アプリケーションを識別するアプリケーション URI が必要です。</span><span class="sxs-lookup"><span data-stu-id="070a6-119">To use OAuth, an application must have a client identifier and an application URI that identifies the application.</span></span> <span data-ttu-id="070a6-120">Azure Active Directory サービスにアプリケーションをまだ登録していない場合は、「[アプリケーションを登録する](https://apps.dev.microsoft.com/#/appList)」の手順に従い、アプリケーションを手動で追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="070a6-120">To use OAuth, an application must have a client identifier and an application URI that identifies the application. If you have not yet registered your application with Azure Active Directory Services, you'll need to manually add your application by following the steps under [Register you app](https://apps.dev.microsoft.com/#/appList).</span></span>

<span data-ttu-id="070a6-121"><a name="bk_getToken"> </a></span><span class="sxs-lookup"><span data-stu-id="070a6-121"></span></span>

## <a name="add-code-to-get-an-authentication-token"></a><span data-ttu-id="070a6-122">認証トークンを取得するコードを追加する</span><span class="sxs-lookup"><span data-stu-id="070a6-122">Add code to get an authentication token</span></span>

<span data-ttu-id="070a6-123">Azure AD Authentication Library for .NET は、Azure Active Directory からの認証トークンの取得を簡略化するため、アプリケーションでトークンを利用できます。</span><span class="sxs-lookup"><span data-stu-id="070a6-123">The Azure AD Authentication Library for .NET simplifies getting an authentication token from Azure Active Directory so that you can use the token in your application.  You need to provide four pieces of information to get the token:</span></span> <span data-ttu-id="070a6-124">4 つのトークンを取得するために、次の情報を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="070a6-124">You need to provide four pieces of information to get the token:</span></span>
  
1. <span data-ttu-id="070a6-p106">トークン サーバーの URI。トークン サーバーは、ユーザーを認証し、アプリケーションが EWS へのアクセスに使用できるトークンを返す**機関**です。</span><span class="sxs-lookup"><span data-stu-id="070a6-p106">The URI of the token server. The token server is the **authority** that authenticates the user and returns a token that your application can use to access EWS.</span></span> 
    
2. <span data-ttu-id="070a6-127">Azure Active Directory にアプリケーションを登録するときに作成されたアプリケーションのクライアント ID。</span><span class="sxs-lookup"><span data-stu-id="070a6-127">The application client ID created when you registered your application with Azure Active Directory.</span></span>
    
3. <span data-ttu-id="070a6-128">Azure Active Directory にアプリケーションを登録するときに作成されたアプリケーションのクライアント URI。</span><span class="sxs-lookup"><span data-stu-id="070a6-128">The application client URI created when you registered your application with Azure Active Directory.</span></span>
    
4. <span data-ttu-id="070a6-129">EWS サーバーの URI と、EWS のエンドポイントの URI。</span><span class="sxs-lookup"><span data-stu-id="070a6-129">The URI of the EWS server and the URI of the EWS endpoint. For Exchange as part of Office 365, this will be https://<server name>/ews/exchange.asmx.</span></span> <span data-ttu-id="070a6-130">Office 365 の一部としての Exchange では、`https://<server name>/ews/exchange.asmx` のようになります。</span><span class="sxs-lookup"><span data-stu-id="070a6-130">For Exchange as part of Office 365, this will be  `https://<server name>/ews/exchange.asmx`.</span></span>
    
<span data-ttu-id="070a6-131">次のコードでは、Azure の AD 認証ライブラリを使用して、認証トークンを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="070a6-131">The following code shows how to use the Azure AD Authentication Library to get an authentication token.</span></span> <span data-ttu-id="070a6-132">認証要求を行うために必要な情報がアプリケーションの App.config ファイルに格納されていると仮定します。</span><span class="sxs-lookup"><span data-stu-id="070a6-132">It assumes that the information required to make the authentication request is stored in the application's App.config file.</span></span> <span data-ttu-id="070a6-133">この例では、エラー チェックは含まれません。完全なコードについては、[コード サンプル](#bk_codeSample)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="070a6-133">This example does not include error checking, see the [Code sample](#bk_codeSample) for the complete code.</span></span> 
  
```cs
string authority = ConfigurationManager.AppSettings["authority"];
string clientID = ConfigurationManager.AppSettings["clientID"];
Uri clientAppUri = new Uri(ConfigurationManager.AppSettings["clientAppUri"];
string serverName = ConfigurationManager.AppSettings["serverName"];
AuthenticationContext authenticationContext = new AuthenticationContext(authority, false);
AuthenticationResult authenticationResult = authenticationContext.AcquireToken(serverName, clientId, clientAppUri);

```

<span data-ttu-id="070a6-134"><a name="bk_useToken"> </a></span><span class="sxs-lookup"><span data-stu-id="070a6-134"></span></span>

## <a name="add-an-authentication-token-to-ews-requests"></a><span data-ttu-id="070a6-135">EWS 要求に認証トークンを追加します。</span><span class="sxs-lookup"><span data-stu-id="070a6-135">Add an authentication token to EWS requests</span></span>

<span data-ttu-id="070a6-136">**AuthenticationResult** オブジェクトを受信すると、**AccessToken** プロパティを使用して、トークン サービスによって発行されるトークンを取得できます。</span><span class="sxs-lookup"><span data-stu-id="070a6-136">Once you've received the **AuthenticationResult** object you can use the **AccessToken** property to get the token issued by the token service.</span></span> 
  
```cs
ExchangeService exchangeService = new ExchangeService(ExchangeVersion.Exchange2013);
exchangeService.Url = new Uri(ConfigurationManager.AppSettings["serverName"]+"ews/exchange.asmx");
exchangeService.TraceEnabled = true;
exchangeService.TraceFlags = TraceFlags.All;
exchangeService.Credentials = new OAuthCredentials(authenticationResult.AccessToken));
exchangeService.FindFolders(WellKnownFolderName.Root, new Folderview(10));
```

<span data-ttu-id="070a6-137"><a name="bk_codeSample"> </a></span><span class="sxs-lookup"><span data-stu-id="070a6-137"></span></span>

## <a name="code-sample"></a><span data-ttu-id="070a6-138">コード サンプル</span><span class="sxs-lookup"><span data-stu-id="070a6-138">Code sample</span></span>

<span data-ttu-id="070a6-139">以下の完全なコード サンプルでは、OAuth 認証が行われる EWS 要求を示します。</span><span class="sxs-lookup"><span data-stu-id="070a6-139">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request.</span></span>
  
```cs
using System;
using System.Collections.Generic;
using System.Configuration;
using System.Globalization;
using System.Linq;
using System.Text;
using System.Threading;
using System.Threading.Tasks;
using System.Web.Script.Serialization;
using Microsoft.Exchange.WebServices.Autodiscover;
using Microsoft.Exchange.WebServices.Data;
using Microsoft.IdentityModel.Clients.ActiveDirectory;
namespace TestV1App
{
    class Program
    {
        static void Main(string[] args)
        {
            var t = new Thread(Run);
            t.SetApartmentState(ApartmentState.STA);
            t.Start();
            t.Join();
        }
        static void Run()
        {
           string authority = ConfigurationManager.AppSettings["authority"];
           string clientID = ConfigurationManager.AppSettings["clientID"];
           Uri clientAppUri = new Uri(ConfigurationManager.AppSettings["clientAppUri"];
           string serverName = ConfigurationManager.AppSettings["serverName"];
            AuthenticationResult authenticationResult = null;
            AuthenticationContext authenticationContext = new AuthenticationContext(authority, false);
            
            string errorMessage = null;
            try
            {
                Console.WriteLine("Trying to acquire token");
                authenticationResult = authenticationContext.AcquireToken(serverName, clientId, clientAppUri);
            }
                catch (AdalException ex)
            {
                errorMessage = ex.Message;
                if (ex.InnerException != null)
                {
                    errorMessage += "\nInnerException : " + ex.InnerException.Message;
                }
            }
            catch (ArgumentException ex)
            {
                errorMessage = ex.Message;
            }
            if (!string.IsNullOrEmpty(errorMessage))
            {
                Console.WriteLine("Failed: {0}" + errorMessage);
                return;
            }
            Console.WriteLine("\nMaking the protocol call\n");
            ExchangeService exchangeService = new ExchangeService(ExchangeVersion.Exchange2013);
            exchangeService.Url = new Uri(resource + "ews/exchange.asmx");
            exchangeService.TraceEnabled = true;
            exchangeService.TraceFlags = TraceFlags.All;
            exchangeService.Credentials = new OAuthCredentials(authenticationResult.AccessToken);
            exchangeService.FindFolders(WellKnownFolderName.Root, new FolderView(10));
        }
    }
}

```

<span data-ttu-id="070a6-140">サンプル コードには、次のエントリを持つ App.config ファイルが必要です。</span><span class="sxs-lookup"><span data-stu-id="070a6-140">The sample code requires an App.config file with the following entries:</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8" ?>
<configuration>
  <startup>
    <supportedRuntime version="v4.0" sku=".NETFramework,Version=v4.5" />
  </startup>
  <appSettings>
    <add key="authority" value="http://login.windows.net/<devAccountName>.onmicrosoft.com" />
    <add key="clientId" value="<ID generated by Azure Active Directory"/>
    <add key="clientAppUri" value="<URI registered with Azure Active Directory"/>
    <add key="serverName" value="outlook.office365.com" />
  </appSettings>
</configuration>
```

## <a name="see-also"></a><span data-ttu-id="070a6-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="070a6-141">See also</span></span>

- [<span data-ttu-id="070a6-142">Exchange における認証と EWS</span><span class="sxs-lookup"><span data-stu-id="070a6-142">Authentication and EWS in Exchange</span></span>](authentication-and-ews-in-exchange.md)    

    


---
title: OAuth を使用して、EWS アプリケーションを認証します。
manager: sethgros
ms.date: 1/15/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: EWS Managed API アプリケーションで、OAuth 認証を使用する方法について説明します。
ms.openlocfilehash: 66bbc0525ecf78407e853da0c8dcdec92791ca56
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758919"
---
# <a name="authenticate-an-ews-application-by-using-oauth"></a><span data-ttu-id="d09b0-103">OAuth を使用して、EWS アプリケーションを認証します。</span><span class="sxs-lookup"><span data-stu-id="d09b0-103">Authenticate an EWS application by using OAuth</span></span>

<span data-ttu-id="d09b0-104">EWS Managed API アプリケーションで、OAuth 認証を使用する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="d09b0-104">Learn how to use OAuth authentication with your EWS Managed API applications.</span></span>
  
<span data-ttu-id="d09b0-105">Azure Active Directory が提供する OAuth の認証サービスを使用すると、Office 365 の他の Api で使用される同じ認証モデルでは、EWS のマネージ API アプリケーションを統合します。</span><span class="sxs-lookup"><span data-stu-id="d09b0-105">You can use the OAuth authentication service provided by Azure Active Directory to integrate your EWS Managed API applications with the same authentication model used by the Office 365 REST APIs.</span></span> <span data-ttu-id="d09b0-106">アプリケーションで、OAuth を使用するには、必要があります。</span><span class="sxs-lookup"><span data-stu-id="d09b0-106">To use OAuth with your application you will need to:</span></span>
  
1. <span data-ttu-id="d09b0-107">Azure Active Directory と[アプリケーションの登録](#bk_register)をします。</span><span class="sxs-lookup"><span data-stu-id="d09b0-107">[Register your application](#bk_register) with Azure Active Directory.</span></span> 
    
2. <span data-ttu-id="d09b0-108">トークン サーバから認証トークンを取得する[認証トークンを取得するコードを追加](#bk_getToken)します。</span><span class="sxs-lookup"><span data-stu-id="d09b0-108">[Add code to get an authentication token](#bk_getToken) to get an authentication token from a token server.</span></span> 
    
3. <span data-ttu-id="d09b0-109">送信する[EWS 要求に認証トークンを追加](#bk_useToken)します。</span><span class="sxs-lookup"><span data-stu-id="d09b0-109">[Add an authentication token to EWS requests](#bk_useToken) that you send.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="d09b0-p102">EWS の OAuth 認証は、Office 365 の一部として Exchange でのみ利用可能です。EWS アプリケーションには、「ユーザーのメールボックスへのフル アクセス」権限が必要です。</span><span class="sxs-lookup"><span data-stu-id="d09b0-p102">OAuth authentication for EWS is only available in Exchange as part of Office 365. EWS applications require the "Full access to user's mailbox" permission.</span></span> 
  
<span data-ttu-id="d09b0-112">この記事のコードを使用するには、次に対するアクセス権が必要です。</span><span class="sxs-lookup"><span data-stu-id="d09b0-112">To use the code in this article, you will need to have access to the following:</span></span>
  
- <span data-ttu-id="d09b0-113">[Office 365 開発者アカウント](http://office.microsoft.com/compare-office-365-for-business-plans-FX102918419.aspx.aspx)です。</span><span class="sxs-lookup"><span data-stu-id="d09b0-113">An [Office 365 developer account](http://office.microsoft.com/compare-office-365-for-business-plans-FX102918419.aspx.aspx).</span></span> <span data-ttu-id="d09b0-114">試用版のアカウントを使用するには、アプリケーションをテストするのには</span><span class="sxs-lookup"><span data-stu-id="d09b0-114">You can use a trial account to test your application</span></span>
    
- <span data-ttu-id="d09b0-115">[.Net の Azure AD 認証ライブラリ](http://msdn.microsoft.com/en-us/library/office/jj573266.aspx.aspx)です。</span><span class="sxs-lookup"><span data-stu-id="d09b0-115">The [Azure AD Authentication Library for .NET](http://msdn.microsoft.com/en-us/library/office/jj573266.aspx.aspx).</span></span>
    
- <span data-ttu-id="d09b0-116">[EWS はマネージ API](https://github.com/officedev/ews-managed-api.aspx)です。</span><span class="sxs-lookup"><span data-stu-id="d09b0-116">[The EWS Managed API](https://github.com/officedev/ews-managed-api.aspx).</span></span>

<span data-ttu-id="d09b0-117"><a name="bk_register"> </a></span><span class="sxs-lookup"><span data-stu-id="d09b0-117"></span></span>

## <a name="register-your-application"></a><span data-ttu-id="d09b0-118">アプリケーションを登録する</span><span class="sxs-lookup"><span data-stu-id="d09b0-118">Register your application</span></span>

<span data-ttu-id="d09b0-119">OAuth を使用するには、アプリケーションは、クライアントの id と、アプリケーション、アプリケーションを識別する URI が必要です。</span><span class="sxs-lookup"><span data-stu-id="d09b0-119">To use OAuth, an application must have a client identifier and an application URI that identifies the application.</span></span> <span data-ttu-id="d09b0-120">Azure Active ディレクトリ サービスとアプリケーションをまだ登録していない場合は、次の手順を実行[するアプリケーションを登録](http://msdn.microsoft.com/en-us/office/office365/howto/test-and-deploy-apps.aspx)して、アプリケーションを手動で追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d09b0-120">If you have not yet registered your application with Azure Active Directory Services, you'll need to manually add your application by following the steps under [Register you app](http://msdn.microsoft.com/en-us/office/office365/howto/test-and-deploy-apps.aspx).</span></span>

<span data-ttu-id="d09b0-121"><a name="bk_getToken"> </a></span><span class="sxs-lookup"><span data-stu-id="d09b0-121"></span></span>

## <a name="add-code-to-get-an-authentication-token"></a><span data-ttu-id="d09b0-122">認証トークンを取得するコードを追加する</span><span class="sxs-lookup"><span data-stu-id="d09b0-122">Add code to get an authentication token</span></span>

<span data-ttu-id="d09b0-123">.NET では、Azure の AD 認証ライブラリでは、Azure Active Directory からの認証トークンの取得をアプリケーションにトークンを使用できるように簡単になります。</span><span class="sxs-lookup"><span data-stu-id="d09b0-123">The Azure AD Authentication Library for .NET simplifies getting an authentication token from Azure Active Directory so that you can use the token in your application.</span></span> <span data-ttu-id="d09b0-124">4 つのトークンを取得する情報を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d09b0-124">You need to provide four pieces of information to get the token:</span></span>
  
1. <span data-ttu-id="d09b0-125">トークン サーバの URI。</span><span class="sxs-lookup"><span data-stu-id="d09b0-125">The URI of the token server.</span></span> <span data-ttu-id="d09b0-126">トークン サーバは、ユーザーを認証し、EWS にアクセスするアプリケーションが使用できるトークンを取得する**機関**です。</span><span class="sxs-lookup"><span data-stu-id="d09b0-126">The token server is the **authority** that authenticates the user and returns a token that your application can use to access EWS.</span></span> 
    
2. <span data-ttu-id="d09b0-127">Azure Active Directory にアプリケーションを登録するときに作成されたアプリケーションのクライアント ID。</span><span class="sxs-lookup"><span data-stu-id="d09b0-127">The application client ID created when you registered your application with Azure Active Directory.</span></span>
    
3. <span data-ttu-id="d09b0-128">Azure Active Directory にアプリケーションを登録するときに作成されたアプリケーションのクライアント URI。</span><span class="sxs-lookup"><span data-stu-id="d09b0-128">The application client URI created when you registered your application with Azure Active Directory.</span></span>
    
4. <span data-ttu-id="d09b0-129">EWS サーバーの URI と、EWS のエンドポイントの URI です。</span><span class="sxs-lookup"><span data-stu-id="d09b0-129">The URI of the EWS server and the URI of the EWS endpoint.</span></span> <span data-ttu-id="d09b0-130">Office 365 の一部として、Exchange になります`https://<server name>/ews/exchange.asmx`。</span><span class="sxs-lookup"><span data-stu-id="d09b0-130">For Exchange as part of Office 365, this will be  `https://<server name>/ews/exchange.asmx`.</span></span>
    
<span data-ttu-id="d09b0-131">次のコードでは、Azure の AD 認証ライブラリを使用して、認証トークンを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="d09b0-131">The following code shows how to use the Azure AD Authentication Library to get an authentication token.</span></span> <span data-ttu-id="d09b0-132">認証要求を行うために必要な情報がアプリケーションの App.config ファイルに格納されていることを仮定します。</span><span class="sxs-lookup"><span data-stu-id="d09b0-132">It assumes that the information required to make the authentication request is stored in the application's App.config file.</span></span> <span data-ttu-id="d09b0-133">この例では、エラー チェックが含まれます、完全なコードの[サンプル コード](#bk_codeSample)を参照してはいません。</span><span class="sxs-lookup"><span data-stu-id="d09b0-133">This example does not include error checking, see the [Code sample](#bk_codeSample) for the complete code.</span></span> 
  
```cs
string authority = ConfigurationManager.AppSettings["authority"];
string clientID = ConfigurationManager.AppSettings["clientID"];
Uri clientAppUri = new Uri(ConfigurationManager.AppSettings["clientAppUri"];
string serverName = ConfigurationManager.AppSettings["serverName"];
AuthenticationContext authenticationContext = new AuthenticationContext(authority, false);
AuthenticationResult authenticationResult = authenticationContext.AcquireToken(serverName, clientId, clientAppUri);

```

<span data-ttu-id="d09b0-134"><a name="bk_useToken"> </a></span><span class="sxs-lookup"><span data-stu-id="d09b0-134"></span></span>

## <a name="add-an-authentication-token-to-ews-requests"></a><span data-ttu-id="d09b0-135">EWS 要求に認証トークンを追加します。</span><span class="sxs-lookup"><span data-stu-id="d09b0-135">Add an authentication token to EWS requests</span></span>

<span data-ttu-id="d09b0-136">**AuthenticationResult**オブジェクトを受信した後は、トークン サービスによって発行されたトークンを取得するのには**AccessToken**プロパティを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="d09b0-136">After you've received the **AuthenticationResult** object you can use the **AccessToken** property to get the token issued by the token service.</span></span> 
  
```cs
ExchangeService exchangeService = new ExchangeService(ExchangeVersion.Exchange2013);
exchangeService.Url = new Uri(ConfigurationManager.AppSettings["serverName"]+"ews/exchange.asmx");
exchangeService.TraceEnabled = true;
exchangeService.TraceFlags = TraceFlags.All;
exchangeService.Credentials = new OAuthCredentials(authenticationResult.AccessToken));
exchangeService.FindFolders(WellKnownFolderName.Root, new Folderview(10));
```

<span data-ttu-id="d09b0-137"><a name="bk_codeSample"> </a></span><span class="sxs-lookup"><span data-stu-id="d09b0-137"></span></span>

## <a name="code-sample"></a><span data-ttu-id="d09b0-138">コード サンプル</span><span class="sxs-lookup"><span data-stu-id="d09b0-138">Code sample</span></span>

<span data-ttu-id="d09b0-139">以下の完全なコード サンプルでは、OAuth 認証が行われる EWS 要求を示します。</span><span class="sxs-lookup"><span data-stu-id="d09b0-139">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request.</span></span>
  
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

<span data-ttu-id="d09b0-140">サンプル コードには、次のエントリを持つ App.config ファイルが必要です。</span><span class="sxs-lookup"><span data-stu-id="d09b0-140">The sample code requires an App.config file with the following entries:</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="d09b0-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="d09b0-141">See also</span></span>

- [<span data-ttu-id="d09b0-142">認証および Exchange での EWS</span><span class="sxs-lookup"><span data-stu-id="d09b0-142">Authentication and EWS in Exchange</span></span>](authentication-and-ews-in-exchange.md)    
- [<span data-ttu-id="d09b0-143">テストし、Office 365 アプリケーションを展開します。</span><span class="sxs-lookup"><span data-stu-id="d09b0-143">Test and deploy Office 365 apps</span></span>](http://msdn.microsoft.com/en-us/office/office365/howto/test-and-deploy-apps.aspx)
    


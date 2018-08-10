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
# <a name="authenticate-an-ews-application-by-using-oauth"></a>OAuth を使用して EWS アプリケーションを認証する

EWS Managed API アプリケーションで、OAuth 認証を使用する方法について説明します。
  
Azure Active Directory が提供する OAuth の認証サービスを使用すると、Office 365 REST API で使用される同じ認証モデルに EWS Managed API アプリケーションを統合できます。 OAuth をアプリケーションで使用するには、次のようにする必要があります。
  
1. Azure Active Directory に[アプリケーションを登録する](#bk_register)。 
    
2. トークン サーバーから認証トークンを取得するために、[認証トークンを取得するコードを追加する](#bk_getToken)。 
    
3. 送信する [EWS 要求に認証トークンを追加する](#bk_useToken)。 
    
> [!NOTE]
> EWS の OAuth 認証は、Office 365 の一部として Exchange でのみ利用可能です。EWS アプリケーションには、「ユーザーのメールボックスへのフル アクセス」権限が必要です。 
  
この記事のコードを使用するには、次に対するアクセス権が必要です。
  
- [Office 365 開発者アカウント](https://docs.microsoft.com/ja-JP/office/developer-program/office-365-developer-program)。 試用版のアカウントを使用して、アプリケーションをテストできます。
    
- [Azure AD Authentication Library for .NET](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-authentication-libraries)。
    
- [EWS マネージ API](https://github.com/officedev/ews-managed-api.aspx)。

<a name="bk_register"> </a>

## <a name="register-your-application"></a>アプリケーションを登録する

OAuth を使用するには、アプリケーションにクライアントの ID と、アプリケーションを識別するアプリケーション URI が必要です。 Azure Active Directory サービスにアプリケーションをまだ登録していない場合は、「[アプリケーションを登録する](https://apps.dev.microsoft.com/#/appList)」の手順に従い、アプリケーションを手動で追加する必要があります。

<a name="bk_getToken"> </a>

## <a name="add-code-to-get-an-authentication-token"></a>認証トークンを取得するコードを追加する

Azure AD Authentication Library for .NET は、Azure Active Directory からの認証トークンの取得を簡略化するため、アプリケーションでトークンを利用できます。 4 つのトークンを取得するために、次の情報を提供する必要があります。
  
1. トークン サーバーの URI。トークン サーバーは、ユーザーを認証し、アプリケーションが EWS へのアクセスに使用できるトークンを返す**機関**です。 
    
2. Azure Active Directory にアプリケーションを登録するときに作成されたアプリケーションのクライアント ID。
    
3. Azure Active Directory にアプリケーションを登録するときに作成されたアプリケーションのクライアント URI。
    
4. EWS サーバーの URI と、EWS のエンドポイントの URI。 Office 365 の一部としての Exchange では、`https://<server name>/ews/exchange.asmx` のようになります。
    
次のコードでは、Azure の AD 認証ライブラリを使用して、認証トークンを取得する方法を示します。 認証要求を行うために必要な情報がアプリケーションの App.config ファイルに格納されていると仮定します。 この例では、エラー チェックは含まれません。完全なコードについては、[コード サンプル](#bk_codeSample)を参照してください。 
  
```cs
string authority = ConfigurationManager.AppSettings["authority"];
string clientID = ConfigurationManager.AppSettings["clientID"];
Uri clientAppUri = new Uri(ConfigurationManager.AppSettings["clientAppUri"];
string serverName = ConfigurationManager.AppSettings["serverName"];
AuthenticationContext authenticationContext = new AuthenticationContext(authority, false);
AuthenticationResult authenticationResult = authenticationContext.AcquireToken(serverName, clientId, clientAppUri);

```

<a name="bk_useToken"> </a>

## <a name="add-an-authentication-token-to-ews-requests"></a>EWS 要求に認証トークンを追加します。

**AuthenticationResult** オブジェクトを受信すると、**AccessToken** プロパティを使用して、トークン サービスによって発行されるトークンを取得できます。 
  
```cs
ExchangeService exchangeService = new ExchangeService(ExchangeVersion.Exchange2013);
exchangeService.Url = new Uri(ConfigurationManager.AppSettings["serverName"]+"ews/exchange.asmx");
exchangeService.TraceEnabled = true;
exchangeService.TraceFlags = TraceFlags.All;
exchangeService.Credentials = new OAuthCredentials(authenticationResult.AccessToken));
exchangeService.FindFolders(WellKnownFolderName.Root, new Folderview(10));
```

<a name="bk_codeSample"> </a>

## <a name="code-sample"></a>コード サンプル

以下の完全なコード サンプルでは、OAuth 認証が行われる EWS 要求を示します。
  
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

サンプル コードには、次のエントリを持つ App.config ファイルが必要です。
  
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

## <a name="see-also"></a>関連項目

- [Exchange における認証と EWS](authentication-and-ews-in-exchange.md)    

    


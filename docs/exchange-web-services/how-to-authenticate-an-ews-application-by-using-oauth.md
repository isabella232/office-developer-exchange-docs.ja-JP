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
# <a name="authenticate-an-ews-application-by-using-oauth"></a>OAuth を使用して、EWS アプリケーションを認証します。

EWS Managed API アプリケーションで、OAuth 認証を使用する方法について説明します。
  
Azure Active Directory が提供する OAuth の認証サービスを使用すると、Office 365 の他の Api で使用される同じ認証モデルでは、EWS のマネージ API アプリケーションを統合します。 アプリケーションで、OAuth を使用するには、必要があります。
  
1. Azure Active Directory と[アプリケーションの登録](#bk_register)をします。 
    
2. トークン サーバから認証トークンを取得する[認証トークンを取得するコードを追加](#bk_getToken)します。 
    
3. 送信する[EWS 要求に認証トークンを追加](#bk_useToken)します。 
    
> [!NOTE]
> EWS の OAuth 認証は、Office 365 の一部として Exchange でのみ利用可能です。EWS アプリケーションには、「ユーザーのメールボックスへのフル アクセス」権限が必要です。 
  
この記事のコードを使用するには、次に対するアクセス権が必要です。
  
- [Office 365 開発者アカウント](http://office.microsoft.com/compare-office-365-for-business-plans-FX102918419.aspx.aspx)です。 試用版のアカウントを使用するには、アプリケーションをテストするのには
    
- [.Net の Azure AD 認証ライブラリ](http://msdn.microsoft.com/en-us/library/office/jj573266.aspx.aspx)です。
    
- [EWS はマネージ API](https://github.com/officedev/ews-managed-api.aspx)です。

<a name="bk_register"> </a>

## <a name="register-your-application"></a>アプリケーションを登録する

OAuth を使用するには、アプリケーションは、クライアントの id と、アプリケーション、アプリケーションを識別する URI が必要です。 Azure Active ディレクトリ サービスとアプリケーションをまだ登録していない場合は、次の手順を実行[するアプリケーションを登録](http://msdn.microsoft.com/en-us/office/office365/howto/test-and-deploy-apps.aspx)して、アプリケーションを手動で追加する必要があります。

<a name="bk_getToken"> </a>

## <a name="add-code-to-get-an-authentication-token"></a>認証トークンを取得するコードを追加する

.NET では、Azure の AD 認証ライブラリでは、Azure Active Directory からの認証トークンの取得をアプリケーションにトークンを使用できるように簡単になります。 4 つのトークンを取得する情報を提供する必要があります。
  
1. トークン サーバの URI。 トークン サーバは、ユーザーを認証し、EWS にアクセスするアプリケーションが使用できるトークンを取得する**機関**です。 
    
2. Azure Active Directory にアプリケーションを登録するときに作成されたアプリケーションのクライアント ID。
    
3. Azure Active Directory にアプリケーションを登録するときに作成されたアプリケーションのクライアント URI。
    
4. EWS サーバーの URI と、EWS のエンドポイントの URI です。 Office 365 の一部として、Exchange になります`https://<server name>/ews/exchange.asmx`。
    
次のコードでは、Azure の AD 認証ライブラリを使用して、認証トークンを取得する方法を示します。 認証要求を行うために必要な情報がアプリケーションの App.config ファイルに格納されていることを仮定します。 この例では、エラー チェックが含まれます、完全なコードの[サンプル コード](#bk_codeSample)を参照してはいません。 
  
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

**AuthenticationResult**オブジェクトを受信した後は、トークン サービスによって発行されたトークンを取得するのには**AccessToken**プロパティを使用することができます。 
  
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

- [認証および Exchange での EWS](authentication-and-ews-in-exchange.md)    
- [テストし、Office 365 アプリケーションを展開します。](http://msdn.microsoft.com/en-us/office/office365/howto/test-and-deploy-apps.aspx)
    


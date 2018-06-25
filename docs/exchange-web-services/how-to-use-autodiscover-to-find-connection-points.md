---
title: 自動検出を使用してコネクション ポイントを検索するには
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 03896542-549b-4c45-973c-98f9025ea26c
description: 自動検出サービスを使用して、適切な Exchange サーバーにクライアント アプリケーションを指示する方法を確認します。
ms.openlocfilehash: 653fcd1c094c23c3e89e903b7194b96720802b51
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759069"
---
# <a name="use-autodiscover-to-find-connection-points"></a>自動検出を使用してコネクション ポイントを検索するには

自動検出サービスを使用して、適切な Exchange サーバーにクライアント アプリケーションを指示する方法を確認します。
  
Exchange 自動検出サービスは、Exchange Online、Office 365 の一部としての Exchange Online、または Exchange 2013 以降のバージョンの Exchange を実行する Exchange サーバー上でホストされているメール アカウントの構成設定をクライアント アプリケーションに提供します。自動検出サービスは、構成設定を提供する Web サービスです。自動検出サービスは、クライアント アプリケーションに Exchange サーバーの構成情報を提供する Web サービスです。クライアント アプリケーションは、自動検出を使用して、特定のメールボックスの自動検出サービスのエンドポイントを決定します。この記事では、Exchange サーバーからの応答に従って適切なエンドポイントを検索する方法について説明します。  
  
電子メール アドレスの構成設定を取得する方法の詳細については、[自動検出を使用して Exchange からのユーザー設定を取得](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)し、 [Exchange サーバーからドメインの設定](how-to-get-domain-settings-from-an-exchange-server.md)を参照してください。
  
> [!NOTE]
> 適切なエンドポイントを検索するプロセスは、ユーザーまたはドメイン設定の要求の一部です。自動検出サービスは、一連のリダイレクト応答を使用して、クライアント アプリケーションにメール アドレスの適切なエンドポイントを指示します。 
  
自動検出サービスにアクセスするには、次の Exchange 開発テクノロジのうちの 1 つを使用できます。
  
> [!NOTE]
> Exchange 開発テクノロジの詳細については、 [EWS のマネージ API のエクスプ ローラー、EWS、および web サービスの Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)を参照してください。 
  
- Exchange Web サービス (EWS) マネージ API
    
- EWS
    
    EWS を使用する場合は、次の方法を使用してユーザー設定を取得できます。
    
  - SOAP ベースの自動検出サービス
    
  - XML (POX) 自動検出サービス
    
  - SOAP または XML の自動検出サービスから生成される、自動生成されたプロキシ
    
    これらのメソッドの詳細については、 [Exchange の自動検出](autodiscover-for-exchange.md)を参照してください。
    
EWS マネージ API は、ユーザー設定を取得するためのオブジェクト ベースのインターフェイスを提供します。クライアント アプリケーションがマネージ コードを使用する場合は、EWS マネージ API を使用することをお勧めします。EWS マネージ API インターフェイスは、標準的な自動生成された Web サービス プロキシよりも、単純なオブジェクト モデルに対してより最適化されています。  
  
EWS を使用している場合は、POX の自動検出サービスよりも豊富な機能をサポートしている SOAP の自動検出サービスの使用をお勧めします。
  
## <a name="prerequisites-for-finding-an-endpoint"></a>エンドポイントを検索するための前提条件
<a name="bk_Prereq"> </a>

自動検出サービスを使用するクライアント アプリケーションを作成するには、次のものにアクセスできる必要があります。
  
- Exchange Online または Exchange 2007 SP1 以降のバージョンの Exchange を実行しているサーバー。SOAP ベースの自動検出サービスを使用している場合は、Exchange Online または Exchange 2010 以降のバージョンの Exchange。
    
- クライアント アプリケーションからの接続を受け付けるように構成されている Exchange サーバーです。 Exchange サーバーを構成する方法の詳細については、 [Exchange クライアント アプリケーションの EWS へのアクセスを制御する](controlling-client-application-access-to-ews-in-exchange.md)を参照してください。
    
- EWS を使用する権限を持つアカウントです。 アカウントを構成する方法の詳細については、 [Exchange クライアント アプリケーションの EWS へのアクセスを制御する](controlling-client-application-access-to-ews-in-exchange.md)を参照してください。
    
> [!NOTE]
> EWS のマネージ API を使用する場合は、状況によっては証明書の検証コールバックを入力しなければなりません。 Visual Studio によって作成されたものなどのいくつかのライブラリの生成されたプロキシで証明書の検証コールバックを必要することもあります。 詳細については、 [EWS のマネージ API のサーバー証明書の検証](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)を参照してください。 
  
### <a name="core-concepts-for-finding-an-endpoint"></a>エンドポイントを検索するための中心概念
<a name="bk_Core"> </a>

自動検出を使用してエンドポイントを検索する前に、次の表に一覧表示されている概念を理解する必要があります。
  
|**概念**|**説明**|
|:-----|:-----|
|[Exchange の自動検出](autodiscover-for-exchange.md) <br/> |自動検出サービスの動作方法の概要を示します。  <br/> |
   
EWS のマネージ API を使用する場合、 [Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/en-us/library/dd633907%28v=exchg.80%29.aspx)名前空間の EWS への接続を管理する[Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)クラスを使用します。 EWS のマネージ API のサンプル コードを使用して、この資料で、コード内で次の名前空間を参照する必要があります。 
  
- **System.Net**
    
- **Microsoft.Exchange.WebServices.Data.ExchangeService**
    
## <a name="find-the-correct-endpoint-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して、適切なエンドポイントを検索する
<a name="bk_Managed"> </a>

EWS のマネージ API を使用する場合、自動検出サービスへの呼び出しは、 **ExchangeService**クラスによって処理されます。 電子メール アカウント用の正しいエンドポイントを判断するのには、 **[ExchangeService]** オブジェクトの**AutodiscoverUrl**メソッドを呼び出します。 EWS のマネージ API を使用して、適切なクライアント アクセス サーバー上の Exchange.asmx ファイルに電子メール アドレスの EWS の web サービス エンドポイントを設定するのには次のコード例を次に示します。 
  
```cs
NetworkCredential credentials = new NetworkCredential(securelyStoredEmail, securelyStoredPassword);
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2013);
service.Credentials = credentials;
service.AutodiscoverUrl("User1@contoso.com");
```

## <a name="find-the-correct-endpoint-by-using-ews"></a>EWS を使用して、適切なエンドポイントを検索する
<a name="bk_SOAP"> </a>

SOAP の自動検出サービスでは、EWS の正しいエンドポイントをアプリケーションに指示するのに一連の要求と応答を使用できます。 電子メール アカウント用の正しいエンドポイントを決定するプロセスについては、 [Exchange の自動検出](autodiscover-for-exchange.md)を参照してください。 次の XML の例では、一連の要求と応答の正しいエンドポイントを検索するのには自動検出の SOAP 要求を行う場合に期待できることを表示します。
  
### <a name="soap-autodiscover-endpoint-request"></a>SOAP の自動検出エンドポイントの要求

次の例では、適切なエンドポイントを検索するために自動検出サービスに送信される XML 要求を示します。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://mail.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>User1@Contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>InternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsUrl</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

### <a name="soap-autodiscover-redirection-response"></a>SOAP 自動検出リダイレクト応答

自動検出サービスは、HTTP 302 リダイレクト応答と SOAP リダイレクト応答の 2 つのうち、いずれかのリダイレクト応答で応答する場合があります。Exchange サーバーからの応答が HTTP 302 リダイレクトである場合、クライアント アプリケーションはリダイレクトのアドレスが受入可能であることを検証してから、リダイレクト応答に従う必要があります。
  
> [!セキュリティに関するメモ]、リダイレクト応答を検証するための条件には、 [Exchange の自動検出](autodiscover-for-exchange.md)が参照してください。 
  
自動検出サービスは、[エラー コード](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx)要素の要素、 **UserResponse** 、によって示される、リダイレクト応答を返した場合、クライアント アプリケーションする必要があります要素を使用して**RedirectTarget**は新しい設定要求を作成リダイレクト応答に指定されたサーバーに送信されます。 サーバーからリダイレクト応答の例を次に示します。 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>682</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>RedirectAddress</ErrorCode>
            <ErrorMessage>Redirection address.</ErrorMessage>
            <RedirectTarget>User1@mail.Contoso.com</RedirectTarget>
            <UserSettingErrors />
            <UserSettings />
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>

```

リダイレクトを行った後は、クライアントはリダイレクト URL を使用して別の要求を準備します。次のコードは、リダイレクト応答から作成される要求の例を示します。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>User1@mail.Contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>InternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsUrl</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

**NoError**を設定し、要求されたが含まれている**UserResponse**の要素の[エラー コード](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx)要素を含む応答をサーバーが送信されますと、クライアント アプリケーションは、自動検出サービス用の正しいエンドポイントが指示されたが、ユーザー設定します。 のみ、要求されたユーザーの設定、 **InternalEwsUrl** **ExternalEwsUrl**が返されます。 次の使用例は、サーバーからの応答を示しています。 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>160</h:MajorBuildNumber>
      <h:MinorBuildNumber>4</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>NoError</ErrorCode>
            <ErrorMessage>No error.</ErrorMessage>
            <RedirectTarget i:nil="true" />
            <UserSettingErrors />
            <UserSettings>
              <UserSetting i:type="StringSetting">
                <Name>InternalEwsUrl</Name>
                <Value>https://server.Contoso.com/ews/exchange.asmx</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ExternalEwsUrl</Name>
                <Value>https://server.Contoso.com/ews/exchange.asmx</Value>
              </UserSetting>
            </UserSettings>
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a>次の手順
<a name="bk_Next"> </a>

自動検出プロセスに従ってエンドポイントを検索すると、要求されたドメインまたはユーザー設定が返されます。特定の設定を要求することについては、次の記事をご覧ください。
  
- [Exchange サーバーからドメインの設定を取得します。](how-to-get-domain-settings-from-an-exchange-server.md)
    
- [Exchange から自動検出を使用してユーザー設定を取得します。](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a>関連項目


- [EWS アプリケーションを設定します。](setting-up-your-ews-application.md)
    
- [Exchange の自動検出](autodiscover-for-exchange.md)
    
- [Exchange の自動検出 web サービスの参照](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)
    
- 
  [Exchange 用 EWS リファレンス](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    


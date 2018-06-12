---
title: Exchange サーバーからドメインの設定を取得します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 2f9acb81-5135-4f72-94e8-65c235d725e6
description: 自動検出サービスを使用して Exchange サーバーからドメインの設定を取得する方法について説明します。
ms.openlocfilehash: 0dd990cc82762936e7827115685ce0178eafb5ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758954"
---
# <a name="get-domain-settings-from-an-exchange-server"></a>Exchange サーバーからドメインの設定を取得します。

自動検出サービスを使用して Exchange サーバーからドメインの設定を取得する方法について説明します。
  
自動検出サービスを使用して、メール ドメインの構成情報を取得できます。自動検出サービスは、アプリケーションが特定のドメインの正しいサービス エンドポイントに接続するためのプロセスを提供します。
  
自動検出サービスにアクセスするには、次の開発テクノロジのうちのいずれかを使用できます。
  
- Exchange Web サービス (EWS) マネージ API
    
- EWS
    
    EWS を使用する場合は、次の方法を使用してユーザー設定を取得できます。
    
  - SOAP ベースの自動検出サービス
    
  - XML (POX) 自動検出サービス
    
  - SOAP または XML の自動検出サービスから生成される、自動生成されたプロキシ
    
    これらのメソッドの詳細については、 [Exchange の自動検出](autodiscover-for-exchange.md)を参照してください。
    
EWS マネージ API は、ユーザー設定を取得するためのオブジェクト ベースのインターフェイスを提供します。クライアント アプリケーションがマネージ コードを使用する場合は、EWS マネージ API を使用することをお勧めします。EWS マネージ API インターフェイスは、標準的な自動生成された Web サービス プロキシよりも、単純なオブジェクト モデルに対してより最適化されています。  
  
EWS を使用している場合は、POX の自動検出サービスよりも豊富な機能をサポートしている SOAP の自動検出サービスの使用をお勧めします。
  
自動検出サービスは、要求された構成設定のみを返します。次の表に、自動検出サービスが返すことができるドメインの構成設定の一覧を示します。
  
**表 1: ドメインの構成設定**

|**構成の設定**|**説明**|
|:-----|:-----|
|ExternalEwsUrl  <br/> |EWS の外部 URL。  <br/> |
|ExternalEwsVersion  <br/> |EWS URL をホストする Exchange Server のバージョン。  <br/> |
   
## <a name="prerequisites-for-getting-domain-settings"></a>ドメインの設定を取得するための前提条件
<a name="bk_Prereq"> </a>

ドメインの設定を取得するために自動検出サービスに接続するアプリケーションを作成する前に、次にアクセスできることを確認します。
  
- Exchange Online、Office 365 の一部としての Exchange Online、または Exchange 2007 以降のバージョンの Exchange を実行しているサーバー。EWS SOAP ベースの自動検出サービスを使用する場合は、Exchange 2010 以降のバージョンの Exchange を実行しているサーバー。
    
- クライアント アプリケーションからの接続を受け付けるように構成されている Exchange サーバーです。 Exchange サーバーを構成する方法の詳細については、 [Exchange クライアント アプリケーションの EWS へのアクセスを制御する](controlling-client-application-access-to-ews-in-exchange.md)を参照してください。
    
- EWS を使用する権限を持つアカウントです。 アカウントを構成する方法の詳細については、 [Exchange クライアント アプリケーションの EWS へのアクセスを制御する](controlling-client-application-access-to-ews-in-exchange.md)を参照してください。
    
> [!NOTE]
> EWS のマネージ API を使用する場合は、状況によっては証明書の検証コールバックを入力しなければなりません。 Visual Studio によって作成されたものなどのいくつかのライブラリの生成されたプロキシで証明書の検証コールバックを必要することもあります。 詳細については、 [EWS のマネージ API のサーバー証明書の検証](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)を参照してください。 
  
### <a name="core-concepts-for-getting-domain-settings"></a>ドメインの設定の取得に関する中心概念
<a name="bk_Core"> </a>

自動検出を使用してドメインの設定を取得する前に、次の表に一覧表示されている概念を理解する必要があります。
  
|**概念**|**説明**|
|:-----|:-----|
|[Exchange の自動検出](autodiscover-for-exchange.md) <br/> |自動検出サービスの動作方法の概要を示します。  <br/> |
|[自動検出を使用してコネクション ポイントを検索するには](how-to-use-autodiscover-to-find-connection-points.md) <br/> |クライアント アプリケーションを適切なサービス エンドポイントにリダイレクトするために自動検出サービスによって使用されるプロセスについて説明します。  <br/> |
   
EWS のマネージ API を使用する場合、 [Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/en-us/library/exchange/dd633907%28v=exchg.80%29.aspx)名前空間の EWS への接続を管理する[Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/en-us/library/exchange/dd635811%28v=exchg.80%29.aspx)クラスを使用します。 このセクションのコード例では、コードでは、次の名前空間を参照することを前提としています。 
  
- **System.Net**
    
- **Microsoft.Exchange.WebServices.Data.ExchangeService**
    
## <a name="get-domain-settings-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して、ドメインの設定を取得する
<a name="bk_Managed"> </a>

要求を生成するのに[Microsoft.Exchange.WebServices.Data.AutodiscoverService](http://msdn.microsoft.com/en-us/library/exchange/dd634321%28v=exchg.80%29.aspx)オブジェクトの[Microsoft.Exchange.WebServices.Data.AutodiscoverSettings.GetUserSettings](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx)メソッドを使用するには、EWS のマネージ API を使用する場合次の例のように、ドメインの構成情報を取得したとします。 この例では、使用可能なドメインの設定の一部だけを要求すると、およびサーバーから要求された設定のみが返されます。 
  
```cs
AutodiscoverService autodiscoverService = new AutodiscoverService("domain.contoso.com");
autodiscoverService.Credentials = new NetworkCredential("User1", "password", "domain.contoso.com");
// Submit a request and get the settings. The response contains only the
// settings that are requested, if they exist.
GetDomainSettingsResponse domainresponse = autodiscoverService.GetDomainSettings(
    "domain",
    ExchangeVersion.Exchang2013,
    DomainSettingName.ExternalEwsUrl,
    DomainSettingName.ExternalEwsVersion);
```

返されたコレクションを解析して、各キー/値ペアにアクセスできます。次の使用例は、返された各要素を解析し、各キー/値ペアの名前と値を表示する方法を示しています。
  
```cs
// Display each retrieved value. The settings are part of a key/value pair.
foreach (KeyValuePair<DomainSettingName, Object> domainsetting in domainresponse.Settings)
{
    Console.WriteLine(domainsetting.Key.ToString() + ": " + domainsetting.Value.ToString());
}
```

または、特定の設定の値を取得できます。 次の例では、 **ExternalEwsUrl**の設定、表示されます。 
  
```cs
// Display a specific setting, such as ExternalEwsUrl.
Console.WriteLine(domainresponse.Settings[DomainSettingName.ExternalEwsUrl]);
```

## <a name="get-user-settings-by-using-ews-soap-autodiscover"></a>EWS SOAP 自動検出を使用してユーザー設定を取得する
<a name="bk_SOAP"> </a>

次の例では、自動検出サービスから両方のドメインの設定を取得する SOAP XML 要求を示しています。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetDomainSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetDomainSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Domains>
          <a:Domain>domain</a:Domain>
        </a:Domains>
        <a:RequestedSettings>
          <a:Setting>ExternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsVersion</a:Setting>
        </a:RequestedSettings>
        <a:RequestedVersion>Exchange2013</a:RequestedVersion>
      </a:Request>
    </a:GetDomainSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>
```

次の例では、サーバーがクライアントからの要求を解析した後に返す XML 応答を示します。
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
          Autodiscover/Autodiscover/GetDomainSettingsResponse</a:Action>
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
    <GetDomainSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <DomainResponses>
          <DomainResponse>
            <ErrorCode>NoError</ErrorCode>
            <ErrorMessage>No error.</ErrorMessage>
            <DomainSettingErrors />
            <DomainSettings>
              <DomainSetting i:type="DomainStringSetting">
                <Name>ExternalEwsUrl</Name>
                <Value>https://failover.exchange.microsoft.com/ews/exchange.asmx</Value>
              </DomainSetting>
              <DomainSetting i:type="DomainStringSetting">
                <Name>ExternalEwsVersion</Name>
                <Value>15.00.0085.000</Value>
              </DomainSetting>
            </DomainSettings>
            <RedirectTarget i:nil="true" />
          </DomainResponse>
        </DomainResponses>
      </Response>
    </GetDomainSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a>次の手順
<a name="bk_Next"> </a>

ドメインの設定は、EWS に接続するときにクライアントが必要とする基本的な情報を提供します。この情報を使用して EWS に接続するか、またはサーバーからメール アカウントの追加の構成設定を取得することができます。詳細については、以下の記事をご覧ください。
  
- [Exchange から自動検出を使用してユーザー設定を取得します。](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a>関連項目


- [EWS アプリケーションを設定します。](setting-up-your-ews-application.md)
    
- [Exchange の自動検出 web サービスの参照](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)
    
- 
  [Exchange 用 EWS リファレンス](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    


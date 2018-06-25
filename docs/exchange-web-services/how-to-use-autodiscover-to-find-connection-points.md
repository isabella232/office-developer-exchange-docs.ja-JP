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
# <a name="use-autodiscover-to-find-connection-points"></a><span data-ttu-id="864ee-103">自動検出を使用してコネクション ポイントを検索するには</span><span class="sxs-lookup"><span data-stu-id="864ee-103">Use Autodiscover to find connection points</span></span>

<span data-ttu-id="864ee-104">自動検出サービスを使用して、適切な Exchange サーバーにクライアント アプリケーションを指示する方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="864ee-104">Find out how to use the Autodiscover service to direct your client application to the correct Exchange server.</span></span>
  
<span data-ttu-id="864ee-p101">Exchange 自動検出サービスは、Exchange Online、Office 365 の一部としての Exchange Online、または Exchange 2013 以降のバージョンの Exchange を実行する Exchange サーバー上でホストされているメール アカウントの構成設定をクライアント アプリケーションに提供します。自動検出サービスは、構成設定を提供する Web サービスです。自動検出サービスは、クライアント アプリケーションに Exchange サーバーの構成情報を提供する Web サービスです。クライアント アプリケーションは、自動検出を使用して、特定のメールボックスの自動検出サービスのエンドポイントを決定します。この記事では、Exchange サーバーからの応答に従って適切なエンドポイントを検索する方法について説明します。 </span><span class="sxs-lookup"><span data-stu-id="864ee-p101">The Exchange Autodiscover service provides your client application with configuration settings for email accounts that are hosted on Exchange Online, Exchange Online as part of Office 365, or an Exchange server running a version of Exchange starting with Exchange 2013. The Autodiscover service is a web service that provides configuration settings. The Autodiscover service is a web service that provides Exchange server configuration information to your client application. Client applications use Autodiscover to determine the endpoint of the Autodiscover service for a specific mailbox. This article explains how to follow the responses from an Exchange server to find the correct endpoint.</span></span> 
  
<span data-ttu-id="864ee-110">電子メール アドレスの構成設定を取得する方法の詳細については、[自動検出を使用して Exchange からのユーザー設定を取得](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)し、 [Exchange サーバーからドメインの設定](how-to-get-domain-settings-from-an-exchange-server.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="864ee-110">For information about how to get email address configuration settings, see [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) and [Get domain settings from an Exchange server](how-to-get-domain-settings-from-an-exchange-server.md).</span></span>
  
> [!NOTE]
> <span data-ttu-id="864ee-p102">適切なエンドポイントを検索するプロセスは、ユーザーまたはドメイン設定の要求の一部です。自動検出サービスは、一連のリダイレクト応答を使用して、クライアント アプリケーションにメール アドレスの適切なエンドポイントを指示します。</span><span class="sxs-lookup"><span data-stu-id="864ee-p102">The process for finding the correct endpoint is part of the request for user or domain settings. The Autodiscover service uses a series of redirect responses to send the client application to the correct endpoint for an email address.</span></span> 
  
<span data-ttu-id="864ee-113">自動検出サービスにアクセスするには、次の Exchange 開発テクノロジのうちの 1 つを使用できます。</span><span class="sxs-lookup"><span data-stu-id="864ee-113">You can use one of the following Exchange development technologies to access the Autodiscover service:</span></span>
  
> [!NOTE]
> <span data-ttu-id="864ee-114">Exchange 開発テクノロジの詳細については、 [EWS のマネージ API のエクスプ ローラー、EWS、および web サービスの Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="864ee-114">For more information about these Exchange development technologies, see [Explore the EWS Managed API, EWS, and web services in Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).</span></span> 
  
- <span data-ttu-id="864ee-115">Exchange Web サービス (EWS) マネージ API</span><span class="sxs-lookup"><span data-stu-id="864ee-115">The Exchange Web Services (EWS) Managed API</span></span>
    
- <span data-ttu-id="864ee-116">EWS</span><span class="sxs-lookup"><span data-stu-id="864ee-116">EWS</span></span>
    
    <span data-ttu-id="864ee-117">EWS を使用する場合は、次の方法を使用してユーザー設定を取得できます。</span><span class="sxs-lookup"><span data-stu-id="864ee-117">If you are using EWS, you can use the following methods to retrieve user settings:</span></span>
    
  - <span data-ttu-id="864ee-118">SOAP ベースの自動検出サービス</span><span class="sxs-lookup"><span data-stu-id="864ee-118">The SOAP-based Autodiscover service</span></span>
    
  - <span data-ttu-id="864ee-119">XML (POX) 自動検出サービス</span><span class="sxs-lookup"><span data-stu-id="864ee-119">The XML (POX) Autodiscover service</span></span>
    
  - <span data-ttu-id="864ee-120">SOAP または XML の自動検出サービスから生成される、自動生成されたプロキシ</span><span class="sxs-lookup"><span data-stu-id="864ee-120">An autogenerated proxy generated from the SOAP or XML Autodiscover service</span></span>
    
    <span data-ttu-id="864ee-121">これらのメソッドの詳細については、 [Exchange の自動検出](autodiscover-for-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="864ee-121">For more information about these methods, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span>
    
<span data-ttu-id="864ee-p103">EWS マネージ API は、ユーザー設定を取得するためのオブジェクト ベースのインターフェイスを提供します。クライアント アプリケーションがマネージ コードを使用する場合は、EWS マネージ API を使用することをお勧めします。EWS マネージ API インターフェイスは、標準的な自動生成された Web サービス プロキシよりも、単純なオブジェクト モデルに対してより最適化されています。 </span><span class="sxs-lookup"><span data-stu-id="864ee-p103">The EWS Managed API provides an object-based interface for retrieving user settings. If your client application uses managed code, we recommend that you use the EWS Managed API. The EWS Managed API interface is better optimized for a simple object model than the typical autogenerated web service proxy.</span></span> 
  
<span data-ttu-id="864ee-125">EWS を使用している場合は、POX の自動検出サービスよりも豊富な機能をサポートしている SOAP の自動検出サービスの使用をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="864ee-125">If you are using EWS, we suggest that you use the SOAP Autodiscover service, because it supports a richer set of features than the POX Autodiscover service.</span></span>
  
## <a name="prerequisites-for-finding-an-endpoint"></a><span data-ttu-id="864ee-126">エンドポイントを検索するための前提条件</span><span class="sxs-lookup"><span data-stu-id="864ee-126">Prerequisites for finding an endpoint</span></span>
<span data-ttu-id="864ee-127"><a name="bk_Prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="864ee-127"></span></span>

<span data-ttu-id="864ee-128">自動検出サービスを使用するクライアント アプリケーションを作成するには、次のものにアクセスできる必要があります。</span><span class="sxs-lookup"><span data-stu-id="864ee-128">Before you can create a client application that uses the Autodiscover service, you need to have access to the following:</span></span>
  
- <span data-ttu-id="864ee-p104">Exchange Online または Exchange 2007 SP1 以降のバージョンの Exchange を実行しているサーバー。SOAP ベースの自動検出サービスを使用している場合は、Exchange Online または Exchange 2010 以降のバージョンの Exchange。</span><span class="sxs-lookup"><span data-stu-id="864ee-p104">Exchange Online or a server that is running a version of Exchange starting with Exchange 2007 SP1. If you are using the SOAP-based Autodiscover service, Exchange Online or a version of Exchange starting with Exchange 2010.</span></span>
    
- <span data-ttu-id="864ee-131">クライアント アプリケーションからの接続を受け付けるように構成されている Exchange サーバーです。</span><span class="sxs-lookup"><span data-stu-id="864ee-131">An Exchange server that is configured to accept connections from your client application.</span></span> <span data-ttu-id="864ee-132">Exchange サーバーを構成する方法の詳細については、 [Exchange クライアント アプリケーションの EWS へのアクセスを制御する](controlling-client-application-access-to-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="864ee-132">For information about how to configure your Exchange server, see [Controlling client application access to EWS in Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span></span>
    
- <span data-ttu-id="864ee-133">EWS を使用する権限を持つアカウントです。</span><span class="sxs-lookup"><span data-stu-id="864ee-133">An account that is authorized to use EWS.</span></span> <span data-ttu-id="864ee-134">アカウントを構成する方法の詳細については、 [Exchange クライアント アプリケーションの EWS へのアクセスを制御する](controlling-client-application-access-to-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="864ee-134">For information about how to configure an account, see [Controlling client application access to EWS in Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span></span>
    
> [!NOTE]
> <span data-ttu-id="864ee-135">EWS のマネージ API を使用する場合は、状況によっては証明書の検証コールバックを入力しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="864ee-135">If you are using the EWS Managed API, you must provide a certificate validation callback in some circumstances.</span></span> <span data-ttu-id="864ee-136">Visual Studio によって作成されたものなどのいくつかのライブラリの生成されたプロキシで証明書の検証コールバックを必要することもあります。</span><span class="sxs-lookup"><span data-stu-id="864ee-136">You may also need a certificate validation callback with some generated proxy libraries, such as those created by Visual Studio.</span></span> <span data-ttu-id="864ee-137">詳細については、 [EWS のマネージ API のサーバー証明書の検証](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="864ee-137">For more information, see [Validate a server certificate for the EWS Managed API](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span> 
  
### <a name="core-concepts-for-finding-an-endpoint"></a><span data-ttu-id="864ee-138">エンドポイントを検索するための中心概念</span><span class="sxs-lookup"><span data-stu-id="864ee-138">Core concepts for finding an endpoint</span></span>
<span data-ttu-id="864ee-139"><a name="bk_Core"> </a></span><span class="sxs-lookup"><span data-stu-id="864ee-139"></span></span>

<span data-ttu-id="864ee-140">自動検出を使用してエンドポイントを検索する前に、次の表に一覧表示されている概念を理解する必要があります。</span><span class="sxs-lookup"><span data-stu-id="864ee-140">Before you use Autodiscover to find an endpoint, you should be familiar with the concepts listed in the following table.</span></span>
  
|<span data-ttu-id="864ee-141">**概念**</span><span class="sxs-lookup"><span data-stu-id="864ee-141">**Concept**</span></span>|<span data-ttu-id="864ee-142">**説明**</span><span class="sxs-lookup"><span data-stu-id="864ee-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="864ee-143">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="864ee-143">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md) <br/> |<span data-ttu-id="864ee-144">自動検出サービスの動作方法の概要を示します。</span><span class="sxs-lookup"><span data-stu-id="864ee-144">Provides an overview of how the Autodiscover service works.</span></span>  <br/> |
   
<span data-ttu-id="864ee-145">EWS のマネージ API を使用する場合、 [Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/en-us/library/dd633907%28v=exchg.80%29.aspx)名前空間の EWS への接続を管理する[Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)クラスを使用します。</span><span class="sxs-lookup"><span data-stu-id="864ee-145">If you are using the EWS Managed API, you use the [Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) class in the [Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/en-us/library/dd633907%28v=exchg.80%29.aspx) namespace to manage your connection to EWS.</span></span> <span data-ttu-id="864ee-146">EWS のマネージ API のサンプル コードを使用して、この資料で、コード内で次の名前空間を参照する必要があります。</span><span class="sxs-lookup"><span data-stu-id="864ee-146">To use the EWS Managed API code samples in this article, you need to reference the following namespaces in your code:</span></span> 
  
- <span data-ttu-id="864ee-147">**System.Net**</span><span class="sxs-lookup"><span data-stu-id="864ee-147">**System.Net**</span></span>
    
- <span data-ttu-id="864ee-148">**Microsoft.Exchange.WebServices.Data.ExchangeService**</span><span class="sxs-lookup"><span data-stu-id="864ee-148">**Microsoft.Exchange.WebServices.Data.ExchangeService**</span></span>
    
## <a name="find-the-correct-endpoint-by-using-the-ews-managed-api"></a><span data-ttu-id="864ee-149">EWS マネージ API を使用して、適切なエンドポイントを検索する</span><span class="sxs-lookup"><span data-stu-id="864ee-149">Find the correct endpoint by using the EWS Managed API</span></span>
<span data-ttu-id="864ee-150"><a name="bk_Managed"> </a></span><span class="sxs-lookup"><span data-stu-id="864ee-150"></span></span>

<span data-ttu-id="864ee-151">EWS のマネージ API を使用する場合、自動検出サービスへの呼び出しは、 **ExchangeService**クラスによって処理されます。</span><span class="sxs-lookup"><span data-stu-id="864ee-151">If you are using the EWS Managed API, calls to the Autodiscover service are handled by the **ExchangeService** class.</span></span> <span data-ttu-id="864ee-152">電子メール アカウント用の正しいエンドポイントを判断するのには、 **[ExchangeService]** オブジェクトの**AutodiscoverUrl**メソッドを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="864ee-152">To determine the correct endpoint for an email account, you call the **AutodiscoverUrl** method on an **[ExchangeService]** object.</span></span> <span data-ttu-id="864ee-153">EWS のマネージ API を使用して、適切なクライアント アクセス サーバー上の Exchange.asmx ファイルに電子メール アドレスの EWS の web サービス エンドポイントを設定するのには次のコード例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="864ee-153">The following code example shows how to set the EWS web service endpoint for an email address to the Exchange.asmx file on the correct Client Access server by using the EWS Managed API.</span></span> 
  
```cs
NetworkCredential credentials = new NetworkCredential(securelyStoredEmail, securelyStoredPassword);
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2013);
service.Credentials = credentials;
service.AutodiscoverUrl("User1@contoso.com");
```

## <a name="find-the-correct-endpoint-by-using-ews"></a><span data-ttu-id="864ee-154">EWS を使用して、適切なエンドポイントを検索する</span><span class="sxs-lookup"><span data-stu-id="864ee-154">Find the correct endpoint by using EWS</span></span>
<span data-ttu-id="864ee-155"><a name="bk_SOAP"> </a></span><span class="sxs-lookup"><span data-stu-id="864ee-155"></span></span>

<span data-ttu-id="864ee-156">SOAP の自動検出サービスでは、EWS の正しいエンドポイントをアプリケーションに指示するのに一連の要求と応答を使用できます。</span><span class="sxs-lookup"><span data-stu-id="864ee-156">The SOAP Autodiscover service may use a series of requests and responses to direct your application to the correct endpoint for EWS.</span></span> <span data-ttu-id="864ee-157">電子メール アカウント用の正しいエンドポイントを決定するプロセスについては、 [Exchange の自動検出](autodiscover-for-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="864ee-157">For information about the process for determining the correct endpoint for an email account, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span> <span data-ttu-id="864ee-158">次の XML の例では、一連の要求と応答の正しいエンドポイントを検索するのには自動検出の SOAP 要求を行う場合に期待できることを表示します。</span><span class="sxs-lookup"><span data-stu-id="864ee-158">The following XML examples show the series of requests and responses that you can expect when making a SOAP Autodiscover request to find the correct endpoint.</span></span>
  
### <a name="soap-autodiscover-endpoint-request"></a><span data-ttu-id="864ee-159">SOAP の自動検出エンドポイントの要求</span><span class="sxs-lookup"><span data-stu-id="864ee-159">SOAP Autodiscover endpoint request</span></span>

<span data-ttu-id="864ee-160">次の例では、適切なエンドポイントを検索するために自動検出サービスに送信される XML 要求を示します。</span><span class="sxs-lookup"><span data-stu-id="864ee-160">The following example shows an XML request that is sent to the Autodiscover service to find the correct endpoint.</span></span>
  
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

### <a name="soap-autodiscover-redirection-response"></a><span data-ttu-id="864ee-161">SOAP 自動検出リダイレクト応答</span><span class="sxs-lookup"><span data-stu-id="864ee-161">SOAP Autodiscover redirection response</span></span>

<span data-ttu-id="864ee-p111">自動検出サービスは、HTTP 302 リダイレクト応答と SOAP リダイレクト応答の 2 つのうち、いずれかのリダイレクト応答で応答する場合があります。Exchange サーバーからの応答が HTTP 302 リダイレクトである場合、クライアント アプリケーションはリダイレクトのアドレスが受入可能であることを検証してから、リダイレクト応答に従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="864ee-p111">The Autodiscover service may respond with one of two redirection responses: an HTTP 302 redirect, or a SOAP redirection response. If the response from the Exchange server is an HTTP 302 redirect, the client application should validate that the redirection address is acceptable and then follow the redirection response.</span></span>
  
> [!セキュリティに関するメモ]<span data-ttu-id="864ee-164">、リダイレクト応答を検証するための条件には、 [Exchange の自動検出](autodiscover-for-exchange.md)が参照してください。</span><span class="sxs-lookup"><span data-stu-id="864ee-164"> For criteria for validating a redirection response, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span> 
  
<span data-ttu-id="864ee-165">自動検出サービスは、[エラー コード](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx)要素の要素、 **UserResponse** 、によって示される、リダイレクト応答を返した場合、クライアント アプリケーションする必要があります要素を使用して**RedirectTarget**は新しい設定要求を作成リダイレクト応答に指定されたサーバーに送信されます。</span><span class="sxs-lookup"><span data-stu-id="864ee-165">If the Autodiscover service returns a redirection response, indicated by the [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) element of the **UserResponse** element, your client application should use the **RedirectTarget** element to construct a new settings request that is sent to the server specified in the redirection response.</span></span> <span data-ttu-id="864ee-166">サーバーからリダイレクト応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="864ee-166">The following example shows a redirection response from the server.</span></span> 
  
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

<span data-ttu-id="864ee-p113">リダイレクトを行った後は、クライアントはリダイレクト URL を使用して別の要求を準備します。次のコードは、リダイレクト応答から作成される要求の例を示します。</span><span class="sxs-lookup"><span data-stu-id="864ee-p113">After a redirection, the client uses the redirection URL to prepare another request. The following code shows an example of the request that you create from the redirection response.</span></span>
  
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

<span data-ttu-id="864ee-169">**NoError**を設定し、要求されたが含まれている**UserResponse**の要素の[エラー コード](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx)要素を含む応答をサーバーが送信されますと、クライアント アプリケーションは、自動検出サービス用の正しいエンドポイントが指示されたが、ユーザー設定します。</span><span class="sxs-lookup"><span data-stu-id="864ee-169">When the client application has been directed to the correct endpoint for the Autodiscover service, the server will send a response with the [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) element of the **UserResponse** element set to **NoError** and containing the requested user settings.</span></span> <span data-ttu-id="864ee-170">のみ、要求されたユーザーの設定、 **InternalEwsUrl** **ExternalEwsUrl**が返されます。</span><span class="sxs-lookup"><span data-stu-id="864ee-170">Only the requested user settings, **InternalEwsUrl** and **ExternalEwsUrl**, are returned.</span></span> <span data-ttu-id="864ee-171">次の使用例は、サーバーからの応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="864ee-171">The following example shows the response from the server.</span></span> 
  
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

## <a name="next-steps"></a><span data-ttu-id="864ee-172">次の手順</span><span class="sxs-lookup"><span data-stu-id="864ee-172">Next steps</span></span>
<span data-ttu-id="864ee-173"><a name="bk_Next"> </a></span><span class="sxs-lookup"><span data-stu-id="864ee-173"></span></span>

<span data-ttu-id="864ee-p115">自動検出プロセスに従ってエンドポイントを検索すると、要求されたドメインまたはユーザー設定が返されます。特定の設定を要求することについては、次の記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="864ee-p115">Finding the endpoint by following the Autodiscover process returns the requested domain or user settings. For information about making a request for specific settings, see the following articles:</span></span>
  
- [<span data-ttu-id="864ee-176">Exchange サーバーからドメインの設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="864ee-176">Get domain settings from an Exchange server</span></span>](how-to-get-domain-settings-from-an-exchange-server.md)
    
- [<span data-ttu-id="864ee-177">Exchange から自動検出を使用してユーザー設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="864ee-177">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a><span data-ttu-id="864ee-178">関連項目</span><span class="sxs-lookup"><span data-stu-id="864ee-178">See also</span></span>


- [<span data-ttu-id="864ee-179">EWS アプリケーションを設定します。</span><span class="sxs-lookup"><span data-stu-id="864ee-179">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)
    
- [<span data-ttu-id="864ee-180">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="864ee-180">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="864ee-181">Exchange の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="864ee-181">Autodiscover web service reference for Exchange</span></span>](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)
    
- <span data-ttu-id="864ee-182">
  [Exchange 用 EWS リファレンス](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="864ee-182">[EWS reference for Exchange](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)</span></span>
    


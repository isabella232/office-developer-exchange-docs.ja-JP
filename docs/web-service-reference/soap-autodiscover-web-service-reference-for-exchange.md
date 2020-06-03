---
title: Exchange 用 SOAP 自動検出 Web サービス リファレンス
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: Exchange の SOAP 自動検出サービスに関する参照情報を検索します。
ms.openlocfilehash: bfca8e8e260a6262d12542bd6834894a2375453f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468426"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="1f72e-103">Exchange 用 SOAP 自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="1f72e-103">SOAP Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="1f72e-104">Exchange の SOAP 自動検出サービスに関する参照情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="1f72e-104">Find reference information for the SOAP Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="1f72e-105">自動検出サービスは、アプリケーションが Exchange サーバーへの接続を作成するために使用する構成情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="1f72e-105">The Autodiscover service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="1f72e-106">SOAP 自動検出サービスを使用して、クライアントアプリケーションと Exchange サーバーの間でメッセージを送信し、アプリケーションが Exchange への接続に使用する設定を見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="1f72e-106">You can use the SOAP Autodiscover service to send messages between the client application and the Exchange server to locate the settings the application will use to connect to Exchange.</span></span> <span data-ttu-id="1f72e-107">POX 自動検出サービスとは異なり、SOAP 自動検出サービスは、多くのユーザーの設定についての自動検出要求をバッチ処理することを許可し、応答で返される設定をより細かく制御します。</span><span class="sxs-lookup"><span data-stu-id="1f72e-107">Unlike the POX Autodiscover service, the SOAP Autodiscover service allows for batched Autodiscover requests for many users' settings and more granular control over which settings are returned in the response.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="1f72e-108">Exchange Server 2010 以降のバージョンの Exchange を対象とするクライアントの場合、SOAP 自動検出サービスを使用することをお勧めします (POX 自動検出サービスではありません)。</span><span class="sxs-lookup"><span data-stu-id="1f72e-108">For clients that target versions of Exchange starting with Exchange Server 2010, we recommend that you use the SOAP Autodiscover service (instead of the POX Autodiscover service).</span></span> <span data-ttu-id="1f72e-109">Exchange 2007 を対象とするクライアントは、POX 自動検出サービスを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1f72e-109">Clients that target Exchange 2007 have to use the POX Autodiscover service.</span></span> <span data-ttu-id="1f72e-110">.NET Framework を使用するクライアントは、堅牢で十分にテストされた SOAP 自動検出クライアントを含んでいるため、EWS マネージ API を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="1f72e-110">We recommend that clients that use the .NET Framework use the EWS Managed API because it contains a robust and well-tested SOAP Autodiscover client.</span></span> <span data-ttu-id="1f72e-111">EWS マネージ API の詳細については、「 [Ews マネージ api クライアントアプリケーションの概要](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f72e-111">For more information about the EWS Managed API, see [Get started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="1f72e-112">このセクションでは、SOAP 自動検出要求のリダイレクト時にクライアントとサーバー間で送信される XML 要素、および応答で返されるユーザー設定について説明します。</span><span class="sxs-lookup"><span data-stu-id="1f72e-112">This section provides information about the XML elements that are sent between the client and server during SOAP Autodiscover request redirections and the user settings that are returned in a response.</span></span> <span data-ttu-id="1f72e-113">XML 要素リファレンスには、要素が表す内容の概要と、要素を含む可能性のある要素階層の説明が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1f72e-113">The XML element reference contains summaries of what the elements represent and a description of the potential element hierarchies that contain the element.</span></span> 
  
<span data-ttu-id="1f72e-114">このセクションの記事では、クライアントとサーバー間で送信される XML インスタンスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1f72e-114">The articles in this section describe the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="1f72e-115">これらの要素を記述するスキーマは、SOAP 自動検出サービスをホストするサーバーの仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1f72e-115">The schema that describes these elements can be found in the virtual directory of the server that hosts the SOAP Autodiscover service.</span></span>
  
<span data-ttu-id="1f72e-116">このセクションの WSDL 操作のトピックでは、操作の内容と操作の要求と応答の例について概要を説明します。</span><span class="sxs-lookup"><span data-stu-id="1f72e-116">The WSDL operation topics in this section provide an overview of what the operation does and operation request and response examples.</span></span> <span data-ttu-id="1f72e-117">提供されているバージョン情報を使用して、使用する機能が、実行している製品バージョンで利用できるかどうかを判断できます。</span><span class="sxs-lookup"><span data-stu-id="1f72e-117">You can use the version information provided to determine whether the features that you want to use are available in the product version that you are running.</span></span> <span data-ttu-id="1f72e-118">また、操作のトピックの例では、サーバーとの間で送受信される SOAP メッセージに含まれる XML の構造を理解するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="1f72e-118">The examples in the operation topics also help you to understand the structure of the XML that is included in the SOAP messages that are sent to and from the server.</span></span>
  
<span data-ttu-id="1f72e-119">このセクションでは、SOAP 自動検出サービスを使用して自動検出構成情報を取得するために使用されるメッセージの例と説明も示します。</span><span class="sxs-lookup"><span data-stu-id="1f72e-119">This section also provides examples and descriptions of the messages that are used to retrieve Autodiscover configuration information by using the SOAP Autodiscover service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="1f72e-120">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="1f72e-120">In this section</span></span>
<span data-ttu-id="1f72e-121"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="1f72e-121"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="1f72e-122">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f72e-122">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
    
- [<span data-ttu-id="1f72e-123">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f72e-123">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)
    
- [<span data-ttu-id="1f72e-124">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f72e-124">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
    
- [<span data-ttu-id="1f72e-125">Get組織の Relationshipsettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f72e-125">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)
    
- [<span data-ttu-id="1f72e-126">Exchange 2013 の SOAP 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="1f72e-126">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="1f72e-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="1f72e-127">See also</span></span>


- [<span data-ttu-id="1f72e-128">Exchange 用自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="1f72e-128">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="1f72e-129">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="1f72e-129">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="1f72e-130">自動検出を使用して接続ポイントを検索する</span><span class="sxs-lookup"><span data-stu-id="1f72e-130">Use Autodiscover to find connection points</span></span>](https://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [<span data-ttu-id="1f72e-131">自動検出を使用して Exchange からユーザー設定を取得する</span><span class="sxs-lookup"><span data-stu-id="1f72e-131">Get user settings from Exchange by using Autodiscover</span></span>](https://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [<span data-ttu-id="1f72e-132">Exchange サーバーからドメイン設定を取得する</span><span class="sxs-lookup"><span data-stu-id="1f72e-132">Get domain settings from an Exchange server</span></span>](https://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [<span data-ttu-id="1f72e-133">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="1f72e-133">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    


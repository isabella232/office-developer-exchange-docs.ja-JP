---
title: Exchange の自動検出 web サービスの参照が SOAP します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: Exchange SOAP の自動検出サービスに関するリファレンス情報を検索します。
ms.openlocfilehash: 1cb24a8667c71028f3dead78d9fa533dc9547a64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833514"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="a530f-103">Exchange の自動検出 web サービスの参照が SOAP します。</span><span class="sxs-lookup"><span data-stu-id="a530f-103">SOAP Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="a530f-104">Exchange SOAP の自動検出サービスに関するリファレンス情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="a530f-104">Find reference information for the SOAP Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="a530f-105">自動検出サービスは、Exchange サーバーへの接続を作成するアプリケーションで使用される構成情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="a530f-105">The Autodiscover service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="a530f-106">SOAP の自動検出サービスを使用すると、アプリケーションが Exchange への接続を使用して、設定を確認するのにには、クライアント アプリケーションと Exchange サーバー間でメッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="a530f-106">You can use the SOAP Autodiscover service to send messages between the client application and the Exchange server to locate the settings the application will use to connect to Exchange.</span></span> <span data-ttu-id="a530f-107">POX の自動検出サービスとは異なり SOAP の自動検出サービスは多くのユーザーの設定とより詳細に制御する設定は応答の自動検出要求のバッチ処理のことができます。</span><span class="sxs-lookup"><span data-stu-id="a530f-107">Unlike the POX Autodiscover service, the SOAP Autodiscover service allows for batched Autodiscover requests for many users' settings and more granular control over which settings are returned in the response.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a530f-108">バージョンの Exchange が Exchange Server 2010 で始まるを対象とするクライアントは、SOAP の自動検出サービスではなく、POX 自動検出サービス) を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="a530f-108">For clients that target versions of Exchange starting with Exchange Server 2010, we recommend that you use the SOAP Autodiscover service (instead of the POX Autodiscover service).</span></span> <span data-ttu-id="a530f-109">Exchange 2007 を対象とするクライアントでは、POX の自動検出サービスを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a530f-109">Clients that target Exchange 2007 have to use the POX Autodiscover service.</span></span> <span data-ttu-id="a530f-110">.NET Framework を使用して、クライアントは、堅牢で十分にテストされた自動検出の SOAP クライアントが含まれているため、EWS のマネージ API を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="a530f-110">We recommend that clients that use the .NET Framework use the EWS Managed API because it contains a robust and well-tested SOAP Autodiscover client.</span></span> <span data-ttu-id="a530f-111">EWS のマネージ API の詳細については、 [EWS のマネージ API のクライアント アプリケーションを使い始める](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a530f-111">For more information about the EWS Managed API, see [Get started with EWS Managed API client applications](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="a530f-112">このセクションでは、SOAP の自動検出要求のリダイレクトと、応答で返されるユーザーの設定中にクライアントとサーバー間で送信される XML 要素に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="a530f-112">This section provides information about the XML elements that are sent between the client and server during SOAP Autodiscover request redirections and the user settings that are returned in a response.</span></span> <span data-ttu-id="a530f-113">XML 要素の参照には、要素が表す内容の概要と要素が含まれている潜在的な要素階層の説明が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a530f-113">The XML element reference contains summaries of what the elements represent and a description of the potential element hierarchies that contain the element.</span></span> 
  
<span data-ttu-id="a530f-114">このセクションの記事では、クライアントとサーバー間で送信される XML インスタンスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="a530f-114">The articles in this section describe the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="a530f-115">これらの要素を記述するスキーマは、SOAP の自動検出サービスをホストしているサーバーの仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a530f-115">The schema that describes these elements can be found in the virtual directory of the server that hosts the SOAP Autodiscover service.</span></span>
  
<span data-ttu-id="a530f-116">どのような操作の概要についてはこのセクションのトピックでは、WSDL 操作と操作の要求と応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a530f-116">The WSDL operation topics in this section provide an overview of what the operation does and operation request and response examples.</span></span> <span data-ttu-id="a530f-117">使用する機能を実行している製品のバージョンで使用できるかどうかを判断するのにはバージョン情報を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="a530f-117">You can use the version information provided to determine whether the features that you want to use are available in the product version that you are running.</span></span> <span data-ttu-id="a530f-118">操作のトピックの例では、サーバーとの間に送信される SOAP メッセージに含まれる XML の構造を理解することができます。</span><span class="sxs-lookup"><span data-stu-id="a530f-118">The examples in the operation topics also help you to understand the structure of the XML that is included in the SOAP messages that are sent to and from the server.</span></span>
  
<span data-ttu-id="a530f-119">このセクションでは、SOAP の自動検出サービスを使用して、自動検出の構成情報を取得するために使用されるメッセージの説明や例も提供します。</span><span class="sxs-lookup"><span data-stu-id="a530f-119">This section also provides examples and descriptions of the messages that are used to retrieve Autodiscover configuration information by using the SOAP Autodiscover service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="a530f-120">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="a530f-120">In this section</span></span>
<span data-ttu-id="a530f-121"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="a530f-121"></span></span>

- [<span data-ttu-id="a530f-122">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a530f-122">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
    
- [<span data-ttu-id="a530f-123">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a530f-123">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)
    
- [<span data-ttu-id="a530f-124">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a530f-124">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
    
- [<span data-ttu-id="a530f-125">GetOrganizationRelationshipSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a530f-125">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)
    
- [<span data-ttu-id="a530f-126">Exchange 2013 の自動検出の XML 要素を SOAP</span><span class="sxs-lookup"><span data-stu-id="a530f-126">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="a530f-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="a530f-127">See also</span></span>


- [<span data-ttu-id="a530f-128">Exchange の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="a530f-128">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="a530f-129">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="a530f-129">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="a530f-130">自動検出を使用してコネクション ポイントを検索するには</span><span class="sxs-lookup"><span data-stu-id="a530f-130">Use Autodiscover to find connection points</span></span>](http://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [<span data-ttu-id="a530f-131">Exchange から自動検出を使用してユーザー設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="a530f-131">Get user settings from Exchange by using Autodiscover</span></span>](http://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [<span data-ttu-id="a530f-132">Exchange サーバーからドメインの設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="a530f-132">Get domain settings from an Exchange server</span></span>](http://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [<span data-ttu-id="a530f-133">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="a530f-133">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    


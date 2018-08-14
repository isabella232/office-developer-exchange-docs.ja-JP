---
title: Exchange の EWS クライアントの設計の概要
manager: sethgros
ms.date: 3/11/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: b26f67aa-7c66-4d7d-98b3-746f26ab37f4
description: Exchange 用に EWS で開発する場合の設計の考慮事項について説明します。
ms.openlocfilehash: 10e1c78bdd93dc5aede6e3f9337aa70b0214b770
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353904"
---
# <a name="ews-client-design-overview-for-exchange"></a><span data-ttu-id="2a740-103">Exchange の EWS クライアントの設計の概要</span><span class="sxs-lookup"><span data-stu-id="2a740-103">EWS client design overview for Exchange</span></span>

<span data-ttu-id="2a740-104">Exchange 用に EWS で開発する場合の設計の考慮事項について説明します。</span><span class="sxs-lookup"><span data-stu-id="2a740-104">Learn about the design considerations for developing with EWS for Exchange.</span></span> 
  
<span data-ttu-id="2a740-105">この記事では、Exchange Web サービス (EWS) アプリケーションの設計に関する概要情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="2a740-105">This article provides overview information about designing an Exchange Web Services (EWS) application.</span></span> <span data-ttu-id="2a740-106">この情報を使用して、EWS がアプリケーションに適した API であるかどうか、そして適している場合、どのような種類のクライアント実装を使用すべきかを判断することができます。</span><span class="sxs-lookup"><span data-stu-id="2a740-106">You can use this information to determine whether EWS is the right API for your application, and if so, what type of client implementation you should use.</span></span> <span data-ttu-id="2a740-107">また、この記事では、1 つのコード ベースで Office 365、Exchange Online、Exchange 2007 以降のバージョンの Exchange をターゲットにできるアプリケーションの設計に関するベスト プラクティス情報や、オンプレミスの Exchange サーバーと Exchange Online のどちらをターゲットにすべきかに関する重要な判断ポイントも提供しています。</span><span class="sxs-lookup"><span data-stu-id="2a740-107">This article provides overview information about designing an Exchange Web Services (EWS) application. You can use this information to determine whether EWS is the right API for your application, and if so, what type of client implementation you should use. This article also provides best practice information for designing applications that can target off365short, Exchange Online, and versions of Exchange starting with Exchange 2007, in one code base, and important decision points for targeting on-premises Exchange servers versus targeting Exchange Online.</span></span>
  
## <a name="is-ews-the-right-api-for-your-application"></a><span data-ttu-id="2a740-108">EWS は作成しようとしているアプリケーションに適した API か</span><span class="sxs-lookup"><span data-stu-id="2a740-108">Is EWS the right API for your application?</span></span>
<span data-ttu-id="2a740-109"><a name="IsEWSRight"> </a></span><span class="sxs-lookup"><span data-stu-id="2a740-109"></span></span>

<span data-ttu-id="2a740-110">アプリケーションの設計を開始する前に、EWS が用途に適した API であるかどうかを考慮することが重要です。</span><span class="sxs-lookup"><span data-stu-id="2a740-110">Before you begin to design your application, it is important to consider whether EWS is the right API for you.</span></span> <span data-ttu-id="2a740-111">Exchange Server または Exchange Online を対象に開発している場合、EWS は優先すべきクライアント アクセス技術です。</span><span class="sxs-lookup"><span data-stu-id="2a740-111">If you are developing against Exchange Server or Exchange Online, EWS is the preferred client access technology.</span></span> <span data-ttu-id="2a740-112">Exchange 2007 以降のバージョンの Exchange 用のクライアント アクセスの開発では、主に EWS に焦点が当てられてきました。</span><span class="sxs-lookup"><span data-stu-id="2a740-112">Client access development for versions of Exchange starting with Exchange 2007 has primarily been focused on EWS.</span></span> <span data-ttu-id="2a740-113">Outlook に実装されているクライアント アクセスの新機能は EWS を使用しています。これには、Exchange 2007 で導入された不在 (OOF) および空き時間の機能や、Exchange 2010 で導入されたメール ヒントと GetRooms 機能が含まれます。</span><span class="sxs-lookup"><span data-stu-id="2a740-113">New client access functionality that is implemented in Outlook uses EWS, including the Out of Office (OOF) and Availability features introduced in Exchange 2007, and the MailTips and Get Rooms functionality introduced in Exchange 2010.</span></span> <span data-ttu-id="2a740-114">これは、Exchange クライアント アプリケーションを開発する社内および社外のパートナーの両方に対して、EWS に集中的に投資していることを示すものです。</span><span class="sxs-lookup"><span data-stu-id="2a740-114">This represents a committed investment in EWS for both internal and external partners who develop Exchange client applications.</span></span>
  
<span data-ttu-id="2a740-p103">EWS は、Exchange クライアント アプリケーションの主なクライアント アクセス API です。ただし、場合によっては、クライアント アプリケーションの開発用として他の Exchange API を検討できます。たとえば、Exchange ActiveSync には、EWS と比較して次の利点があります。</span><span class="sxs-lookup"><span data-stu-id="2a740-p103">EWS is the primary client access API for your Exchange client applications. However, in some cases, you might consider other Exchange APIs for client application development. For example, Exchange ActiveSync provides the following advantages over EWS:</span></span>
  
- <span data-ttu-id="2a740-118">XML データ構造がトークン化されたので、Exchange ActiveSync はよりコンパクトなプロトコルになります。</span><span class="sxs-lookup"><span data-stu-id="2a740-118">The XML structure has been tokenized to make Exchange ActiveSync a more compact protocol.</span></span>  
- <span data-ttu-id="2a740-119">Exchange ActiveSync には、クライアントのアクセスを制御したり、その他の堅牢なエンタープライズ モバイル メッセージング ソリューションを提供したりするポリシー メカニズムが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2a740-119">Exchange ActiveSync contains a policy mechanism to control client access and to provide other robust enterprise mobile messaging solutions.</span></span>
    
> [!NOTE]
> <span data-ttu-id="2a740-120">Exchange ActiveSync クライアントを開発するには、ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="2a740-120">You need a license in order to develop Exchange ActiveSync clients.</span></span> <span data-ttu-id="2a740-121">Exchange ActiveSync と EWS の違いについては、[「Exchange ActiveSync と EWS のどちらかを選ぶ」](http://msdn.microsoft.com/ja-JP/library/dn144954%28v=exchg.140%29.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a740-121">You need a license in order to develop Exchange ActiveSync clients. To learn about the differences between Exchange ActiveSync and EWS, see [Choosing between Exchange ActiveSync and Exchange Web Services (EWS)http://msdn.microsoft.com/en-us/library/dn144954(v=exchg.140).aspx](http://msdn.microsoft.com/ja-JP/library/dn144954%28v=exchg.140%29.aspx).</span></span> 
  
<span data-ttu-id="2a740-p105">MAPI RPC over HTTP は、Exchange クライアントのアプリケーション用のもう 1 つのプログラミング オプションです。しかし、MAPI RPC over HTTP は、クライアントとサーバー間の通信に直感的なインターフェイスを提供しません。</span><span class="sxs-lookup"><span data-stu-id="2a740-p105">MAPI RPC over HTTP is another programmability option for Exchange client applications. However, MAPI RPC over HTTP does not provide an intuitive interface for communicating between clients and the server.</span></span>
  
<span data-ttu-id="2a740-124">Exchange 開発技術の詳細については、[「Exchange の EWS Managed API、EWS、および Web サービスについて学ぶ」](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a740-124">For more information about these Exchange development technologies, see [EWS Managed API, EWS, and web services in Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).</span></span>
  
## <a name="options-for-ews-client-development"></a><span data-ttu-id="2a740-125">EWS クライアント開発のためのオプション</span><span class="sxs-lookup"><span data-stu-id="2a740-125">Options for EWS client development</span></span>
<span data-ttu-id="2a740-126"><a name="EWSClientOptions"> </a></span><span class="sxs-lookup"><span data-stu-id="2a740-126"></span></span>

<span data-ttu-id="2a740-p106">EWS を使用して Exchange を対象に開発を行うためのいくつかのオプションがあります。最良のオプションは、開発プラットフォーム、ツール、使用可能な実装、組織のアプリケーションの要件によって異なります。EWS のクライアント アプリケーションを構築するために利用可能な 4 つの主要なオプションは、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2a740-p106">Several options are available for developing against Exchange by using EWS. The best option for you will depend on the development platform, tools, available implementations, and application requirements for your organization. The following are the four primary options that are available for building EWS client applications:</span></span>
  
- <span data-ttu-id="2a740-130">EWS マネージ API</span><span class="sxs-lookup"><span data-stu-id="2a740-130">The EWS Managed API</span></span>
- <span data-ttu-id="2a740-131">EWS Java API</span><span class="sxs-lookup"><span data-stu-id="2a740-131">The EWS Java API</span></span>
- <span data-ttu-id="2a740-132">EWS の自動生成されたプロキシ</span><span class="sxs-lookup"><span data-stu-id="2a740-132">The EWS autogenerated proxies</span></span>
- <span data-ttu-id="2a740-133">カスタム EWS クライアント API</span><span class="sxs-lookup"><span data-stu-id="2a740-133">A custom EWS client API</span></span>
    
### <a name="ews-managed-api"></a><span data-ttu-id="2a740-134">EWS マネージ AP</span><span class="sxs-lookup"><span data-stu-id="2a740-134">EWS Managed API</span></span>

<span data-ttu-id="2a740-135">[EWS マネージ API](http://aka.ms/ews-managed-api-readme) は、カスタム Web サービス クライアントです。</span><span class="sxs-lookup"><span data-stu-id="2a740-135">The [EWS Managed API](http://aka.ms/ews-managed-api-readme) is a custom web service client.</span></span> <span data-ttu-id="2a740-136">これは、.NET Framework アプリケーションのための標準的なクライアント アクセス API です。</span><span class="sxs-lookup"><span data-stu-id="2a740-136">It is the standard client access API for .NET Framework applications.</span></span> 
  
<span data-ttu-id="2a740-137">以下は、EWS マネージ API を使用する利点の一部です。</span><span class="sxs-lookup"><span data-stu-id="2a740-137">The following are some of the benefits of using the EWS Managed API:</span></span>
  
- <span data-ttu-id="2a740-138">直感的なオブジェクト モデルが用意されています。</span><span class="sxs-lookup"><span data-stu-id="2a740-138">It provides an intuitive object model.</span></span>   
- <span data-ttu-id="2a740-139">WSDL ファイルとスキーマ ファイルでのサービス記述の複雑さを軽減します。</span><span class="sxs-lookup"><span data-stu-id="2a740-139">It abstracts the complexities of the service description in the WSDL and schema files.</span></span>   
- <span data-ttu-id="2a740-140">クライアント側のビジネス ロジックが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2a740-140">It includes client-side business logic.</span></span>   
- <span data-ttu-id="2a740-141">Web 要求と応答や、オブジェクトのシリアル化と逆シリアル化を処理します。</span><span class="sxs-lookup"><span data-stu-id="2a740-141">It handles the web requests and responses and object serialization and deserialization.</span></span>   
- <span data-ttu-id="2a740-142">Microsoft によるサポートがあります。</span><span class="sxs-lookup"><span data-stu-id="2a740-142">It is Microsoft-supported.</span></span>
    
<span data-ttu-id="2a740-143">ただし、EWS マネージ API は、完全なソリューションではないことにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="2a740-143">Note, however, that the EWS Managed API is not a complete solution.</span></span> <span data-ttu-id="2a740-144">一部の機能は、EWS マネージ API では実装されていません。</span><span class="sxs-lookup"><span data-stu-id="2a740-144">When functionality that you might want to use is not implemented in the EWS Managed API.</span></span> <span data-ttu-id="2a740-145">EWS マネージ API は EWS のすべての機能を実装してはいませんが、次の理由により、クライアント アプリケーション開発の最良の選択肢になり得ます。</span><span class="sxs-lookup"><span data-stu-id="2a740-145">Note, however, that the EWS Managed API is not a complete solution. Some functionality is not implemented in the EWS Managed API.  Although the EWS Managed API doesn’t implement all EWS functionality, it might be the best choice for your client application development, for the following reasons:</span></span>
  
- <span data-ttu-id="2a740-146">開発に .NET Framework を使用できます。</span><span class="sxs-lookup"><span data-stu-id="2a740-146">You can use the .NET Framework for development.</span></span>
- <span data-ttu-id="2a740-147">EWS オブジェクト モデルの大部分に加えて、自動検出を実装しています。</span><span class="sxs-lookup"><span data-stu-id="2a740-147">It implements Autodiscover in addition to most parts of the EWS object model.</span></span>
- <span data-ttu-id="2a740-148">EWS と連携するためのクライアント側のビジネス ロジックが [ExchangeService](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) クラスで実装されています。</span><span class="sxs-lookup"><span data-stu-id="2a740-148">It implements client-side business logic for working with EWS, in the [ExchangeServicehttp://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) class.</span></span> 
    
<span data-ttu-id="2a740-149">次の理由のいずれかにより、EWS マネージ API ではなく EWS の Web サービス API を使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="2a740-149">You might choose to use the EWS web service API instead of the EWS Managed API for any of the following reasons:</span></span>
  
- <span data-ttu-id="2a740-150">アプリケーションが .NET Framework を使用しない場合。</span><span class="sxs-lookup"><span data-stu-id="2a740-150">Your application does not use the .NET Framework.</span></span> 
- <span data-ttu-id="2a740-151">EWS マネージ API のアセンブリを配布することを望まない場合。</span><span class="sxs-lookup"><span data-stu-id="2a740-151">You don’t want to distribute the EWS Managed API assembly.</span></span> 
- <span data-ttu-id="2a740-152">EWS マネージ API で実装されていない機能をアプリケーションで使用する場合。</span><span class="sxs-lookup"><span data-stu-id="2a740-152">Your application uses features that aren’t implemented in the EWS Managed API.</span></span>
    
<span data-ttu-id="2a740-153">詳細については、「[EWS マネージ API クライアント アプリケーションの概要](get-started-with-ews-managed-api-client-applications.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2a740-153">To learn more, see [Get started with EWS Managed API client applications](get-started-with-ews-managed-api-client-applications.md).</span></span>
  
> [!NOTE]
> <span data-ttu-id="2a740-154">EWS マネージ API は、[GitHub](http://aka.ms/ews-managed-api-github) でオープンソース プロジェクトとして利用可能になりました。</span><span class="sxs-lookup"><span data-stu-id="2a740-154">The EWS Managed API is now available as an open source project on  GitHub http://aka.ms/ews-managed-api-github . You can use the open source library to:</span></span> <span data-ttu-id="2a740-155">オープン ソース ライブラリを使用して、以下のことができます。</span><span class="sxs-lookup"><span data-stu-id="2a740-155">You can use the open source library to:</span></span> 
> - <span data-ttu-id="2a740-156">バグ修正と API の機能強化に貢献します。</span><span class="sxs-lookup"><span data-stu-id="2a740-156">Contribute bug fixes and enhancements to the API.</span></span> 
> - <span data-ttu-id="2a740-157">公式のリリースで利用可能になる前に、修正プログラムや拡張機能を取得できます。</span><span class="sxs-lookup"><span data-stu-id="2a740-157">Get fixes and enhancements before they are available in an official release.</span></span>
> - <span data-ttu-id="2a740-158">API の最も包括的かつ最新の実装にアクセスして、参照として使用するか、新しいプラットフォームで新しいライブラリを作成します。</span><span class="sxs-lookup"><span data-stu-id="2a740-158">Access the most comprehensive and up-to-date implementation of the API, to use as a reference or to create new libraries on new platforms.</span></span>
> 
> <span data-ttu-id="2a740-159">GitHub を通した皆様の[貢献](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md)を歓迎いたします。</span><span class="sxs-lookup"><span data-stu-id="2a740-159">We welcome your [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span></span> 
  
### <a name="ews-java-api"></a><span data-ttu-id="2a740-160">EWS Java API</span><span class="sxs-lookup"><span data-stu-id="2a740-160">EWS Java API</span></span>

<span data-ttu-id="2a740-161">EWS Java API は、コミュニティが更新および拡張できる [GitHub](https://github.com/OfficeDev/ews-java-api) のオープン ソース プロジェクトです。</span><span class="sxs-lookup"><span data-stu-id="2a740-161">The EWS Java API is an open source project on [GitHub](https://github.com/OfficeDev/ews-java-api) that can be updated and extended by the community.</span></span> <span data-ttu-id="2a740-162">形式的には [EWS マネージ API](http://msdn.microsoft.com/ja-JP/library/office/jj220535%28v=exchg.80%29.aspx) と似ており、EWS SOAP 要求と応答をネットワーク経由で使用します。</span><span class="sxs-lookup"><span data-stu-id="2a740-162">It is stylistically similar to the [EWS Managed API](http://msdn.microsoft.com/ja-JP/library/office/jj220535%28v=exchg.80%29.aspx) and uses EWS SOAP requests and responses over the wire.</span></span> <span data-ttu-id="2a740-163">EWS Java API を使用してすべての [EWS SOAP 操作](http://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx)にアクセスできるわけではありませんが、[最近作成された](http://blogs.office.com/2014/08/28/open-sourcing-exchange-web-services-ews-java-api/)オープン ソース プロジェクトにより、コミュニティがこのギャップを埋めることが期待されます。</span><span class="sxs-lookup"><span data-stu-id="2a740-163">Although you can't access all [EWS SOAP operations](http://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) by using the EWS Java API, with the [recent creation](http://blogs.office.com/2014/08/28/open-sourcing-exchange-web-services-ews-java-api/) of the open source project, we are looking to the community to bridge this gap.</span></span> <span data-ttu-id="2a740-164">Microsoft サポートは、適切なサポート契約がある場合に、EWS SOAP プロトコルに関連する質問には対応しますが、EWS Java API 自体に関連する質問には対応しないことにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="2a740-164">Note that Microsoft Support, with an appropriate support contract, will address any questions related to the EWS SOAP protocol but not the EWS Java API itself.</span></span> <span data-ttu-id="2a740-165">[GitHub](https://github.com/OfficeDev/ews-java-api) で EWS Java API をダウンロードしたり、そのコミュニティに貢献したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="2a740-165">The EWS Java API is available for download and community contribution on [GitHub](https://github.com/OfficeDev/ews-java-api).</span></span>
  
### <a name="ews-autogenerated-proxies"></a><span data-ttu-id="2a740-166">EWS の自動生成されたプロキシ</span><span class="sxs-lookup"><span data-stu-id="2a740-166">EWS autogenerated proxies</span></span>

<span data-ttu-id="2a740-p111">自動生成されたクライアント API は、EWS の WSDL および XML スキーマ定義から生成されます。多くの言語でクライアント オブジェクト モデルのジェネレーターが用意されています。一般に、自動生成されたオブジェクト モデルは、オブジェクトのシリアル化および逆シリアル化を管理します。これにビジネス ロジックは含まれておらず、自動生成プロセスによって成果物が作成される結果、直感的には使用しにくいオブジェクト モデルになることが少なくありません。Exchange のサポートはクライアントによって送受信される XML を対象としますが、オブジェクト モデルは対象となりません。</span><span class="sxs-lookup"><span data-stu-id="2a740-p111">Autogenerated client APIs are generated from the EWS WSDL and XML schema definitions. Client object model generators are available for many languages. In general, the autogenerated object models manage object serialization and deserialization. They do not include business logic and the autogeneration process often creates artifacts that make the object model less intuitive to use. Exchange support covers the XML that is sent and received by the client but not the object model.</span></span>
  
### <a name="custom-ews-client-api"></a><span data-ttu-id="2a740-172">カスタム EWS クライアント API</span><span class="sxs-lookup"><span data-stu-id="2a740-172">Custom EWS client API</span></span>

<span data-ttu-id="2a740-p112">EWS 機能の小さなセットを使用する一部のアプリケーション用に、Exchange と通信するためのカスタム クライアント API を作成できます。これにより、使用するシステム リソースが少なくなります。これは、.NET Micro Framework を実行するクライアントなど、メモリに制約のあるデバイス上で実行されるクライアントに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="2a740-p112">For some applications that use a small set of EWS functionality, you might create a custom client API to communicate with Exchange. This enables you to consume fewer system resources. This is useful for clients that run on memory-constrained devices, such as clients running the .NET Micro Framework.</span></span>
  
## <a name="ews-client-features"></a><span data-ttu-id="2a740-176">EWS のクライアント機能</span><span class="sxs-lookup"><span data-stu-id="2a740-176">EWS client features</span></span>
<span data-ttu-id="2a740-177"><a name="EWSFeatures"> </a></span><span class="sxs-lookup"><span data-stu-id="2a740-177"></span></span>

<span data-ttu-id="2a740-p113">どの開発オプションを選ぶにせよ、EWS 機能をクライアントでどのように実装するかをご検討ください。機能が使用可能かどうかは、アプリケーションが対象とする EWS のスキーマのバージョン次第です。EWS のスキーマは後方互換性と前方互換性を持つため、Exchange Server 2007 SP1 などの以前のバージョンのスキーマを対象とするアプリケーションを作成する場合、アプリケーションは Exchange Server 2013 SP1 のサービスや Exchange Online など、後のバージョンのスキーマでも動作します。 </span><span class="sxs-lookup"><span data-stu-id="2a740-p113">Regardless of the development option that you choose, you should consider how EWS features are implemented in your client. Feature availability is based on the EWS schema version that your application targets. Because EWS schemas are backward- and forward-compatible, if you create an application that targets an earlier schema version, such as Exchange Server 2007 SP1, your application will also work against a later schema version, such as the Exchange Server 2013 SP1 service, as well as Exchange Online.</span></span> 
  
<span data-ttu-id="2a740-p114">機能および機能の更新はスキーマによって決定されるため、クライアント アプリケーションに実装する EWS 機能を対象としているもののうち、最も古い共通のコード ベースを使用することをお勧めします。多くのアプリケーションは Exchange2007_SP1 バージョンを対象にできます。なぜなら、Exchange 2007 SP1 のスキーマには、Exchange のストアのアイテムやフォルダーを操作するための Exchange のほとんどすべての主要機能が含まれているためです。EWS のスキーマのバージョンごとに、コードの分岐を維持することをお勧めします。現在利用可能なスキーマのバージョンを次に示します。</span><span class="sxs-lookup"><span data-stu-id="2a740-p114">Because features and feature updates are driven by the schema, we recommend that you use the earliest common code base that targets the EWS features that you want to implement in your client application. Many applications can target the Exchange2007_SP1 version, because the Exchange 2007 SP1 schema contains almost all the core Exchange functionality for working with items and folders in the Exchange store. We recommend that you maintain code forks for each EWS schema version. The following are the schema versions that are currently available.</span></span> 
  
```XML
  <xs:simpleType name="ExchangeVersionType">
    <xs:restriction base="xs:string">
      <xs:enumeration value="Exchange2007" />
      <xs:enumeration value="Exchange2007_SP1" />
      <xs:enumeration value="Exchange2010" />
      <xs:enumeration value="Exchange2010_SP1" />
      <xs:enumeration value="Exchange2010_SP2" />
      <xs:enumeration value="Exchange2013" />
      <xs:enumeration value="Exchange2013_SP1" />
    </xs:restriction>
  </xs:simpleType>
```

<span data-ttu-id="2a740-185">スキーマのバージョンは **ExchangeVersionType** の単純型で保持されます。</span><span class="sxs-lookup"><span data-stu-id="2a740-185">The schema versions are maintained in the **ExchangeVersionType** simple type.</span></span> 
  
<span data-ttu-id="2a740-186">EWS スキーマの各バージョンで利用可能な機能については、「[Exchange の EWS スキーマのバージョン](ews-schema-versions-in-exchange.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2a740-186">For information about the features that are available in each EWS schema version, see [EWS schema versions in Exchange](ews-schema-versions-in-exchange.md).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="2a740-187">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="2a740-187">In this section</span></span>
<span data-ttu-id="2a740-188"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="2a740-188"></span></span>

- [<span data-ttu-id="2a740-189">Exchange および EWS Managed API の Web サービス API 機能の可用性</span><span class="sxs-lookup"><span data-stu-id="2a740-189">Web service API feature availability in Exchange and the EWS Managed API</span></span>](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)   
- [<span data-ttu-id="2a740-190">Exchange の EWS スキーマのバージョン</span><span class="sxs-lookup"><span data-stu-id="2a740-190">EWS schema versions in Exchange</span></span>](ews-schema-versions-in-exchange.md)  
- [<span data-ttu-id="2a740-191">Exchange 内の EWS の構成オプション</span><span class="sxs-lookup"><span data-stu-id="2a740-191">Configuration options for EWS in Exchange</span></span>](configuration-options-for-ews-in-exchange.md)  
- [<span data-ttu-id="2a740-192">Exchange Online と Exchange オンプレミス クライアント プログラミングの比較</span><span class="sxs-lookup"><span data-stu-id="2a740-192">Comparing Exchange Online and Exchange on-premises client programming</span></span>](comparing-exchange-online-and-exchange-on-premises-client-programming.md)   
- [<span data-ttu-id="2a740-193">Exchange での EWS 調整</span><span class="sxs-lookup"><span data-stu-id="2a740-193">EWS throttling in Exchange</span></span>](ews-throttling-in-exchange.md)  
- [<span data-ttu-id="2a740-194">EWS マネージ API の再配布の要件</span><span class="sxs-lookup"><span data-stu-id="2a740-194">Redistribution requirements for the EWS Managed API</span></span>](redistribution-requirements-for-the-ews-managed-api.md)  
- [<span data-ttu-id="2a740-195">Exchange で EWS と REST のクライアントの要求をインストルメント化する</span><span class="sxs-lookup"><span data-stu-id="2a740-195">Instrumenting client requests for EWS and REST in Exchange</span></span>](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="2a740-196">関連項目</span><span class="sxs-lookup"><span data-stu-id="2a740-196">See also</span></span>
 
- [<span data-ttu-id="2a740-197">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="2a740-197">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
- [<span data-ttu-id="2a740-198">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="2a740-198">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md) 
- [<span data-ttu-id="2a740-199">EWS アプリケーションの種類</span><span class="sxs-lookup"><span data-stu-id="2a740-199">EWS application types</span></span>](ews-application-types.md)
    


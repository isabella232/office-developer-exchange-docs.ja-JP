---
title: Exchange の EWS クライアントの設計の概要
manager: sethgros
ms.date: 3/11/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: b26f67aa-7c66-4d7d-98b3-746f26ab37f4
description: 'Exchange 用に EWS で開発する場合の設計の考慮事項について説明します。  '
ms.openlocfilehash: ea0e1ad3f8402d19a6163f3320a2a17f08f3ea2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758895"
---
# <a name="ews-client-design-overview-for-exchange"></a><span data-ttu-id="6b6e3-103">Exchange の EWS クライアントの設計の概要</span><span class="sxs-lookup"><span data-stu-id="6b6e3-103">EWS client design overview for Exchange</span></span>

<span data-ttu-id="6b6e3-104">Exchange 用に EWS で開発する場合の設計の考慮事項について説明します。  </span><span class="sxs-lookup"><span data-stu-id="6b6e3-104">Learn about the design considerations for developing with EWS for Exchange.</span></span> 
  
<span data-ttu-id="6b6e3-105">この資料では、Exchange Web サービス (EWS) アプリケーションの設計に関する概要情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-105">This article provides overview information about designing an Exchange Web Services (EWS) application.</span></span> <span data-ttu-id="6b6e3-106">EWS では、アプリケーションの右側の API と、使用する必要がある場合は、どのようなタイプのクライアントの実装かどうか確認するのには、この情報を使用できます。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-106">You can use this information to determine whether EWS is the right API for your application, and if so, what type of client implementation you should use.</span></span> <span data-ttu-id="6b6e3-107">この資料も用意されています Office 365、オンラインの Exchange および Exchange のバージョンを対象とするアプリケーションを設計するためのベスト プラクティス情報 Exchange 2007 では、基本、1 つのコードで、オンプレミスの Exchange を対象とするための重要な意思決定ポイントで始まるサーバーは Exchange Online を対象とするとします。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-107">This article also provides best practice information for designing applications that can target Office 365, Exchange Online, and versions of Exchange starting with Exchange 2007, in one code base, and important decision points for targeting on-premises Exchange servers versus targeting Exchange Online.</span></span>
  
## <a name="is-ews-the-right-api-for-your-application"></a><span data-ttu-id="6b6e3-108">EWS は作成しようとしているアプリケーションに適した API か</span><span class="sxs-lookup"><span data-stu-id="6b6e3-108">Is EWS the right API for your application?</span></span>
<span data-ttu-id="6b6e3-109"><a name="IsEWSRight"> </a></span><span class="sxs-lookup"><span data-stu-id="6b6e3-109"></span></span>

<span data-ttu-id="6b6e3-110">アプリケーションの設計を開始する前にすることが重要 EWS が右の API であるかを考慮します。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-110">Before you begin to design your application, it is important to consider whether EWS is the right API for you.</span></span> <span data-ttu-id="6b6e3-111">Exchange Server または Exchange Online を開発している場合 EWS は、優先するクライアントのアクセス技術です。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-111">If you are developing against Exchange Server or Exchange Online, EWS is the preferred client access technology.</span></span> <span data-ttu-id="6b6e3-112">EWS 上のバージョンの Exchange が Exchange 2007 以降のクライアント アクセスの開発が主されています。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-112">Client access development for versions of Exchange starting with Exchange 2007 has primarily been focused on EWS.</span></span> <span data-ttu-id="6b6e3-113">Outlook に実装されているクライアント アクセスの新機能は、Exchange 2007 で導入された Office (OOF) と可用性の機能など、Exchange 2010 で導入されたメール ヒントとルームの取得機能、EWS を使用します。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-113">New client access functionality that is implemented in Outlook uses EWS, including the Out of Office (OOF) and Availability features introduced in Exchange 2007, and the MailTips and Get Rooms functionality introduced in Exchange 2010.</span></span> <span data-ttu-id="6b6e3-114">これは、Exchange クライアントのアプリケーションを開発している内部および外部の両方のパートナーの EWS でコミット投資を表します。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-114">This represents a committed investment in EWS for both internal and external partners who develop Exchange client applications.</span></span>
  
<span data-ttu-id="6b6e3-p103">EWS は、Exchange クライアント アプリケーションの主なクライアント アクセス API です。ただし、場合によっては、クライアント アプリケーションの開発用として他の Exchange API を検討できます。たとえば、Exchange ActiveSync には、EWS と比較して次の利点があります。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-p103">EWS is the primary client access API for your Exchange client applications. However, in some cases, you might consider other Exchange APIs for client application development. For example, Exchange ActiveSync provides the following advantages over EWS:</span></span>
  
- <span data-ttu-id="6b6e3-118">XML データ構造がトークン化されたので、Exchange ActiveSync はよりコンパクトなプロトコルになります。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-118">The XML structure has been tokenized to make Exchange ActiveSync a more compact protocol.</span></span>  
- <span data-ttu-id="6b6e3-119">Exchange ActiveSync には、クライアントのアクセスを制御したり、その他の堅牢なエンタープライズ モバイル メッセージング ソリューションを提供したりするポリシー メカニズムが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-119">Exchange ActiveSync contains a policy mechanism to control client access and to provide other robust enterprise mobile messaging solutions.</span></span>
    
> [!NOTE]
> <span data-ttu-id="6b6e3-120">Exchange ActiveSync クライアントを開発するためにライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-120">You need a license in order to develop Exchange ActiveSync clients.</span></span> <span data-ttu-id="6b6e3-121">Exchange ActiveSync と EWS の違いについては、 [Exchange ActiveSync と Exchange Web サービス (EWS) との間の選択](http://msdn.microsoft.com/ja-jp/library/dn144954%28v=exchg.140%29.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-121">To learn about the differences between Exchange ActiveSync and EWS, see [Choosing between Exchange ActiveSync and Exchange Web Services (EWS)](http://msdn.microsoft.com/ja-jp/library/dn144954%28v=exchg.140%29.aspx).</span></span> 
  
<span data-ttu-id="6b6e3-p105">MAPI RPC over HTTP は、Exchange クライアントのアプリケーション用のもう 1 つのプログラミング オプションです。しかし、MAPI RPC over HTTP は、クライアントとサーバー間の通信に直感的なインターフェイスを提供しません。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-p105">MAPI RPC over HTTP is another programmability option for Exchange client applications. However, MAPI RPC over HTTP does not provide an intuitive interface for communicating between clients and the server.</span></span>
  
<span data-ttu-id="6b6e3-124">Exchange 開発テクノロジに関する詳細については、 [EWS のマネージ API のエクスプ ローラー、EWS、および web サービスの Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-124">For more information about Exchange development technologies, see [Explore the EWS Managed API, EWS, and web services in Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).</span></span>
  
## <a name="options-for-ews-client-development"></a><span data-ttu-id="6b6e3-125">EWS クライアント開発のためのオプション</span><span class="sxs-lookup"><span data-stu-id="6b6e3-125">Options for EWS client development</span></span>
<span data-ttu-id="6b6e3-126"><a name="EWSClientOptions"> </a></span><span class="sxs-lookup"><span data-stu-id="6b6e3-126"></span></span>

<span data-ttu-id="6b6e3-p106">EWS を使用して Exchange を対象に開発を行うためのいくつかのオプションがあります。最良のオプションは、開発プラットフォーム、ツール、使用可能な実装、組織のアプリケーションの要件によって異なります。EWS のクライアント アプリケーションを構築するために利用可能な 4 つの主要なオプションは、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-p106">Several options are available for developing against Exchange by using EWS. The best option for you will depend on the development platform, tools, available implementations, and application requirements for your organization. The following are the four primary options that are available for building EWS client applications:</span></span>
  
- <span data-ttu-id="6b6e3-130">EWS マネージ API</span><span class="sxs-lookup"><span data-stu-id="6b6e3-130">The EWS Managed API</span></span>
- <span data-ttu-id="6b6e3-131">EWS Java API</span><span class="sxs-lookup"><span data-stu-id="6b6e3-131">The EWS Java API</span></span>
- <span data-ttu-id="6b6e3-132">EWS の自動生成されたプロキシ</span><span class="sxs-lookup"><span data-stu-id="6b6e3-132">The EWS autogenerated proxies</span></span>
- <span data-ttu-id="6b6e3-133">カスタム EWS クライアント API</span><span class="sxs-lookup"><span data-stu-id="6b6e3-133">A custom EWS client API</span></span>
    
### <a name="ews-managed-api"></a><span data-ttu-id="6b6e3-134">EWS Managed API</span><span class="sxs-lookup"><span data-stu-id="6b6e3-134">EWS Managed API</span></span>

<span data-ttu-id="6b6e3-135">[EWS のマネージ API](http://aka.ms/ews-managed-api-readme)は、カスタム web サービス クライアントです。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-135">The [EWS Managed API](http://aka.ms/ews-managed-api-readme) is a custom web service client.</span></span> <span data-ttu-id="6b6e3-136">.NET Framework アプリケーションの標準的なクライアント アクセス API です。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-136">It is the standard client access API for .NET Framework applications.</span></span> 
  
<span data-ttu-id="6b6e3-137">以下は、EWS マネージ API を使用する利点の一部です。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-137">The following are some of the benefits of using the EWS Managed API:</span></span>
  
- <span data-ttu-id="6b6e3-138">直感的なオブジェクト モデルが用意されています。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-138">It provides an intuitive object model.</span></span>   
- <span data-ttu-id="6b6e3-139">WSDL ファイルとスキーマ ファイルでのサービス記述の複雑さを軽減します。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-139">It abstracts the complexities of the service description in the WSDL and schema files.</span></span>   
- <span data-ttu-id="6b6e3-140">クライアント側のビジネス ロジックが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-140">It includes client-side business logic.</span></span>   
- <span data-ttu-id="6b6e3-141">Web 要求と応答や、オブジェクトのシリアル化と逆シリアル化を処理します。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-141">It handles the web requests and responses and object serialization and deserialization.</span></span>   
- <span data-ttu-id="6b6e3-142">Microsoft によるサポートがあります。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-142">It is Microsoft-supported.</span></span>
    
<span data-ttu-id="6b6e3-143">ただし、EWS のマネージ API は、完全なソリューションではないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-143">Note, however, that the EWS Managed API is not a complete solution.</span></span> <span data-ttu-id="6b6e3-144">EWS のマネージ API では、いくつかの機能は実装されていません。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-144">Some functionality is not implemented in the EWS Managed API.</span></span> <span data-ttu-id="6b6e3-145">EWS のマネージ API では、EWS のすべての機能を実装しないが次の理由により、クライアント アプリケーションの開発に最適な選択肢があります。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-145">Although the EWS Managed API doesn't implement all EWS functionality, it might be the best choice for your client application development, for the following reasons:</span></span>
  
- <span data-ttu-id="6b6e3-146">開発に .NET Framework を使用できます。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-146">You can use the .NET Framework for development.</span></span>
- <span data-ttu-id="6b6e3-147">EWS オブジェクト モデルの大部分に加えて、自動検出を実装しています。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-147">It implements Autodiscover in addition to most parts of the EWS object model.</span></span>
- <span data-ttu-id="6b6e3-148">[ExchangeService](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)クラスでの EWS を操作するためのクライアント側のビジネス ロジックを実装します。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-148">It implements client-side business logic for working with EWS, in the [ExchangeService](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) class.</span></span> 
    
<span data-ttu-id="6b6e3-149">次の理由のいずれかにより、EWS マネージ API ではなく EWS の Web サービス API を使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-149">You might choose to use the EWS web service API instead of the EWS Managed API for any of the following reasons:</span></span>
  
- <span data-ttu-id="6b6e3-150">アプリケーションが .NET Framework を使用しない場合。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-150">Your application does not use the .NET Framework.</span></span> 
- <span data-ttu-id="6b6e3-151">EWS のマネージ API のアセンブリを配布したくないです。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-151">You don't want to distribute the EWS Managed API assembly.</span></span> 
- <span data-ttu-id="6b6e3-152">アプリケーションでは、EWS のマネージ API で実装されていない機能を使用します。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-152">Your application uses features that aren't implemented in the EWS Managed API.</span></span>
    
<span data-ttu-id="6b6e3-153">詳細については、 [EWS のマネージ API のクライアント アプリケーションを使い始める](get-started-with-ews-managed-api-client-applications.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-153">To learn more, see [Get started with EWS Managed API client applications](get-started-with-ews-managed-api-client-applications.md).</span></span>
  
> [!NOTE]
> <span data-ttu-id="6b6e3-154">EWS のマネージ API は、 [GitHub](http://aka.ms/ews-managed-api-github)のオープン ソース プロジェクトとしてされています。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-154">The EWS Managed API is now available as an open source project on [GitHub](http://aka.ms/ews-managed-api-github).</span></span> <span data-ttu-id="6b6e3-155">オープン ソース ライブラリを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-155">You can use the open source library to:</span></span> 
> - <span data-ttu-id="6b6e3-156">バグ修正と API の機能強化に貢献します。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-156">Contribute bug fixes and enhancements to the API.</span></span> 
> - <span data-ttu-id="6b6e3-157">公式のリリースで利用可能になる前に、修正プログラムや拡張機能を取得できます。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-157">Get fixes and enhancements before they are available in an official release.</span></span>
> - <span data-ttu-id="6b6e3-158">API の最も包括的かつ最新の実装にアクセスして、参照として使用するか、新しいプラットフォームで新しいライブラリを作成します。 </span><span class="sxs-lookup"><span data-stu-id="6b6e3-158">Access the most comprehensive and up-to-date implementation of the API, to use as a reference or to create new libraries on new platforms.</span></span>
> 
> <span data-ttu-id="6b6e3-159">GitHub を使用してあなたの[投稿](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md)をお待ちします。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-159">We welcome your [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span></span> 
  
### <a name="ews-java-api"></a><span data-ttu-id="6b6e3-160">EWS Java API</span><span class="sxs-lookup"><span data-stu-id="6b6e3-160">EWS Java API</span></span>

<span data-ttu-id="6b6e3-161">EWS の Java API は、更新およびコミュニティによって拡張できる[GitHub](https://github.com/OfficeDev/ews-java-api)のオープン ソース プロジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-161">The EWS Java API is an open source project on [GitHub](https://github.com/OfficeDev/ews-java-api) that can be updated and extended by the community.</span></span> <span data-ttu-id="6b6e3-162">[EWS のマネージ API](http://msdn.microsoft.com/ja-jp/library/office/jj220535%28v=exchg.80%29.aspx)のような stylistically と、EWS の SOAP 要求と応答を使用して、ネットワーク経由で。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-162">It is stylistically similar to the [EWS Managed API](http://msdn.microsoft.com/ja-jp/library/office/jj220535%28v=exchg.80%29.aspx) and uses EWS SOAP requests and responses over the wire.</span></span> <span data-ttu-id="6b6e3-163">すべての[EWS の SOAP 操作](http://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx)をアクセスできない場合は、オープン ソース プロジェクトの[最新の作成](http://blogs.office.com/2014/08/28/open-sourcing-exchange-web-services-ews-java-api/)時に、EWS の Java API を使用して、私たちはこのギャップを埋めるためのコミュニティを模索しています。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-163">Although you can't access all [EWS SOAP operations](http://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) by using the EWS Java API, with the [recent creation](http://blogs.office.com/2014/08/28/open-sourcing-exchange-web-services-ews-java-api/) of the open source project, we are looking to the community to bridge this gap.</span></span> <span data-ttu-id="6b6e3-164">マイクロソフト サポート、適切なサポートの契約には質問に対応 EWS の SOAP プロトコルがない、EWS Java API 自体に関連する注意してください。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-164">Note that Microsoft Support, with an appropriate support contract, will address any questions related to the EWS SOAP protocol but not the EWS Java API itself.</span></span> <span data-ttu-id="6b6e3-165">EWS の Java API は、 [GitHub](https://github.com/OfficeDev/ews-java-api)のダウンロードとコミュニティの貢献度を使用できます。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-165">The EWS Java API is available for download and community contribution on [GitHub](https://github.com/OfficeDev/ews-java-api).</span></span>
  
### <a name="ews-autogenerated-proxies"></a><span data-ttu-id="6b6e3-166">EWS の自動生成されたプロキシ</span><span class="sxs-lookup"><span data-stu-id="6b6e3-166">EWS autogenerated proxies</span></span>

<span data-ttu-id="6b6e3-p111">自動生成されたクライアント API は、EWS の WSDL および XML スキーマ定義から生成されます。多くの言語でクライアント オブジェクト モデルのジェネレーターが用意されています。一般に、自動生成されたオブジェクト モデルは、オブジェクトのシリアル化および逆シリアル化を管理します。これにビジネス ロジックは含まれておらず、自動生成プロセスによって成果物が作成される結果、直感的には使用しにくいオブジェクト モデルになることが少なくありません。Exchange のサポートはクライアントによって送受信される XML を対象としますが、オブジェクト モデルは対象となりません。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-p111">Autogenerated client APIs are generated from the EWS WSDL and XML schema definitions. Client object model generators are available for many languages. In general, the autogenerated object models manage object serialization and deserialization. They do not include business logic and the autogeneration process often creates artifacts that make the object model less intuitive to use. Exchange support covers the XML that is sent and received by the client but not the object model.</span></span>
  
### <a name="custom-ews-client-api"></a><span data-ttu-id="6b6e3-172">カスタム EWS クライアント API</span><span class="sxs-lookup"><span data-stu-id="6b6e3-172">Custom EWS client API</span></span>

<span data-ttu-id="6b6e3-p112">EWS 機能の小さなセットを使用する一部のアプリケーション用に、Exchange と通信するためのカスタム クライアント API を作成できます。これにより、使用するシステム リソースが少なくなります。これは、.NET Micro Framework を実行するクライアントなど、メモリに制約のあるデバイス上で実行されるクライアントに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-p112">For some applications that use a small set of EWS functionality, you might create a custom client API to communicate with Exchange. This enables you to consume fewer system resources. This is useful for clients that run on memory-constrained devices, such as clients running the .NET Micro Framework.</span></span>
  
## <a name="ews-client-features"></a><span data-ttu-id="6b6e3-176">EWS のクライアント機能</span><span class="sxs-lookup"><span data-stu-id="6b6e3-176">EWS client features</span></span>
<span data-ttu-id="6b6e3-177"><a name="EWSFeatures"> </a></span><span class="sxs-lookup"><span data-stu-id="6b6e3-177"></span></span>

<span data-ttu-id="6b6e3-p113">どの開発オプションを選ぶにせよ、EWS 機能をクライアントでどのように実装するかをご検討ください。機能が使用可能かどうかは、アプリケーションが対象とする EWS のスキーマのバージョン次第です。EWS のスキーマは後方互換性と前方互換性を持つため、Exchange Server 2007 SP1 などの以前のバージョンのスキーマを対象とするアプリケーションを作成する場合、アプリケーションは Exchange Server 2013 SP1 のサービスや Exchange Online など、後のバージョンのスキーマでも動作します。 </span><span class="sxs-lookup"><span data-stu-id="6b6e3-p113">Regardless of the development option that you choose, you should consider how EWS features are implemented in your client. Feature availability is based on the EWS schema version that your application targets. Because EWS schemas are backward- and forward-compatible, if you create an application that targets an earlier schema version, such as Exchange Server 2007 SP1, your application will also work against a later schema version, such as the Exchange Server 2013 SP1 service, as well as Exchange Online.</span></span> 
  
<span data-ttu-id="6b6e3-p114">機能および機能の更新はスキーマによって決定されるため、クライアント アプリケーションに実装する EWS 機能を対象としているもののうち、最も古い共通のコード ベースを使用することをお勧めします。多くのアプリケーションは Exchange2007_SP1 バージョンを対象にできます。なぜなら、Exchange 2007 SP1 のスキーマには、Exchange のストアのアイテムやフォルダーを操作するための Exchange のほとんどすべての主要機能が含まれているためです。EWS のスキーマのバージョンごとに、コードの分岐を維持することをお勧めします。現在利用可能なスキーマのバージョンを次に示します。 </span><span class="sxs-lookup"><span data-stu-id="6b6e3-p114">Because features and feature updates are driven by the schema, we recommend that you use the earliest common code base that targets the EWS features that you want to implement in your client application. Many applications can target the Exchange2007_SP1 version, because the Exchange 2007 SP1 schema contains almost all the core Exchange functionality for working with items and folders in the Exchange store. We recommend that you maintain code forks for each EWS schema version. The following are the schema versions that are currently available.</span></span> 
  
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

<span data-ttu-id="6b6e3-185">**ExchangeVersionType**単純型では、スキーマのバージョンが維持されます。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-185">The schema versions are maintained in the **ExchangeVersionType** simple type.</span></span> 
  
<span data-ttu-id="6b6e3-186">EWS スキーマの各バージョンで利用可能な機能の詳細については、 [Exchange での EWS のスキーマ バージョン](ews-schema-versions-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-186">For information about the features that are available in each EWS schema version, see [EWS schema versions in Exchange](ews-schema-versions-in-exchange.md).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="6b6e3-187">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="6b6e3-187">In this section</span></span>
<span data-ttu-id="6b6e3-188"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="6b6e3-188"></span></span>

- [<span data-ttu-id="6b6e3-189">Exchange および EWS のマネージ API の web サービス API 機能の可用性</span><span class="sxs-lookup"><span data-stu-id="6b6e3-189">Web service API feature availability in Exchange and the EWS Managed API</span></span>](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)
    
- [<span data-ttu-id="6b6e3-190">Exchange のスキーマ バージョンの EWS</span><span class="sxs-lookup"><span data-stu-id="6b6e3-190">EWS schema versions in Exchange</span></span>](ews-schema-versions-in-exchange.md)
    
- [<span data-ttu-id="6b6e3-191">Exchange 内の構成オプション</span><span class="sxs-lookup"><span data-stu-id="6b6e3-191">Configuration options for EWS in Exchange</span></span>](configuration-options-for-ews-in-exchange.md)
    
- [<span data-ttu-id="6b6e3-192">オンラインの Exchange および Exchange、オンプレミスのクライアントがプログラミングを比較します。</span><span class="sxs-lookup"><span data-stu-id="6b6e3-192">Comparing Exchange Online and Exchange on-premises client programming</span></span>](comparing-exchange-online-and-exchange-on-premises-client-programming.md)
    
- [<span data-ttu-id="6b6e3-193">EWS の交換で調整</span><span class="sxs-lookup"><span data-stu-id="6b6e3-193">EWS throttling in Exchange</span></span>](ews-throttling-in-exchange.md)
    
- [<span data-ttu-id="6b6e3-194">EWS のマネージ API の再配布の条件</span><span class="sxs-lookup"><span data-stu-id="6b6e3-194">Redistribution requirements for the EWS Managed API</span></span>](redistribution-requirements-for-the-ews-managed-api.md)
    
- [<span data-ttu-id="6b6e3-195">EWS および他の Exchange クライアントの要求を実装</span><span class="sxs-lookup"><span data-stu-id="6b6e3-195">Instrumenting client requests for EWS and REST in Exchange</span></span>](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="6b6e3-196">関連項目</span><span class="sxs-lookup"><span data-stu-id="6b6e3-196">See also</span></span>
 
- [<span data-ttu-id="6b6e3-197">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="6b6e3-197">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
- [<span data-ttu-id="6b6e3-198">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="6b6e3-198">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md) 
- [<span data-ttu-id="6b6e3-199">EWS アプリケーションの種類</span><span class="sxs-lookup"><span data-stu-id="6b6e3-199">EWS application types</span></span>](ews-application-types.md)
    


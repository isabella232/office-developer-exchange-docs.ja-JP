---
title: Exchange の自動検出
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: da0f9402-4e35-42c7-a15e-1e9e4e966e8b
description: Exchange 自動検出サービスについて説明します。
ms.openlocfilehash: f56717eaced5db9028c556c6c2d9aa7794f4988e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758903"
---
# <a name="autodiscover-for-exchange"></a><span data-ttu-id="40036-103">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="40036-103">Autodiscover for Exchange</span></span>

<span data-ttu-id="40036-104">Exchange 自動検出サービスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="40036-104">Learn about the Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="40036-p101">Exchange 自動検出サービスは、最小限のユーザー入力でカスタムのクライアント アプリケーションが構成されるようにするための簡単な方法を提供します。ほとんどのユーザーは、自分の電子メール アドレスとパスワードを知っています。それら 2 つの情報の断片によって、稼働に必要なその他の詳細のすべてを取得できます。Exchange Web サービス (EWS) クライアントの場合、通常、自動検出は EWS エンドポイント URL を見つけるために使用されますが、その他のプロトコルを使用するクライアントを構成する情報も自動検出によって得られます。自動検出は、ファイアウォールの内側または外側のクライアント アプリケーションに有効であり、リソース フォレストおよび複数フォレストのシナリオで動作します。</span><span class="sxs-lookup"><span data-stu-id="40036-p101">The Exchange Autodiscover service provides an easy way for your client application to configure itself with minimal user input. Most users know their email address and password, and with those two pieces of information, you can retrieve all the other details you need to get up and running. For Exchange Web Services (EWS) clients, Autodiscover is typically used to find the EWS endpoint URL, but Autodiscover can also provide information to configure clients that use other protocols. Autodiscover works for client applications that are inside or outside firewalls and will work in resource forest and multiple forest scenarios.</span></span>
  
## <a name="overview-of-the-autodiscover-process"></a><span data-ttu-id="40036-109">自動検出プロセスの概要</span><span class="sxs-lookup"><span data-stu-id="40036-109">Overview of the Autodiscover process</span></span>
<span data-ttu-id="40036-110"><a name="bk_Before"> </a></span><span class="sxs-lookup"><span data-stu-id="40036-110"></span></span>

<span data-ttu-id="40036-p102">自動検出プロセスには、基本的に 3 つのフェーズがあります。フェーズ 1 では潜在的な自動検出サーバーの一覧を生成して、フェーズ 2 では成功の応答 (可能な場合) が得られるまで一覧の各サーバーを試します。いずれの候補もうまくいかなかった場合は、フェーズ 3 に移行します。このフェーズは、自動検出エンドポイントを見つけるための「最後の努力」を表します。</span><span class="sxs-lookup"><span data-stu-id="40036-p102">The Autodiscover process essentially has three phases. In phase one, you generate a list of potential Autodiscover servers, and in phase two, you try each server in your list until you (hopefully) get a successful response. If none of your candidates worked out, you move on to phase three, which represents a "last ditch" attempt to find an Autodiscover endpoint.</span></span>
  
<span data-ttu-id="40036-114">EWS のマネージ API では、 [ExchangeService.AutodiscoverUrl](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx)メソッドは、このプロセスのすべての 3 つのフェーズを実装するため自分で自動検出を実装することについて心配する必要がある、EWS のマネージ API を使用する場合。</span><span class="sxs-lookup"><span data-stu-id="40036-114">The [ExchangeService.AutodiscoverUrl](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) method in the EWS Managed API implements all three phases of this process for you, so if you are using the EWS Managed API, you don't need to worry about implementing Autodiscover yourself.</span></span> <span data-ttu-id="40036-115">次の図は、自動検出プロセスの 3 つのフェーズを示しています。</span><span class="sxs-lookup"><span data-stu-id="40036-115">The following figure shows the three phases of the Autodiscover process.</span></span> 
  
<span data-ttu-id="40036-116">**図 1 です。自動検出プロセスの 3 つのフェーズ**</span><span class="sxs-lookup"><span data-stu-id="40036-116">**Figure 1. Three phases of the Autodiscover process**</span></span>

![自動検出プロセスの図は、候補者プールの定義、エンドポイントの試行、他の選択肢の試行の3 つの段階を示しています。](media/Ex15_Autodiscover_Overview.png)
  
### <a name="phase-1-defining-the-candidate-pool"></a><span data-ttu-id="40036-118">フェーズ 1:候補プールを定義する</span><span class="sxs-lookup"><span data-stu-id="40036-118">Phase 1: Defining the candidate pool</span></span>
<span data-ttu-id="40036-119"><a name="bk_Phase1"> </a></span><span class="sxs-lookup"><span data-stu-id="40036-119"></span></span>

<span data-ttu-id="40036-120">自動検出を使用することができます、前に、ユーザーの適切な自動検出サーバーを検索する必要があります。</span><span class="sxs-lookup"><span data-stu-id="40036-120">Before you can use Autodiscover, you have to locate the right Autodiscover server for your user.</span></span> <span data-ttu-id="40036-121">幸運にも、自動検出では、限られた場所を検索する場所を定義します。</span><span class="sxs-lookup"><span data-stu-id="40036-121">Luckily, Autodiscover defines a limited number of places for you to look.</span></span> <span data-ttu-id="40036-122">自動検出では複数の候補がある場合[を生成し、リストの優先順位を設定する方法](how-to-generate-a-list-of-autodiscover-endpoints.md)も定義します。</span><span class="sxs-lookup"><span data-stu-id="40036-122">In the case where multiple candidates are found, Autodiscover also defines [a way to generate and prioritize the list](how-to-generate-a-list-of-autodiscover-endpoints.md).</span></span>
  
<span data-ttu-id="40036-123">**表 1: 自動検出エンドポイント候補のソース**</span><span class="sxs-lookup"><span data-stu-id="40036-123">**Table 1: Autodiscover endpoint candidate sources**</span></span>

|<span data-ttu-id="40036-124">**参照**</span><span class="sxs-lookup"><span data-stu-id="40036-124">**Place to look**</span></span>|<span data-ttu-id="40036-125">**どのようなことがわかります**</span><span class="sxs-lookup"><span data-stu-id="40036-125">**What you'll find**</span></span>|
|:-----|:-----|
|<span data-ttu-id="40036-126">Active Directory ドメイン サービス (AD DS)</span><span class="sxs-lookup"><span data-stu-id="40036-126">Active Directory Domain Services (AD DS)</span></span>  <br/> |<span data-ttu-id="40036-127">クライアントがドメインに参加している、これは、検索する最初の場所です。</span><span class="sxs-lookup"><span data-stu-id="40036-127">For domain-joined clients, this is the first place to look.</span></span> <span data-ttu-id="40036-128">Exchange では、自動検出要求をサーバーにルーティングするが、AD DS で (SCP) オブジェクトが Active Directory サイトに基づくサービスの接続ポイントを公開します。</span><span class="sxs-lookup"><span data-stu-id="40036-128">Exchange publishes service connection point (SCP) objects in AD DS, which allows Autodiscover requests to be routed to servers based on Active Directory sites.</span></span> <span data-ttu-id="40036-129">[SCP の検索](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)の結果は、[候補] ボックスの一覧の上部にあるはずです。</span><span class="sxs-lookup"><span data-stu-id="40036-129">The results of an [SCP lookup](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) should be at the top of your candidate list.</span></span>  <br/><br/><span data-ttu-id="40036-130">**注**: SCP 検索はドメインに参加していない、または Active Directory サーバーへのアクセス権を持っていないクライアントは使用できません。</span><span class="sxs-lookup"><span data-stu-id="40036-130">**NOTE**: SCP lookup isn't available for clients that are not joined to a domain or that do not have access to Active Directory servers.</span></span> <span data-ttu-id="40036-131">この例では、SCP の参照を省略してください。</span><span class="sxs-lookup"><span data-stu-id="40036-131">In this case, you should skip SCP lookup.</span></span> <br/>|
|<span data-ttu-id="40036-132">ユーザーの電子メール アドレス ドメイン</span><span class="sxs-lookup"><span data-stu-id="40036-132">The user's email address domain</span></span>  <br/> | <span data-ttu-id="40036-133">自動検出では、標準エンドポイント URL の形式が 2 つ定義されています。これは、ユーザーの電子メール アドレスのドメイン部分から派生します。</span><span class="sxs-lookup"><span data-stu-id="40036-133">Autodiscover defines two standard endpoint URL forms that are derived from the domain portion of the user's email address:</span></span>  <br/>`"https://" + domain + "/autodiscover/autodiscover" +  *fileExtension*`  <br/>`"https://autodiscover." + domain + "/autodiscover/autodiscover" +  *fileExtension*`<br/><br/>  <span data-ttu-id="40036-134">*FileExtension*の値は、自動検出のアクセス方法を使用して、 [SOAP](http://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx)または[POX](http://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx)によって異なります。</span><span class="sxs-lookup"><span data-stu-id="40036-134">The value of  *fileExtension*  depends on which Autodiscover access method you are using, [SOAP](http://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx) or [POX](http://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx).</span></span> <span data-ttu-id="40036-135">SOAP サービスを使用して、".svc"ファイルの拡張子です。POX は".xml"を使用します。</span><span class="sxs-lookup"><span data-stu-id="40036-135">The SOAP service uses a ".svc" file extension; POX uses ".xml".</span></span>  <br/> |
   
<span data-ttu-id="40036-136">次の図は、自動検出エンドポイント一覧の生成方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="40036-136">The following figure shows how to generate an Autodiscover endpoint list.</span></span>
  
<span data-ttu-id="40036-137">**図 2 になります。自動検出エンドポイントのリストを生成するためのプロセス**</span><span class="sxs-lookup"><span data-stu-id="40036-137">**Figure 2. Process for generating an Autodiscover endpoint list**</span></span>

![図は自動検出エンドポイントのリストを生成するためのプロセスを示しています。矢印は、エンドポイントのリストが SCP 参照や、ユーザーの電子メールアドレスから生じることを示しています。](media/Ex15_Autodiscover_Overview_Phase1.png)
  
### <a name="phase-2-trying-each-candidate"></a><span data-ttu-id="40036-140">フェーズ 2:各候補を試してみる</span><span class="sxs-lookup"><span data-stu-id="40036-140">Phase 2: Trying each candidate</span></span>
<span data-ttu-id="40036-141"><a name="bk_Phase2"> </a></span><span class="sxs-lookup"><span data-stu-id="40036-141"></span></span>

<span data-ttu-id="40036-142">潜在的な候補者の順序付きリストを生成した後、次の手順は[URL に要求を送信すること](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)によってリスト内の各 1 を実行してくださいし、図 3 に示すように、結果を検証しています。</span><span class="sxs-lookup"><span data-stu-id="40036-142">After you generate an ordered list of potential candidates, the next step is try each one in the list by [sending a request to the URL](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) and validating the results, as shown in Figure 3.</span></span> <span data-ttu-id="40036-143">正常な応答を取得する場合、完了です。</span><span class="sxs-lookup"><span data-stu-id="40036-143">When you get a successful response, you're done!</span></span> 
  
<span data-ttu-id="40036-144">**図 3 です。順序で各端点の候補をしようとしてください。**</span><span class="sxs-lookup"><span data-stu-id="40036-144">**Figure 3. Trying each endpoint candidate in order**</span></span>

![図はサーバーが正常な応答を受信するまで優先順位順に各エンドポイントを試行しすることを示しています。](media/Ex15_Autodiscover_Overview_Phase2.png)
  
<span data-ttu-id="40036-p110">候補に要求を送信する前に、その候補が信頼可能であることを確認します。ユーザーの資格情報を送信することを忘れてはいけません。その情報の共有は信頼できるサーバーに限定することが重要です。少なくとも、次の事項を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="40036-p110">Before you send a request to a candidate, make sure it is trustworthy. Remember that you're sending the user's credentials, so it's important to make sure that you're only sharing them with a server you can trust. At a minimum, you should verify:</span></span>
  
- <span data-ttu-id="40036-p111">エンドポイントが HTTPS エンドポイントであること。クライアント アプリケーションは、非 SSL エンドポイントに対して認証やデータの送信を行ってはいけません。</span><span class="sxs-lookup"><span data-stu-id="40036-p111">That the endpoint is an HTTPS endpoint. Client applications should not authenticate or send data to a non-SSL endpoint.</span></span>
    
- <span data-ttu-id="40036-151">サーバーが提示した SSL 証明書が信頼された機関からのものであり有効であること。</span><span class="sxs-lookup"><span data-stu-id="40036-151">That the SSL certificate presented by the server is valid and from a trusted authority.</span></span>
    
> [!NOTE]
> <span data-ttu-id="40036-p112">これらは、基本的なセキュリティの推奨事項にすぎません。認証を扱うときには、コードが組織のセキュリティ要件を満たしていることを常に確認します。</span><span class="sxs-lookup"><span data-stu-id="40036-p112">These are just basic security suggestions. Whenever you are working with authentication, make sure that your code meets the security requirements of your organization.</span></span> 
  
<span data-ttu-id="40036-154">送信する要求の種類は、自動検出サービスにアクセスする方法によって決まります。</span><span class="sxs-lookup"><span data-stu-id="40036-154">The type of request you send depends on how you are accessing the Autodiscover service.</span></span>
  
<span data-ttu-id="40036-155">**表 2 になります。自動検出要求の種類**</span><span class="sxs-lookup"><span data-stu-id="40036-155">**Table 2. Types of Autodiscover requests**</span></span>

|<span data-ttu-id="40036-156">**使用している場合.**</span><span class="sxs-lookup"><span data-stu-id="40036-156">**If you are using…**</span></span>|<span data-ttu-id="40036-157">**使用して要求を送信してください.**</span><span class="sxs-lookup"><span data-stu-id="40036-157">**Send a request by using…**</span></span>|
|:-----|:-----|
|<span data-ttu-id="40036-158">EWS マネージ API</span><span class="sxs-lookup"><span data-stu-id="40036-158">The EWS Managed API</span></span>  <br/> |<span data-ttu-id="40036-159">[GetUserSettings](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx)メソッドです。</span><span class="sxs-lookup"><span data-stu-id="40036-159">The [GetUserSettings](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) method.</span></span>  <br/> |
|<span data-ttu-id="40036-160">SOAP 自動検出サービス</span><span class="sxs-lookup"><span data-stu-id="40036-160">The SOAP Autodiscover service</span></span>  <br/> |<span data-ttu-id="40036-161">[GetUserSettings](http://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx)操作します。</span><span class="sxs-lookup"><span data-stu-id="40036-161">The [GetUserSettings](http://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx) operation.</span></span>  <br/> |
|<span data-ttu-id="40036-162">POX 自動検出サービス</span><span class="sxs-lookup"><span data-stu-id="40036-162">The POX Autodiscover service</span></span>  <br/> |<span data-ttu-id="40036-163">[自動検出要求の本文](http://msdn.microsoft.com/library/75671b1d-f35b-497b-8d8c-706f3f2535fd%28Office.15%29.aspx)を含む HTTP POST します。</span><span class="sxs-lookup"><span data-stu-id="40036-163">An HTTP POST with an [Autodiscover request body](http://msdn.microsoft.com/library/75671b1d-f35b-497b-8d8c-706f3f2535fd%28Office.15%29.aspx).</span></span>  <br/> |
   
### <a name="phase-3-trying-other-alternatives"></a><span data-ttu-id="40036-164">フェーズ 3:その他の方法を試す</span><span class="sxs-lookup"><span data-stu-id="40036-164">Phase 3: Trying other alternatives</span></span>
<span data-ttu-id="40036-165"><a name="bk_Phase3"> </a></span><span class="sxs-lookup"><span data-stu-id="40036-165"></span></span>

<span data-ttu-id="40036-p113">一覧に含まれるすべてのエンドポイントを試してみたときに、それらすべてがエラーを返すことがあります。あきらめる前に、いくつか別のものを試してみることができます。認証されていない GET 要求を送信したり、SRV レコードについて DNS を照会したりできます。これらの試行でも成果が得られない場合は、自動検出サービスに接続できません。</span><span class="sxs-lookup"><span data-stu-id="40036-p113">In some cases you might try all the endpoints in your list, only to find that all of them return an error. Before throwing in the towel, you can try a couple more things: you can send an unauthenticated GET request, or query DNS for an SRV record. If these attempts also don't yield results, you cannot contact the Autodiscover service.</span></span>
  
<span data-ttu-id="40036-169">**図 4 です。他の方法をしようとしてください。**</span><span class="sxs-lookup"><span data-stu-id="40036-169">**Figure 4. Trying other alternatives**</span></span>

![図は認証されていない GET 要求および DNS クエリを介して生成された新しいエンドポイントを示しています。](media/Ex15_Autodiscover_Overview_Phase3.png)
  
#### <a name="sending-an-unauthenticated-get-request"></a><span data-ttu-id="40036-171">認証されていない GET 要求の送信</span><span class="sxs-lookup"><span data-stu-id="40036-171">Sending an unauthenticated GET request</span></span>

<span data-ttu-id="40036-172">ユーザーの電子メール アドレスから派生したエンドポイントを認証されていない GET 要求を送信するは、まず最初に実行してください。</span><span class="sxs-lookup"><span data-stu-id="40036-172">The first thing to try is to send an unauthenticated GET request to an endpoint derived from the user's email address.</span></span> <span data-ttu-id="40036-173">そのエンドポイントの形式は、"http://autodiscover.」</span><span class="sxs-lookup"><span data-stu-id="40036-173">The format of that endpoint is "http://autodiscover."</span></span> <span data-ttu-id="40036-174">+ ドメイン +"/autodiscover/autodiscover.xml"です。</span><span class="sxs-lookup"><span data-stu-id="40036-174">+ domain + "/autodiscover/autodiscover.xml".</span></span> <span data-ttu-id="40036-175">SSL エンドポイントではないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="40036-175">Note that this is NOT an SSL endpoint.</span></span> <span data-ttu-id="40036-176">サーバーでは、302 リダイレクト応答が返された場合ことができますし、しようとする応答の Location ヘッダーにエンドポイントの URL に[自動検出の要求を再送信](handling-autodiscover-error-messages.md#bk_ResendRequest)をします。</span><span class="sxs-lookup"><span data-stu-id="40036-176">If the server returns a 302 redirect response, you can then attempt to [resend the Autodiscover request](handling-autodiscover-error-messages.md#bk_ResendRequest) to the endpoint URL in the Location header of the response.</span></span> 
  
#### <a name="querying-dns-for-an-srv-record"></a><span data-ttu-id="40036-177">SRV レコードについての DNS の照会</span><span class="sxs-lookup"><span data-stu-id="40036-177">Querying DNS for an SRV record</span></span>

<span data-ttu-id="40036-p115">認証されていない GET 要求が失敗した場合に、最後に試してみることは、自動検出サービスに関する SRV レコードに対する DNS クエリです。このレコードは、"_autodiscover._tcp." + ドメインの形式になります。このクエリは複数のレコードを返すことがありますが、最高の優先度と重みが付けられた SSL エンドポイントをポイントするレコードのみを使用します。</span><span class="sxs-lookup"><span data-stu-id="40036-p115">If the unauthenticated GET request doesn't work out, the last thing to try is a DNS query for SRV records for the Autodiscover service. The record will take the form "_autodiscover._tcp." + domain. This query might return multiple records, but you should only use records that point to an SSL endpoint and that have the highest priority and weight.</span></span>
  
## <a name="options-for-using-autodiscover"></a><span data-ttu-id="40036-182">自動検出を使用する場合のオプション</span><span class="sxs-lookup"><span data-stu-id="40036-182">Options for using Autodiscover</span></span>
<span data-ttu-id="40036-183"><a name="bk_Options"> </a></span><span class="sxs-lookup"><span data-stu-id="40036-183"></span></span>

<span data-ttu-id="40036-p116">自動検出には、SOAP Web サービスまたは POX Web サービスを使用してアクセスできます。どのメソッドを使用するかは、要件と環境に応じて決まります。ただし、可能であれば SOAP Web サービスの使用をお勧めします。EWS マネージ API も選択肢の 1 つになります。これにより、SOAP と POX の両方の自動検出サービスのクライアント部分が実装されます。</span><span class="sxs-lookup"><span data-stu-id="40036-p116">You can access Autodiscover either by using the SOAP or the POX web service. The method you use depends on your requirements and environment; however, we recommend using the SOAP web service, if possible. The EWS Managed API is also an option. It implements the client portion of both the SOAP and POX Autodiscover services.</span></span>
  
<span data-ttu-id="40036-188">**表 3: 自動検出にアクセスする方法**</span><span class="sxs-lookup"><span data-stu-id="40036-188">**Table 3: Options for accessing Autodiscover**</span></span>

|<span data-ttu-id="40036-189">**オプション**</span><span class="sxs-lookup"><span data-stu-id="40036-189">**Option**</span></span>|<span data-ttu-id="40036-190">**プロフェッショナル**</span><span class="sxs-lookup"><span data-stu-id="40036-190">**Pros**</span></span>|<span data-ttu-id="40036-191">**短所**</span><span class="sxs-lookup"><span data-stu-id="40036-191">**Cons**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="40036-192">EWS Managed API</span><span class="sxs-lookup"><span data-stu-id="40036-192">EWS Managed API</span></span>](get-started-with-ews-managed-api-client-applications.md) <br/> | <span data-ttu-id="40036-193">自動検出プロセスが実装される。</span><span class="sxs-lookup"><span data-stu-id="40036-193">Implements the Autodiscover process for you.</span></span><br/><br/><span data-ttu-id="40036-194">SOAP と POX の両方の自動検出サービスを使用する。</span><span class="sxs-lookup"><span data-stu-id="40036-194">Uses both the SOAP and POX Autodiscover services.</span></span><br/><br/><span data-ttu-id="40036-195">Exchange Online、Office 365 の一部としての Exchange Online、または Exchange 2007 SP1 以降の Exchange の各バージョンで動作する。</span><span class="sxs-lookup"><span data-stu-id="40036-195">Works with Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2007 SP1.</span></span><br/><br/><span data-ttu-id="40036-196">使いやすい。</span><span class="sxs-lookup"><span data-stu-id="40036-196">Easy to use.</span></span>  <br/> | <span data-ttu-id="40036-197">[Microsoft.Exchange.WebServices.Autodiscover.UserSettingName](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=EXCHG.80%29.aspx)列挙体で使用可能なユーザーの設定に制限されます。</span><span class="sxs-lookup"><span data-stu-id="40036-197">Limited to the user settings that are available in the [Microsoft.Exchange.WebServices.Autodiscover.UserSettingName](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=EXCHG.80%29.aspx) enumeration.</span></span><br/><br/><span data-ttu-id="40036-198">.NET Framework アプリケーションにのみ使用できる。</span><span class="sxs-lookup"><span data-stu-id="40036-198">Only available for .NET Framework applications.</span></span>  <br/> |
|[<span data-ttu-id="40036-199">SOAP の自動検出</span><span class="sxs-lookup"><span data-stu-id="40036-199">SOAP Autodiscover</span></span>](http://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx) <br/> | <span data-ttu-id="40036-200">プラットフォームに依存しない。</span><span class="sxs-lookup"><span data-stu-id="40036-200">Platform independent.</span></span><br/><br/><span data-ttu-id="40036-201">監視のある設定のみを要求できる。</span><span class="sxs-lookup"><span data-stu-id="40036-201">Allows you to request just the settings you are interested in.</span></span>  <br/> | <span data-ttu-id="40036-202">Exchange 2007 では使用できない。</span><span class="sxs-lookup"><span data-stu-id="40036-202">Not available in Exchange 2007.</span></span>  <br/> |
|[<span data-ttu-id="40036-203">POX の自動検出</span><span class="sxs-lookup"><span data-stu-id="40036-203">POX Autodiscover</span></span>](http://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx) <br/> | <span data-ttu-id="40036-204">プラットフォームに依存しない。</span><span class="sxs-lookup"><span data-stu-id="40036-204">Platform independent.</span></span><br/><br/><span data-ttu-id="40036-205">Exchange Online および Exchange 2007 SP1 以降のすべてのバージョンでサポートされる。</span><span class="sxs-lookup"><span data-stu-id="40036-205">Supported in Exchange Online and all versions of Exchange starting with Exchange 2007 SP1.</span></span>  <br/> | <span data-ttu-id="40036-206">特定の設定を要求できない。</span><span class="sxs-lookup"><span data-stu-id="40036-206">Does not allow you to request specific settings.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="40036-207">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="40036-207">In this section</span></span>

- [<span data-ttu-id="40036-208">Exchange SCP のルックアップを使用して自動検出エンドポイントを検索します。</span><span class="sxs-lookup"><span data-stu-id="40036-208">Find Autodiscover endpoints by using SCP lookup in Exchange</span></span>](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [<span data-ttu-id="40036-209">自動検出エンドポイントの一覧を生成します。</span><span class="sxs-lookup"><span data-stu-id="40036-209">Generate a list of Autodiscover endpoints</span></span>](how-to-generate-a-list-of-autodiscover-endpoints.md)
    
- [<span data-ttu-id="40036-210">自動検出を使用してコネクション ポイントを検索するには</span><span class="sxs-lookup"><span data-stu-id="40036-210">Use Autodiscover to find connection points</span></span>](how-to-use-autodiscover-to-find-connection-points.md)
    
- [<span data-ttu-id="40036-211">Exchange から自動検出を使用してユーザー設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="40036-211">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [<span data-ttu-id="40036-212">Exchange サーバーからドメインの設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="40036-212">Get domain settings from an Exchange server</span></span>](how-to-get-domain-settings-from-an-exchange-server.md)
    
- [<span data-ttu-id="40036-213">自動検出を使用して構成情報を更新します。</span><span class="sxs-lookup"><span data-stu-id="40036-213">Refresh configuration information by using Autodiscover</span></span>](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [<span data-ttu-id="40036-214">自動検出のエラー メッセージの処理</span><span class="sxs-lookup"><span data-stu-id="40036-214">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
- [<span data-ttu-id="40036-215">Exchange の自動検出を使用する場合は、パフォーマンスを向上させる</span><span class="sxs-lookup"><span data-stu-id="40036-215">Improving performance when using Autodiscover for Exchange</span></span>](improving-performance-when-using-autodiscover-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="40036-216">関連項目</span><span class="sxs-lookup"><span data-stu-id="40036-216">See also</span></span>

- [<span data-ttu-id="40036-217">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="40036-217">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)    
- [<span data-ttu-id="40036-218">Exchange 2013: 自動検出とユーザー設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="40036-218">Exchange 2013: Get user settings with Autodiscover</span></span>](http://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e)
- [<span data-ttu-id="40036-219">自動検出チェック サンプル</span><span class="sxs-lookup"><span data-stu-id="40036-219">Autodiscover Checker sample</span></span>](http://code.msdn.microsoft.com/exchange/Autodiscover-Checker-e1ebca42)  
- [<span data-ttu-id="40036-220">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="40036-220">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    


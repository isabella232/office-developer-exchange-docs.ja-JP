---
title: Exchange の自動検出
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: da0f9402-4e35-42c7-a15e-1e9e4e966e8b
description: Exchange 自動検出サービスについて説明します。
localization_priority: Priority
ms.openlocfilehash: 913ec3fef93900a1b5fa7aa342e8bca149c88b7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44437760"
---
# <a name="autodiscover-for-exchange"></a><span data-ttu-id="ffa80-103">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="ffa80-103">Autodiscover for Exchange</span></span>

<span data-ttu-id="ffa80-104">Exchange 自動検出サービスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="ffa80-104">Learn about the Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="ffa80-p101">Exchange 自動検出サービスは、最小限のユーザー入力でカスタムのクライアント アプリケーションが構成されるようにするための簡単な方法を提供します。ほとんどのユーザーは、自分の電子メール アドレスとパスワードを知っています。それら 2 つの情報の断片によって、稼働に必要なその他の詳細のすべてを取得できます。Exchange Web サービス (EWS) クライアントの場合、通常、自動検出は EWS エンドポイント URL を見つけるために使用されますが、その他のプロトコルを使用するクライアントを構成する情報も自動検出によって得られます。自動検出は、ファイアウォールの内側または外側のクライアント アプリケーションに有効であり、リソース フォレストおよび複数フォレストのシナリオで動作します。</span><span class="sxs-lookup"><span data-stu-id="ffa80-p101">The Exchange Autodiscover service provides an easy way for your client application to configure itself with minimal user input. Most users know their email address and password, and with those two pieces of information, you can retrieve all the other details you need to get up and running. For Exchange Web Services (EWS) clients, Autodiscover is typically used to find the EWS endpoint URL, but Autodiscover can also provide information to configure clients that use other protocols. Autodiscover works for client applications that are inside or outside firewalls and will work in resource forest and multiple forest scenarios.</span></span>
  
## <a name="overview-of-the-autodiscover-process"></a><span data-ttu-id="ffa80-109">自動検出プロセスの概要</span><span class="sxs-lookup"><span data-stu-id="ffa80-109">Overview of the Autodiscover process</span></span>
<span data-ttu-id="ffa80-110"><a name="bk_Before"> </a></span><span class="sxs-lookup"><span data-stu-id="ffa80-110"><a name="bk_Before"> </a></span></span>

<span data-ttu-id="ffa80-p102">自動検出プロセスには、基本的に 3 つのフェーズがあります。フェーズ 1 では潜在的な自動検出サーバーの一覧を生成して、フェーズ 2 では成功の応答 (可能な場合) が得られるまで一覧の各サーバーを試します。いずれの候補もうまくいかなかった場合は、フェーズ 3 に移行します。このフェーズは、自動検出エンドポイントを見つけるための「最後の努力」を表します。</span><span class="sxs-lookup"><span data-stu-id="ffa80-p102">The Autodiscover process essentially has three phases. In phase one, you generate a list of potential Autodiscover servers, and in phase two, you try each server in your list until you (hopefully) get a successful response. If none of your candidates worked out, you move on to phase three, which represents a "last ditch" attempt to find an Autodiscover endpoint.</span></span>
  
<span data-ttu-id="ffa80-114">EWS マネージ API の [ExchangeService.AutodiscoverUrl](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) メソッドにより、このプロセスの 3 つのフェーズはすべて実装されます。そのため、EWS マネージ API を使用する場合は、独自に自動検出を実装することについて心配する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="ffa80-114">The [ExchangeService.AutodiscoverUrl](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) method in the EWS Managed API implements all three phases of this process for you, so if you are using the EWS Managed API, you don't need to worry about implementing Autodiscover yourself.</span></span> <span data-ttu-id="ffa80-115">次の図は、自動検出プロセスの 3 つのフェーズを示しています。</span><span class="sxs-lookup"><span data-stu-id="ffa80-115">The following figure shows the three phases of the Autodiscover process.</span></span> 
  
<span data-ttu-id="ffa80-116">**図 1. 自動検出プロセスの 3 つのフェーズ**</span><span class="sxs-lookup"><span data-stu-id="ffa80-116">**Figure 1. Three phases of the Autodiscover process**</span></span>

![候補プールの定義、エンドポイントの試行、他の選択肢の試行の 3 つのフェーズを示す自動検出プロセスの図。](media/Ex15_Autodiscover_Overview.png)
  
### <a name="phase-1-defining-the-candidate-pool"></a><span data-ttu-id="ffa80-118">フェーズ 1: 候補プールを定義する</span><span class="sxs-lookup"><span data-stu-id="ffa80-118">Phase 1: Defining the candidate pool</span></span>
<span data-ttu-id="ffa80-119"><a name="bk_Phase1"> </a></span><span class="sxs-lookup"><span data-stu-id="ffa80-119"><a name="bk_Phase1"> </a></span></span>

<span data-ttu-id="ffa80-p104">自動検出を使用するには、まず、ユーザーに正しい自動検出サーバーの場所を示す必要があります。好都合なことに、自動検出の定義により、探す場所の数は限られています。複数の候補が見つかった場合、自動検出では[一覧の生成して優先度を設定する方法](how-to-generate-a-list-of-autodiscover-endpoints.md)も定義されています。</span><span class="sxs-lookup"><span data-stu-id="ffa80-p104">Before you can use Autodiscover, you have to locate the right Autodiscover server for your user. Luckily, Autodiscover defines a limited number of places for you to look. In the case where multiple candidates are found, Autodiscover also defines [a way to generate and prioritize the list](how-to-generate-a-list-of-autodiscover-endpoints.md).</span></span>
  
<span data-ttu-id="ffa80-123">**表 1. 自動検出エンドポイント候補のソース**</span><span class="sxs-lookup"><span data-stu-id="ffa80-123">**Table 1: Autodiscover endpoint candidate sources**</span></span>

|<span data-ttu-id="ffa80-124">**探す場所**</span><span class="sxs-lookup"><span data-stu-id="ffa80-124">**Place to look**</span></span>|<span data-ttu-id="ffa80-125">**見つかるもの**</span><span class="sxs-lookup"><span data-stu-id="ffa80-125">**What you'll find**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ffa80-126">Active Directory Domain Services (AD DS)</span><span class="sxs-lookup"><span data-stu-id="ffa80-126">Active Directory Domain Services (AD DS)</span></span>  <br/> |<span data-ttu-id="ffa80-p105">ドメインに参加しているクライアントの場合は、最初に探す場所になります。Exchange は AD DS にサービス接続ポイント (SCP) オブジェクトを公開します。これにより、自動検出の要求は Active Directory サイトに基づいてサーバーにルーティングできるようになります。[SCP 検索](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)の結果は、候補一覧の最上位にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="ffa80-p105">For domain-joined clients, this is the first place to look. Exchange publishes service connection point (SCP) objects in AD DS, which allows Autodiscover requests to be routed to servers based on Active Directory sites. The results of an [SCP lookup](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) should be at the top of your candidate list.  </span></span><br/><br/><span data-ttu-id="ffa80-130">**注**: SCP 検索は、ドメインに参加していないクライアントや Active Directory サーバーにアクセスできないクライアントには使用できません。</span><span class="sxs-lookup"><span data-stu-id="ffa80-130">**NOTE**: SCP lookup isn't available for clients that are not joined to a domain or that do not have access to Active Directory servers.</span></span> <span data-ttu-id="ffa80-131">この場合は、SCP 検索を省略する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ffa80-131">In this case, you should skip SCP lookup.</span></span> <br/>|
|<span data-ttu-id="ffa80-132">ユーザーの電子メール アドレス ドメイン</span><span class="sxs-lookup"><span data-stu-id="ffa80-132">The user's email address domain</span></span>  <br/> | <span data-ttu-id="ffa80-133">自動検出では、標準エンドポイント URL の形式が 2 つ定義されています。これは、ユーザーの電子メール アドレスのドメイン部分から派生します。</span><span class="sxs-lookup"><span data-stu-id="ffa80-133">Autodiscover defines two standard endpoint URL forms that are derived from the domain portion of the user's email address:</span></span>  <br/>`"https://" + domain + "/autodiscover/autodiscover" +  *fileExtension*`  <br/>`"https://autodiscover." + domain + "/autodiscover/autodiscover" +  *fileExtension*`<br/><br/>  <span data-ttu-id="ffa80-134">*fileExtension* の値は、自動検出のアクセス方式に [SOAP](https://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx) と [POX](https://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx) のどちらを使用しているかによって決まります。</span><span class="sxs-lookup"><span data-stu-id="ffa80-134">The value of  *fileExtension*  depends on which Autodiscover access method you are using, [SOAP](https://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx) or [POX](https://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx).</span></span> <span data-ttu-id="ffa80-135">SOAP サービスではファイル拡張子 ".svc" が使用され、POX では ".xml" が使用されます。</span><span class="sxs-lookup"><span data-stu-id="ffa80-135">The SOAP service uses a ".svc" file extension; POX uses ".xml".</span></span>  <br/> |
   
<span data-ttu-id="ffa80-136">次の図は、自動検出エンドポイント一覧の生成方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="ffa80-136">The following figure shows how to generate an Autodiscover endpoint list.</span></span>
  
<span data-ttu-id="ffa80-137">**図 2. 自動検出エンドポイント一覧の生成プロセス**</span><span class="sxs-lookup"><span data-stu-id="ffa80-137">**Figure 2. Process for generating an Autodiscover endpoint list**</span></span>

![図は自動検出エンドポイントのリストを生成するためのプロセスを示しています。矢印は、エンドポイントのリストが SCP 参照や、ユーザーの電子メールアドレスから生じることを示しています。](media/Ex15_Autodiscover_Overview_Phase1.png)
  
### <a name="phase-2-trying-each-candidate"></a><span data-ttu-id="ffa80-140">フェーズ 2: 各候補を試してみる</span><span class="sxs-lookup"><span data-stu-id="ffa80-140">Phase 2: Trying each candidate</span></span>
<span data-ttu-id="ffa80-141"><a name="bk_Phase2"> </a></span><span class="sxs-lookup"><span data-stu-id="ffa80-141"><a name="bk_Phase2"> </a></span></span>

<span data-ttu-id="ffa80-p109">潜在的な候補の順序付き一覧を生成したら、[URL に要求を送信](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)して結果を検証することで、一覧の各候補を試してみます。図 3 を参照してください。成功の応答が得られた時点で完了です。</span><span class="sxs-lookup"><span data-stu-id="ffa80-p109">After you generate an ordered list of potential candidates, the next step is try each one in the list by [sending a request to the URL](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) and validating the results, as shown in Figure 3. When you get a successful response, you're done!</span></span> 
  
<span data-ttu-id="ffa80-144">**図 3. 各エンドポイント候補を順に試す**</span><span class="sxs-lookup"><span data-stu-id="ffa80-144">**Figure 3. Trying each endpoint candidate in order**</span></span>

![サーバーが正常な応答を受信するまで優先順位順に各エンドポイントを試行することを示す図。](media/Ex15_Autodiscover_Overview_Phase2.png)
  
<span data-ttu-id="ffa80-p110">候補に要求を送信する前に、その候補が信頼可能であることを確認します。ユーザーの資格情報を送信することを忘れてはいけません。その情報の共有は信頼できるサーバーに限定することが重要です。少なくとも、次の事項を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ffa80-p110">Before you send a request to a candidate, make sure it is trustworthy. Remember that you're sending the user's credentials, so it's important to make sure that you're only sharing them with a server you can trust. At a minimum, you should verify:</span></span>
  
- <span data-ttu-id="ffa80-p111">エンドポイントが HTTPS エンドポイントであること。クライアント アプリケーションは、非 SSL エンドポイントに対して認証やデータの送信を行ってはいけません。</span><span class="sxs-lookup"><span data-stu-id="ffa80-p111">That the endpoint is an HTTPS endpoint. Client applications should not authenticate or send data to a non-SSL endpoint.</span></span>
    
- <span data-ttu-id="ffa80-151">サーバーが提示した SSL 証明書が信頼された機関からのものであり有効であること。</span><span class="sxs-lookup"><span data-stu-id="ffa80-151">That the SSL certificate presented by the server is valid and from a trusted authority.</span></span>
    
> [!NOTE]
> <span data-ttu-id="ffa80-p112">これらは、基本的なセキュリティの推奨事項にすぎません。認証を扱うときには、コードが組織のセキュリティ要件を満たしていることを常に確認します。</span><span class="sxs-lookup"><span data-stu-id="ffa80-p112">These are just basic security suggestions. Whenever you are working with authentication, make sure that your code meets the security requirements of your organization.</span></span> 
  
<span data-ttu-id="ffa80-154">送信する要求の種類は、自動検出サービスにアクセスする方法によって決まります。</span><span class="sxs-lookup"><span data-stu-id="ffa80-154">The type of request you send depends on how you are accessing the Autodiscover service.</span></span>
  
<span data-ttu-id="ffa80-155">**表 2. 自動検出の要求の種類**</span><span class="sxs-lookup"><span data-stu-id="ffa80-155">**Table 2. Types of Autodiscover requests**</span></span>

|<span data-ttu-id="ffa80-156">**使用するもの**</span><span class="sxs-lookup"><span data-stu-id="ffa80-156">**If you are using…**</span></span>|<span data-ttu-id="ffa80-157">**要求を送信する手段**</span><span class="sxs-lookup"><span data-stu-id="ffa80-157">**Send a request by using…**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ffa80-158">EWS マネージ API</span><span class="sxs-lookup"><span data-stu-id="ffa80-158">The EWS Managed API</span></span>  <br/> |<span data-ttu-id="ffa80-159">[GetUserSettings](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) メソッド。</span><span class="sxs-lookup"><span data-stu-id="ffa80-159">The [GetUserSettings](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) method.</span></span>  <br/> |
|<span data-ttu-id="ffa80-160">SOAP 自動検出サービス</span><span class="sxs-lookup"><span data-stu-id="ffa80-160">The SOAP Autodiscover service</span></span>  <br/> |<span data-ttu-id="ffa80-161">[GetUserSettings](https://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx) 操作。</span><span class="sxs-lookup"><span data-stu-id="ffa80-161">The [GetUserSettings](https://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx) operation.</span></span>  <br/> |
|<span data-ttu-id="ffa80-162">POX 自動検出サービス</span><span class="sxs-lookup"><span data-stu-id="ffa80-162">The POX Autodiscover service</span></span>  <br/> |<span data-ttu-id="ffa80-163">[自動検出要求本文](https://msdn.microsoft.com/library/75671b1d-f35b-497b-8d8c-706f3f2535fd%28Office.15%29.aspx)が含まれる HTTP POST。</span><span class="sxs-lookup"><span data-stu-id="ffa80-163">An HTTP POST with an [Autodiscover request body](https://msdn.microsoft.com/library/75671b1d-f35b-497b-8d8c-706f3f2535fd%28Office.15%29.aspx).</span></span>  <br/> |
   
### <a name="phase-3-trying-other-alternatives"></a><span data-ttu-id="ffa80-164">フェーズ 3: その他の方法を試す</span><span class="sxs-lookup"><span data-stu-id="ffa80-164">Phase 3: Trying other alternatives</span></span>
<span data-ttu-id="ffa80-165"><a name="bk_Phase3"> </a></span><span class="sxs-lookup"><span data-stu-id="ffa80-165"><a name="bk_Phase3"> </a></span></span>

<span data-ttu-id="ffa80-p113">一覧に含まれるすべてのエンドポイントを試してみたときに、それらすべてがエラーを返すことがあります。あきらめる前に、いくつか別のものを試してみることができます。認証されていない GET 要求を送信したり、SRV レコードについて DNS を照会したりできます。これらの試行でも成果が得られない場合は、自動検出サービスに接続できません。</span><span class="sxs-lookup"><span data-stu-id="ffa80-p113">In some cases you might try all the endpoints in your list, only to find that all of them return an error. Before throwing in the towel, you can try a couple more things: you can send an unauthenticated GET request, or query DNS for an SRV record. If these attempts also don't yield results, you cannot contact the Autodiscover service.</span></span>
  
<span data-ttu-id="ffa80-169">**図 4. その他の方法を試す**</span><span class="sxs-lookup"><span data-stu-id="ffa80-169">**Figure 4. Trying other alternatives**</span></span>

![認証されていない GET 要求および DNS クエリを介して生成された新しいエンドポイントを示す図。](media/Ex15_Autodiscover_Overview_Phase3.png)
  
#### <a name="sending-an-unauthenticated-get-request"></a><span data-ttu-id="ffa80-171">認証されていない GET 要求の送信</span><span class="sxs-lookup"><span data-stu-id="ffa80-171">Sending an unauthenticated GET request</span></span>

<span data-ttu-id="ffa80-172">最初に試してみることは、ユーザーの電子メール アドレスから派生したエンドポイントに向けて、認証されていない GET 要求を送信することです。</span><span class="sxs-lookup"><span data-stu-id="ffa80-172">The first thing to try is to send an unauthenticated GET request to an endpoint derived from the user's email address.</span></span> <span data-ttu-id="ffa80-173">そのエンドポイントは、"http://autodiscover"</span><span class="sxs-lookup"><span data-stu-id="ffa80-173">The format of that endpoint is "http://autodiscover."</span></span> <span data-ttu-id="ffa80-174">+ domain + "/autodiscover/autodiscover.xml" の形式です。</span><span class="sxs-lookup"><span data-stu-id="ffa80-174">+ domain + "/autodiscover/autodiscover.xml".</span></span> <span data-ttu-id="ffa80-175">これは SSL エンドポイントでない点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="ffa80-175">Note that this is NOT an SSL endpoint.</span></span> <span data-ttu-id="ffa80-176">サーバーが 302 リダイレクト応答を返す場合は、その応答の Location ヘッダーに含まれるエンドポイント URL に向けて[自動検出要求の再送信](handling-autodiscover-error-messages.md#bk_ResendRequest)を試してみます。</span><span class="sxs-lookup"><span data-stu-id="ffa80-176">If the server returns a 302 redirect response, you can then attempt to [resend the Autodiscover request](handling-autodiscover-error-messages.md#bk_ResendRequest) to the endpoint URL in the Location header of the response.</span></span> 
  
#### <a name="querying-dns-for-an-srv-record"></a><span data-ttu-id="ffa80-177">SRV レコードについての DNS の照会</span><span class="sxs-lookup"><span data-stu-id="ffa80-177">Querying DNS for an SRV record</span></span>

<span data-ttu-id="ffa80-p115">認証されていない GET 要求が失敗した場合に、最後に試してみることは、自動検出サービスに関する SRV レコードに対する DNS クエリです。このレコードは、"_autodiscover._tcp." + ドメインの形式になります。このクエリは複数のレコードを返すことがありますが、最高の優先度と重みが付けられた SSL エンドポイントをポイントするレコードのみを使用します。</span><span class="sxs-lookup"><span data-stu-id="ffa80-p115">If the unauthenticated GET request doesn't work out, the last thing to try is a DNS query for SRV records for the Autodiscover service. The record will take the form "_autodiscover._tcp." + domain. This query might return multiple records, but you should only use records that point to an SSL endpoint and that have the highest priority and weight.</span></span>
  
## <a name="options-for-using-autodiscover"></a><span data-ttu-id="ffa80-182">自動検出を使用する場合のオプション</span><span class="sxs-lookup"><span data-stu-id="ffa80-182">Options for using Autodiscover</span></span>
<span data-ttu-id="ffa80-183"><a name="bk_Options"> </a></span><span class="sxs-lookup"><span data-stu-id="ffa80-183"><a name="bk_Options"> </a></span></span>

<span data-ttu-id="ffa80-p116">自動検出には、SOAP Web サービスまたは POX Web サービスを使用してアクセスできます。どのメソッドを使用するかは、要件と環境に応じて決まります。ただし、可能であれば SOAP Web サービスの使用をお勧めします。EWS マネージ API も選択肢の 1 つになります。これにより、SOAP と POX の両方の自動検出サービスのクライアント部分が実装されます。</span><span class="sxs-lookup"><span data-stu-id="ffa80-p116">You can access Autodiscover either by using the SOAP or the POX web service. The method you use depends on your requirements and environment; however, we recommend using the SOAP web service, if possible. The EWS Managed API is also an option. It implements the client portion of both the SOAP and POX Autodiscover services.</span></span>
  
<span data-ttu-id="ffa80-188">**表 3: 自動検出にアクセスする場合のオプション**</span><span class="sxs-lookup"><span data-stu-id="ffa80-188">**Table 3: Options for accessing Autodiscover**</span></span>

|<span data-ttu-id="ffa80-189">**オプション**</span><span class="sxs-lookup"><span data-stu-id="ffa80-189">**Option**</span></span>|<span data-ttu-id="ffa80-190">**利点**</span><span class="sxs-lookup"><span data-stu-id="ffa80-190">**Pros**</span></span>|<span data-ttu-id="ffa80-191">**欠点**</span><span class="sxs-lookup"><span data-stu-id="ffa80-191">**Cons**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="ffa80-192">EWS マネージ API</span><span class="sxs-lookup"><span data-stu-id="ffa80-192">EWS Managed API</span></span>](get-started-with-ews-managed-api-client-applications.md) <br/> | <span data-ttu-id="ffa80-193">自動検出プロセスが実装される。</span><span class="sxs-lookup"><span data-stu-id="ffa80-193">Implements the Autodiscover process for you.</span></span><br/><br/><span data-ttu-id="ffa80-194">SOAP と POX の両方の自動検出サービスを使用する。</span><span class="sxs-lookup"><span data-stu-id="ffa80-194">Uses both the SOAP and POX Autodiscover services.</span></span><br/><br/><span data-ttu-id="ffa80-195">Exchange Online、Office 365 の一部としての Exchange Online、または Exchange 2007 SP1 以降の Exchange の各バージョンで動作する。</span><span class="sxs-lookup"><span data-stu-id="ffa80-195">Works with Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2007 SP1.</span></span><br/><br/><span data-ttu-id="ffa80-196">使いやすい。</span><span class="sxs-lookup"><span data-stu-id="ffa80-196">Easy to use.</span></span>  <br/> | <span data-ttu-id="ffa80-197">[Microsoft.Exchange.WebServices.Autodiscover.UserSettingName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=EXCHG.80%29.aspx) 列挙体で使用できるユーザー設定に制限される。</span><span class="sxs-lookup"><span data-stu-id="ffa80-197">Limited to the user settings that are available in the [Microsoft.Exchange.WebServices.Autodiscover.UserSettingName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=EXCHG.80%29.aspx) enumeration.</span></span><br/><br/><span data-ttu-id="ffa80-198">.NET Framework アプリケーションにのみ使用できる。</span><span class="sxs-lookup"><span data-stu-id="ffa80-198">Only available for .NET Framework applications.</span></span>  <br/> |
|[<span data-ttu-id="ffa80-199">SOAP 自動検出</span><span class="sxs-lookup"><span data-stu-id="ffa80-199">SOAP Autodiscover</span></span>](https://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx) <br/> | <span data-ttu-id="ffa80-200">プラットフォームに依存しない。</span><span class="sxs-lookup"><span data-stu-id="ffa80-200">Platform independent.</span></span><br/><br/><span data-ttu-id="ffa80-201">監視のある設定のみを要求できる。</span><span class="sxs-lookup"><span data-stu-id="ffa80-201">Allows you to request just the settings you are interested in.</span></span>  <br/> | <span data-ttu-id="ffa80-202">Exchange 2007 では使用できない。</span><span class="sxs-lookup"><span data-stu-id="ffa80-202">Not available in Exchange 2007.</span></span>  <br/> |
|[<span data-ttu-id="ffa80-203">POX 自動検出</span><span class="sxs-lookup"><span data-stu-id="ffa80-203">POX Autodiscover</span></span>](https://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx) <br/> | <span data-ttu-id="ffa80-204">プラットフォームに依存しない。</span><span class="sxs-lookup"><span data-stu-id="ffa80-204">Platform independent.</span></span><br/><br/><span data-ttu-id="ffa80-205">Exchange Online および Exchange 2007 SP1 以降のすべてのバージョンでサポートされる。</span><span class="sxs-lookup"><span data-stu-id="ffa80-205">Supported in Exchange Online and all versions of Exchange starting with Exchange 2007 SP1.</span></span>  <br/> | <span data-ttu-id="ffa80-206">特定の設定を要求できない。</span><span class="sxs-lookup"><span data-stu-id="ffa80-206">Does not allow you to request specific settings.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="ffa80-207">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="ffa80-207">In this section</span></span>

- [<span data-ttu-id="ffa80-208">Exchange の SCP 参照を使用して自動検出エンドポイントを見つける</span><span class="sxs-lookup"><span data-stu-id="ffa80-208">Find Autodiscover endpoints by using SCP lookup in Exchange</span></span>](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [<span data-ttu-id="ffa80-209">自動検出エンドポイントの一覧を生成する</span><span class="sxs-lookup"><span data-stu-id="ffa80-209">Generate a list of Autodiscover endpoints</span></span>](how-to-generate-a-list-of-autodiscover-endpoints.md)
    
- [<span data-ttu-id="ffa80-210">自動検出を使用して接続ポイントを検索する</span><span class="sxs-lookup"><span data-stu-id="ffa80-210">Use Autodiscover to find connection points</span></span>](how-to-use-autodiscover-to-find-connection-points.md)
    
- [<span data-ttu-id="ffa80-211">自動検出を使用して Exchange からユーザー設定を取得する</span><span class="sxs-lookup"><span data-stu-id="ffa80-211">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [<span data-ttu-id="ffa80-212">Exchange サーバーからドメイン設定を取得する</span><span class="sxs-lookup"><span data-stu-id="ffa80-212">Get domain settings from an Exchange server</span></span>](how-to-get-domain-settings-from-an-exchange-server.md)
    
- [<span data-ttu-id="ffa80-213">自動検出を使用して構成情報を更新する</span><span class="sxs-lookup"><span data-stu-id="ffa80-213">Refresh configuration information by using Autodiscover</span></span>](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [<span data-ttu-id="ffa80-214">自動検出のエラー メッセージを処理する</span><span class="sxs-lookup"><span data-stu-id="ffa80-214">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
- [<span data-ttu-id="ffa80-215">Exchange の自動検出を使用するときにパフォーマンスを向上させる</span><span class="sxs-lookup"><span data-stu-id="ffa80-215">Improving performance when using Autodiscover for Exchange</span></span>](improving-performance-when-using-autodiscover-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="ffa80-216">関連項目</span><span class="sxs-lookup"><span data-stu-id="ffa80-216">See also</span></span>

- [<span data-ttu-id="ffa80-217">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="ffa80-217">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)    
- [<span data-ttu-id="ffa80-218">Exchange 2013: 自動検出によるユーザー設定の取得</span><span class="sxs-lookup"><span data-stu-id="ffa80-218">Exchange 2013: Get user settings with Autodiscover</span></span>](https://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e)
- [<span data-ttu-id="ffa80-219">Autodiscover Checker サンプル</span><span class="sxs-lookup"><span data-stu-id="ffa80-219">Autodiscover Checker sample</span></span>](https://code.msdn.microsoft.com/exchange/Autodiscover-Checker-e1ebca42)  
- [<span data-ttu-id="ffa80-220">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="ffa80-220">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    


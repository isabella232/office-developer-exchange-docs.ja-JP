---
title: 自動検出エンドポイントの一覧を生成する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 82394d3c-9fc7-4b3c-b48d-1fe983c198f7
description: 自動検出エンドポイントの優先順位を付けた一覧を生成する方法について説明します。
localization_priority: Priority
ms.openlocfilehash: db888c8d562f57bd46edc251f4917e9e03d85d95
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528100"
---
# <a name="generate-a-list-of-autodiscover-endpoints"></a><span data-ttu-id="3975d-103">自動検出エンドポイントの一覧を生成する</span><span class="sxs-lookup"><span data-stu-id="3975d-103">Generate a list of Autodiscover endpoints</span></span>

<span data-ttu-id="3975d-104">自動検出エンドポイントの優先順位を付けた一覧を生成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="3975d-104">Find out how to generate a prioritized list of Autodiscover endpoints.</span></span>
  
<span data-ttu-id="3975d-p101">[自動検出プロセス](autodiscover-for-exchange.md)の最初のタスクは、アプリケーションが試用する自動検出エンドポイントの一覧を生成することです。これらの自動検出エンドポイントは、[SCP 参照](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)で見つけるか、ユーザーのメール アドレスから派生します。最終的に、たくさんのエンドポイントが存在する結果になる場合があります。優先度ごとに整理する方法を見てみましょう。</span><span class="sxs-lookup"><span data-stu-id="3975d-p101">The first task in the [Autodiscover process](autodiscover-for-exchange.md) is to generate a list of Autodiscover endpoints for your application to try. These Autodiscover endpoints can come from an [SCP lookup](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) or can be derived from the user's email address. In the end, you can end up with a large number of endpoints. Let's take a look at how you can organize them by priority.</span></span> 
  
## <a name="start-with-scp-lookup"></a><span data-ttu-id="3975d-109">SCP 参照から始める</span><span class="sxs-lookup"><span data-stu-id="3975d-109">Start with SCP lookup</span></span>
<span data-ttu-id="3975d-110"><a name="bk_StartWithScp"> </a></span><span class="sxs-lookup"><span data-stu-id="3975d-110"><a name="bk_StartWithScp"> </a></span></span>

<span data-ttu-id="3975d-p102">[SCP 参照](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)で見つかる自動検出エンドポイントは、一覧での優先度が最上位になります。管理者は、クライアントを最も近い自動検出エンドポイントまたは最も効率的なエンドポイントにルーティングするよう SCP オブジェクトを構成できるので、これらのエンドポイントから始めることをお勧めします。SCP 参照プロセスには独自の優先度スキーマがあるため、SCP 参照の結果は次の順位で既に優先度が設定されています。</span><span class="sxs-lookup"><span data-stu-id="3975d-p102">Autodiscover endpoints that come from an [SCP lookup](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) should have top priority in your list. Administrators can configure SCP objects to route your client to the closest or most efficient Autodiscover endpoint, so it is a good idea to start with these endpoints. Because the SCP lookup process has its own prioritization scheme, the results of an SCP lookup are already prioritized, as follows:</span></span> 
  
1. <span data-ttu-id="3975d-114">クライアント コンピューターが属する Active Directory サイトを対象とする SCP オブジェクトからの自動検出エンドポイント。</span><span class="sxs-lookup"><span data-stu-id="3975d-114">Autodiscover endpoints from SCP objects scoped to the Active Directory site that the client computer belongs to.</span></span>
    
2. <span data-ttu-id="3975d-115">Active Directory サイトのいずれをも対象としない SCP オブジェクトからの自動検出エンドポイント。</span><span class="sxs-lookup"><span data-stu-id="3975d-115">Autodiscover endpoints from SCP objects not scoped to any Active Directory site.</span></span>
    
3. <span data-ttu-id="3975d-116">クライアント コンピューターが属するサイトとは別の Active Directory サイトを対象とする SCP オブジェクトからの自動検出エンドポイント。</span><span class="sxs-lookup"><span data-stu-id="3975d-116">Autodiscover endpoints from SCP objects scoped to a different Active Directory site than the site that the client computer belongs to.</span></span>
    
<span data-ttu-id="3975d-117">SCP 参照プロセスの結果を取得したら、ユーザーのメール アドレスから派生するエンドポイントを追加できます。</span><span class="sxs-lookup"><span data-stu-id="3975d-117">After you have the results of the SCP lookup process, you can add endpoints that derive from the user's email address.</span></span> <span data-ttu-id="3975d-118">これらのエンドポイントは、既定のエンドポイントのセットおよび、SCP の結果がない、または SCP 参照から返されたエンドポイントが不十分な場合のフォールバックとして使用できます。</span><span class="sxs-lookup"><span data-stu-id="3975d-118">These can serve as a default set of endpoints and a fallback in case there are no SCP results or the endpoints returned from the SCP lookup are not sufficient.</span></span>
  
## <a name="add-endpoints-derived-from-the-users-email-address"></a><span data-ttu-id="3975d-119">ユーザーのメール アドレスから派生したエンドポイントを追加する</span><span class="sxs-lookup"><span data-stu-id="3975d-119">Add endpoints derived from the user's email address</span></span>
<span data-ttu-id="3975d-120"><a name="bk_AddDerivedEndpoints"> </a></span><span class="sxs-lookup"><span data-stu-id="3975d-120"><a name="bk_AddDerivedEndpoints"> </a></span></span>

<span data-ttu-id="3975d-p104">SCP 参照が動作しない場合、または SCP 参照によって返されたエンドポイントが正常な応答を返さない場合、ユーザーのメール アドレスから既定の自動検出エンドポイントのセットを得ることができます。これらのエンドポイントは SCP 参照からのどのエンドポイントよりも優先度は低くなりますが、SCP 参照が失敗する場合に必要になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3975d-p104">When SCP lookup doesn't work, or the endpoints returned by the SCP lookup don't return a successful response, you can derive a set of default Autodiscover endpoints from the user's email address. These endpoints should be a lower priority than any that come from an SCP lookup, but you might need them if the SCP lookup was not successful.</span></span>
  
### <a name="to-derive-autodiscover-endpoints"></a><span data-ttu-id="3975d-123">自動検出エンドポイントを取得する方法</span><span class="sxs-lookup"><span data-stu-id="3975d-123">To derive Autodiscover endpoints</span></span>

1. <span data-ttu-id="3975d-p105">ユーザーのメール アドレスからドメイン名を抽出します。たとえば、ユーザーのメール アドレスが Sadie.Daniels@contoso.com である場合、ドメイン名は contoso.com になります。</span><span class="sxs-lookup"><span data-stu-id="3975d-p105">Extract the domain name from the user's email address. For example, if the user's email address is Sadie.Daniels@contoso.com, the domain name would be contoso.com.</span></span>
    
2. <span data-ttu-id="3975d-126">ファイル拡張子を持たないエンドポイント URL を、次の形式で作成します。</span><span class="sxs-lookup"><span data-stu-id="3975d-126">Construct endpoint URLs without file extensions in the following formats:</span></span>
    
  - <span data-ttu-id="3975d-127">"https://" + ドメイン + "/autodiscover/autodiscover"</span><span class="sxs-lookup"><span data-stu-id="3975d-127">"https://" + domain + "/autodiscover/autodiscover"</span></span>
    
  - <span data-ttu-id="3975d-128">"https://autodiscover."</span><span class="sxs-lookup"><span data-stu-id="3975d-128">"https://autodiscover."</span></span> <span data-ttu-id="3975d-129">+ ドメイン + "/autodiscover/autodiscover"</span><span class="sxs-lookup"><span data-stu-id="3975d-129">+ domain + "/autodiscover/autodiscover"</span></span>
    
<span data-ttu-id="3975d-130">SCP 参照とユーザーのメール アドレスの両方から派生するエンドポイント URL の一覧をコンパイルすると、[SOAP 自動検出 Web サービス](https://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx)または [POX 自動検出 Web サービス](https://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx)を使用しているかどうかによって、それらの URL のファイル名拡張子を変更する必要が生じる場合があります。</span><span class="sxs-lookup"><span data-stu-id="3975d-130">After you compile the list of endpoint URLs that derive from both SCP lookup and the user's email address, you might need to revise file name extensions in those URLs, depending on whether you're using the [SOAP Autodiscover web service](https://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx) or the [POX Autodiscover web service](https://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx).</span></span>
  
## <a name="add-or-replace-file-name-extensions-in-endpoint-urls"></a><span data-ttu-id="3975d-131">エンドポイント URL のファイル名拡張子を追加または置き換える</span><span class="sxs-lookup"><span data-stu-id="3975d-131">Add or replace file name extensions in endpoint URLs</span></span>
<span data-ttu-id="3975d-132"><a name="bk_FileExtensions"> </a></span><span class="sxs-lookup"><span data-stu-id="3975d-132"><a name="bk_FileExtensions"> </a></span></span>

<span data-ttu-id="3975d-p107">自動検出サービスにアクセスするには、SOAP 自動検出 Web サービスまたは POX 自動検出 Web サービスを使用します。各サービスでは、類似したエンドポイント URL (ファイル名拡張子だけが異なる) が使用されます。SOAP 自動検出 Web サービスでは ".svc" ファイル名拡張子が使用され、POX 自動検出 Web サービスでは ".xml" ファイル名拡張子が使用されます。</span><span class="sxs-lookup"><span data-stu-id="3975d-p107">You can access the Autodiscover service by using either the SOAP Autodiscover web service or the POX Autodiscover web service. Each service uses similar endpoint URLs, with the only difference being the file name extension. The SOAP Autodiscover web service uses the ".svc" file name extension, and the POX Autodiscover web service uses the ".xml" file name extension.</span></span>
  
<span data-ttu-id="3975d-p108">既定では、SCP 参照から返された自動検出エンドポイント URL は POX URL です。ただし、SOAP 自動検出を使用している場合は、ファイル名拡張子を ".xml" から ".svc" に変更するだけで、SOAP 要求を試行できます。</span><span class="sxs-lookup"><span data-stu-id="3975d-p108">By default, the Autodiscover endpoint URLs returned from an SCP lookup are POX URLs. However, if you are using SOAP Autodiscover, you can simply change the file name extension from ".xml" to ".svc" and try a SOAP request.</span></span>
  
<span data-ttu-id="3975d-p109">派生した自動検出エンドポイント URL の場合、ファイル拡張子は省略されています。URL を試用する前に、使用中の自動検出 Web サービスに適切なファイル拡張子を追加します。</span><span class="sxs-lookup"><span data-stu-id="3975d-p109">For the derived Autodiscover endpoint URLs, the file extension is omitted. Add the appropriate file extension for the Autodiscover web service you are using prior to trying the URL.</span></span>
  
## <a name="example-generating-a-list-of-autodiscover-endpoints"></a><span data-ttu-id="3975d-140">例: 自動検出エンドポイントの一覧を生成する</span><span class="sxs-lookup"><span data-stu-id="3975d-140">Example: Generating a list of Autodiscover endpoints</span></span>
<span data-ttu-id="3975d-141"><a name="bk_Example"> </a></span><span class="sxs-lookup"><span data-stu-id="3975d-141"><a name="bk_Example"> </a></span></span>

<span data-ttu-id="3975d-p110">例を見てみましょう。Sadie Daniels (Sadie.Daniels@contoso.com) は、Exchange Web サービス (EWS) アプリケーションを初めて使用しています。アプリケーションでは、アプリケーション自体を構成するのに自動検出を使用します。Sadie のコンピューターは、contoso.com ドメインに参加し、Redmond Active Directory サイトにあります。アプリケーションでは、図 1 に示すように自動検出エンドポイントの一覧が生成されます。</span><span class="sxs-lookup"><span data-stu-id="3975d-p110">Let's take a look at an example. Sadie Daniels (Sadie.Daniels@contoso.com) is using an Exchange Web Services (EWS) application for the first time. The application uses Autodiscover to configure itself. Sadie's computer is joined to the contoso.com domain and is in the Redmond Active Directory site. The application generates the list of Autodiscover endpoints shown in Figure 1.</span></span>
  
<span data-ttu-id="3975d-147">**図 1: 自動検出エンドポイントのサンプルの一覧**</span><span class="sxs-lookup"><span data-stu-id="3975d-147">**Figure 1: Sample list of Autodiscover endpoints**</span></span>

![導出されたエンドポイントよりも高い優先順位を持つエンドポイントとして SCP ルックアップから取得された、Autodiscover エンドポイントのサンプル リスト。](media/Ex15_Autodiscover_GenerateList_Example.png)
  
<span data-ttu-id="3975d-149">この例の EWS アプリケーションでは SOAP 自動検出 Web サービスが使用されるため、SCP 結果のファイル名拡張子を ".svc" に変更してから SOAP 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="3975d-149">The EWS application in this example prefers the SOAP Autodiscover web service, so it changes the file name extension for the SCP results to ".svc" before sending SOAP requests to them.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="3975d-150">次の手順</span><span class="sxs-lookup"><span data-stu-id="3975d-150">Next steps</span></span>
<span data-ttu-id="3975d-151"><a name="bk_NextSteps"> </a></span><span class="sxs-lookup"><span data-stu-id="3975d-151"><a name="bk_NextSteps"> </a></span></span>

<span data-ttu-id="3975d-152">自動検出エンドポイントの一覧を生成したら、[それらのエンドポイントに要求を送信する](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)ことによって試用します。</span><span class="sxs-lookup"><span data-stu-id="3975d-152">After you generate a list of Autodiscover endpoints, try them by [sending requests to those endpoints](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="3975d-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="3975d-153">See also</span></span>


- [<span data-ttu-id="3975d-154">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="3975d-154">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="3975d-155">Exchange の SCP 参照を使用して自動検出エンドポイントを見つける</span><span class="sxs-lookup"><span data-stu-id="3975d-155">Find Autodiscover endpoints by using SCP lookup in Exchange</span></span>](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [<span data-ttu-id="3975d-156">自動検出のエラー メッセージの処理</span><span class="sxs-lookup"><span data-stu-id="3975d-156">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    


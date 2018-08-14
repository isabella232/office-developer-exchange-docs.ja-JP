---
title: Exchange の EWS アプリケーションのトラブルシューティングに使用するツールとリソース
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ee7fcd05-35d7-47bf-bac4-e719c49c11fe
description: EWS マネージ API アプリケーションまたは EWS アプリケーションのトラブルシューティングに役立つリソースを紹介します。
ms.openlocfilehash: d8d8ea736ca3b896642ad06f5987caeba8d8d059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759189"
---
# <a name="tools-and-resources-for-troubleshooting-ews-applications-for-exchange"></a><span data-ttu-id="9b3b8-103">Exchange の EWS アプリケーションのトラブルシューティングに使用するツールとリソース</span><span class="sxs-lookup"><span data-stu-id="9b3b8-103">Tools and resources for troubleshooting EWS applications for Exchange</span></span>

<span data-ttu-id="9b3b8-104">EWS マネージ API アプリケーションまたは EWS アプリケーションのトラブルシューティングに役立つリソースを紹介します。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-104">Find resources to help you troubleshoot your EWS Managed API or EWS application.</span></span>
  
<span data-ttu-id="9b3b8-p101">物事は計画どおりに進まないことがあります。ときには EWS の要求が失敗することや、予期しない結果が生じることがあります。これは、特に理由が明らかでないときにはイライラするかもしれません。この状況に陥らないことが何よりですが、もしものために、この記事では問題のトラブルシューティングに役立つツールとリソースに関する情報をご提供します。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-p101">Things don't always go as planned. Sometimes EWS requests fail, or provide unexpected results. This can be frustrating, especially if the reason isn't obvious. Hopefully this never happens to you, but if it does, this article provides information about tools and resources that you can use to help troubleshoot your problem.</span></span>
  
> [!NOTE]
> <span data-ttu-id="9b3b8-109">この記事では、一般的なトラブルシューティングのアドバイスと、トラブルシューティング情報のソースを提供します。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-109">This article provides general troubleshooting advice and sources for troubleshooting information.</span></span> <span data-ttu-id="9b3b8-110">残念なことに、トラブルシューティング手順の詳細について説明することはできません。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-110">Unfortunately it isn't possible to give detailed troubleshooting steps.</span></span> <span data-ttu-id="9b3b8-111">特定のエラーをトラブルシューティングする際の支援については、「[次の手順](#bk_NextSteps)」をご参照ください。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-111">For assistance troubleshooting your specific error, see [Next steps](#bk_NextSteps).</span></span> 
  
## <a name="examine-the-soap-requests-and-responses"></a><span data-ttu-id="9b3b8-112">SOAP の要求と応答を調べる</span><span class="sxs-lookup"><span data-stu-id="9b3b8-112">Examine the SOAP requests and responses</span></span>

<span data-ttu-id="9b3b8-113">物事が適切に動作しないときには、何が起こっているかが確認できると、とても助かります。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-113">When things aren't working correctly, it really helps to be able to see what's going on.</span></span> <span data-ttu-id="9b3b8-114">EWS または EWS マネージ API に関わる問題を調査しているときに最初に調べることは、アプリケーションがネットワークを通じて送信している要求とサーバーが送り返してきた応答を調べることです。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-114">When things aren’t working correctly, it really helps to be able to see what's going on. The first line of inquiry when investigating a problem with EWS or the EWS Managed API is to examine the requests that your application is sending over the network and the responses that the server is sending back.</span></span>
  
<span data-ttu-id="9b3b8-115">EWS マネージ API には[組み込みのトレース機能](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)があるため、SOAP の要求と応答を簡単に調べることができます。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-115">The EWS Managed API makes examining SOAP requests and responses easy with its [built in tracing functionality](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md).</span></span> <span data-ttu-id="9b3b8-116">EWS を使用している場合、同様のトレース機能にアクセスできるかどうかは、要求の送信に使用しているプラットフォームやクラスによって決まります。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-116">If you are using EWS, you might or might not have access to similar tracing functionality, depending on what platform or classes you use to send your requests.</span></span> <span data-ttu-id="9b3b8-117">ただし、[Network Monitor](http://www.microsoft.com/en-us/download/details.aspx?id=4865) や [Fiddler](http://www.telerik.com/fiddler) などのネットワーク トレース ツールは、ネットワーク トラフィックを調べたり、要求と応答のペイロードを表示したりするためにいつでも使用できます。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-117">However, you can always use a network tracing tool like [Network Monitor](http://www.microsoft.com/en-us/download/details.aspx?id=4865) or [Fiddler](http://www.telerik.com/fiddler) to examine the network traffic and view the request and response payloads.</span></span> 
  
<span data-ttu-id="9b3b8-118">さらに、[クライアントの要求をインストルメント化する](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)ことで、要求と応答から得られる情報の質が高まります。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-118">Additionally, you can [instrument your client requests](instrumenting-client-requests-for-ews-and-rest-in-exchange.md) to enhance the information available in requests and responses.</span></span> 
  
<span data-ttu-id="9b3b8-p105">要求と応答を手に入れたら、次の点について自問してください。それらは正しいように見えるか。アプリケーションは期待どおりの値を送信しているか。応答に矛盾がないか。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-p105">After you have the requests and responses, ask yourself the following: Do they look correct? Are the values that your application is sending expected? Do the responses make sense?</span></span>
  
## <a name="examine-error-codes"></a><span data-ttu-id="9b3b8-122">エラー コードを調べる</span><span class="sxs-lookup"><span data-stu-id="9b3b8-122">Examine error codes</span></span>

<span data-ttu-id="9b3b8-123">エラー コードは、一見無意味に見えるものであっても、問題を特定するために非常に役立つことがあります。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-123">Sometimes the error code can go a long way toward pinpointing the problem, even if at first glance it doesn't seem to make sense. Does the error indicate that your client is being throttled? Perhaps a call to Autodiscover to refresh configuration information is in order?</span></span> <span data-ttu-id="9b3b8-124">クライアントが[調整されている](ews-throttling-in-exchange.md)ことをエラーが示していないか。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-124">Does the error indicate that your client is being [throttled](ews-throttling-in-exchange.md)?</span></span> <span data-ttu-id="9b3b8-125">おそらく[構成情報を更新する](how-to-refresh-configuration-information-by-using-autodiscover.md)ための自動検出の呼び出しが適切であるか。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-125">Perhaps a call to Autodiscover to [refresh configuration information](how-to-refresh-configuration-information-by-using-autodiscover.md) is in order?</span></span> 
  
<span data-ttu-id="9b3b8-126">特定のエラー処理の詳細については、次の記事をご参照ください。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-126">For more information about handling specific errors, see the following articles:</span></span>
  
- [<span data-ttu-id="9b3b8-127">自動検出のエラー メッセージの処理</span><span class="sxs-lookup"><span data-stu-id="9b3b8-127">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
- [<span data-ttu-id="9b3b8-128">Exchange の EWS での通知に関連するエラーの処理</span><span class="sxs-lookup"><span data-stu-id="9b3b8-128">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="9b3b8-129">Exchange の EWS での同期に関連するエラーの処理</span><span class="sxs-lookup"><span data-stu-id="9b3b8-129">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="9b3b8-130">Exchange の EWS での削除に関連するエラーの処理</span><span class="sxs-lookup"><span data-stu-id="9b3b8-130">Handling deletion-related errors in EWS in Exchange</span></span>](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="verify-versions"></a><span data-ttu-id="9b3b8-131">バージョンを確認する</span><span class="sxs-lookup"><span data-stu-id="9b3b8-131">Verify versions</span></span>

<span data-ttu-id="9b3b8-132">EWS 操作に関連するコンポーネントは数種類あり、それらのコンポーネントのバージョンが結果に影響することがあります。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-132">There are a number of different components involved in EWS operations, and the versions of those components can influence the results.</span></span>
  
<span data-ttu-id="9b3b8-133">**表 1. EWS プロセスに影響する可能性のあるバージョン付きコンポーネント**</span><span class="sxs-lookup"><span data-stu-id="9b3b8-133">**Table 1.  Versioned components that can affect EWS processes**</span></span>

|<span data-ttu-id="9b3b8-134">**コンポーネント**</span><span class="sxs-lookup"><span data-stu-id="9b3b8-134">**Component**</span></span>|<span data-ttu-id="9b3b8-135">**EWS マネージ API**</span><span class="sxs-lookup"><span data-stu-id="9b3b8-135">**EWS Managed API**</span></span>|<span data-ttu-id="9b3b8-136">**EWS**</span><span class="sxs-lookup"><span data-stu-id="9b3b8-136">**EWS**</span></span>|<span data-ttu-id="9b3b8-137">**メモ**</span><span class="sxs-lookup"><span data-stu-id="9b3b8-137">**Notes**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="9b3b8-138">要求されるサーバーのバージョン</span><span class="sxs-lookup"><span data-stu-id="9b3b8-138">Requested server version</span></span>  <br/> |<span data-ttu-id="9b3b8-139">[ExchangeServiceBase.RequestedServerVersion](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b3b8-139">[ExchangeServiceBase.RequestedServerVersion](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="9b3b8-140">[RequestServerVersion](http://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx) 要素</span><span class="sxs-lookup"><span data-stu-id="9b3b8-140">[RequestServerVersion](http://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx) element</span></span>  <br/> |<span data-ttu-id="9b3b8-p107">この値により、EWS 要求の処理に使用される EWS スキーマのバージョンが制御されます。ここで指定されたスキーマのバージョンが、送信する要求に適していることを確認します。一部のプロパティと操作は、以前のスキーマのバージョンでは利用できません。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-p107">This value controls which version of the EWS schema is used to process the EWS request. Make sure that the schema version specified here makes sense for the request you are sending. Some properties and operations are not available in earlier versions of the schema.</span></span>  <br/> |
|<span data-ttu-id="9b3b8-144">サーバーのバージョン</span><span class="sxs-lookup"><span data-stu-id="9b3b8-144">The server version</span></span>  <br/> |<span data-ttu-id="9b3b8-145">[ExchangeServiceBase.ServerInfo](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservicebase.serverinfo%28v=exchg.80%29.aspx) プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b3b8-145">[ExchangeServiceBase.ServerInfo](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservicebase.serverinfo%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="9b3b8-146">[ServerVersionInfo](http://msdn.microsoft.com/library/c04a6872-ca27-432b-aac2-36b023d0afc6%28Office.15%29.aspx) 要素</span><span class="sxs-lookup"><span data-stu-id="9b3b8-146">[ServerVersionInfo](http://msdn.microsoft.com/library/c04a6872-ca27-432b-aac2-36b023d0afc6%28Office.15%29.aspx) element</span></span>  <br/> |<span data-ttu-id="9b3b8-p108">この値は EWS の応答でサーバーから返され、応答を処理したサーバーのバージョンを表します。この値が期待していたものであることを確認します。可能な場合は、Exchange サーバーが Exchange のメジャー バージョンに向けた最新の更新プログラムを実行していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-p108">This value is returned by the server in EWS responses, and indicates the version of the server that processed the response. Make sure this value is what you expect. If possible, make sure that the Exchange server is running the most recent update for your major version of Exchange.</span></span>  <br/> |
|<span data-ttu-id="9b3b8-150">EWS マネージ API のバージョン</span><span class="sxs-lookup"><span data-stu-id="9b3b8-150">The EWS Managed API version</span></span>  <br/> |<span data-ttu-id="9b3b8-151">Microsoft.Exchange.WebServices.dll ファイルの製品バージョン プロパティ。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-151">The Product version property of the Microsoft.Exchange.WebServices.dll file.</span></span>  <br/> |<span data-ttu-id="9b3b8-152">該当なし</span><span class="sxs-lookup"><span data-stu-id="9b3b8-152">Not applicable</span></span>  <br/> |<span data-ttu-id="9b3b8-153">EWS マネージ API を使用している場合は、[最新のバージョン](http://aka.ms/ews-managed-api-readme)を使用していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-153">If you're using the EWS Managed API, make sure that you are using [the most recent versionhttp://aka.ms/ews-managed-api-readme](http://aka.ms/ews-managed-api-readme).</span></span>  <br/> |
   
## <a name="verify-access"></a><span data-ttu-id="9b3b8-154">アクセスを確認する</span><span class="sxs-lookup"><span data-stu-id="9b3b8-154">Verify access</span></span>

<span data-ttu-id="9b3b8-155">EWS は既定で有効化されていますが、[既定値は変更可能](how-to-control-access-to-ews-in-exchange.md)です。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-155">EWS is enabled by default, but [defaults can be changed](how-to-control-access-to-ews-in-exchange.md).</span></span> <span data-ttu-id="9b3b8-156">[Get-OrganizationConfig](http://technet.microsoft.com/ja-JP/library/bb124754.aspx) コマンドレットを使用して EWS がサーバー上で有効化されていることを確認し、[Get-CASMailbox](http://technet.microsoft.com/ja-JP/library/aa997571.aspx) コマンドレットを使用して EWS がユーザーのメールボックスに対して有効化されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-156">Use the [Get-OrganizationConfig](http://technet.microsoft.com/ja-JP/library/bb124754.aspx) cmdlet to make sure that EWS is enabled on the server, and the [Get-CASMailbox](http://technet.microsoft.com/ja-JP/library/aa997571.aspx) cmdlet to make sure that EWS is enabled for the user's mailbox.</span></span> <span data-ttu-id="9b3b8-157">また、EWS の許可または禁止リストについて両方のコマンドレットの応答を調べて、目的のアプリケーションが EWS の使用を禁止されていないことも確認します。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-157">Also check both cmdlet responses for an EWS allow or block list, and make sure that your application isn't blocked from using EWS.</span></span> 
  
<span data-ttu-id="9b3b8-158">さらに、EWS 仮想ディレクトリの[既定の認証設定](http://technet.microsoft.com/ja-JP/library/gg247612%28v=exchg.150%29.aspx)が変更されていないことも確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-158">You should also verify that the [default authentication settingshttp://technet.microsoft.com/en-us/library/gg247612(v=exchg.150).aspx](http://technet.microsoft.com/ja-JP/library/gg247612%28v=exchg.150%29.aspx) on the EWS virtual directory have not been modified.</span></span> 
  
## <a name="try-another-ews-client"></a><span data-ttu-id="9b3b8-159">別の EWS クライアントを試してみる</span><span class="sxs-lookup"><span data-stu-id="9b3b8-159">Try another EWS client</span></span>

<span data-ttu-id="9b3b8-p110">ときには別のクライアントから同じ要求を試してみて、結果を比較することが役立つことがあります。別のクライアントの結果が異なっているならば、違いは何でしょうか。成功した要求と失敗した要求の違いを見つけることは、特定の要求が失敗する理由を説明する際に役立つことがあります。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-p110">Sometimes it is helpful to try the same request from another client and compare results. If another client gets different results, what is different? Figuring out what is different between a successful request and a failed request can help explain why a particular request is failing.</span></span>
  
<span data-ttu-id="9b3b8-163">テストに使用する別のクライアントを記述することもできますが、その必要はありません。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-163">While you can certainly write another client to test with, you don't have to!</span></span> <span data-ttu-id="9b3b8-164">[EWSEditor](http://ewseditor.codeplex.com/) は、EWS マネージ API と EWS を使用するサンプル クライアントです。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-164">[EWSEditor](http://ewseditor.codeplex.com/) is a sample client that uses the EWS Managed API and EWS.</span></span> <span data-ttu-id="9b3b8-165">このクライアントはダウンロードが可能です (ソース コードを含む)。これを使用して、目的のアプリケーションで失敗したものと同じ要求を試してみることができます。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-165">While you can certainly write another client to test with, you don't have to! EWSEditorhttp://ewseditor.codeplex.com/ is a sample client that uses the EWS Managed API and EWS. You can download the client (including the source code) and use it to try the same requests that are failing in your application.</span></span> 
  
## <a name="examine-iis-logs"></a><span data-ttu-id="9b3b8-166">IIS のログを調べる</span><span class="sxs-lookup"><span data-stu-id="9b3b8-166">Examine IIS logs</span></span>

<span data-ttu-id="9b3b8-p112">Exchange サーバーにアクセスしている場合は、クライアント アクセス サーバー上のインターネット インフォメーション サービス (IIS) が提供するログ記録機能により、失敗に関する詳細な情報が得られます。ただし、IIS のログは HTTP エラーを受信した場合にのみ役立つものだという点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-p112">If you have access to the Exchange server, the logging functionality provided by Internet Information Services (IIS) on the Client Access servers can provide more information about failures. However, keep in mind that IIS logs will only be helpful if you are receiving an HTTP error.</span></span>
  
<span data-ttu-id="9b3b8-169">IIS には、2 種類のログ記録方式があります。[IIS ログ記録](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis)と[失敗した要求のトレース](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)です。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-169">IIS provides two different logging methods: [IIS logging](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis) and [failed requests tracing](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis).</span></span> <span data-ttu-id="9b3b8-170">IIS のログを扱う場合は、いくつかの組み込み EWS クエリが含まれている [Log Parser Studio](http://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-170">To work with IIS logs, you can use [Log Parser Studio](http://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx), which includes a number of built-in EWS queries.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="9b3b8-171">次の手順</span><span class="sxs-lookup"><span data-stu-id="9b3b8-171">Next steps</span></span>
<span data-ttu-id="9b3b8-172"><a name="bk_NextSteps"> </a></span><span class="sxs-lookup"><span data-stu-id="9b3b8-172"></span></span>

<span data-ttu-id="9b3b8-173">トラブルシューティングに使用できるツールとリソースについて理解すると、それらのツールが提示する情報を理解するための支援が必要になることでしょう。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-173">Now that you’ve learned about the tools and resources that you can use to troubleshoot, you might need help understanding the information provided by those tools. The following are some options for getting help:</span></span> <span data-ttu-id="9b3b8-174">次に、支援を得るためのオプションを示します。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-174">The following are some options for getting help:</span></span>
  
- <span data-ttu-id="9b3b8-175">[MSDN の Exchange Server 開発者フォーラム](http://social.msdn.microsoft.com/Forums/en-US/home?category=exchangeserver) — MSDN Exchange Server 開発者コミュニティに質問してください。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-175">[Exchange Server Development forum on MSDNhttp://social.msdn.microsoft.com/Forums/en-US/home?category=exchangeserver](http://social.msdn.microsoft.com/Forums/en-US/home?category=exchangeserver) — Ask a question of the MSDN Exchange Server development community.</span></span> 
    
- <span data-ttu-id="9b3b8-176">[StackOverflow](http://stackoverflow.com/tags/ews) — StackOverflow コミュニティに質問してください。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-176">[StackOverflow](http://stackoverflow.com/tags/ews) — Ask a question of the StackOverflow community.</span></span> <span data-ttu-id="9b3b8-177">投稿には必ず "ews" のタグを付けてください。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-177">Be sure to tag your question with microsoft-graph.</span></span> 
    
- <span data-ttu-id="9b3b8-178">[Microsoft サポート](http://support.microsoft.com/ph/730/en-us) — Microsoft サポート担当者にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-178">[Microsoft Supporthttp://support.microsoft.com/ph/730/en-us](http://support.microsoft.com/ph/730/en-us) — Contact a Microsoft support professional for assistance.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="9b3b8-179">関連項目</span><span class="sxs-lookup"><span data-stu-id="9b3b8-179">See also</span></span>


<span data-ttu-id="9b3b8-180">次の記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-180">See the following articles:</span></span>
  
- [<span data-ttu-id="9b3b8-181">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="9b3b8-181">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="9b3b8-182">要求と応答をトレースして、EWS マネージ API アプリケーションのトラブルシューティングを行う</span><span class="sxs-lookup"><span data-stu-id="9b3b8-182">How to: Trace requests and responses to troubleshoot EWS Managed API applications</span></span>](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    
- [<span data-ttu-id="9b3b8-183">Exchange で EWS と REST のクライアントの要求をインストルメント化する</span><span class="sxs-lookup"><span data-stu-id="9b3b8-183">Instrumenting client requests for EWS and REST in Exchange</span></span>](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)
    
- [<span data-ttu-id="9b3b8-184">Exchange での EWS 調整</span><span class="sxs-lookup"><span data-stu-id="9b3b8-184">EWS throttling in Exchange</span></span>](ews-throttling-in-exchange.md)
    
- [<span data-ttu-id="9b3b8-185">自動検出を使用して構成情報を更新する</span><span class="sxs-lookup"><span data-stu-id="9b3b8-185">How to: Refresh configuration information by using Autodiscover</span></span>](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [<span data-ttu-id="9b3b8-186">自動検出のエラー メッセージの処理</span><span class="sxs-lookup"><span data-stu-id="9b3b8-186">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
- [<span data-ttu-id="9b3b8-187">Exchange の EWS での通知に関連するエラーの処理</span><span class="sxs-lookup"><span data-stu-id="9b3b8-187">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="9b3b8-188">Exchange の EWS での同期に関連するエラーの処理</span><span class="sxs-lookup"><span data-stu-id="9b3b8-188">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="9b3b8-189">Exchange の EWS での削除に関連するエラーの処理</span><span class="sxs-lookup"><span data-stu-id="9b3b8-189">Handling deletion-related errors in EWS in Exchange</span></span>](handling-deletion-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="9b3b8-190">IIS のログ記録の構成</span><span class="sxs-lookup"><span data-stu-id="9b3b8-190">Configuring Logging in IIS</span></span>](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis)
    
- [<span data-ttu-id="9b3b8-191">IIS 7 のトレースを使用して失敗した要求をトラブルシューティングする</span><span class="sxs-lookup"><span data-stu-id="9b3b8-191">Troubleshooting Failed Requests Using Tracing in IIS 7http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis</span></span>](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)
    
- [<span data-ttu-id="9b3b8-192">概要: Log Parser Studio</span><span class="sxs-lookup"><span data-stu-id="9b3b8-192">Introducing: Log Parser Studio</span></span>](http://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx)
    
- [<span data-ttu-id="9b3b8-193">Exchange 仮想ディレクトリの既定の設定</span><span class="sxs-lookup"><span data-stu-id="9b3b8-193">Default Settings for Exchange Virtual Directories</span></span>](http://technet.microsoft.com/ja-JP/library/gg247612%28v=exchg.150%29.aspx)
    
<span data-ttu-id="9b3b8-194">次のものをダウンロードしてください。</span><span class="sxs-lookup"><span data-stu-id="9b3b8-194">Download the following:</span></span>
  
- [<span data-ttu-id="9b3b8-195">Microsoft ネットワーク モニター 3.4</span><span class="sxs-lookup"><span data-stu-id="9b3b8-195">Microsoft Network Monitor 3.4</span></span>](http://www.microsoft.com/en-us/download/details.aspx?id=4865)
    
- [<span data-ttu-id="9b3b8-196">Fiddler</span><span class="sxs-lookup"><span data-stu-id="9b3b8-196">Fiddler</span></span>](http://www.telerik.com/fiddler)
    
- [<span data-ttu-id="9b3b8-197">EWSEditor</span><span class="sxs-lookup"><span data-stu-id="9b3b8-197">EWSEditor</span></span>](http://ewseditor.codeplex.com/)
    
- [<span data-ttu-id="9b3b8-198">Exchange Web サービス マネージ API</span><span class="sxs-lookup"><span data-stu-id="9b3b8-198">Exchange Web Services Managed API</span></span>](http://go.microsoft.com/fwlink/?LinkID=255472)
    


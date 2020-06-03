---
title: Exchange の自動検出を使用するときにパフォーマンスを向上させる
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e65ff6b2-3810-43ad-9728-27308891b193
description: カスタム アプリケーションで自動検出プロセスのパフォーマンスを向上させる方法について説明します。
ms.openlocfilehash: 844b56084b4f0b5e49b4ee095688d58ce469baca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456333"
---
# <a name="improving-performance-when-using-autodiscover-for-exchange"></a><span data-ttu-id="03dc2-103">Exchange の自動検出を使用するときにパフォーマンスを向上させる</span><span class="sxs-lookup"><span data-stu-id="03dc2-103">Improving performance when using Autodiscover for Exchange</span></span>

<span data-ttu-id="03dc2-104">カスタム アプリケーションで自動検出プロセスのパフォーマンスを向上させる方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="03dc2-104">Learn about ways to improve the performance of the Autodiscover process in your application.</span></span>
  
<span data-ttu-id="03dc2-105">自動検出が優れている理由はいくつもあります。</span><span class="sxs-lookup"><span data-stu-id="03dc2-105">There are a lot of reasons to like Autodiscover.</span></span> <span data-ttu-id="03dc2-106">ユーザーの操作なしに、Exchange に接続するようにカスタム アプリケーションを構成できることは、特に優れています。</span><span class="sxs-lookup"><span data-stu-id="03dc2-106">Configuring your application to connect to Exchange with no user intervention is great!</span></span> <span data-ttu-id="03dc2-107">この記事の読者は自動検出が優秀であることと、これを使用することの理由をすべて理解しているはずなので、ここではその説明を省きます。</span><span class="sxs-lookup"><span data-stu-id="03dc2-107">If you're reading this article, you probably already know all the reasons to use and love Autodiscover, so we won't list them here.</span></span> <span data-ttu-id="03dc2-108">その代わりに、潜在的な短所であるパフォーマンスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="03dc2-108">Instead, we're going to talk about a potential downside: performance.</span></span>
  
<span data-ttu-id="03dc2-p102">自動検出は本質的に遅いプロセスではありません。ただし、本質的に高速なプロセスでもありません。[自動検出プロセス](autodiscover-for-exchange.md)には、多くのネットワーク アクティビティが伴われ、それが多くの遅延の可能性を招くことになります。自動検出プロセスには 3 つのフェーズがあります。すべてのフェーズが潜在的にパフォーマンスに影響を与えます。</span><span class="sxs-lookup"><span data-stu-id="03dc2-p102">Autodiscover isn't inherently a slow process, but it's not inherently fast either. The [Autodiscover process](autodiscover-for-exchange.md) involves a lot of network activity, and that introduces a lot of potential for delays. The Autodiscover process has three phases; all three have the potential to affect performance:</span></span> 
  
- <span data-ttu-id="03dc2-112">自動検出エンドポイント候補のプールを定義する: ドメインに参加しているコンピューター上で実行中のアプリケーションの場合は、Active Directory ドメイン サービス (AD DS) との通信が必要になる [SCP 参照](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)を伴うことがあります。</span><span class="sxs-lookup"><span data-stu-id="03dc2-112">Defining the Autodiscover endpoint candidate pool — For applications running on domain-joined computers, this can involve [SCP lookups](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md), which involves communicating with Active Directory Domain Services (AD DS).</span></span>
    
- <span data-ttu-id="03dc2-113">各候補を試してみる: これには、候補のエンドポイントごとの HTTP 要求/応答が必要になります。</span><span class="sxs-lookup"><span data-stu-id="03dc2-113">Trying each candidate — This requires an HTTP request/response to each candidate endpoint.</span></span>
    
- <span data-ttu-id="03dc2-114">その他の候補を試してみる: 自動検出エンドポイント候補のプールに含まれる候補から成果が得られなかったときには、認証されていない GET 要求 (HTTP 要求/応答) と DNS の参照を実行することになります。</span><span class="sxs-lookup"><span data-stu-id="03dc2-114">Trying other alternatives — When the candidates in your Autodiscover endpoint candidate pool don't produce results, you can do an unauthenticated GET request (HTTP request/response) and a DNS lookup.</span></span>
    
<span data-ttu-id="03dc2-p103">一見したところでは、それほど大量ではないようです。ただし、自動検出エンドポイント候補のプールが複数の URL であり、プール内で最後の URL まで機能するエンドポイントが見つからないというシナリオではどうなるでしょう。遅延が顕著に現れるようになります。そこで、何ができるかを考えてみましょう。</span><span class="sxs-lookup"><span data-stu-id="03dc2-p103">On the surface this might not seem like much. However, imagine a scenario where the Autodiscover endpoint candidate pool is more than one or two URLs, and you don't find a working one until the last URL in your pool. The delay can become a bit more noticeable. So, what can you do?</span></span>
  
## <a name="consider-the-need-for-scp-lookup"></a><span data-ttu-id="03dc2-119">SCP 参照の必要性について検討する</span><span class="sxs-lookup"><span data-stu-id="03dc2-119">Consider the need for SCP lookup</span></span>

<span data-ttu-id="03dc2-p104">SCP オブジェクトが存在していて適切に構成されている場合は、それによって自動検出プロセスを高速化できます。それ以外の状況では、速度を低下させることがあります。目的の環境内で SCP が使用されていない場合は、自動検出プロセスの SCP 参照の部分をすべて省略して時間を短縮します。</span><span class="sxs-lookup"><span data-stu-id="03dc2-p104">When SCP objects are present and configured well, they can speed up the Autodiscover process. In other situations, however, they can slow it down. If SCP isn't used in your environment, skip the entire SCP lookup portion of the Autodiscover process to save time.</span></span>
  
<span data-ttu-id="03dc2-123">これは、EWS マネージ API によって簡単に実施できます。単に [ExchangeService.AutodiscoverUrl](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) メソッドを呼び出す前に [ExchangeService.EnableScpLookup](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.enablescplookup%28v=exchg.80%29.aspx) プロパティを **false** に設定するだけです。</span><span class="sxs-lookup"><span data-stu-id="03dc2-123">The EWS Managed API makes this easy: just set the [ExchangeService.EnableScpLookup](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.enablescplookup%28v=exchg.80%29.aspx) property to **false** before calling the [ExchangeService.AutodiscoverUrl](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="03dc2-124">[AutodiscoverService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice%28v=exchg.80%29.aspx) クラスを使用している場合は、そのクラスのメソッドを呼び出す前に、[AutodiscoverService.EnableScpLookup](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.enablescplookup%28v=exchg.80%29.aspx) プロパティを **false** に設定します。</span><span class="sxs-lookup"><span data-stu-id="03dc2-124">If you're using the [AutodiscoverService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice%28v=exchg.80%29.aspx) class, set the [AutodiscoverService.EnableScpLookup](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.enablescplookup%28v=exchg.80%29.aspx) property to **false** before calling any of its methods.</span></span> 
  
## <a name="use-autodiscover-less-often"></a><span data-ttu-id="03dc2-125">自動検出の使用頻度を下げる</span><span class="sxs-lookup"><span data-stu-id="03dc2-125">Use Autodiscover less often</span></span>

<span data-ttu-id="03dc2-p106">自動検出は、アプリケーションで頻繁に使用されるようには設計されていません。自動検出の暗黙的な対象は、構成情報を検出するために自動検出を使用して、その情報を一定期間キャッシュするアプリケーションです。構成情報をキャッシュしていない場合は、自動検出の使用回数を減らすために、カスタム アプリケーションへのキャッシュ機能の追加を検討します。</span><span class="sxs-lookup"><span data-stu-id="03dc2-p106">Autodiscover isn't designed to be used frequently use by applications. The intent behind Autodiscover is for an application to use it to discover configuration information, and then cache that information for a period of time. If you aren't caching configuration information, consider adding caching to your application to reduce the number of times you use Autodiscover.</span></span>
  
<span data-ttu-id="03dc2-p107">既にキャッシュしている場合でも、構成情報のキャッシュ期間を査定します。標準では、[24 時間ごとに自動検出の情報を更新](how-to-refresh-configuration-information-by-using-autodiscover.md)しますが、この時間は延長してもかまいません。対象の環境でテストして、目的どおりに動作する構成の "有効時間" を導き出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="03dc2-p107">Even if you are already caching, evaluate how long you cache configuration information. The standard is to [refresh Autodiscover information every 24 hours](how-to-refresh-configuration-information-by-using-autodiscover.md), but you might be able to extend that time. You should test with your target environments and come up with a "time-to-live" for your configuration that works for you.</span></span>
  
## <a name="minimize-requested-data"></a><span data-ttu-id="03dc2-132">要求データを最小限に抑える</span><span class="sxs-lookup"><span data-stu-id="03dc2-132">Minimize requested data</span></span>

<span data-ttu-id="03dc2-133">EWS マネージ API の **AutodiscoverService** クラスを使用している場合や、SOAP で [GetUserSettings 操作 (SOAP)](https://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx) を使用している場合は、応答で返される設定の内容を直接制御できます。</span><span class="sxs-lookup"><span data-stu-id="03dc2-133">If you're using the **AutodiscoverService** class in the EWS Managed API, or the [GetUserSettings operation (SOAP)](https://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx) operation via SOAP, you have direct control over what settings are returned in the response.</span></span> <span data-ttu-id="03dc2-134">多数の設定を要求できますが、アプリケーションに必要な設定は、そのうちのわずかなものである可能性があります。</span><span class="sxs-lookup"><span data-stu-id="03dc2-134">Although you can request quite a few settings, chances are that your application only needs a handful of them.</span></span> <span data-ttu-id="03dc2-135">要求した設定ごとにサーバー上での処理が増えるため、応答の待機時間が長引くようになります。</span><span class="sxs-lookup"><span data-stu-id="03dc2-135">Every setting that you request requires more processing on the server, which means more time waiting for a response.</span></span> <span data-ttu-id="03dc2-136">要求している設定を査定して、不要なものを省きます。</span><span class="sxs-lookup"><span data-stu-id="03dc2-136">Evaluate the settings you are requesting, and eliminate any that you don't need.</span></span> 
  
<span data-ttu-id="03dc2-137">EWS マネージ API の **ExchangeService.AutodiscoverUrl** メソッドを使用している場合は、要求する設定を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="03dc2-137">If you're using the **ExchangeService.AutodiscoverUrl** method in the EWS Managed API, you cannot change the settings you request.</span></span> <span data-ttu-id="03dc2-138">ただし、このメソッドはすでに非常に効率的なものになっています。このメソッドは、[UserSettingName enumeration](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=exchg.80%29.aspx) 列挙体の **ExternalEwsUrl** と **InternalEwsUrl** の設定のみを要求します。</span><span class="sxs-lookup"><span data-stu-id="03dc2-138">However, this method is already fairly efficient; it only requests the **ExternalEwsUrl** and **InternalEwsUrl** settings from the [UserSettingName enumeration](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=exchg.80%29.aspx).</span></span>
  
<span data-ttu-id="03dc2-139">POX 自動検出サービスを使用している場合は、[特定のプロパティを要求できません ](autodiscover-for-exchange.md#bk_Options)。</span><span class="sxs-lookup"><span data-stu-id="03dc2-139">If you're using the POX Autodiscover service, [you cannot request specific properties](autodiscover-for-exchange.md#bk_Options).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="03dc2-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="03dc2-140">See also</span></span>


- [<span data-ttu-id="03dc2-141">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="03dc2-141">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="03dc2-142">Exchange の SCP 参照を使用して自動検出エンドポイントを見つける</span><span class="sxs-lookup"><span data-stu-id="03dc2-142">Find Autodiscover endpoints by using SCP lookup in Exchange</span></span>](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [<span data-ttu-id="03dc2-143">自動検出を使用して構成情報を更新する</span><span class="sxs-lookup"><span data-stu-id="03dc2-143">Refresh configuration information by using Autodiscover</span></span>](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [<span data-ttu-id="03dc2-144">ExchangeService クラス</span><span class="sxs-lookup"><span data-stu-id="03dc2-144">ExchangeService class</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="03dc2-145">AutodiscoverService クラス</span><span class="sxs-lookup"><span data-stu-id="03dc2-145">AutodiscoverService class</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice%28v=exchg.80%29.aspx)
    


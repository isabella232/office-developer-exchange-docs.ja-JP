---
title: EWS のマネージ API を使用して、EWS のサービスの URL を設定します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: cddf6525-1c04-484b-a911-56c2f0f1f7b6
description: EWS マネージ API アプリケーションでの EWS サービス URL の設定方法について説明します。
ms.openlocfilehash: e1a414f7c6f13bd61a58403c9d2be546c0226a69
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759051"
---
# <a name="set-the-ews-service-url-by-using-the-ews-managed-api"></a><span data-ttu-id="c5755-103">EWS のマネージ API を使用して、EWS のサービスの URL を設定します。</span><span class="sxs-lookup"><span data-stu-id="c5755-103">Set the EWS service URL by using the EWS Managed API</span></span>

<span data-ttu-id="c5755-104">EWS マネージ API アプリケーションでの EWS サービス URL の設定方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="c5755-104">Find information about how to set the EWS service URL in your EWS Managed API application.</span></span>
  
<span data-ttu-id="c5755-105">サービスの URL は、Exchange は、Exchange Web サービス (EWS) との通信に使用するアドレスです。</span><span class="sxs-lookup"><span data-stu-id="c5755-105">The service URL is the address that Exchange uses to communicate with Exchange Web Services (EWS).</span></span> <span data-ttu-id="c5755-106">EWS のマネージ API アプリケーションはこのアドレスを持ち、 [EWS を使って通信](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)するために適切なアクセス権を持つ後、 [ExchangeService クラス](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)への呼び出しが行えます。</span><span class="sxs-lookup"><span data-stu-id="c5755-106">After your EWS Managed API application has this address, and has appropriate access to [communicate with EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md), it can make calls to the [ExchangeService class](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="c5755-107">オンプレミスの Exchange サーバーのサービスの URL は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="c5755-107">The service URL for an on-premises Exchange server might look like the following.</span></span> 
  
```HTML
https://computer.domain.contoso.com/EWS/Exchange.asmx
```

<span data-ttu-id="c5755-108">いくつかの方法では、アプリケーションでは、EWS の URL を設定できます。</span><span class="sxs-lookup"><span data-stu-id="c5755-108">You can set the EWS URL in your application in a couple of ways.</span></span> <span data-ttu-id="c5755-109">[自動検出サービス](http://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)を使用して、URL を取得する別のサーバーにメールボックスを移行する場合、大規模なフォレスト内のサーバー、URL を変更することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="c5755-109">We recommend that you use the [Autodiscover service](http://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx) to get the URL because in a large forest of servers, the URL can change if the mailbox is migrated to another server.</span></span> <span data-ttu-id="c5755-110">ただし、自動検出を呼び出す時間がかかることができ、キャッシュすることができます、時間の短い期間に複数の呼び出しを実行する必要がある場合、アプリケーションの速度が低下するため URL の値自動検出からを取得し、キャッシュされたこの va の EWS のサービスの URL を手動で設定lue。</span><span class="sxs-lookup"><span data-stu-id="c5755-110">However, because calling Autodiscover can take some time and can slow down your application if you need to make multiple calls in a short period of time, you might want to cache the URL value you get from Autodiscover and manually set the EWS service URL with this cached value.</span></span> <span data-ttu-id="c5755-111">これにより、アプリケーションのパフォーマンスが向上します。だけで自動検出を使用して、サーバーの値が変更された場合でも定期的にキャッシュされた値を更新することを確認します。</span><span class="sxs-lookup"><span data-stu-id="c5755-111">This will improve the performance of your application; just make sure that you use Autodiscover to update your cached value periodically in case the value changes on the server.</span></span> 
  
## <a name="set-the-ews-service-url-by-using-the-autodiscover-service"></a><span data-ttu-id="c5755-112">自動検出サービスを使用して EWS サービス URL を設定する</span><span class="sxs-lookup"><span data-stu-id="c5755-112">Set the EWS service URL by using the Autodiscover service</span></span>
<span data-ttu-id="c5755-113"><a name="bk_SetURLusingAutoDiscover"> </a></span><span class="sxs-lookup"><span data-stu-id="c5755-113"></span></span>

<span data-ttu-id="c5755-114">[AutodiscoverUrl](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx)メソッドでは、 [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)エンドポイントを設定するのには電子メール アドレスを使用し、 **ExchangeService**プロキシ クラスに含まれるすべてのメソッドを使用するアプリケーションを有効にします。</span><span class="sxs-lookup"><span data-stu-id="c5755-114">The [AutodiscoverUrl](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) method uses the email address to set the [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) endpoint and enables your application to use any methods included in the **ExchangeService** proxy classes.</span></span> <span data-ttu-id="c5755-115">次の例では、 **AutodiscoverURL**メソッドを使用する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="c5755-115">The following example shows how to use the **AutodiscoverURL** method.</span></span> 
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.AutodiscoverUrl("User1@contoso.com");

```

## <a name="set-the-exchange-service-url-manually"></a><span data-ttu-id="c5755-116">Exchange サービス URL を手動で設定する</span><span class="sxs-lookup"><span data-stu-id="c5755-116">Set the Exchange service URL manually</span></span>
<span data-ttu-id="c5755-117"><a name="bk_SetURLmanually"> </a></span><span class="sxs-lookup"><span data-stu-id="c5755-117"></span></span>

<span data-ttu-id="c5755-p104">次の例は、キャッシュされた値を使用して EWS サービス URL を設定する方法を示しています。これを行う前に、自動検出サービスを使用して EWS URL を必ず取得するようにしてください。</span><span class="sxs-lookup"><span data-stu-id="c5755-p104">The following example shows you how to set the EWS service URL by using a cached value. Before you do this, make sure to use the Autodiscover service to get the EWS URL.</span></span>
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.Url = new Uri("https://computername.domain.contoso.com/EWS/Exchange.asmx");

```

## <a name="see-also"></a><span data-ttu-id="c5755-120">関連項目</span><span class="sxs-lookup"><span data-stu-id="c5755-120">See also</span></span>

- [<span data-ttu-id="c5755-121">EWS マネージ API クライアント アプリケーションの概要</span><span class="sxs-lookup"><span data-stu-id="c5755-121">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)   
- [<span data-ttu-id="c5755-122">Exchange アプリケーションの開発環境を設定します。</span><span class="sxs-lookup"><span data-stu-id="c5755-122">Setting up your Exchange application development environment</span></span>](setting-up-your-exchange-application-development-environment.md)   
- [<span data-ttu-id="c5755-123">Exchange EWS へのアクセスを制御します。</span><span class="sxs-lookup"><span data-stu-id="c5755-123">Control access to EWS in Exchange</span></span>](how-to-control-access-to-ews-in-exchange.md) 
- [<span data-ttu-id="c5755-124">EWS のマネージ API を使用して通信 EWS</span><span class="sxs-lookup"><span data-stu-id="c5755-124">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)  
- [<span data-ttu-id="c5755-125">自動検出を使用してコネクション ポイントを検索するには</span><span class="sxs-lookup"><span data-stu-id="c5755-125">Use Autodiscover to find connection points</span></span>](how-to-use-autodiscover-to-find-connection-points.md)
    


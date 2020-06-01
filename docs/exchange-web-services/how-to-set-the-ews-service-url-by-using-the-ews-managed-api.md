---
title: EWS マネージ API を使用して EWS サービス URL を設定する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: cddf6525-1c04-484b-a911-56c2f0f1f7b6
description: EWS マネージ API アプリケーションでの EWS サービス URL の設定方法について説明します。
localization_priority: Priority
ms.openlocfilehash: 5ba79b48d4eb4fec62110448c5924de16b67ce10
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456739"
---
# <a name="set-the-ews-service-url-by-using-the-ews-managed-api"></a><span data-ttu-id="47dc8-103">EWS マネージ API を使用して EWS サービス URL を設定する</span><span class="sxs-lookup"><span data-stu-id="47dc8-103">Set the EWS service URL by using the EWS Managed API</span></span>

<span data-ttu-id="47dc8-104">EWS マネージ API アプリケーションでの EWS サービス URL の設定方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="47dc8-104">Find information about how to set the EWS service URL in your EWS Managed API application.</span></span>
  
<span data-ttu-id="47dc8-105">サービス URL は、Exchange が Exchange Web サービス (EWS) との通信に使用するアドレスです。</span><span class="sxs-lookup"><span data-stu-id="47dc8-105">The service URL is the address that Exchange uses to communicate with Exchange Web Services (EWS).</span></span> <span data-ttu-id="47dc8-106">このアドレスを認識していて、[EWS と通信する](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)ための適切なアクセス権のある EWS マネージ API アプリケーションは、[ExchangeService クラス](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)の呼び出しを行えます。</span><span class="sxs-lookup"><span data-stu-id="47dc8-106">After your EWS Managed API application has this address, and has appropriate access to [communicate with EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md), it can make calls to the [ExchangeService class](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="47dc8-107">オンプレミス Exchange サーバーのサービス URL は、たとえば次のようになります。</span><span class="sxs-lookup"><span data-stu-id="47dc8-107">The service URL for an on-premises Exchange server might look like the following.</span></span> 
  
```HTML
https://computer.domain.contoso.com/EWS/Exchange.asmx
```

<span data-ttu-id="47dc8-p102">アプリケーションで EWS URL を設定するには、2 とおりの方法があります。[自動検出サービス](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)を使用して URL を取得することをお勧めします。大規模なサーバー フォレストでは、メールボックスが別のサーバーに移行されると、URL が変わることがあるからです。ただし、自動検出の呼び出しはある程度時間がかかることがあるため、短時間に複数の呼び出しを行う必要がある場合は、アプリケーションの速度が低下することがあります。したがって、自動検出から取得した URL 値をキャッシュし、キャッシュされたこの値を使用して EWS サービス URL を手動で設定した方がよい場合があります。この方法をとれば、アプリケーションのパフォーマンスが向上します。ただし、サーバーの値が変わった場合に備えて、キャッシュされた値を自動検出を使用して定期的に更新するようにしてください。</span><span class="sxs-lookup"><span data-stu-id="47dc8-p102">You can set the EWS URL in your application in a couple of ways. We recommend that you use the [Autodiscover service](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx) to get the URL because in a large forest of servers, the URL can change if the mailbox is migrated to another server. However, because calling Autodiscover can take some time and can slow down your application if you need to make multiple calls in a short period of time, you might want to cache the URL value you get from Autodiscover and manually set the EWS service URL with this cached value. This will improve the performance of your application; just make sure that you use Autodiscover to update your cached value periodically in case the value changes on the server.</span></span> 
  
## <a name="set-the-ews-service-url-by-using-the-autodiscover-service"></a><span data-ttu-id="47dc8-112">自動検出サービスを使用して EWS サービス URL を設定する</span><span class="sxs-lookup"><span data-stu-id="47dc8-112">Set the EWS service URL by using the Autodiscover service</span></span>
<span data-ttu-id="47dc8-113"><a name="bk_SetURLusingAutoDiscover"> </a></span><span class="sxs-lookup"><span data-stu-id="47dc8-113"><a name="bk_SetURLusingAutoDiscover"> </a></span></span>

<span data-ttu-id="47dc8-114">[AutodiscoverUrl](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) メソッドは、メール アドレスを使用して [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) エンドポイントを設定し、**ExchangeService** プロキシ クラスに含まれるどのメソッドもアプリケーションが使用できるようにします。</span><span class="sxs-lookup"><span data-stu-id="47dc8-114">The [AutodiscoverUrl](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) method uses the email address to set the [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) endpoint and enables your application to use any methods included in the **ExchangeService** proxy classes.</span></span> <span data-ttu-id="47dc8-115">次の例に、**AutodiscoverURL** メソッドの使用方法を示します。</span><span class="sxs-lookup"><span data-stu-id="47dc8-115">The following example shows how to use the **AutodiscoverURL** method.</span></span> 
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.AutodiscoverUrl("User1@contoso.com");

```

## <a name="set-the-exchange-service-url-manually"></a><span data-ttu-id="47dc8-116">Exchange サービス URL を手動で設定する</span><span class="sxs-lookup"><span data-stu-id="47dc8-116">Set the Exchange service URL manually</span></span>
<span data-ttu-id="47dc8-117"><a name="bk_SetURLmanually"> </a></span><span class="sxs-lookup"><span data-stu-id="47dc8-117"><a name="bk_SetURLmanually"> </a></span></span>

<span data-ttu-id="47dc8-p104">次の例は、キャッシュされた値を使用して EWS サービス URL を設定する方法を示しています。これを行う前に、自動検出サービスを使用して EWS URL を必ず取得するようにしてください。</span><span class="sxs-lookup"><span data-stu-id="47dc8-p104">The following example shows you how to set the EWS service URL by using a cached value. Before you do this, make sure to use the Autodiscover service to get the EWS URL.</span></span>
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.Url = new Uri("https://computername.domain.contoso.com/EWS/Exchange.asmx");

```

## <a name="see-also"></a><span data-ttu-id="47dc8-120">関連項目</span><span class="sxs-lookup"><span data-stu-id="47dc8-120">See also</span></span>

- [<span data-ttu-id="47dc8-121">EWS マネージ API クライアント アプリケーションの概要</span><span class="sxs-lookup"><span data-stu-id="47dc8-121">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)   
- [<span data-ttu-id="47dc8-122">Exchange アプリケーションの開発環境をセットアップする</span><span class="sxs-lookup"><span data-stu-id="47dc8-122">Setting up your Exchange application development environment</span></span>](setting-up-your-exchange-application-development-environment.md)   
- [<span data-ttu-id="47dc8-123">Exchange で EWS へのアクセスを制御する</span><span class="sxs-lookup"><span data-stu-id="47dc8-123">Control access to EWS in Exchange</span></span>](how-to-control-access-to-ews-in-exchange.md) 
- [<span data-ttu-id="47dc8-124">EWS マネージ API を使用して EWS と通信する</span><span class="sxs-lookup"><span data-stu-id="47dc8-124">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)  
- [<span data-ttu-id="47dc8-125">自動検出を使用して接続ポイントを検索する</span><span class="sxs-lookup"><span data-stu-id="47dc8-125">Use Autodiscover to find connection points</span></span>](how-to-use-autodiscover-to-find-connection-points.md)
    


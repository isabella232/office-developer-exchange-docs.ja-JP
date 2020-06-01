---
title: Exchange 用自動検出 Web サービス リファレンス
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a01124a8-a8cf-4b80-8625-d7ee05690bca
description: Exchange の自動検出 web サービスの参照コンテンツを検索します。
ms.openlocfilehash: ce7f2bbd662a5e61959c7e3c6748f0cf40cc4fb3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466872"
---
# <a name="autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="499d3-103">Exchange 用自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="499d3-103">Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="499d3-104">Exchange の自動検出 web サービスの参照コンテンツを検索します。</span><span class="sxs-lookup"><span data-stu-id="499d3-104">Find reference content for the Autodiscover web service in Exchange.</span></span>
  
<span data-ttu-id="499d3-105">自動検出 web サービスは、アプリケーションが Exchange サーバーへの接続を作成するために使用する構成情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="499d3-105">The Autodiscover web service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="499d3-106">次のいずれかのオプションを使用して自動検出に接続できます。</span><span class="sxs-lookup"><span data-stu-id="499d3-106">You can use one of the following options to connect to Autodiscover:</span></span>
  
- <span data-ttu-id="499d3-107">SOAP 自動検出サービス: exchange Online を含む exchange 2010 以降のバージョンの Exchange に接続するクライアントが使用できます。</span><span class="sxs-lookup"><span data-stu-id="499d3-107">SOAP Autodiscover service —Available to clients that connect to versions of Exchange starting with Exchange 2010, including Exchange Online.</span></span>
    
- <span data-ttu-id="499d3-108">"プレーン旧 XML" (POX) 自動検出サービス— exchange Online (exchange Online など) から2007始まる Exchange のバージョンに接続するクライアントが利用できます。</span><span class="sxs-lookup"><span data-stu-id="499d3-108">"plain old XML" (POX) Autodiscover service — Available to clients that connect to versions of Exchange starting with Exchange 2007, including Exchange Online.</span></span> 
    
<span data-ttu-id="499d3-109">SOAP と POX 自動検出サービスの両方で、クライアントが Exchange サーバーへの接続を作成するために使用する構成情報を提供できます。</span><span class="sxs-lookup"><span data-stu-id="499d3-109">Both the SOAP and the POX Autodiscover service can provide the configuration information that your client will use to create a connection to an Exchange server.</span></span>
  
> [!NOTE]
> <span data-ttu-id="499d3-110">Exchange 2010 以降のバージョンの Exchange では、POX 自動検出サービスの代わりに SOAP 自動検出サービスを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="499d3-110">For versions of Exchange starting with Exchange 2010, we recommend that you use the SOAP Autodiscover service instead of the POX Autodiscover service.</span></span> <span data-ttu-id="499d3-111">SOAP 自動検出サービスは、バッチ自動検出設定要求を提供し、応答で返される設定をより細かく制御します。</span><span class="sxs-lookup"><span data-stu-id="499d3-111">The SOAP Autodiscover service provides batched Autodiscover setting requests and more granular control over which settings are returned in the response.</span></span> 
  
<span data-ttu-id="499d3-112">このセクションには、SOAP 自動検出サービスおよび POX 自動検出サービスに関するリファレンス情報が記載されています。</span><span class="sxs-lookup"><span data-stu-id="499d3-112">This section contains reference information for the SOAP Autodiscover service and the POX Autodiscover service.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="499d3-113">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="499d3-113">In this section</span></span>
<span data-ttu-id="499d3-114"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="499d3-114"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="499d3-115">Exchange 用 SOAP 自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="499d3-115">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)
    
- [<span data-ttu-id="499d3-116">Exchange 用 POX 自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="499d3-116">POX Autodiscover web service reference for Exchange</span></span>](pox-autodiscover-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="499d3-117">関連項目</span><span class="sxs-lookup"><span data-stu-id="499d3-117">See also</span></span>

- [<span data-ttu-id="499d3-118">Exchange の Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="499d3-118">Web services reference for Exchange</span></span>](web-services-reference-for-exchange.md)
- [<span data-ttu-id="499d3-119">自動検出サービス (SOAP)</span><span class="sxs-lookup"><span data-stu-id="499d3-119">Autodiscover Service (SOAP)</span></span>](https://msdn.microsoft.com/library/e24d1a1f-0d20-4bd9-ae4c-9112ecacea78%28Office.15%29.aspx)
- [<span data-ttu-id="499d3-120">自動検出サービス (POX)</span><span class="sxs-lookup"><span data-stu-id="499d3-120">Autodiscover Service (POX)</span></span>](https://msdn.microsoft.com/library/13c54de3-a91c-4424-8732-99dd8f2162ec%28Office.15%29.aspx)
    


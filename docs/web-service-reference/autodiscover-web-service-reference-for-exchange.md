---
title: Exchange の自動検出 web サービスの参照
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a01124a8-a8cf-4b80-8625-d7ee05690bca
description: Exchange 自動検出 web サービスのコンテンツの参照を検索します。
ms.openlocfilehash: 48ca4a93c2120079cb675eabbc460bf0e75570b2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759474"
---
# <a name="autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="e0821-103">Exchange の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="e0821-103">Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="e0821-104">Exchange 自動検出 web サービスのコンテンツの参照を検索します。</span><span class="sxs-lookup"><span data-stu-id="e0821-104">Find reference content for the Autodiscover web service in Exchange.</span></span>
  
<span data-ttu-id="e0821-105">自動検出 web サービスは、Exchange サーバーへの接続を作成するアプリケーションで使用される構成情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="e0821-105">The Autodiscover web service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="e0821-106">自動検出に接続するには、次のオプションのいずれかを使用します。</span><span class="sxs-lookup"><span data-stu-id="e0821-106">You can use one of the following options to connect to Autodiscover:</span></span>
  
- <span data-ttu-id="e0821-107">SOAP サービスを自動検出-から Exchange 2010 を Exchange Online を含む Exchange のバージョンに接続するクライアントに使用可能です。</span><span class="sxs-lookup"><span data-stu-id="e0821-107">SOAP Autodiscover service —Available to clients that connect to versions of Exchange starting with Exchange 2010, including Exchange Online.</span></span>
    
- <span data-ttu-id="e0821-108">"標準古い XML"(POX) の自動検出サービスなどのバージョンの Exchange Online を含め、Exchange 2007 から Exchange に接続するクライアントに使用可能です。</span><span class="sxs-lookup"><span data-stu-id="e0821-108">"plain old XML" (POX) Autodiscover service — Available to clients that connect to versions of Exchange starting with Exchange 2007, including Exchange Online.</span></span> 
    
<span data-ttu-id="e0821-109">SOAP と POX の自動検出サービスの両方が、クライアントが Exchange サーバーへの接続を作成するのに使用される構成情報を提供できます。</span><span class="sxs-lookup"><span data-stu-id="e0821-109">Both the SOAP and the POX Autodiscover service can provide the configuration information that your client will use to create a connection to an Exchange server.</span></span>
  
> [!NOTE]
> <span data-ttu-id="e0821-110">Exchange が Exchange 2010 以降のバージョンでは、POX の自動検出サービスではなく、SOAP の自動検出サービスを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="e0821-110">For versions of Exchange starting with Exchange 2010, we recommend that you use the SOAP Autodiscover service instead of the POX Autodiscover service.</span></span> <span data-ttu-id="e0821-111">SOAP の自動検出サービスは、自動検出の設定要求のバッチ処理しより詳細に制御する設定は応答を提供します。</span><span class="sxs-lookup"><span data-stu-id="e0821-111">The SOAP Autodiscover service provides batched Autodiscover setting requests and more granular control over which settings are returned in the response.</span></span> 
  
<span data-ttu-id="e0821-112">このセクションには、SOAP の自動検出サービスと POX の自動検出サービスに関するリファレンス情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e0821-112">This section contains reference information for the SOAP Autodiscover service and the POX Autodiscover service.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="e0821-113">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="e0821-113">In this section</span></span>
<span data-ttu-id="e0821-114"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="e0821-114"></span></span>

- [<span data-ttu-id="e0821-115">Exchange の自動検出 web サービスの参照が SOAP します。</span><span class="sxs-lookup"><span data-stu-id="e0821-115">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)
    
- [<span data-ttu-id="e0821-116">Exchange の POX の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="e0821-116">POX Autodiscover web service reference for Exchange</span></span>](pox-autodiscover-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="e0821-117">関連項目</span><span class="sxs-lookup"><span data-stu-id="e0821-117">See also</span></span>

- [<span data-ttu-id="e0821-118">Exchange web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="e0821-118">Web services reference for Exchange</span></span>](web-services-reference-for-exchange.md)
- [<span data-ttu-id="e0821-119">自動検出サービス (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e0821-119">Autodiscover Service (SOAP)</span></span>](http://msdn.microsoft.com/library/e24d1a1f-0d20-4bd9-ae4c-9112ecacea78%28Office.15%29.aspx)
- [<span data-ttu-id="e0821-120">自動検出サービス (POX)</span><span class="sxs-lookup"><span data-stu-id="e0821-120">Autodiscover Service (POX)</span></span>](http://msdn.microsoft.com/library/13c54de3-a91c-4424-8732-99dd8f2162ec%28Office.15%29.aspx)
    


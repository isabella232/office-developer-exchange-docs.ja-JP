---
title: Exchange 用ユニファイドメッセージング web サービスのリファレンス
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Unified
api_type:
- schema
ms.assetid: 83afea8a-c716-41df-9eb2-e1000357afb6
description: Exchange のユニファイドメッセージング (UM) web サービスの参照コンテンツを検索します。
ms.openlocfilehash: e4bb63f34650dae8fc28016196c97a6b79e69df0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467376"
---
# <a name="unified-messaging-web-service-reference-for-exchange"></a><span data-ttu-id="1ed27-103">Exchange 用ユニファイドメッセージング web サービスのリファレンス</span><span class="sxs-lookup"><span data-stu-id="1ed27-103">Unified Messaging web service reference for Exchange</span></span>

<span data-ttu-id="1ed27-104">Exchange のユニファイドメッセージング (UM) web サービスの参照コンテンツを検索します。</span><span class="sxs-lookup"><span data-stu-id="1ed27-104">Find reference content for the Unified Messaging (UM) web service in Exchange.</span></span>
  
<span data-ttu-id="1ed27-105">ユニファイドメッセージング (UM) web サービスは、クライアントが UM プロパティに関する情報を読み取って変更できるようにする機能拡張ポイントを提供し、テレフォニーデバイス上でメールボックスストアアイテムを解析してディクテーションすることを要求します。</span><span class="sxs-lookup"><span data-stu-id="1ed27-105">The Unified Messaging (UM) web service provides an extensibility point that enables clients to read and change information about UM properties and request that mailbox store items be parsed and dictated over a telephony device.</span></span> <span data-ttu-id="1ed27-106">このセクションには、UM web サービスの XML メッセージを構成する操作と要素に関する情報が記載されています。</span><span class="sxs-lookup"><span data-stu-id="1ed27-106">This section contains information about the operations and elements that make up the XML messages for the UM web service.</span></span> <span data-ttu-id="1ed27-107">このコンテンツは、https:// \<yourclientaccessserver\> /EWS/UM2007Legacy に似たサービスエンドポイント URL に適用されます。</span><span class="sxs-lookup"><span data-stu-id="1ed27-107">This content applies to the service endpoint URL that is similar to https://\<yourclientaccessserver\>.com/EWS/UM2007Legacy.asmx.</span></span> 
  
<span data-ttu-id="1ed27-108">自動検出サービスを使用して、UM web サービスエンドポイントへの URL を取得できます。</span><span class="sxs-lookup"><span data-stu-id="1ed27-108">You can use the Autodiscover service to get the URL to the UM web service endpoint.</span></span> <span data-ttu-id="1ed27-109">自動検出の詳細については、「 [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ed27-109">For more information about Autodiscover, see [Autodiscover for Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="1ed27-110">Exchange 2010 以降のバージョンの Exchange では、次の理由から、UM web サービスの代わりに[Exchange Web サービス (EWS)](https://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx)で使用可能なユニファイドメッセージング操作を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="1ed27-110">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](https://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the UM web service, for the following reasons:</span></span> 
> - <span data-ttu-id="1ed27-111">EWS ベースの UM 機能には、EWS マネージ API でのファーストクラスのサポートが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1ed27-111">The EWS-based UM features have first-class support in the EWS Managed API.</span></span> 
> - <span data-ttu-id="1ed27-112">Exchange 2010 以降のバージョンの Exchange では、新しい UM 機能が EWS に追加されますが、ユニファイドメッセージング web サービスには追加されません。</span><span class="sxs-lookup"><span data-stu-id="1ed27-112">In versions of Exchange starting with Exchange 2010, new UM features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
<span data-ttu-id="1ed27-113">UM web サービスには明示的なスキーマがありません。</span><span class="sxs-lookup"><span data-stu-id="1ed27-113">The UM web service does not have an explicit schema.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="1ed27-114">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="1ed27-114">In this section</span></span>
<span data-ttu-id="1ed27-115"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="1ed27-115"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="1ed27-116">Exchange のユニファイドメッセージング web サービスの操作</span><span class="sxs-lookup"><span data-stu-id="1ed27-116">Unified Messaging web service operations for Exchange</span></span>](unified-messaging-web-service-operations-for-exchange.md)   
- [<span data-ttu-id="1ed27-117">Exchange 用のユニファイドメッセージング web サービスの XML 要素</span><span class="sxs-lookup"><span data-stu-id="1ed27-117">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="1ed27-118">関連項目</span><span class="sxs-lookup"><span data-stu-id="1ed27-118">See also</span></span>

- [<span data-ttu-id="1ed27-119">Exchange 用自動検出 Web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="1ed27-119">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="1ed27-120">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="1ed27-120">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="1ed27-121">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="1ed27-121">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    


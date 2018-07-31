---
title: Exchange ユニファイド メッセージング web サービス リファレンス
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
description: Exchange ユニファイド メッセージング (UM) web サービスのコンテンツの参照を検索します。
ms.openlocfilehash: 9e124f504ecee517edc51610696f06729904d75f
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354275"
---
# <a name="unified-messaging-web-service-reference-for-exchange"></a><span data-ttu-id="d054f-103">Exchange ユニファイド メッセージング web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="d054f-103">Unified Messaging web service reference for Exchange</span></span>

<span data-ttu-id="d054f-104">Exchange ユニファイド メッセージング (UM) web サービスのコンテンツの参照を検索します。</span><span class="sxs-lookup"><span data-stu-id="d054f-104">Find reference content for the Unified Messaging (UM) web service in Exchange.</span></span>
  
<span data-ttu-id="d054f-105">ユニファイド メッセージング (UM) の web サービスには、読み取り、UM プロパティに関する情報を変更して、メールボックス ストアの項目の構文解析やテレフォニー デバイス経由で音声入力を要求するクライアントを有効にする機能拡張ポイントが用意されています。</span><span class="sxs-lookup"><span data-stu-id="d054f-105">The Unified Messaging (UM) web service provides an extensibility point that enables clients to read and change information about UM properties and request that mailbox store items be parsed and dictated over a telephony device.</span></span> <span data-ttu-id="d054f-106">このセクションには、操作および UM web サービスの XML メッセージを構成する要素に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d054f-106">This section contains information about the operations and elements that make up the XML messages for the UM web service.</span></span> <span data-ttu-id="d054f-107">このコンテンツは、https:// のようなサービス エンドポイントの URL に適用されます\<yourclientaccessserver\>.com/EWS/UM2007Legacy.asmx。</span><span class="sxs-lookup"><span data-stu-id="d054f-107">This content applies to the service endpoint URL that is similar to https://\<yourclientaccessserver\>.com/EWS/UM2007Legacy.asmx.</span></span> 
  
<span data-ttu-id="d054f-108">UM web サービス エンドポイントの URL を取得するのに自動検出サービスを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="d054f-108">You can use the Autodiscover service to get the URL to the UM web service endpoint.</span></span> <span data-ttu-id="d054f-109">自動検出の詳細については、 [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d054f-109">For more information about Autodiscover, see [Autodiscover for Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="d054f-110">Exchange が Exchange 2010 以降のバージョンでは、次の理由により、UM web サービスではなく[Exchange Web サービス (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx)で利用可能なユニファイド メッセージングの操作を使用することお勧めします。</span><span class="sxs-lookup"><span data-stu-id="d054f-110">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the UM web service, for the following reasons:</span></span> 
> - <span data-ttu-id="d054f-111">UM の EWS ベースの機能では、EWS のマネージ API でファースト クラスのサポートがあります。</span><span class="sxs-lookup"><span data-stu-id="d054f-111">The EWS-based UM features have first-class support in the EWS Managed API.</span></span> 
> - <span data-ttu-id="d054f-112">Exchange が Exchange 2010 以降のバージョンでは、ユニファイド メッセージング web サービスではなく、EWS に UM の新機能が追加されます。</span><span class="sxs-lookup"><span data-stu-id="d054f-112">In versions of Exchange starting with Exchange 2010, new UM features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
<span data-ttu-id="d054f-113">UM web サービスには、明示的なスキーマがありません。</span><span class="sxs-lookup"><span data-stu-id="d054f-113">The UM web service does not have an explicit schema.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="d054f-114">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="d054f-114">In this section</span></span>
<span data-ttu-id="d054f-115"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="d054f-115"></span></span>

- [<span data-ttu-id="d054f-116">ユニファイド メッセージング web サービスの操作の交換</span><span class="sxs-lookup"><span data-stu-id="d054f-116">Unified Messaging web service operations for Exchange</span></span>](unified-messaging-web-service-operations-for-exchange.md)   
- [<span data-ttu-id="d054f-117">ユニファイド メッセージング web サービスの XML 要素の交換</span><span class="sxs-lookup"><span data-stu-id="d054f-117">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="d054f-118">関連項目</span><span class="sxs-lookup"><span data-stu-id="d054f-118">See also</span></span>

- [<span data-ttu-id="d054f-119">Exchange の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="d054f-119">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="d054f-120">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="d054f-120">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="d054f-121">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="d054f-121">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    


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
ms.openlocfilehash: 12ee91c5a8b7e1ba23b937f142a9ae2835697fef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839780"
---
# <a name="unified-messaging-web-service-reference-for-exchange"></a><span data-ttu-id="4bc5b-103">Exchange ユニファイド メッセージング web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="4bc5b-103">Unified Messaging web service reference for Exchange</span></span>

<span data-ttu-id="4bc5b-104">Exchange ユニファイド メッセージング (UM) web サービスのコンテンツの参照を検索します。</span><span class="sxs-lookup"><span data-stu-id="4bc5b-104">Find reference content for the Unified Messaging (UM) web service in Exchange.</span></span>
  
<span data-ttu-id="4bc5b-105">ユニファイド メッセージング (UM) の web サービスには、読み取り、UM プロパティに関する情報を変更して、メールボックス ストアの項目の構文解析やテレフォニー デバイス経由で音声入力を要求するクライアントを有効にする機能拡張ポイントが用意されています。</span><span class="sxs-lookup"><span data-stu-id="4bc5b-105">The Unified Messaging (UM) web service provides an extensibility point that enables clients to read and change information about UM properties and request that mailbox store items be parsed and dictated over a telephony device.</span></span> <span data-ttu-id="4bc5b-106">このセクションには、操作および UM web サービスの XML メッセージを構成する要素に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4bc5b-106">This section contains information about the operations and elements that make up the XML messages for the UM web service.</span></span> <span data-ttu-id="4bc5b-107">このコンテンツは、https:// のようなサービス エンドポイントの URL に適用されます\<yourclientaccessserver\>.com/EWS/UM2007Legacy.asmx。</span><span class="sxs-lookup"><span data-stu-id="4bc5b-107">This content applies to the service endpoint URL that is similar to https://\<yourclientaccessserver\>.com/EWS/UM2007Legacy.asmx.</span></span> 
  
<span data-ttu-id="4bc5b-108">UM web サービス エンドポイントの URL を取得するのに自動検出サービスを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="4bc5b-108">You can use the Autodiscover service to get the URL to the UM web service endpoint.</span></span> <span data-ttu-id="4bc5b-109">自動検出の詳細については、 [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4bc5b-109">For more information about Autodiscover, see [Autodiscover for Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="4bc5b-110">Exchange が Exchange 2010 以降のバージョンでは、ことをお勧め UM web サービスの次の理由からではなく[Exchange Web サービス (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx)で利用可能なユニファイド メッセージングの操作を使用すること: > の EWS ベースの UM 機能を持つEWS のマネージ API の高度にサポートします。</span><span class="sxs-lookup"><span data-stu-id="4bc5b-110">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the UM web service, for the following reasons: >  The EWS-based UM features have first-class support in the EWS Managed API.</span></span> <span data-ttu-id="4bc5b-111">> Exchange が Exchange 2010 以降のバージョンでは、ユニファイド メッセージング web サービスではなく、EWS に UM の新機能が追加されます。</span><span class="sxs-lookup"><span data-stu-id="4bc5b-111">>  In versions of Exchange starting with Exchange 2010, new UM features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
<span data-ttu-id="4bc5b-112">UM web サービスには、明示的なスキーマがありません。</span><span class="sxs-lookup"><span data-stu-id="4bc5b-112">The UM web service does not have an explicit schema.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="4bc5b-113">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="4bc5b-113">In this section</span></span>
<span data-ttu-id="4bc5b-114"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="4bc5b-114"></span></span>

- [<span data-ttu-id="4bc5b-115">ユニファイド メッセージング web サービスの操作の交換</span><span class="sxs-lookup"><span data-stu-id="4bc5b-115">Unified Messaging web service operations for Exchange</span></span>](unified-messaging-web-service-operations-for-exchange.md)
    
- [<span data-ttu-id="4bc5b-116">ユニファイド メッセージング web サービスの XML 要素の交換</span><span class="sxs-lookup"><span data-stu-id="4bc5b-116">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="4bc5b-117">関連項目</span><span class="sxs-lookup"><span data-stu-id="4bc5b-117">See also</span></span>

- [<span data-ttu-id="4bc5b-118">Exchange の自動検出 web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="4bc5b-118">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="4bc5b-119">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="4bc5b-119">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="4bc5b-120">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="4bc5b-120">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    


---
title: ポート (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4046821a-d6f3-4764-82be-4011221ce7a3
description: Port 要素は、ストアへの接続に使用されるポートを指定します。
ms.openlocfilehash: 2da59e03a57b44fb12d14368d1b585ba845eacfe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464015"
---
# <a name="port-pox"></a><span data-ttu-id="63a9e-103">ポート (POX)</span><span class="sxs-lookup"><span data-stu-id="63a9e-103">Port (POX)</span></span>

<span data-ttu-id="63a9e-104">**Port**要素は、ストアへの接続に使用されるポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="63a9e-104">The **Port** element specifies the port that is used to connect to the store.</span></span> 
  
[<span data-ttu-id="63a9e-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="63a9e-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="63a9e-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="63a9e-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="63a9e-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="63a9e-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="63a9e-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="63a9e-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="63a9e-109">ポート (POX)</span><span class="sxs-lookup"><span data-stu-id="63a9e-109">Port (POX)</span></span>](port-pox.md)
  
```xml
<Port/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="63a9e-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="63a9e-110">Attributes and elements</span></span>

<span data-ttu-id="63a9e-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="63a9e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63a9e-112">属性</span><span class="sxs-lookup"><span data-stu-id="63a9e-112">Attributes</span></span>

<span data-ttu-id="63a9e-113">なし。</span><span class="sxs-lookup"><span data-stu-id="63a9e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63a9e-114">子要素</span><span class="sxs-lookup"><span data-stu-id="63a9e-114">Child elements</span></span>

<span data-ttu-id="63a9e-115">なし。</span><span class="sxs-lookup"><span data-stu-id="63a9e-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="63a9e-116">親要素</span><span class="sxs-lookup"><span data-stu-id="63a9e-116">Parent elements</span></span>

|<span data-ttu-id="63a9e-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="63a9e-117">**Element**</span></span>|<span data-ttu-id="63a9e-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="63a9e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63a9e-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="63a9e-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="63a9e-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="63a9e-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="63a9e-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="63a9e-121">Text value</span></span>

<span data-ttu-id="63a9e-122">Text 値は、Exchange サーバーへのアクセスに使用されるポートを表します。</span><span class="sxs-lookup"><span data-stu-id="63a9e-122">The text value represents the port that is used to access the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="63a9e-123">注釈</span><span class="sxs-lookup"><span data-stu-id="63a9e-123">Remarks</span></span>

<span data-ttu-id="63a9e-124">[サーバー (POX)](server-pox.md)要素に URL が含まれている場合、**ポート**値は使用されません。</span><span class="sxs-lookup"><span data-stu-id="63a9e-124">The **Port** value is not used if the [Server (POX)](server-pox.md) element contains a URL.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="63a9e-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="63a9e-125">See also</span></span>



[<span data-ttu-id="63a9e-126">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="63a9e-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


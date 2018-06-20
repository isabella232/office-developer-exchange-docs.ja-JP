---
title: NetworkRequirements (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1555fd2e-05b6-4b94-907b-dae9174049d9
description: NetworkRequirements 要素には、クライアント コンピューターがネットワークでサーバーに接続するインターネット サービス プロバイダー (ISP) の要件を満たしているかどうかを使用する基準が含まれています。
ms.openlocfilehash: f3abcff04cd4121b8dcc7ceff7658ad389e6d0b0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832529"
---
# <a name="networkrequirements-pox"></a><span data-ttu-id="b7c63-103">NetworkRequirements (POX)</span><span class="sxs-lookup"><span data-stu-id="b7c63-103">NetworkRequirements (POX)</span></span>

<span data-ttu-id="b7c63-104">**NetworkRequirements**要素には、クライアント コンピューターがネットワークでサーバーに接続するインターネット サービス プロバイダー (ISP) の要件を満たしているかどうかを使用する基準が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b7c63-104">The **NetworkRequirements** element contains the criteria that are used to determine whether the client computer is on a network that meets the requirements of the Internet service provider (ISP) to connect to the server.</span></span> 
  
[<span data-ttu-id="b7c63-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="b7c63-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="b7c63-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="b7c63-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="b7c63-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="b7c63-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="b7c63-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="b7c63-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="b7c63-109">NetworkRequirements (POX)</span><span class="sxs-lookup"><span data-stu-id="b7c63-109">NetworkRequirements (POX)</span></span>](networkrequirements-pox.md)
  
```xml
<NetworkRequirements>
   <IPv4Start/>
   <IPv4End/>
   <IPv6Start/>
   <IPv6End/>
</NetworkRequirements>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="b7c63-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b7c63-110">Attributes and elements</span></span>

<span data-ttu-id="b7c63-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b7c63-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7c63-112">属性</span><span class="sxs-lookup"><span data-stu-id="b7c63-112">Attributes</span></span>

<span data-ttu-id="b7c63-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b7c63-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b7c63-114">子要素</span><span class="sxs-lookup"><span data-stu-id="b7c63-114">Child elements</span></span>

|<span data-ttu-id="b7c63-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="b7c63-115">**Element**</span></span>|<span data-ttu-id="b7c63-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="b7c63-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7c63-117">IPv4Start (POX)</span><span class="sxs-lookup"><span data-stu-id="b7c63-117">IPv4Start (POX)</span></span>](ipv4start-pox.md) <br/> |<span data-ttu-id="b7c63-118">範囲の IP バージョン 4 (IPv4) の開始を示すものを使用して、ネットワーク上のコンピューターを識別するアドレスです。</span><span class="sxs-lookup"><span data-stu-id="b7c63-118">Identifies the start of a range of IP version 4 (IPv4) addresses that are used to identify a computer on a network.</span></span>  <br/> |
|[<span data-ttu-id="b7c63-119">IPv4End (POX)</span><span class="sxs-lookup"><span data-stu-id="b7c63-119">IPv4End (POX)</span></span>](ipv4end-pox.md) <br/> |<span data-ttu-id="b7c63-120">範囲の IP バージョン 4 (IPv4) の終了位置を示すアドレス、ネットワーク上のコンピューターを識別するために使用します。</span><span class="sxs-lookup"><span data-stu-id="b7c63-120">Identifies the end of a range of IP version 4 (IPv4) addresses that are used to identify a computer on the network.</span></span>  <br/> |
|[<span data-ttu-id="b7c63-121">IPv6Start (POX)</span><span class="sxs-lookup"><span data-stu-id="b7c63-121">IPv6Start (POX)</span></span>](ipv6start-pox.md) <br/> |<span data-ttu-id="b7c63-122">範囲の IP バージョン 6 (IPv6) の開始を示すものを使用して、ネットワーク上のコンピューターを識別するアドレスです。</span><span class="sxs-lookup"><span data-stu-id="b7c63-122">Identifies the start of a range of IP version 6 (IPv6) addresses that are used to identify a computer on a network.</span></span>  <br/> |
|[<span data-ttu-id="b7c63-123">IPv6End (POX)</span><span class="sxs-lookup"><span data-stu-id="b7c63-123">IPv6End (POX)</span></span>](ipv6end-pox.md) <br/> |<span data-ttu-id="b7c63-124">範囲の IP バージョン 6 (IPv6) の終了位置を示す、ネットワーク上のコンピューターの識別に使用されるアドレスです。</span><span class="sxs-lookup"><span data-stu-id="b7c63-124">Identifies the end of a range of IP version 6 (IPv6) addresses that are used to identify a computer on a network.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b7c63-125">親要素</span><span class="sxs-lookup"><span data-stu-id="b7c63-125">Parent elements</span></span>

|<span data-ttu-id="b7c63-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="b7c63-126">**Element**</span></span>|<span data-ttu-id="b7c63-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="b7c63-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7c63-128">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="b7c63-128">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="b7c63-129">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b7c63-129">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b7c63-130">備考</span><span class="sxs-lookup"><span data-stu-id="b7c63-130">Remarks</span></span>

<span data-ttu-id="b7c63-131">電子メール クライアントがネットワークの要件に一致しない場合は、他のプロトコルの種類にしてください。</span><span class="sxs-lookup"><span data-stu-id="b7c63-131">If the e-mail client does not match the network requirements, it should try other protocol types.</span></span> <span data-ttu-id="b7c63-132">Isp は、ISP のネットワーク上にある認証を必要としないが、必要な[プロトコル (POX)](protocol-pox.md)タグを持つサーバーの 1 つのセットを提供することができます。</span><span class="sxs-lookup"><span data-stu-id="b7c63-132">ISPs may provide one set of servers with [Protocol (POX)](protocol-pox.md) tags that do not require authentication but are required to be on the ISP network.</span></span> <span data-ttu-id="b7c63-133">Isp には、認証を必要とするが、特定のネットワーク上に存在する必要はありませんサーバーの別のセットが一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b7c63-133">ISPs may list another set of servers that require authentication but are not required to be on a specific network.</span></span> 
  
<span data-ttu-id="b7c63-134">**NetworkRequirements**要素は、オプションです。</span><span class="sxs-lookup"><span data-stu-id="b7c63-134">The **NetworkRequirements** element is optional.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="b7c63-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="b7c63-135">See also</span></span>



[<span data-ttu-id="b7c63-136">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b7c63-136">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


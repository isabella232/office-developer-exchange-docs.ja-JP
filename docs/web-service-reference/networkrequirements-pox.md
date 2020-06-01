---
title: NetworkRequirements 要件 (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1555fd2e-05b6-4b94-907b-dae9174049d9
description: NetworkRequirements 要件要素には、サーバーに接続するためにインターネットサービスプロバイダー (ISP) の要件を満たすネットワーク上にクライアントコンピューターがあるかどうかを判断するために使用される条件が含まれています。
ms.openlocfilehash: d588f7eb12a445fba9c997c4b9db0a6842105b4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462725"
---
# <a name="networkrequirements-pox"></a><span data-ttu-id="540f9-103">NetworkRequirements 要件 (POX)</span><span class="sxs-lookup"><span data-stu-id="540f9-103">NetworkRequirements (POX)</span></span>

<span data-ttu-id="540f9-104">**Networkrequirements 要件**要素には、サーバーに接続するためにインターネットサービスプロバイダー (ISP) の要件を満たすネットワーク上にクライアントコンピューターがあるかどうかを判断するために使用される条件が含まれています。</span><span class="sxs-lookup"><span data-stu-id="540f9-104">The **NetworkRequirements** element contains the criteria that are used to determine whether the client computer is on a network that meets the requirements of the Internet service provider (ISP) to connect to the server.</span></span> 
  
[<span data-ttu-id="540f9-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="540f9-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="540f9-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="540f9-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="540f9-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="540f9-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="540f9-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="540f9-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="540f9-109">NetworkRequirements 要件 (POX)</span><span class="sxs-lookup"><span data-stu-id="540f9-109">NetworkRequirements (POX)</span></span>](networkrequirements-pox.md)
  
```xml
<NetworkRequirements>
   <IPv4Start/>
   <IPv4End/>
   <IPv6Start/>
   <IPv6End/>
</NetworkRequirements>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="540f9-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="540f9-110">Attributes and elements</span></span>

<span data-ttu-id="540f9-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="540f9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="540f9-112">属性</span><span class="sxs-lookup"><span data-stu-id="540f9-112">Attributes</span></span>

<span data-ttu-id="540f9-113">なし。</span><span class="sxs-lookup"><span data-stu-id="540f9-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="540f9-114">子要素</span><span class="sxs-lookup"><span data-stu-id="540f9-114">Child elements</span></span>

|<span data-ttu-id="540f9-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="540f9-115">**Element**</span></span>|<span data-ttu-id="540f9-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="540f9-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="540f9-117">IPv4Start (POX)</span><span class="sxs-lookup"><span data-stu-id="540f9-117">IPv4Start (POX)</span></span>](ipv4start-pox.md) <br/> |<span data-ttu-id="540f9-118">ネットワーク上のコンピューターを識別するために使用される IP version 4 (IPv4) アドレスの範囲の開始を識別します。</span><span class="sxs-lookup"><span data-stu-id="540f9-118">Identifies the start of a range of IP version 4 (IPv4) addresses that are used to identify a computer on a network.</span></span>  <br/> |
|[<span data-ttu-id="540f9-119">IPv4End (POX)</span><span class="sxs-lookup"><span data-stu-id="540f9-119">IPv4End (POX)</span></span>](ipv4end-pox.md) <br/> |<span data-ttu-id="540f9-120">ネットワーク上のコンピューターを識別するために使用される IP version 4 (IPv4) アドレスの範囲の末尾を識別します。</span><span class="sxs-lookup"><span data-stu-id="540f9-120">Identifies the end of a range of IP version 4 (IPv4) addresses that are used to identify a computer on the network.</span></span>  <br/> |
|[<span data-ttu-id="540f9-121">IPv6Start (POX)</span><span class="sxs-lookup"><span data-stu-id="540f9-121">IPv6Start (POX)</span></span>](ipv6start-pox.md) <br/> |<span data-ttu-id="540f9-122">ネットワーク上のコンピューターを識別するために使用される IP version 6 (IPv6) アドレスの範囲の開始を識別します。</span><span class="sxs-lookup"><span data-stu-id="540f9-122">Identifies the start of a range of IP version 6 (IPv6) addresses that are used to identify a computer on a network.</span></span>  <br/> |
|[<span data-ttu-id="540f9-123">IPv6End (POX)</span><span class="sxs-lookup"><span data-stu-id="540f9-123">IPv6End (POX)</span></span>](ipv6end-pox.md) <br/> |<span data-ttu-id="540f9-124">ネットワーク上のコンピューターを識別するために使用される IP version 6 (IPv6) アドレスの範囲の末尾を識別します。</span><span class="sxs-lookup"><span data-stu-id="540f9-124">Identifies the end of a range of IP version 6 (IPv6) addresses that are used to identify a computer on a network.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="540f9-125">親要素</span><span class="sxs-lookup"><span data-stu-id="540f9-125">Parent elements</span></span>

|<span data-ttu-id="540f9-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="540f9-126">**Element**</span></span>|<span data-ttu-id="540f9-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="540f9-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="540f9-128">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="540f9-128">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="540f9-129">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="540f9-129">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="540f9-130">注釈</span><span class="sxs-lookup"><span data-stu-id="540f9-130">Remarks</span></span>

<span data-ttu-id="540f9-131">電子メールクライアントがネットワーク要件を満たしていない場合は、他のプロトコルの種類を試す必要があります。</span><span class="sxs-lookup"><span data-stu-id="540f9-131">If the e-mail client does not match the network requirements, it should try other protocol types.</span></span> <span data-ttu-id="540f9-132">Isp は、認証を必要とせず、ISP ネットワーク上で必要な[プロトコル (POX)](protocol-pox.md)タグを備えたサーバーのセットを提供することがあります。</span><span class="sxs-lookup"><span data-stu-id="540f9-132">ISPs may provide one set of servers with [Protocol (POX)](protocol-pox.md) tags that do not require authentication but are required to be on the ISP network.</span></span> <span data-ttu-id="540f9-133">Isp は、認証を必要とする別のサーバーセットを一覧表示することができますが、特定のネットワークである必要はありません。</span><span class="sxs-lookup"><span data-stu-id="540f9-133">ISPs may list another set of servers that require authentication but are not required to be on a specific network.</span></span> 
  
<span data-ttu-id="540f9-134">**Networkrequirements 要件**要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="540f9-134">The **NetworkRequirements** element is optional.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="540f9-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="540f9-135">See also</span></span>



[<span data-ttu-id="540f9-136">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="540f9-136">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


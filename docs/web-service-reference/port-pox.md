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
description: ポートの要素は、ストアへの接続に使用されるポートを指定します。
ms.openlocfilehash: f5a2155d97061a87fdf819549ec29898efe4d201
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832842"
---
# <a name="port-pox"></a><span data-ttu-id="f03d0-103">ポート (POX)</span><span class="sxs-lookup"><span data-stu-id="f03d0-103">Port (POX)</span></span>

<span data-ttu-id="f03d0-104">**ポート**の要素は、ストアへの接続に使用されるポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="f03d0-104">The **Port** element specifies the port that is used to connect to the store.</span></span> 
  
[<span data-ttu-id="f03d0-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="f03d0-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="f03d0-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="f03d0-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="f03d0-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="f03d0-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="f03d0-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="f03d0-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="f03d0-109">ポート (POX)</span><span class="sxs-lookup"><span data-stu-id="f03d0-109">Port (POX)</span></span>](port-pox.md)
  
```xml
<Port/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="f03d0-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f03d0-110">Attributes and elements</span></span>

<span data-ttu-id="f03d0-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f03d0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f03d0-112">属性</span><span class="sxs-lookup"><span data-stu-id="f03d0-112">Attributes</span></span>

<span data-ttu-id="f03d0-113">なし。</span><span class="sxs-lookup"><span data-stu-id="f03d0-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f03d0-114">子要素</span><span class="sxs-lookup"><span data-stu-id="f03d0-114">Child elements</span></span>

<span data-ttu-id="f03d0-115">なし。</span><span class="sxs-lookup"><span data-stu-id="f03d0-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f03d0-116">親要素</span><span class="sxs-lookup"><span data-stu-id="f03d0-116">Parent elements</span></span>

|<span data-ttu-id="f03d0-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="f03d0-117">**Element**</span></span>|<span data-ttu-id="f03d0-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="f03d0-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f03d0-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="f03d0-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="f03d0-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f03d0-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f03d0-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f03d0-121">Text value</span></span>

<span data-ttu-id="f03d0-122">テキスト値は、Exchange サーバーへのアクセスに使用するポートを表します。</span><span class="sxs-lookup"><span data-stu-id="f03d0-122">The text value represents the port that is used to access the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f03d0-123">備考</span><span class="sxs-lookup"><span data-stu-id="f03d0-123">Remarks</span></span>

<span data-ttu-id="f03d0-124">[サーバー (POX)](server-pox.md)要素には、URL が含まれている場合、**ポート**の値は使用されません。</span><span class="sxs-lookup"><span data-stu-id="f03d0-124">The **Port** value is not used if the [Server (POX)](server-pox.md) element contains a URL.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f03d0-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="f03d0-125">See also</span></span>



[<span data-ttu-id="f03d0-126">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f03d0-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


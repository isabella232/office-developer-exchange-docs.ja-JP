---
title: EcpUrl-tmCreating (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: c942758e-5ff3-4acb-9080-b8672e56f696
description: EcpUrl tmCreating 要素は、サイトの新しいメールボックスを作成するのに使用できる URL を生成する EcpUrl (POX) 要素の値と組み合わせて使用できますが、部分的な URL を指定します。
ms.openlocfilehash: c7dbaf3f3954f9233b888957fe79bf6db7ae5880
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760186"
---
# <a name="ecpurl-tmcreating-pox"></a><span data-ttu-id="01bb3-103">EcpUrl-tmCreating (POX)</span><span class="sxs-lookup"><span data-stu-id="01bb3-103">EcpUrl-tmCreating (POX)</span></span>

<span data-ttu-id="01bb3-104">**EcpUrl tmCreating**要素は、サイトの新しいメールボックスを作成するのに使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="01bb3-104">The **EcpUrl-tmCreating** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to create a new site mailbox.</span></span> 
  
[<span data-ttu-id="01bb3-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="01bb3-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="01bb3-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="01bb3-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="01bb3-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="01bb3-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="01bb3-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="01bb3-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="01bb3-109">EcpUrl-tmCreating (POX)</span><span class="sxs-lookup"><span data-stu-id="01bb3-109">EcpUrl-tmCreating (POX)</span></span>](ecpurl-tmcreating-pox.md)
  
```XML
<EcpUrl-tmCreating/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="01bb3-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="01bb3-110">Attributes and elements</span></span>

<span data-ttu-id="01bb3-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="01bb3-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01bb3-112">属性</span><span class="sxs-lookup"><span data-stu-id="01bb3-112">Attributes</span></span>

<span data-ttu-id="01bb3-113">なし。</span><span class="sxs-lookup"><span data-stu-id="01bb3-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01bb3-114">子要素</span><span class="sxs-lookup"><span data-stu-id="01bb3-114">Child elements</span></span>

<span data-ttu-id="01bb3-115">なし。</span><span class="sxs-lookup"><span data-stu-id="01bb3-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="01bb3-116">親要素</span><span class="sxs-lookup"><span data-stu-id="01bb3-116">Parent elements</span></span>

|<span data-ttu-id="01bb3-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="01bb3-117">**Element**</span></span>|<span data-ttu-id="01bb3-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="01bb3-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01bb3-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="01bb3-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="01bb3-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="01bb3-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="01bb3-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="01bb3-121">Text value</span></span>

<span data-ttu-id="01bb3-122">テキスト値は、新しいサイトのメールボックスを作成するのに使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を表します。</span><span class="sxs-lookup"><span data-stu-id="01bb3-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to create a new site mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="01bb3-123">備考</span><span class="sxs-lookup"><span data-stu-id="01bb3-123">Remarks</span></span>

<span data-ttu-id="01bb3-124">**EcpUrl tmCreating**要素は、**プロトコル**要素の省略可能な子要素です。</span><span class="sxs-lookup"><span data-stu-id="01bb3-124">The **EcpUrl-tmCreating** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="01bb3-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="01bb3-125">See also</span></span>



[<span data-ttu-id="01bb3-126">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="01bb3-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


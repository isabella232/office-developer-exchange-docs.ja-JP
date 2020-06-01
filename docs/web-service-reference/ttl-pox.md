---
title: TTL (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 178eefa1-995c-4bea-930b-e51293961191
description: TTL 要素は、設定が有効な状態が保たれる時間 (時間単位) を指定します。
ms.openlocfilehash: 9a17cbe4e669d1afe9f3ef4a24f2a9a2889a7d52
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467383"
---
# <a name="ttl-pox"></a><span data-ttu-id="a2520-103">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="a2520-103">TTL (POX)</span></span>

<span data-ttu-id="a2520-104">**TTL**要素は、設定が有効な状態が保たれる時間 (時間単位) を指定します。</span><span class="sxs-lookup"><span data-stu-id="a2520-104">The **TTL** element specifies the Time to Live, in hours, during which the settings remain valid.</span></span> 
  
[<span data-ttu-id="a2520-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="a2520-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="a2520-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="a2520-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="a2520-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="a2520-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="a2520-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="a2520-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="a2520-109">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="a2520-109">TTL (POX)</span></span>](ttl-pox.md)
  
```xml
<TTL/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="a2520-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a2520-110">Attributes and elements</span></span>

<span data-ttu-id="a2520-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a2520-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2520-112">属性</span><span class="sxs-lookup"><span data-stu-id="a2520-112">Attributes</span></span>

<span data-ttu-id="a2520-113">なし。</span><span class="sxs-lookup"><span data-stu-id="a2520-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2520-114">子要素</span><span class="sxs-lookup"><span data-stu-id="a2520-114">Child elements</span></span>

<span data-ttu-id="a2520-115">なし。</span><span class="sxs-lookup"><span data-stu-id="a2520-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a2520-116">親要素</span><span class="sxs-lookup"><span data-stu-id="a2520-116">Parent elements</span></span>

|<span data-ttu-id="a2520-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="a2520-117">**Element**</span></span>|<span data-ttu-id="a2520-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="a2520-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2520-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="a2520-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="a2520-120">クライアントアクセスサーバーの役割がインストールされている Exchange Server 2007 コンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a2520-120">Contains the specifications for connecting a client to the Exchange Server 2007 computer on which the Client Access server role is installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a2520-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a2520-121">Text value</span></span>

<span data-ttu-id="a2520-122">Text 値は、設定が有効な期間 (時間単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="a2520-122">The text value represents the Time to Live, in hours, during which the settings remain valid.</span></span> <span data-ttu-id="a2520-123">値が0の場合は、再検出が不要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="a2520-123">A value of zero indicates that rediscovery is not required.</span></span> <span data-ttu-id="a2520-124">値が指定されていない場合、この要素の既定値は1時間です。</span><span class="sxs-lookup"><span data-stu-id="a2520-124">If no value is specified, the default value for this element is 1 hour.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a2520-125">注釈</span><span class="sxs-lookup"><span data-stu-id="a2520-125">Remarks</span></span>

<span data-ttu-id="a2520-126">**TTL**要素で表される時間が経過した後、自動検出要求を使用して設定を再検出する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2520-126">After the time that is represented by the **TTL** element has elapsed, the settings should be rediscovered by using an Autodiscover request.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a2520-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="a2520-127">See also</span></span>



[<span data-ttu-id="a2520-128">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="a2520-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


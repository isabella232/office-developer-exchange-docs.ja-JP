---
title: ServerDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2ef73d13-e8bb-43f6-96c7-3ee157fed739
description: ServerDN 要素は、Microsoft Exchange Server 2007 を実行しているコンピューターの識別名を指定します。
ms.openlocfilehash: d2b9ce663d8245a78acd088b0622406c0dfcb4da
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833374"
---
# <a name="serverdn-pox"></a><span data-ttu-id="eea2a-103">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="eea2a-103">ServerDN (POX)</span></span>

<span data-ttu-id="eea2a-104">**ServerDN**要素は、Microsoft Exchange Server 2007 を実行しているコンピューターの識別名を指定します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-104">The **ServerDN** element specifies the distinguished name of the computer that is running Microsoft Exchange Server 2007.</span></span> 
  
[<span data-ttu-id="eea2a-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="eea2a-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="eea2a-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="eea2a-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="eea2a-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="eea2a-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="eea2a-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="eea2a-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="eea2a-109">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="eea2a-109">ServerDN (POX)</span></span>](serverdn-pox.md)
  
```xml
<ServerDN/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="eea2a-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="eea2a-110">Attributes and elements</span></span>

<span data-ttu-id="eea2a-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eea2a-112">属性</span><span class="sxs-lookup"><span data-stu-id="eea2a-112">Attributes</span></span>

<span data-ttu-id="eea2a-113">なし。</span><span class="sxs-lookup"><span data-stu-id="eea2a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eea2a-114">子要素</span><span class="sxs-lookup"><span data-stu-id="eea2a-114">Child elements</span></span>

<span data-ttu-id="eea2a-115">なし。</span><span class="sxs-lookup"><span data-stu-id="eea2a-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="eea2a-116">親要素</span><span class="sxs-lookup"><span data-stu-id="eea2a-116">Parent elements</span></span>

|<span data-ttu-id="eea2a-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="eea2a-117">**Element**</span></span>|<span data-ttu-id="eea2a-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="eea2a-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eea2a-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="eea2a-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="eea2a-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="eea2a-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eea2a-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="eea2a-121">Text value</span></span>

<span data-ttu-id="eea2a-122">テキスト値は、Exchange サーバーの識別名を表します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-122">The text value represents the distinguished name of the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="eea2a-123">備考</span><span class="sxs-lookup"><span data-stu-id="eea2a-123">Remarks</span></span>

<span data-ttu-id="eea2a-124">**ServerDN**値は、[種類 (POX)](type-pox.md)が為替にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="eea2a-124">The **ServerDN** value is only used when [Type (POX)](type-pox.md) is equal to EXCH.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="eea2a-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="eea2a-125">See also</span></span>



[<span data-ttu-id="eea2a-126">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="eea2a-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833374"
---
# <a name="serverdn-pox"></a><span data-ttu-id="285db-103">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="285db-103">ServerDN (POX)</span></span>

<span data-ttu-id="285db-104">**ServerDN**要素は、Microsoft Exchange Server 2007 を実行しているコンピューターの識別名を指定します。</span><span class="sxs-lookup"><span data-stu-id="285db-104">The **ServerDN** element specifies the distinguished name of the computer that is running Microsoft Exchange Server 2007.</span></span> 
  
[<span data-ttu-id="285db-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="285db-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="285db-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="285db-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="285db-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="285db-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="285db-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="285db-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="285db-109">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="285db-109">ServerDN (POX)</span></span>](serverdn-pox.md)
  
```xml
<ServerDN/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="285db-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="285db-110">Attributes and elements</span></span>

<span data-ttu-id="285db-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="285db-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="285db-112">属性</span><span class="sxs-lookup"><span data-stu-id="285db-112">Attributes</span></span>

<span data-ttu-id="285db-113">なし。</span><span class="sxs-lookup"><span data-stu-id="285db-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="285db-114">子要素</span><span class="sxs-lookup"><span data-stu-id="285db-114">Child elements</span></span>

<span data-ttu-id="285db-115">なし。</span><span class="sxs-lookup"><span data-stu-id="285db-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="285db-116">親要素</span><span class="sxs-lookup"><span data-stu-id="285db-116">Parent elements</span></span>

|<span data-ttu-id="285db-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="285db-117">**Element**</span></span>|<span data-ttu-id="285db-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="285db-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="285db-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="285db-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="285db-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="285db-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="285db-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="285db-121">Text value</span></span>

<span data-ttu-id="285db-122">テキスト値は、Exchange サーバーの識別名を表します。</span><span class="sxs-lookup"><span data-stu-id="285db-122">The text value represents the distinguished name of the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="285db-123">備考</span><span class="sxs-lookup"><span data-stu-id="285db-123">Remarks</span></span>

<span data-ttu-id="285db-124">**ServerDN**値は、[種類 (POX)](type-pox.md)が為替にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="285db-124">The **ServerDN** value is only used when [Type (POX)](type-pox.md) is equal to EXCH.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="285db-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="285db-125">See also</span></span>



[<span data-ttu-id="285db-126">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="285db-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


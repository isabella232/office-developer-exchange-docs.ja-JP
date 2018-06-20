---
title: EcpUrl-aggr (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0e7879e3-9b8f-4f23-8291-bacec0e479c0
description: EcpUrl aggr の要素では、メールが有効なユーザーの e メールの集計の設定へのアクセスに使用できる URL を生成する EcpUrl (POX) 要素の値と組み合わせて使用できますが、部分的な URL を指定します。
ms.openlocfilehash: fb9bd92611998acc52fab0ea3e3c1ecb3e507faa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760174"
---
# <a name="ecpurl-aggr-pox"></a><span data-ttu-id="0178a-103">EcpUrl-aggr (POX)</span><span class="sxs-lookup"><span data-stu-id="0178a-103">EcpUrl-aggr (POX)</span></span>

<span data-ttu-id="0178a-104">**EcpUrl aggr**の要素では、メールが有効なユーザーの e メールの集計の設定へのアクセスに使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="0178a-104">The **EcpUrl-aggr** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email aggregation settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="0178a-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="0178a-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="0178a-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="0178a-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="0178a-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="0178a-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="0178a-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="0178a-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="0178a-109">EcpUrl-aggr (POX)</span><span class="sxs-lookup"><span data-stu-id="0178a-109">EcpUrl-aggr (POX)</span></span>](ecpurl-aggr-pox.md)
  
```XML
<EcpUrl-aggr/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="0178a-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0178a-110">Attributes and elements</span></span>

<span data-ttu-id="0178a-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0178a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0178a-112">属性</span><span class="sxs-lookup"><span data-stu-id="0178a-112">Attributes</span></span>

<span data-ttu-id="0178a-113">なし。</span><span class="sxs-lookup"><span data-stu-id="0178a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0178a-114">子要素</span><span class="sxs-lookup"><span data-stu-id="0178a-114">Child elements</span></span>

<span data-ttu-id="0178a-115">なし。</span><span class="sxs-lookup"><span data-stu-id="0178a-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0178a-116">親要素</span><span class="sxs-lookup"><span data-stu-id="0178a-116">Parent elements</span></span>

|<span data-ttu-id="0178a-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="0178a-117">**Element**</span></span>|<span data-ttu-id="0178a-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="0178a-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0178a-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="0178a-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="0178a-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0178a-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0178a-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0178a-121">Text value</span></span>

<span data-ttu-id="0178a-122">テキスト値は、ユーザーの電子メールの集計の設定へのアクセスに使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を表します。</span><span class="sxs-lookup"><span data-stu-id="0178a-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email aggregation settings for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0178a-123">備考</span><span class="sxs-lookup"><span data-stu-id="0178a-123">Remarks</span></span>

<span data-ttu-id="0178a-124">**EcpUrl aggr**の要素は、**プロトコル**要素の省略可能な子要素です。</span><span class="sxs-lookup"><span data-stu-id="0178a-124">The **EcpUrl-aggr** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="0178a-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="0178a-125">See also</span></span>



[<span data-ttu-id="0178a-126">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0178a-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


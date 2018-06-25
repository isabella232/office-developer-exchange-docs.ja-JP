---
title: ReferralPort (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: cd693f1e-fed4-4eb9-8297-178906f47050
description: ReferralPort 要素は、ディレクトリへの参照を取得するために使用されるポートを指定します。
ms.openlocfilehash: 5045c0c5a9f15d5a31ac2e884b942e00dfb1f520
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833037"
---
# <a name="referralport-pox"></a><span data-ttu-id="78864-103">ReferralPort (POX)</span><span class="sxs-lookup"><span data-stu-id="78864-103">ReferralPort (POX)</span></span>

<span data-ttu-id="78864-104">**ReferralPort**要素は、ディレクトリへの参照を取得するために使用されるポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="78864-104">The **ReferralPort** element specifies the port that is used to get a referral to a directory.</span></span> 
  
[<span data-ttu-id="78864-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="78864-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="78864-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="78864-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="78864-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="78864-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="78864-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="78864-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="78864-109">ReferralPort (POX)</span><span class="sxs-lookup"><span data-stu-id="78864-109">ReferralPort (POX)</span></span>](referralport-pox.md)
  
```xml
<ReferralPort/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="78864-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="78864-110">Attributes and elements</span></span>

<span data-ttu-id="78864-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="78864-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78864-112">属性</span><span class="sxs-lookup"><span data-stu-id="78864-112">Attributes</span></span>

<span data-ttu-id="78864-113">なし。</span><span class="sxs-lookup"><span data-stu-id="78864-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78864-114">子要素</span><span class="sxs-lookup"><span data-stu-id="78864-114">Child elements</span></span>

<span data-ttu-id="78864-115">なし。</span><span class="sxs-lookup"><span data-stu-id="78864-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="78864-116">親要素</span><span class="sxs-lookup"><span data-stu-id="78864-116">Parent elements</span></span>

|<span data-ttu-id="78864-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="78864-117">**Element**</span></span>|<span data-ttu-id="78864-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="78864-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78864-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="78864-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="78864-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="78864-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="78864-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="78864-121">Text value</span></span>

<span data-ttu-id="78864-122">テキスト値は、Exchange サーバーへのアクセスに使用するポートを表します。</span><span class="sxs-lookup"><span data-stu-id="78864-122">The text value represents the port that is used to access the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="78864-123">備考</span><span class="sxs-lookup"><span data-stu-id="78864-123">Remarks</span></span>

<span data-ttu-id="78864-124">**ReferralPort**要素は、EXCH または EXPR[型 (POX)](type-pox.md)の要素が等しい場合にのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="78864-124">The **ReferralPort** element is only used when the [Type (POX)](type-pox.md) element equals EXCH or EXPR.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="78864-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="78864-125">See also</span></span>



[<span data-ttu-id="78864-126">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="78864-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


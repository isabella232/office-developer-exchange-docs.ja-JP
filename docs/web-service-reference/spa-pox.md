---
title: SPA (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: fba018d5-0c65-4e1b-9767-d1ce8b356278
description: SPA の要素は、セキュリティで保護されたパスワード認証 (SPA) が必要かどうかを示します。
ms.openlocfilehash: 1fb0f3bb40e64be89eae7dfc208d51387f532191
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833533"
---
# <a name="spa-pox"></a><span data-ttu-id="2047e-103">SPA (POX)</span><span class="sxs-lookup"><span data-stu-id="2047e-103">SPA (POX)</span></span>

<span data-ttu-id="2047e-104">**SPA**の要素は、セキュリティで保護されたパスワード認証 (SPA) が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2047e-104">The **SPA** element indicates whether Secure Password Authentication (SPA) is required.</span></span> 
  
[<span data-ttu-id="2047e-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="2047e-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="2047e-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="2047e-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="2047e-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="2047e-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="2047e-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="2047e-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="2047e-109">SPA (POX)</span><span class="sxs-lookup"><span data-stu-id="2047e-109">SPA (POX)</span></span>](spa-pox.md)
  
```xml
<SPA/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="2047e-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2047e-110">Attributes and elements</span></span>

<span data-ttu-id="2047e-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2047e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2047e-112">属性</span><span class="sxs-lookup"><span data-stu-id="2047e-112">Attributes</span></span>

<span data-ttu-id="2047e-113">なし。</span><span class="sxs-lookup"><span data-stu-id="2047e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2047e-114">子要素</span><span class="sxs-lookup"><span data-stu-id="2047e-114">Child elements</span></span>

<span data-ttu-id="2047e-115">なし。</span><span class="sxs-lookup"><span data-stu-id="2047e-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2047e-116">親要素</span><span class="sxs-lookup"><span data-stu-id="2047e-116">Parent elements</span></span>

|<span data-ttu-id="2047e-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="2047e-117">**Element**</span></span>|<span data-ttu-id="2047e-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="2047e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2047e-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="2047e-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="2047e-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2047e-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2047e-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2047e-121">Text value</span></span>

<span data-ttu-id="2047e-122">テキスト値は、SPA が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2047e-122">The text value indicates whether SPA is required.</span></span> <span data-ttu-id="2047e-123">テキスト値が**上**にある場合は、SPA が必要です。</span><span class="sxs-lookup"><span data-stu-id="2047e-123">If the text value is **on**, SPA is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2047e-124">備考</span><span class="sxs-lookup"><span data-stu-id="2047e-124">Remarks</span></span>

<span data-ttu-id="2047e-125">この要素が存在しない場合は、既定値は**on**に設定します。</span><span class="sxs-lookup"><span data-stu-id="2047e-125">If this element is not present, the default value is set to **on**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="2047e-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="2047e-126">See also</span></span>



[<span data-ttu-id="2047e-127">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2047e-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


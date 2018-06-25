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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833533"
---
# <a name="spa-pox"></a><span data-ttu-id="206dc-103">SPA (POX)</span><span class="sxs-lookup"><span data-stu-id="206dc-103">SPA (POX)</span></span>

<span data-ttu-id="206dc-104">**SPA**の要素は、セキュリティで保護されたパスワード認証 (SPA) が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="206dc-104">The **SPA** element indicates whether Secure Password Authentication (SPA) is required.</span></span> 
  
[<span data-ttu-id="206dc-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="206dc-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="206dc-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="206dc-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="206dc-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="206dc-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="206dc-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="206dc-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="206dc-109">SPA (POX)</span><span class="sxs-lookup"><span data-stu-id="206dc-109">SPA (POX)</span></span>](spa-pox.md)
  
```xml
<SPA/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="206dc-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="206dc-110">Attributes and elements</span></span>

<span data-ttu-id="206dc-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="206dc-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="206dc-112">属性</span><span class="sxs-lookup"><span data-stu-id="206dc-112">Attributes</span></span>

<span data-ttu-id="206dc-113">なし。</span><span class="sxs-lookup"><span data-stu-id="206dc-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="206dc-114">子要素</span><span class="sxs-lookup"><span data-stu-id="206dc-114">Child elements</span></span>

<span data-ttu-id="206dc-115">なし。</span><span class="sxs-lookup"><span data-stu-id="206dc-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="206dc-116">親要素</span><span class="sxs-lookup"><span data-stu-id="206dc-116">Parent elements</span></span>

|<span data-ttu-id="206dc-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="206dc-117">**Element**</span></span>|<span data-ttu-id="206dc-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="206dc-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="206dc-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="206dc-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="206dc-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="206dc-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="206dc-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="206dc-121">Text value</span></span>

<span data-ttu-id="206dc-122">テキスト値は、SPA が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="206dc-122">The text value indicates whether SPA is required.</span></span> <span data-ttu-id="206dc-123">テキスト値が**上**にある場合は、SPA が必要です。</span><span class="sxs-lookup"><span data-stu-id="206dc-123">If the text value is **on**, SPA is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="206dc-124">備考</span><span class="sxs-lookup"><span data-stu-id="206dc-124">Remarks</span></span>

<span data-ttu-id="206dc-125">この要素が存在しない場合は、既定値は**on**に設定します。</span><span class="sxs-lookup"><span data-stu-id="206dc-125">If this element is not present, the default value is set to **on**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="206dc-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="206dc-126">See also</span></span>



[<span data-ttu-id="206dc-127">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="206dc-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


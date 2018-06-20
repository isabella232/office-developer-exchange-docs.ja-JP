---
title: SharingUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: d590188a-5aa6-46c6-ab5f-2a0dd6793109
description: SharingUrl 要素には、組織間の予定表と連絡先の共有に使用する共有サーバーの URL が含まれています。
ms.openlocfilehash: 0a62c5145da97976de12e7cdc29800a332877b44
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833489"
---
# <a name="sharingurl-pox"></a><span data-ttu-id="cb10e-103">SharingUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="cb10e-103">SharingUrl (POX)</span></span>

<span data-ttu-id="cb10e-104">**SharingUrl**要素には、組織間の予定表と連絡先の共有に使用する共有サーバーの URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cb10e-104">The **SharingUrl** element contains the URL of the sharing server used for cross-organization sharing of calendars and contacts.</span></span> 
  
[<span data-ttu-id="cb10e-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="cb10e-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="cb10e-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="cb10e-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="cb10e-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="cb10e-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="cb10e-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="cb10e-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="cb10e-109">SharingUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="cb10e-109">SharingUrl (POX)</span></span>](sharingurl-pox.md)
  
```XML
<SharingUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="cb10e-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cb10e-110">Attributes and elements</span></span>

<span data-ttu-id="cb10e-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cb10e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cb10e-112">属性</span><span class="sxs-lookup"><span data-stu-id="cb10e-112">Attributes</span></span>

<span data-ttu-id="cb10e-113">なし。</span><span class="sxs-lookup"><span data-stu-id="cb10e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cb10e-114">子要素</span><span class="sxs-lookup"><span data-stu-id="cb10e-114">Child elements</span></span>

<span data-ttu-id="cb10e-115">なし。</span><span class="sxs-lookup"><span data-stu-id="cb10e-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cb10e-116">親要素</span><span class="sxs-lookup"><span data-stu-id="cb10e-116">Parent elements</span></span>

|<span data-ttu-id="cb10e-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="cb10e-117">**Element**</span></span>|<span data-ttu-id="cb10e-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="cb10e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb10e-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="cb10e-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="cb10e-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cb10e-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cb10e-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cb10e-121">Text value</span></span>

<span data-ttu-id="cb10e-122">テキスト値は、組織間の予定表と連絡先の共有に使用する共有サーバーの URL を表します。</span><span class="sxs-lookup"><span data-stu-id="cb10e-122">The text value represents the URL of the sharing server used for cross-organization sharing of calendars and contacts.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cb10e-123">備考</span><span class="sxs-lookup"><span data-stu-id="cb10e-123">Remarks</span></span>

<span data-ttu-id="cb10e-124">**SharingUrl**要素は、**プロトコル**要素の省略可能な子要素です。</span><span class="sxs-lookup"><span data-stu-id="cb10e-124">The **SharingUrl** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="cb10e-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="cb10e-125">See also</span></span>



[<span data-ttu-id="cb10e-126">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="cb10e-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


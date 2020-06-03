---
title: EcpUrl-tmCreating 作成 (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: c942758e-5ff3-4acb-9080-b8672e56f696
description: EcpUrl-tmCreating 要素は、EcpUrl (POX) 要素の値と組み合わせて、新しいサイトメールボックスの作成に使用できる URL を生成できる部分的な URL を指定します。
ms.openlocfilehash: 93ea3f5752dab0028c0732e5e79c5690e35bd059
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462060"
---
# <a name="ecpurl-tmcreating-pox"></a><span data-ttu-id="05aed-103">EcpUrl-tmCreating 作成 (POX)</span><span class="sxs-lookup"><span data-stu-id="05aed-103">EcpUrl-tmCreating (POX)</span></span>

<span data-ttu-id="05aed-104">**EcpUrl-tmcreating**要素は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、新しいサイトメールボックスの作成に使用できる url を生成できる部分的な url を指定します。</span><span class="sxs-lookup"><span data-stu-id="05aed-104">The **EcpUrl-tmCreating** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to create a new site mailbox.</span></span> 
  
[<span data-ttu-id="05aed-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="05aed-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="05aed-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="05aed-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="05aed-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="05aed-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="05aed-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="05aed-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="05aed-109">EcpUrl-tmCreating 作成 (POX)</span><span class="sxs-lookup"><span data-stu-id="05aed-109">EcpUrl-tmCreating (POX)</span></span>](ecpurl-tmcreating-pox.md)
  
```XML
<EcpUrl-tmCreating/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="05aed-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="05aed-110">Attributes and elements</span></span>

<span data-ttu-id="05aed-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="05aed-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05aed-112">属性</span><span class="sxs-lookup"><span data-stu-id="05aed-112">Attributes</span></span>

<span data-ttu-id="05aed-113">なし。</span><span class="sxs-lookup"><span data-stu-id="05aed-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05aed-114">子要素</span><span class="sxs-lookup"><span data-stu-id="05aed-114">Child elements</span></span>

<span data-ttu-id="05aed-115">なし。</span><span class="sxs-lookup"><span data-stu-id="05aed-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05aed-116">親要素</span><span class="sxs-lookup"><span data-stu-id="05aed-116">Parent elements</span></span>

|<span data-ttu-id="05aed-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="05aed-117">**Element**</span></span>|<span data-ttu-id="05aed-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="05aed-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05aed-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="05aed-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="05aed-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="05aed-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="05aed-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="05aed-121">Text value</span></span>

<span data-ttu-id="05aed-122">テキスト値は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、新しいサイトメールボックスの作成に使用できる url を生成できる url の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="05aed-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to create a new site mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="05aed-123">注釈</span><span class="sxs-lookup"><span data-stu-id="05aed-123">Remarks</span></span>

<span data-ttu-id="05aed-124">**EcpUrl-tmcreating**は、 **Protocol**要素のオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="05aed-124">The **EcpUrl-tmCreating** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="05aed-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="05aed-125">See also</span></span>



[<span data-ttu-id="05aed-126">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="05aed-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


---
title: EcpUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 455c77c6-c03f-49a7-a8ca-aa0023b6e73b
description: EcpUrl 要素は、EcpUrl (POX) 要素の値と組み合わせて、メールが有効なユーザーのボイスメール設定にアクセスするために使用できる URL を生成できる、部分的な URL を指定します。
ms.openlocfilehash: 0fa3d42113d7d9accd6bba3d3b065477baf4d484
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463490"
---
# <a name="ecpurl-um-pox"></a><span data-ttu-id="64060-103">EcpUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="64060-103">EcpUrl-um (POX)</span></span>

<span data-ttu-id="64060-104">**EcpUrl**要素は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーのボイスメール設定にアクセスするために使用できる url を生成できる、部分的な url を指定します。</span><span class="sxs-lookup"><span data-stu-id="64060-104">The **EcpUrl-um** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access voice mail settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="64060-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="64060-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="64060-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="64060-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="64060-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="64060-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="64060-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="64060-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="64060-109">EcpUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="64060-109">EcpUrl-um (POX)</span></span>](ecpurl-um-pox.md)
  
```XML
<EcpUrl-um/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="64060-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="64060-110">Attributes and elements</span></span>

<span data-ttu-id="64060-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="64060-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64060-112">属性</span><span class="sxs-lookup"><span data-stu-id="64060-112">Attributes</span></span>

<span data-ttu-id="64060-113">なし。</span><span class="sxs-lookup"><span data-stu-id="64060-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64060-114">子要素</span><span class="sxs-lookup"><span data-stu-id="64060-114">Child elements</span></span>

<span data-ttu-id="64060-115">なし。</span><span class="sxs-lookup"><span data-stu-id="64060-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="64060-116">親要素</span><span class="sxs-lookup"><span data-stu-id="64060-116">Parent elements</span></span>

|<span data-ttu-id="64060-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="64060-117">**Element**</span></span>|<span data-ttu-id="64060-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="64060-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64060-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="64060-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="64060-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="64060-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="64060-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="64060-121">Text value</span></span>

<span data-ttu-id="64060-122">テキスト値は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、ユーザーのボイスメール設定にアクセスするために使用できる url を生成できる url の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="64060-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access voice mail settings for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="64060-123">注釈</span><span class="sxs-lookup"><span data-stu-id="64060-123">Remarks</span></span>

<span data-ttu-id="64060-124">**EcpUrl**要素は、 **Protocol**要素のオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="64060-124">The **EcpUrl-um** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="64060-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="64060-125">See also</span></span>



[<span data-ttu-id="64060-126">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="64060-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


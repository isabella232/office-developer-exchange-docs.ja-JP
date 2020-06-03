---
title: EcpUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4a37bbfb-c763-4a3c-93ea-14c2e7355dbc
description: EcpUrl 要素は、EcpUrl (POX) 要素の値と組み合わせて、メールが有効なユーザーの現在の写真を表示または変更するために使用できる URL を生成できる url の部分を指定します。
ms.openlocfilehash: 2be930e8d9e4c2bbdb26eff49a429569fc0a1d5d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461283"
---
# <a name="ecpurl-photo-pox"></a><span data-ttu-id="35324-103">EcpUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="35324-103">EcpUrl-photo (POX)</span></span>

<span data-ttu-id="35324-104">**EcpUrl**要素は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーの現在の写真を表示または変更するために使用できる url を生成できる url の部分を指定します。</span><span class="sxs-lookup"><span data-stu-id="35324-104">The **EcpUrl-photo** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to view or change a mail-enabled user's current photo.</span></span> 
  
[<span data-ttu-id="35324-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="35324-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="35324-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="35324-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="35324-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="35324-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="35324-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="35324-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="35324-109">EcpUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="35324-109">EcpUrl-photo (POX)</span></span>](ecpurl-photo-pox.md)
  
```XML
<EcpUrl-photo/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="35324-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="35324-110">Attributes and elements</span></span>

<span data-ttu-id="35324-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="35324-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="35324-112">属性</span><span class="sxs-lookup"><span data-stu-id="35324-112">Attributes</span></span>

<span data-ttu-id="35324-113">なし。</span><span class="sxs-lookup"><span data-stu-id="35324-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="35324-114">子要素</span><span class="sxs-lookup"><span data-stu-id="35324-114">Child elements</span></span>

<span data-ttu-id="35324-115">なし。</span><span class="sxs-lookup"><span data-stu-id="35324-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="35324-116">親要素</span><span class="sxs-lookup"><span data-stu-id="35324-116">Parent elements</span></span>

|<span data-ttu-id="35324-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="35324-117">**Element**</span></span>|<span data-ttu-id="35324-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="35324-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35324-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="35324-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="35324-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="35324-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="35324-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="35324-121">Text value</span></span>

<span data-ttu-id="35324-122">テキスト値は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、ユーザーの現在の写真を表示または変更するために使用できる url を生成できる url の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="35324-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to view or change the user's current photo.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="35324-123">注釈</span><span class="sxs-lookup"><span data-stu-id="35324-123">Remarks</span></span>

<span data-ttu-id="35324-124">**EcpUrl**要素は、 **Protocol**要素のオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="35324-124">The **EcpUrl-photo** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="35324-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="35324-125">See also</span></span>



[<span data-ttu-id="35324-126">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="35324-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


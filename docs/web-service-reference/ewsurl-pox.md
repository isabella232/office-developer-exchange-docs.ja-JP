---
title: EwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 73cebc8c-770a-4f1b-b93e-51e7e2f3e342
description: EwsUrl 要素は、メールが有効なユーザーのために、Exchange Web サービス (EWS) の最適なエンドポイントインスタンスの URL を指定します。
ms.openlocfilehash: 295e65ddf14524a41c5cb714df78703dbf855a05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454352"
---
# <a name="ewsurl-pox"></a><span data-ttu-id="a0cba-103">EwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="a0cba-103">EwsUrl (POX)</span></span>

<span data-ttu-id="a0cba-104">**Ewsurl**要素は、メールが有効なユーザーのために、Exchange Web サービス (EWS) の最適なエンドポイントインスタンスの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="a0cba-104">The **EwsUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="a0cba-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="a0cba-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="a0cba-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="a0cba-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="a0cba-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="a0cba-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="a0cba-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="a0cba-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="a0cba-109">EwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="a0cba-109">EwsUrl (POX)</span></span>](ewsurl-pox.md)
  
```XML
<EwsUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="a0cba-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a0cba-110">Attributes and elements</span></span>

<span data-ttu-id="a0cba-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a0cba-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0cba-112">属性</span><span class="sxs-lookup"><span data-stu-id="a0cba-112">Attributes</span></span>

<span data-ttu-id="a0cba-113">なし。</span><span class="sxs-lookup"><span data-stu-id="a0cba-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0cba-114">子要素</span><span class="sxs-lookup"><span data-stu-id="a0cba-114">Child elements</span></span>

<span data-ttu-id="a0cba-115">なし。</span><span class="sxs-lookup"><span data-stu-id="a0cba-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a0cba-116">親要素</span><span class="sxs-lookup"><span data-stu-id="a0cba-116">Parent elements</span></span>

|<span data-ttu-id="a0cba-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="a0cba-117">**Element**</span></span>|<span data-ttu-id="a0cba-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="a0cba-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0cba-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="a0cba-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="a0cba-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a0cba-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a0cba-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a0cba-121">Text value</span></span>

<span data-ttu-id="a0cba-122">Text 値は、ユーザーの EWS エンドポイントの URL を表します。</span><span class="sxs-lookup"><span data-stu-id="a0cba-122">The text value represents the URL of the EWS endpoint for the user.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a0cba-123">注釈</span><span class="sxs-lookup"><span data-stu-id="a0cba-123">Remarks</span></span>

<span data-ttu-id="a0cba-124">**Ewsurl**要素は、**プロトコル**要素のオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="a0cba-124">The **EwsUrl** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a0cba-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="a0cba-125">See also</span></span>



[<span data-ttu-id="a0cba-126">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="a0cba-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


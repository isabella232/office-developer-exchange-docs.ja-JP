---
title: EwsPartnerUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ebae21c-3efa-4239-9b49-4a3a8871449b
description: EwsPartnerUrl 要素は、メールが有効なユーザーのために、Exchange Web サービス (EWS) の最適なエンドポイントインスタンスの URL を指定します。
ms.openlocfilehash: a67eb17bb3db67a922c53ba5e37900ee0a9b956b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526110"
---
# <a name="ewspartnerurl-pox"></a><span data-ttu-id="f362b-103">EwsPartnerUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="f362b-103">EwsPartnerUrl (POX)</span></span>

<span data-ttu-id="f362b-104">**EwsPartnerUrl**要素は、メールが有効なユーザーのために、Exchange Web サービス (EWS) の最適なエンドポイントインスタンスの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="f362b-104">The **EwsPartnerUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="f362b-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="f362b-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="f362b-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="f362b-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="f362b-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="f362b-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="f362b-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="f362b-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="f362b-109">EwsPartnerUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="f362b-109">EwsPartnerUrl (POX)</span></span>](ewspartnerurl-pox.md)
  
```XML
<EwsPartnerUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="f362b-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f362b-110">Attributes and elements</span></span>

<span data-ttu-id="f362b-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f362b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f362b-112">属性</span><span class="sxs-lookup"><span data-stu-id="f362b-112">Attributes</span></span>

<span data-ttu-id="f362b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="f362b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f362b-114">子要素</span><span class="sxs-lookup"><span data-stu-id="f362b-114">Child elements</span></span>

<span data-ttu-id="f362b-115">なし。</span><span class="sxs-lookup"><span data-stu-id="f362b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f362b-116">親要素</span><span class="sxs-lookup"><span data-stu-id="f362b-116">Parent elements</span></span>

|<span data-ttu-id="f362b-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="f362b-117">**Element**</span></span>|<span data-ttu-id="f362b-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="f362b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f362b-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="f362b-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="f362b-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f362b-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f362b-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f362b-121">Text value</span></span>

<span data-ttu-id="f362b-122">Text 値は、ユーザーの EWS エンドポイントの URL を表します。</span><span class="sxs-lookup"><span data-stu-id="f362b-122">The text value represents the URL of the EWS endpoint for the user.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f362b-123">注釈</span><span class="sxs-lookup"><span data-stu-id="f362b-123">Remarks</span></span>

<span data-ttu-id="f362b-124">**EwsPartnerUrl**要素は、 **Protocol**要素のオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="f362b-124">The **EwsPartnerUrl** element is an optional child element of the **Protocol** element.</span></span> <span data-ttu-id="f362b-125">[Ewsurl (POX)](ewsurl-pox.md)要素と同じです。</span><span class="sxs-lookup"><span data-stu-id="f362b-125">It is equivalent to the [EwsUrl (POX)](ewsurl-pox.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f362b-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="f362b-126">See also</span></span>



[<span data-ttu-id="f362b-127">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="f362b-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


---
title: EwsPartnerUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ebae21c-3efa-4239-9b49-4a3a8871449b
description: EwsPartnerUrl 要素は、メールが有効なユーザーの Exchange Web サービス (EWS) の最適なエンドポイントのインスタンスの URL を指定します。
ms.openlocfilehash: 97c33e1fed4adc8a9e8542d85e67c942118f6096
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760356"
---
# <a name="ewspartnerurl-pox"></a><span data-ttu-id="f08c4-103">EwsPartnerUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="f08c4-103">EwsPartnerUrl (POX)</span></span>

<span data-ttu-id="f08c4-104">**EwsPartnerUrl**要素は、メールが有効なユーザーの Exchange Web サービス (EWS) の最適なエンドポイントのインスタンスの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="f08c4-104">The **EwsPartnerUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="f08c4-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="f08c4-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="f08c4-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="f08c4-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="f08c4-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="f08c4-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="f08c4-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="f08c4-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="f08c4-109">EwsPartnerUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="f08c4-109">EwsPartnerUrl (POX)</span></span>](ewspartnerurl-pox.md)
  
```XML
<EwsPartnerUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="f08c4-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f08c4-110">Attributes and elements</span></span>

<span data-ttu-id="f08c4-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f08c4-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f08c4-112">属性</span><span class="sxs-lookup"><span data-stu-id="f08c4-112">Attributes</span></span>

<span data-ttu-id="f08c4-113">なし。</span><span class="sxs-lookup"><span data-stu-id="f08c4-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f08c4-114">子要素</span><span class="sxs-lookup"><span data-stu-id="f08c4-114">Child elements</span></span>

<span data-ttu-id="f08c4-115">なし。</span><span class="sxs-lookup"><span data-stu-id="f08c4-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f08c4-116">親要素</span><span class="sxs-lookup"><span data-stu-id="f08c4-116">Parent elements</span></span>

|<span data-ttu-id="f08c4-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="f08c4-117">**Element**</span></span>|<span data-ttu-id="f08c4-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="f08c4-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f08c4-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="f08c4-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="f08c4-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f08c4-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f08c4-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f08c4-121">Text value</span></span>

<span data-ttu-id="f08c4-122">テキスト値は、ユーザーの EWS のエンドポイントの URL を表します。</span><span class="sxs-lookup"><span data-stu-id="f08c4-122">The text value represents the URL of the EWS endpoint for the user.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f08c4-123">備考</span><span class="sxs-lookup"><span data-stu-id="f08c4-123">Remarks</span></span>

<span data-ttu-id="f08c4-124">**EwsPartnerUrl**要素は、**プロトコル**要素の省略可能な子要素です。</span><span class="sxs-lookup"><span data-stu-id="f08c4-124">The **EwsPartnerUrl** element is an optional child element of the **Protocol** element.</span></span> <span data-ttu-id="f08c4-125">[EwsUrl (POX)](ewsurl-pox.md)の要素と同じであります。</span><span class="sxs-lookup"><span data-stu-id="f08c4-125">It is equivalent to the [EwsUrl (POX)](ewsurl-pox.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f08c4-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="f08c4-126">See also</span></span>



[<span data-ttu-id="f08c4-127">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f08c4-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


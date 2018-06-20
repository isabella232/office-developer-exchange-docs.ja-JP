---
title: TTL (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 178eefa1-995c-4bea-930b-e51293961191
description: TTL 要素は、時間、期間の設定が有効なままで、Live までの時間を指定します。
ms.openlocfilehash: 5fecf3103553a82ed2aeeecfc1e4e1b9fe38583c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839757"
---
# <a name="ttl-pox"></a><span data-ttu-id="8fb43-103">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="8fb43-103">TTL (POX)</span></span>

<span data-ttu-id="8fb43-104">**TTL**要素は、時間、期間の設定が有効なままで、Live までの時間を指定します。</span><span class="sxs-lookup"><span data-stu-id="8fb43-104">The **TTL** element specifies the Time to Live, in hours, during which the settings remain valid.</span></span> 
  
[<span data-ttu-id="8fb43-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="8fb43-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="8fb43-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="8fb43-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="8fb43-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="8fb43-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="8fb43-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="8fb43-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="8fb43-109">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="8fb43-109">TTL (POX)</span></span>](ttl-pox.md)
  
```xml
<TTL/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="8fb43-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8fb43-110">Attributes and elements</span></span>

<span data-ttu-id="8fb43-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8fb43-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8fb43-112">属性</span><span class="sxs-lookup"><span data-stu-id="8fb43-112">Attributes</span></span>

<span data-ttu-id="8fb43-113">なし。</span><span class="sxs-lookup"><span data-stu-id="8fb43-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8fb43-114">子要素</span><span class="sxs-lookup"><span data-stu-id="8fb43-114">Child elements</span></span>

<span data-ttu-id="8fb43-115">なし。</span><span class="sxs-lookup"><span data-stu-id="8fb43-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8fb43-116">親要素</span><span class="sxs-lookup"><span data-stu-id="8fb43-116">Parent elements</span></span>

|<span data-ttu-id="8fb43-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="8fb43-117">**Element**</span></span>|<span data-ttu-id="8fb43-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="8fb43-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8fb43-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="8fb43-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="8fb43-120">クライアント アクセス サーバーの役割がインストールされている Exchange Server 2007 コンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8fb43-120">Contains the specifications for connecting a client to the Exchange Server 2007 computer on which the Client Access server role is installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8fb43-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8fb43-121">Text value</span></span>

<span data-ttu-id="8fb43-122">テキスト値は、時間、期間の設定が有効なままで、Live までの時間を表します。</span><span class="sxs-lookup"><span data-stu-id="8fb43-122">The text value represents the Time to Live, in hours, during which the settings remain valid.</span></span> <span data-ttu-id="8fb43-123">0 の値は、その再検出する必要はありませんを示します。</span><span class="sxs-lookup"><span data-stu-id="8fb43-123">A value of zero indicates that rediscovery is not required.</span></span> <span data-ttu-id="8fb43-124">値が指定されていない場合、この要素の既定値が 1 時間です。</span><span class="sxs-lookup"><span data-stu-id="8fb43-124">If no value is specified, the default value for this element is 1 hour.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8fb43-125">備考</span><span class="sxs-lookup"><span data-stu-id="8fb43-125">Remarks</span></span>

<span data-ttu-id="8fb43-126">**TTL**要素で表される時間が経過した後設定は、自動検出要求を使用して再検出する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8fb43-126">After the time that is represented by the **TTL** element has elapsed, the settings should be rediscovered by using an Autodiscover request.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8fb43-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="8fb43-127">See also</span></span>



[<span data-ttu-id="8fb43-128">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8fb43-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


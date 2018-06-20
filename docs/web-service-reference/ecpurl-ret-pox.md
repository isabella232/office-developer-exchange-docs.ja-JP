---
title: EcpUrl-ret (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 5f090fd2-b0c4-4ca0-a959-1433d73a2069
description: EcpUrl ret 要素では、メールが有効なユーザーの保持タグの設定にアクセスするために使用する URL を生成するのには EcpUrl (POX) 要素の値と組み合わせて使用できますが、部分的な URL を指定します。
ms.openlocfilehash: 366a7a79c0f3c19b2cfef21c01826e62b0e95793
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760191"
---
# <a name="ecpurl-ret-pox"></a><span data-ttu-id="5aa95-103">EcpUrl-ret (POX)</span><span class="sxs-lookup"><span data-stu-id="5aa95-103">EcpUrl-ret (POX)</span></span>

<span data-ttu-id="5aa95-104">**EcpUrl ret**要素では、メールが有効なユーザーの保持タグの設定にアクセスするために使用する URL を生成するのには[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5aa95-104">The **EcpUrl-ret** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access retention tag settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="5aa95-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="5aa95-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="5aa95-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="5aa95-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="5aa95-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="5aa95-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="5aa95-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="5aa95-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="5aa95-109">EcpUrl-ret (POX)</span><span class="sxs-lookup"><span data-stu-id="5aa95-109">EcpUrl-ret (POX)</span></span>](ecpurl-ret-pox.md)
  
```XML
<EcpUrl-ret/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="5aa95-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5aa95-110">Attributes and elements</span></span>

<span data-ttu-id="5aa95-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5aa95-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5aa95-112">属性</span><span class="sxs-lookup"><span data-stu-id="5aa95-112">Attributes</span></span>

<span data-ttu-id="5aa95-113">なし。</span><span class="sxs-lookup"><span data-stu-id="5aa95-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5aa95-114">子要素</span><span class="sxs-lookup"><span data-stu-id="5aa95-114">Child elements</span></span>

<span data-ttu-id="5aa95-115">なし。</span><span class="sxs-lookup"><span data-stu-id="5aa95-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5aa95-116">親要素</span><span class="sxs-lookup"><span data-stu-id="5aa95-116">Parent elements</span></span>

|<span data-ttu-id="5aa95-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="5aa95-117">**Element**</span></span>|<span data-ttu-id="5aa95-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="5aa95-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5aa95-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="5aa95-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="5aa95-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5aa95-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5aa95-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5aa95-121">Text value</span></span>

<span data-ttu-id="5aa95-122">テキスト値は、ユーザーの保持タグの設定にアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を表します。</span><span class="sxs-lookup"><span data-stu-id="5aa95-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access retention tag settings for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5aa95-123">備考</span><span class="sxs-lookup"><span data-stu-id="5aa95-123">Remarks</span></span>

<span data-ttu-id="5aa95-124">**EcpUrl ret**の要素は、**プロトコル**要素の省略可能な子要素です。</span><span class="sxs-lookup"><span data-stu-id="5aa95-124">The **EcpUrl-ret** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="5aa95-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="5aa95-125">See also</span></span>



[<span data-ttu-id="5aa95-126">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5aa95-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


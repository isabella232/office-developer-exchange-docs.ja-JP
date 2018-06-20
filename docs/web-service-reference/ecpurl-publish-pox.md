---
title: (POX) を EcpUrl 発行
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a51189db-f6e5-428d-833d-65a209204a5b
description: EcpUrl 発行要素では、メールが有効なユーザーの設定を公開する予定表にアクセスするために使用する URL を生成する EcpUrl (POX) 要素の値と組み合わせて使用できますが、部分的な URL を指定します。
ms.openlocfilehash: 82f55be3ce529f6e57db5ffe18bbdea609b13595
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760185"
---
# <a name="ecpurl-publish-pox"></a><span data-ttu-id="2a0c5-103">(POX) を EcpUrl 発行</span><span class="sxs-lookup"><span data-stu-id="2a0c5-103">EcpUrl-publish (POX)</span></span>

<span data-ttu-id="2a0c5-104">**EcpUrl 発行**要素では、メールが有効なユーザーの設定を公開する予定表にアクセスするために使用する URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="2a0c5-104">The **EcpUrl-publish** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access calendar publishing settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="2a0c5-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="2a0c5-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="2a0c5-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="2a0c5-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="2a0c5-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="2a0c5-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="2a0c5-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="2a0c5-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="2a0c5-109">(POX) を EcpUrl 発行</span><span class="sxs-lookup"><span data-stu-id="2a0c5-109">EcpUrl-publish (POX)</span></span>](ecpurl-publish-pox.md)
  
```XML
<EcpUrl-publish/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="2a0c5-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2a0c5-110">Attributes and elements</span></span>

<span data-ttu-id="2a0c5-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2a0c5-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a0c5-112">属性</span><span class="sxs-lookup"><span data-stu-id="2a0c5-112">Attributes</span></span>

<span data-ttu-id="2a0c5-113">なし。</span><span class="sxs-lookup"><span data-stu-id="2a0c5-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2a0c5-114">子要素</span><span class="sxs-lookup"><span data-stu-id="2a0c5-114">Child elements</span></span>

<span data-ttu-id="2a0c5-115">なし。</span><span class="sxs-lookup"><span data-stu-id="2a0c5-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2a0c5-116">親要素</span><span class="sxs-lookup"><span data-stu-id="2a0c5-116">Parent elements</span></span>

|<span data-ttu-id="2a0c5-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="2a0c5-117">**Element**</span></span>|<span data-ttu-id="2a0c5-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="2a0c5-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a0c5-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="2a0c5-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="2a0c5-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2a0c5-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2a0c5-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2a0c5-121">Text value</span></span>

<span data-ttu-id="2a0c5-122">テキスト値は、ユーザーの予定表の公開設定にアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を表します。</span><span class="sxs-lookup"><span data-stu-id="2a0c5-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access calendar publishing settings for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2a0c5-123">備考</span><span class="sxs-lookup"><span data-stu-id="2a0c5-123">Remarks</span></span>

<span data-ttu-id="2a0c5-124">**EcpUrl 発行**要素は、**プロトコル**要素の省略可能な子要素です。</span><span class="sxs-lookup"><span data-stu-id="2a0c5-124">The **EcpUrl-publish** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="2a0c5-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="2a0c5-125">See also</span></span>



[<span data-ttu-id="2a0c5-126">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2a0c5-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


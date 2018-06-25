---
title: EcpUrl-um (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 455c77c6-c03f-49a7-a8ca-aa0023b6e73b
description: Um の EcpUrl 要素は、メールが有効なユーザーのボイス メールの設定にアクセスするために使用できる URL を生成する EcpUrl (POX) 要素の値と組み合わせて使用できますが、部分的な URL を指定します。
ms.openlocfilehash: 5f9be67f02703bbdfeb114eda13c5ce59f83290d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760189"
---
# <a name="ecpurl-um-pox"></a><span data-ttu-id="868dc-103">EcpUrl-um (POX)</span><span class="sxs-lookup"><span data-stu-id="868dc-103">EcpUrl-um (POX)</span></span>

<span data-ttu-id="868dc-104">**Um の EcpUrl**要素は、メールが有効なユーザーのボイス メールの設定にアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="868dc-104">The **EcpUrl-um** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access voice mail settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="868dc-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="868dc-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="868dc-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="868dc-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="868dc-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="868dc-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="868dc-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="868dc-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="868dc-109">EcpUrl-um (POX)</span><span class="sxs-lookup"><span data-stu-id="868dc-109">EcpUrl-um (POX)</span></span>](ecpurl-um-pox.md)
  
```XML
<EcpUrl-um/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="868dc-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="868dc-110">Attributes and elements</span></span>

<span data-ttu-id="868dc-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="868dc-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="868dc-112">属性</span><span class="sxs-lookup"><span data-stu-id="868dc-112">Attributes</span></span>

<span data-ttu-id="868dc-113">なし。</span><span class="sxs-lookup"><span data-stu-id="868dc-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="868dc-114">子要素</span><span class="sxs-lookup"><span data-stu-id="868dc-114">Child elements</span></span>

<span data-ttu-id="868dc-115">なし。</span><span class="sxs-lookup"><span data-stu-id="868dc-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="868dc-116">親要素</span><span class="sxs-lookup"><span data-stu-id="868dc-116">Parent elements</span></span>

|<span data-ttu-id="868dc-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="868dc-117">**Element**</span></span>|<span data-ttu-id="868dc-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="868dc-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="868dc-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="868dc-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="868dc-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="868dc-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="868dc-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="868dc-121">Text value</span></span>

<span data-ttu-id="868dc-122">テキスト値は、ユーザーのボイス メールの設定にアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を表します。</span><span class="sxs-lookup"><span data-stu-id="868dc-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access voice mail settings for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="868dc-123">備考</span><span class="sxs-lookup"><span data-stu-id="868dc-123">Remarks</span></span>

<span data-ttu-id="868dc-124">**Um の EcpUrl**要素は、**プロトコル**要素の省略可能な子要素です。</span><span class="sxs-lookup"><span data-stu-id="868dc-124">The **EcpUrl-um** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="868dc-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="868dc-125">See also</span></span>



[<span data-ttu-id="868dc-126">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="868dc-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


---
title: EcpUrl-tm (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 3f35d5ac-55be-4d3a-ad03-7d6e9349d923
description: EcpUrl tm の要素は、先のすべてのサイトのメールボックスのメールが有効なユーザーは、現在メンバー リストにアクセスするために使用できる URL を生成する EcpUrl (POX) 要素の値と組み合わせて使用できますが、部分的な URL を指定します。
ms.openlocfilehash: 786459cab98f8c169f768b6ef850792e8111761a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760187"
---
# <a name="ecpurl-tm-pox"></a><span data-ttu-id="f5a14-103">EcpUrl-tm (POX)</span><span class="sxs-lookup"><span data-stu-id="f5a14-103">EcpUrl-tm (POX)</span></span>

<span data-ttu-id="f5a14-104">**EcpUrl tm**の要素は、先のすべてのサイトのメールボックスのメールが有効なユーザーは、現在メンバー リストにアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5a14-104">The **EcpUrl-tm** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access a list of all site mailboxes of which a mail-enabled user is currently a member.</span></span> 
  
[<span data-ttu-id="f5a14-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="f5a14-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="f5a14-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="f5a14-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="f5a14-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="f5a14-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="f5a14-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="f5a14-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="f5a14-109">EcpUrl-tm (POX)</span><span class="sxs-lookup"><span data-stu-id="f5a14-109">EcpUrl-tm (POX)</span></span>](ecpurl-tm-pox.md)
  
```XML
<EcpUrl-tm/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="f5a14-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f5a14-110">Attributes and elements</span></span>

<span data-ttu-id="f5a14-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f5a14-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f5a14-112">属性</span><span class="sxs-lookup"><span data-stu-id="f5a14-112">Attributes</span></span>

<span data-ttu-id="f5a14-113">なし。</span><span class="sxs-lookup"><span data-stu-id="f5a14-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f5a14-114">子要素</span><span class="sxs-lookup"><span data-stu-id="f5a14-114">Child elements</span></span>

<span data-ttu-id="f5a14-115">なし。</span><span class="sxs-lookup"><span data-stu-id="f5a14-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f5a14-116">親要素</span><span class="sxs-lookup"><span data-stu-id="f5a14-116">Parent elements</span></span>

|<span data-ttu-id="f5a14-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="f5a14-117">**Element**</span></span>|<span data-ttu-id="f5a14-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="f5a14-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5a14-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="f5a14-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="f5a14-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f5a14-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f5a14-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f5a14-121">Text value</span></span>

<span data-ttu-id="f5a14-122">テキスト値は、ユーザーのメールボックスをサイトの一覧にアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を表します。</span><span class="sxs-lookup"><span data-stu-id="f5a14-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access a list of site mailboxes for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f5a14-123">備考</span><span class="sxs-lookup"><span data-stu-id="f5a14-123">Remarks</span></span>

<span data-ttu-id="f5a14-124">**EcpUrl tm**の要素は、**プロトコル**要素の省略可能な子要素です。</span><span class="sxs-lookup"><span data-stu-id="f5a14-124">The **EcpUrl-tm** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f5a14-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="f5a14-125">See also</span></span>



[<span data-ttu-id="f5a14-126">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f5a14-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


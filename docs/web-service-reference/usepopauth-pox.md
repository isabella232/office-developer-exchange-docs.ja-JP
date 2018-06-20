---
title: UsePOPAuth (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 28f552d8-6bb8-49b4-a45c-b2053670f1cc
description: UsePOPAuth 要素は、POP3 アカウントの種類の指定された認証情報は、簡易メール転送プロトコル (SMTP) を使用してもかどうかを示します。
ms.openlocfilehash: be03568d697b1f5461d49dba388a1d3f1008a67e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839916"
---
# <a name="usepopauth-pox"></a><span data-ttu-id="869d0-103">UsePOPAuth (POX)</span><span class="sxs-lookup"><span data-stu-id="869d0-103">UsePOPAuth (POX)</span></span>

<span data-ttu-id="869d0-104">**UsePOPAuth**要素は、POP3 アカウントの種類の指定された認証情報は、簡易メール転送プロトコル (SMTP) を使用してもかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="869d0-104">The **UsePOPAuth** element indicates whether the authentication information that is provided for a POP3 type of account is also used for Simple Mail Transfer Protocol (SMTP).</span></span> 
  
[<span data-ttu-id="869d0-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="869d0-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="869d0-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="869d0-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="869d0-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="869d0-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="869d0-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="869d0-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="869d0-109">UsePOPAuth (POX)</span><span class="sxs-lookup"><span data-stu-id="869d0-109">UsePOPAuth (POX)</span></span>](usepopauth-pox.md)
  
```xml
<UsePOPAuth>on or off</UsePOPAuth>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="869d0-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="869d0-110">Attributes and elements</span></span>

<span data-ttu-id="869d0-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="869d0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="869d0-112">属性</span><span class="sxs-lookup"><span data-stu-id="869d0-112">Attributes</span></span>

<span data-ttu-id="869d0-113">なし。</span><span class="sxs-lookup"><span data-stu-id="869d0-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="869d0-114">子要素</span><span class="sxs-lookup"><span data-stu-id="869d0-114">Child elements</span></span>

<span data-ttu-id="869d0-115">なし。</span><span class="sxs-lookup"><span data-stu-id="869d0-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="869d0-116">親要素</span><span class="sxs-lookup"><span data-stu-id="869d0-116">Parent elements</span></span>

|<span data-ttu-id="869d0-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="869d0-117">**Element**</span></span>|<span data-ttu-id="869d0-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="869d0-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="869d0-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="869d0-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="869d0-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="869d0-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="869d0-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="869d0-121">Text value</span></span>

<span data-ttu-id="869d0-122">テキスト値は、POP3 アカウントの種類に用意されている認証情報が smtp も使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="869d0-122">The text value indicates whether the authentication information that is provided for a POP3 type of account is also used for SMTP.</span></span> <span data-ttu-id="869d0-123">使用可能な値は、**オン**と**オフを**します。</span><span class="sxs-lookup"><span data-stu-id="869d0-123">The possible values are **on** and **off**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="869d0-124">備考</span><span class="sxs-lookup"><span data-stu-id="869d0-124">Remarks</span></span>

<span data-ttu-id="869d0-125">**UsePOPAuth**要素は、[型 (POX)](type-pox.md)が SMTP である場合にのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="869d0-125">The **UsePOPAuth** element is only used when [Type (POX)](type-pox.md) is SMTP.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="869d0-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="869d0-126">See also</span></span>



[<span data-ttu-id="869d0-127">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="869d0-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


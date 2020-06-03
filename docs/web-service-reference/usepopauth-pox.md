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
description: UsePOPAuth 要素は、POP3 の種類のアカウントに対して提供された認証情報が簡易メール転送プロトコル (SMTP) にも使用されるかどうかを示します。
ms.openlocfilehash: 8d5bfffaab31c382ad43915e18b8a7a2b2737c21
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466508"
---
# <a name="usepopauth-pox"></a><span data-ttu-id="f3778-103">UsePOPAuth (POX)</span><span class="sxs-lookup"><span data-stu-id="f3778-103">UsePOPAuth (POX)</span></span>

<span data-ttu-id="f3778-104">**Usepopauth**要素は、POP3 の種類のアカウントに対して提供された認証情報が簡易メール転送プロトコル (SMTP) にも使用されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3778-104">The **UsePOPAuth** element indicates whether the authentication information that is provided for a POP3 type of account is also used for Simple Mail Transfer Protocol (SMTP).</span></span> 
  
[<span data-ttu-id="f3778-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="f3778-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="f3778-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="f3778-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="f3778-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="f3778-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="f3778-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="f3778-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="f3778-109">UsePOPAuth (POX)</span><span class="sxs-lookup"><span data-stu-id="f3778-109">UsePOPAuth (POX)</span></span>](usepopauth-pox.md)
  
```xml
<UsePOPAuth>on or off</UsePOPAuth>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="f3778-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f3778-110">Attributes and elements</span></span>

<span data-ttu-id="f3778-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f3778-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3778-112">属性</span><span class="sxs-lookup"><span data-stu-id="f3778-112">Attributes</span></span>

<span data-ttu-id="f3778-113">なし。</span><span class="sxs-lookup"><span data-stu-id="f3778-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3778-114">子要素</span><span class="sxs-lookup"><span data-stu-id="f3778-114">Child elements</span></span>

<span data-ttu-id="f3778-115">なし。</span><span class="sxs-lookup"><span data-stu-id="f3778-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f3778-116">親要素</span><span class="sxs-lookup"><span data-stu-id="f3778-116">Parent elements</span></span>

|<span data-ttu-id="f3778-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="f3778-117">**Element**</span></span>|<span data-ttu-id="f3778-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="f3778-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3778-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="f3778-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="f3778-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3778-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f3778-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f3778-121">Text value</span></span>

<span data-ttu-id="f3778-122">テキスト値は、POP3 の種類のアカウントに対して提供された認証情報が SMTP にも使用されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3778-122">The text value indicates whether the authentication information that is provided for a POP3 type of account is also used for SMTP.</span></span> <span data-ttu-id="f3778-123">有効な値は、 **[オン**] または [**オフ**] です。</span><span class="sxs-lookup"><span data-stu-id="f3778-123">The possible values are **on** and **off**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f3778-124">注釈</span><span class="sxs-lookup"><span data-stu-id="f3778-124">Remarks</span></span>

<span data-ttu-id="f3778-125">**Usepopauth**要素は、 [Type (POX)](type-pox.md)が SMTP の場合にのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="f3778-125">The **UsePOPAuth** element is only used when [Type (POX)](type-pox.md) is SMTP.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f3778-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="f3778-126">See also</span></span>



[<span data-ttu-id="f3778-127">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="f3778-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


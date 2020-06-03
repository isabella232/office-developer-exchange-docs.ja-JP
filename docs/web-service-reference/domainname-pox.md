---
title: DomainName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2b4af2b2-58b5-4f28-9cb3-c07a11377747
description: DomainName 要素は、ユーザーのドメインを指定します。
ms.openlocfilehash: ff38d6a876e396317dedece0a81a9f9f0db0f587
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458426"
---
# <a name="domainname-pox"></a><span data-ttu-id="cc713-103">DomainName (POX)</span><span class="sxs-lookup"><span data-stu-id="cc713-103">DomainName (POX)</span></span>

<span data-ttu-id="cc713-104">**DomainName**要素は、ユーザーのドメインを指定します。</span><span class="sxs-lookup"><span data-stu-id="cc713-104">The **DomainName** element specifies the user's domain.</span></span> 
  
- [<span data-ttu-id="cc713-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="cc713-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="cc713-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="cc713-106">Response (POX)</span></span>](response-pox.md)  
- [<span data-ttu-id="cc713-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="cc713-107">Account (POX)</span></span>](account-pox.md) 
- [<span data-ttu-id="cc713-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="cc713-108">Protocol (POX)</span></span>](protocol-pox.md) 
- [<span data-ttu-id="cc713-109">DomainName (POX)</span><span class="sxs-lookup"><span data-stu-id="cc713-109">DomainName (POX)</span></span>](domainname-pox.md)
  
```xml
<DomainName/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="cc713-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cc713-110">Attributes and elements</span></span>

<span data-ttu-id="cc713-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cc713-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc713-112">属性</span><span class="sxs-lookup"><span data-stu-id="cc713-112">Attributes</span></span>

<span data-ttu-id="cc713-113">なし。</span><span class="sxs-lookup"><span data-stu-id="cc713-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc713-114">子要素</span><span class="sxs-lookup"><span data-stu-id="cc713-114">Child elements</span></span>

<span data-ttu-id="cc713-115">なし。</span><span class="sxs-lookup"><span data-stu-id="cc713-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cc713-116">親要素</span><span class="sxs-lookup"><span data-stu-id="cc713-116">Parent elements</span></span>

|<span data-ttu-id="cc713-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="cc713-117">**Element**</span></span>|<span data-ttu-id="cc713-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="cc713-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc713-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="cc713-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="cc713-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cc713-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cc713-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cc713-121">Text value</span></span>

<span data-ttu-id="cc713-122">Text 値は、ユーザーのドメインを指定します。</span><span class="sxs-lookup"><span data-stu-id="cc713-122">The text value specifies the user's domain.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cc713-123">注釈</span><span class="sxs-lookup"><span data-stu-id="cc713-123">Remarks</span></span>

<span data-ttu-id="cc713-124">値が指定されていない場合、既定の認証では電子メールアドレスがユーザープリンシパル名 (UPN) 形式として使用されます。</span><span class="sxs-lookup"><span data-stu-id="cc713-124">If no value is specified, the default authentication is to use the e-mail address as a user principal name (UPN) format.</span></span> <span data-ttu-id="cc713-125">次に例を示します \<Username\> @ \<Domain\> 。</span><span class="sxs-lookup"><span data-stu-id="cc713-125">For example: \<Username\>@\<Domain\>.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="cc713-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="cc713-126">See also</span></span>

- [<span data-ttu-id="cc713-127">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="cc713-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


---
title: ドメイン名 (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2b4af2b2-58b5-4f28-9cb3-c07a11377747
description: ドメイン名の要素は、ユーザーのドメインを指定します。
ms.openlocfilehash: c38d2e470bd174ab6dd7e5e1dd3eee23daea5e69
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760150"
---
# <a name="domainname-pox"></a><span data-ttu-id="18fe8-103">ドメイン名 (POX)</span><span class="sxs-lookup"><span data-stu-id="18fe8-103">DomainName (POX)</span></span>

<span data-ttu-id="18fe8-104">**ドメイン名**の要素は、ユーザーのドメインを指定します。</span><span class="sxs-lookup"><span data-stu-id="18fe8-104">The **DomainName** element specifies the user's domain.</span></span> 
  
- [<span data-ttu-id="18fe8-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="18fe8-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="18fe8-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="18fe8-106">Response (POX)</span></span>](response-pox.md)  
- [<span data-ttu-id="18fe8-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="18fe8-107">Account (POX)</span></span>](account-pox.md) 
- [<span data-ttu-id="18fe8-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="18fe8-108">Protocol (POX)</span></span>](protocol-pox.md) 
- [<span data-ttu-id="18fe8-109">ドメイン名 (POX)</span><span class="sxs-lookup"><span data-stu-id="18fe8-109">DomainName (POX)</span></span>](domainname-pox.md)
  
```xml
<DomainName/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="18fe8-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="18fe8-110">Attributes and elements</span></span>

<span data-ttu-id="18fe8-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="18fe8-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18fe8-112">属性</span><span class="sxs-lookup"><span data-stu-id="18fe8-112">Attributes</span></span>

<span data-ttu-id="18fe8-113">なし。</span><span class="sxs-lookup"><span data-stu-id="18fe8-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18fe8-114">子要素</span><span class="sxs-lookup"><span data-stu-id="18fe8-114">Child elements</span></span>

<span data-ttu-id="18fe8-115">なし。</span><span class="sxs-lookup"><span data-stu-id="18fe8-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="18fe8-116">親要素</span><span class="sxs-lookup"><span data-stu-id="18fe8-116">Parent elements</span></span>

|<span data-ttu-id="18fe8-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="18fe8-117">**Element**</span></span>|<span data-ttu-id="18fe8-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="18fe8-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18fe8-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="18fe8-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="18fe8-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="18fe8-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="18fe8-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="18fe8-121">Text value</span></span>

<span data-ttu-id="18fe8-122">テキスト値は、ユーザーのドメインを指定します。</span><span class="sxs-lookup"><span data-stu-id="18fe8-122">The text value specifies the user's domain.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="18fe8-123">備考</span><span class="sxs-lookup"><span data-stu-id="18fe8-123">Remarks</span></span>

<span data-ttu-id="18fe8-124">値が指定されていない場合は、ユーザー プリンシパル名 (UPN) 形式で電子メール アドレスを使用する既定の認証。</span><span class="sxs-lookup"><span data-stu-id="18fe8-124">If no value is specified, the default authentication is to use the e-mail address as a user principal name (UPN) format.</span></span> <span data-ttu-id="18fe8-125">例:\<ユーザー名\>@\<ドメイン\>。</span><span class="sxs-lookup"><span data-stu-id="18fe8-125">For example: \<Username\>@\<Domain\>.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="18fe8-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="18fe8-126">See also</span></span>

- [<span data-ttu-id="18fe8-127">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="18fe8-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


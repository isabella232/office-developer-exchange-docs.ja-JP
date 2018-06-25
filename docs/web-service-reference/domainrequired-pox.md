---
title: DomainRequired (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1f26b691-7331-4c7f-a92b-dfcc66c26963
description: DomainRequired 要素は、ドメインが認証に必要かどうかを示します。
ms.openlocfilehash: f314b9d27d1b4ee472d249ec49af1a785ff9ac25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760146"
---
# <a name="domainrequired-pox"></a><span data-ttu-id="4e68d-103">DomainRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="4e68d-103">DomainRequired (POX)</span></span>

<span data-ttu-id="4e68d-104">**DomainRequired**要素は、ドメインが認証に必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4e68d-104">The **DomainRequired** element indicates whether the domain is required for authentication.</span></span> 
  
- [<span data-ttu-id="4e68d-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="4e68d-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="4e68d-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="4e68d-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="4e68d-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="4e68d-107">Account (POX)</span></span>](account-pox.md)  
- [<span data-ttu-id="4e68d-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="4e68d-108">Protocol (POX)</span></span>](protocol-pox.md)  
- [<span data-ttu-id="4e68d-109">DomainRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="4e68d-109">DomainRequired (POX)</span></span>](domainrequired-pox.md)
  
```xml
<DomainRequired>on or off</DomainRequired>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="4e68d-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4e68d-110">Attributes and elements</span></span>

<span data-ttu-id="4e68d-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4e68d-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4e68d-112">属性</span><span class="sxs-lookup"><span data-stu-id="4e68d-112">Attributes</span></span>

<span data-ttu-id="4e68d-113">なし。</span><span class="sxs-lookup"><span data-stu-id="4e68d-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4e68d-114">子要素</span><span class="sxs-lookup"><span data-stu-id="4e68d-114">Child elements</span></span>

<span data-ttu-id="4e68d-115">なし。</span><span class="sxs-lookup"><span data-stu-id="4e68d-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4e68d-116">親要素</span><span class="sxs-lookup"><span data-stu-id="4e68d-116">Parent elements</span></span>

|<span data-ttu-id="4e68d-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="4e68d-117">**Element**</span></span>|<span data-ttu-id="4e68d-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="4e68d-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e68d-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="4e68d-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="4e68d-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4e68d-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4e68d-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4e68d-121">Text value</span></span>

<span data-ttu-id="4e68d-122">テキスト値は、ドメインが認証に必要なかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4e68d-122">The text value indicates whether the domain is required for authentication.</span></span> <span data-ttu-id="4e68d-123">使用可能な値は、**オン**と**オフを**します。</span><span class="sxs-lookup"><span data-stu-id="4e68d-123">The possible values are **on** and **off**.</span></span> <span data-ttu-id="4e68d-124">**** 値がある場合、後続の要求では、ユーザーのアカウントのドメインを含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="4e68d-124">If the value is **on**, the subsequent request must contain the domain of the user's account.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4e68d-125">備考</span><span class="sxs-lookup"><span data-stu-id="4e68d-125">Remarks</span></span>

<span data-ttu-id="4e68d-126">[LoginName (POX)](loginname-pox.md)要素では、ドメインが指定されていない、または**ログイン名が表示**要素が指定されていません、ユーザーは認証が成功する前にドメインを入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4e68d-126">If the domain is not specified in the [LoginName (POX)](loginname-pox.md) element, or the **LoginName** element was not specified, the user must enter the domain before authentication will succeed.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="4e68d-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="4e68d-127">See also</span></span>

- [<span data-ttu-id="4e68d-128">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4e68d-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


---
title: AutoDiscoverSMTPAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 7763d11a-b338-4a02-8a01-938859c05dfb
description: AutoDiscoverSMTPAddress 要素には、自動検出プロセスで使用されるユーザーの SMTP アドレスが含まれています。
ms.openlocfilehash: 6f44fc30fcf96bc059aa9412f5c3c5b8f596d2fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759477"
---
# <a name="autodiscoversmtpaddress-pox"></a><span data-ttu-id="5f4c9-103">AutoDiscoverSMTPAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="5f4c9-103">AutoDiscoverSMTPAddress (POX)</span></span>

<span data-ttu-id="5f4c9-104">**AutoDiscoverSMTPAddress**要素には、自動検出プロセスで使用されるユーザーの SMTP アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5f4c9-104">The **AutoDiscoverSMTPAddress** element contains the user's SMTP address that is used for the Autodiscover process.</span></span> 
  
- [<span data-ttu-id="5f4c9-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="5f4c9-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="5f4c9-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="5f4c9-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="5f4c9-107">ユーザー (POX)</span><span class="sxs-lookup"><span data-stu-id="5f4c9-107">User (POX)</span></span>](user-pox.md)
  
- [<span data-ttu-id="5f4c9-108">AutoDiscoverSMTPAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="5f4c9-108">AutoDiscoverSMTPAddress (POX)</span></span>](autodiscoversmtpaddress-pox.md)
  
```XML
<AutoDiscoverSMTPAddress/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="5f4c9-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5f4c9-109">Attributes and elements</span></span>

<span data-ttu-id="5f4c9-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5f4c9-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5f4c9-111">属性</span><span class="sxs-lookup"><span data-stu-id="5f4c9-111">Attributes</span></span>

<span data-ttu-id="5f4c9-112">なし。</span><span class="sxs-lookup"><span data-stu-id="5f4c9-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5f4c9-113">子要素</span><span class="sxs-lookup"><span data-stu-id="5f4c9-113">Child elements</span></span>

<span data-ttu-id="5f4c9-114">なし。</span><span class="sxs-lookup"><span data-stu-id="5f4c9-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5f4c9-115">親要素</span><span class="sxs-lookup"><span data-stu-id="5f4c9-115">Parent elements</span></span>

|<span data-ttu-id="5f4c9-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="5f4c9-116">**Element**</span></span>|<span data-ttu-id="5f4c9-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="5f4c9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f4c9-118">ユーザー (POX)</span><span class="sxs-lookup"><span data-stu-id="5f4c9-118">User (POX)</span></span>](user-pox.md) <br/> |<span data-ttu-id="5f4c9-119">ユーザー固有の情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="5f4c9-119">Provides user-specific information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5f4c9-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5f4c9-120">Text value</span></span>

<span data-ttu-id="5f4c9-121">テキスト値は、自動検出プロセスで使用されるユーザーの SMTP アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="5f4c9-121">The text value represents the user's SMTP address that is used for the Autodiscover process.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5f4c9-122">備考</span><span class="sxs-lookup"><span data-stu-id="5f4c9-122">Remarks</span></span>

<span data-ttu-id="5f4c9-123">**AutoDiscoverSMTPAddress**要素は、**ユーザー**要素の省略可能な子要素です。</span><span class="sxs-lookup"><span data-stu-id="5f4c9-123">The **AutoDiscoverSMTPAddress** element is an optional child element of the **User** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="5f4c9-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="5f4c9-124">See also</span></span>

- [<span data-ttu-id="5f4c9-125">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5f4c9-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


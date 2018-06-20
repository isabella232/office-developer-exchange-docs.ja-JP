---
title: LegacyDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9fb9529f-52c5-4907-a84b-935b78de16c3
description: LegacyDN 要素は、従来の識別名によって、ユーザーのメールボックスを識別します。
ms.openlocfilehash: f7ec1dea29a7d3ad6d470ef7812390d179fe1d2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832243"
---
# <a name="legacydn-pox"></a><span data-ttu-id="d6e56-103">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="d6e56-103">LegacyDN (POX)</span></span>

<span data-ttu-id="d6e56-104">**LegacyDN**要素は、従来の識別名によって、ユーザーのメールボックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="d6e56-104">The **LegacyDN** element identifies a user's mailbox by legacy distinguished name.</span></span> 
  
```xml
<LegacyDN/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d6e56-105">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d6e56-105">Attributes and elements</span></span>

<span data-ttu-id="d6e56-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d6e56-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6e56-107">属性</span><span class="sxs-lookup"><span data-stu-id="d6e56-107">Attributes</span></span>

<span data-ttu-id="d6e56-108">なし。</span><span class="sxs-lookup"><span data-stu-id="d6e56-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d6e56-109">子要素</span><span class="sxs-lookup"><span data-stu-id="d6e56-109">Child elements</span></span>

<span data-ttu-id="d6e56-110">なし。</span><span class="sxs-lookup"><span data-stu-id="d6e56-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d6e56-111">親要素</span><span class="sxs-lookup"><span data-stu-id="d6e56-111">Parent elements</span></span>

|<span data-ttu-id="d6e56-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="d6e56-112">**Element**</span></span>|<span data-ttu-id="d6e56-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="d6e56-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6e56-114">要求 (POX)</span><span class="sxs-lookup"><span data-stu-id="d6e56-114">Request (POX)</span></span>](request-pox.md) <br/> |<span data-ttu-id="d6e56-115">自動検出サービスへの要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d6e56-115">Contains the request to the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="d6e56-116">ユーザー (POX)</span><span class="sxs-lookup"><span data-stu-id="d6e56-116">User (POX)</span></span>](user-pox.md) <br/> |<span data-ttu-id="d6e56-117">ユーザー固有の情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="d6e56-117">Provides user-specific information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d6e56-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d6e56-118">Text value</span></span>

<span data-ttu-id="d6e56-119">テキスト値は、ユーザーの既存の電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="d6e56-119">The text value represents a user's legacy e-mail address.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d6e56-120">備考</span><span class="sxs-lookup"><span data-stu-id="d6e56-120">Remarks</span></span>

<span data-ttu-id="d6e56-121">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)の要素は、自動検出要求の代替要素です。</span><span class="sxs-lookup"><span data-stu-id="d6e56-121">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element is an alternative element for an Autodiscover request.</span></span> <span data-ttu-id="d6e56-122">Microsoft Exchange Server 2007 を実行しているコンピューター上にメールボックスが存在する場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="d6e56-122">It is used when a mailbox exists on a computer that is running Microsoft Exchange Server 2007.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d6e56-123">関連項目</span><span class="sxs-lookup"><span data-stu-id="d6e56-123">See also</span></span>

- [<span data-ttu-id="d6e56-124">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d6e56-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


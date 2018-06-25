---
title: 要求 (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: da54eb32-7ce5-4384-9893-255a2243a959
description: 要求要素には、自動検出サービスへの要求が含まれています。
ms.openlocfilehash: ed6b0a80e83e160287f382a881dc5405bfb47a37
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833124"
---
# <a name="request-pox"></a><span data-ttu-id="9ad61-103">要求 (POX)</span><span class="sxs-lookup"><span data-stu-id="9ad61-103">Request (POX)</span></span>

<span data-ttu-id="9ad61-104">**要求**要素には、自動検出サービスへの要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ad61-104">The **Request** element contains the request to the Autodiscover service.</span></span> 
  
[<span data-ttu-id="9ad61-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="9ad61-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="9ad61-106">要求 (POX)</span><span class="sxs-lookup"><span data-stu-id="9ad61-106">Request (POX)</span></span>](request-pox.md)
  
```xml
<Request>
   <AcceptableResponseSchema/>
   <EMailAddress/>
</Request>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="9ad61-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9ad61-107">Attributes and elements</span></span>

<span data-ttu-id="9ad61-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9ad61-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ad61-109">属性</span><span class="sxs-lookup"><span data-stu-id="9ad61-109">Attributes</span></span>

<span data-ttu-id="9ad61-110">なし。</span><span class="sxs-lookup"><span data-stu-id="9ad61-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ad61-111">子要素</span><span class="sxs-lookup"><span data-stu-id="9ad61-111">Child elements</span></span>

|<span data-ttu-id="9ad61-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="9ad61-112">**Element**</span></span>|<span data-ttu-id="9ad61-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ad61-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ad61-114">AcceptableResponseSchema (POX)</span><span class="sxs-lookup"><span data-stu-id="9ad61-114">AcceptableResponseSchema (POX)</span></span>](acceptableresponseschema-pox.md) <br/> |<span data-ttu-id="9ad61-115">自動検出応答スキーマを識別します。</span><span class="sxs-lookup"><span data-stu-id="9ad61-115">Identifies the schema for an Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="9ad61-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="9ad61-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="9ad61-117">ユーザーの電子メール アドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="9ad61-117">Identifies the user's e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="9ad61-118">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="9ad61-118">LegacyDN (POX)</span></span>](legacydn-pox.md) <br/> |<span data-ttu-id="9ad61-119">従来の識別名によって、ユーザーのメールボックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="9ad61-119">Identifies a user's mailbox by legacy distinguished name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9ad61-120">親要素</span><span class="sxs-lookup"><span data-stu-id="9ad61-120">Parent elements</span></span>

|<span data-ttu-id="9ad61-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="9ad61-121">**Element**</span></span>|<span data-ttu-id="9ad61-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ad61-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ad61-123">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="9ad61-123">AutoDiscover (POX)</span></span>](autodiscover-pox.md) <br/> |<span data-ttu-id="9ad61-124">自動検出要求のルート要素です。</span><span class="sxs-lookup"><span data-stu-id="9ad61-124">The root element in an Autodiscover request.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ad61-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="9ad61-125">See also</span></span>



[<span data-ttu-id="9ad61-126">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9ad61-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


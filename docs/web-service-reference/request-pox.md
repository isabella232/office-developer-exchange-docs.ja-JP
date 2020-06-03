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
description: Request 要素には、自動検出サービスへの要求が含まれています。
ms.openlocfilehash: bc215d614441ed8f12c0f1490f4abdbb7b574ad0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459547"
---
# <a name="request-pox"></a><span data-ttu-id="b21dd-103">要求 (POX)</span><span class="sxs-lookup"><span data-stu-id="b21dd-103">Request (POX)</span></span>

<span data-ttu-id="b21dd-104">**Request**要素には、自動検出サービスへの要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b21dd-104">The **Request** element contains the request to the Autodiscover service.</span></span> 
  
- [<span data-ttu-id="b21dd-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="b21dd-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="b21dd-106">要求 (POX)</span><span class="sxs-lookup"><span data-stu-id="b21dd-106">Request (POX)</span></span>](request-pox.md)
  
```xml
<Request>
   <AcceptableResponseSchema/>
   <EMailAddress/>
</Request>
```

```xml
<Request>
   <AcceptableResponseSchema/> 
   <LegacyDN/>
</Request>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="b21dd-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b21dd-107">Attributes and elements</span></span>

<span data-ttu-id="b21dd-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b21dd-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b21dd-109">属性</span><span class="sxs-lookup"><span data-stu-id="b21dd-109">Attributes</span></span>

<span data-ttu-id="b21dd-110">なし。</span><span class="sxs-lookup"><span data-stu-id="b21dd-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b21dd-111">子要素</span><span class="sxs-lookup"><span data-stu-id="b21dd-111">Child elements</span></span>

|<span data-ttu-id="b21dd-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="b21dd-112">**Element**</span></span>|<span data-ttu-id="b21dd-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="b21dd-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b21dd-114">AcceptableResponseSchema (POX)</span><span class="sxs-lookup"><span data-stu-id="b21dd-114">AcceptableResponseSchema (POX)</span></span>](acceptableresponseschema-pox.md) <br/> |<span data-ttu-id="b21dd-115">自動検出応答のスキーマを識別します。</span><span class="sxs-lookup"><span data-stu-id="b21dd-115">Identifies the schema for an Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="b21dd-116">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="b21dd-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="b21dd-117">ユーザーの電子メールアドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="b21dd-117">Identifies the user's e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="b21dd-118">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="b21dd-118">LegacyDN (POX)</span></span>](legacydn-pox.md) <br/> |<span data-ttu-id="b21dd-119">従来の識別名でユーザーのメールボックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="b21dd-119">Identifies a user's mailbox by legacy distinguished name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b21dd-120">親要素</span><span class="sxs-lookup"><span data-stu-id="b21dd-120">Parent elements</span></span>

|<span data-ttu-id="b21dd-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="b21dd-121">**Element**</span></span>|<span data-ttu-id="b21dd-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="b21dd-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b21dd-123">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="b21dd-123">AutoDiscover (POX)</span></span>](autodiscover-pox.md) <br/> |<span data-ttu-id="b21dd-124">自動検出要求のルート要素。</span><span class="sxs-lookup"><span data-stu-id="b21dd-124">The root element in an Autodiscover request.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b21dd-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="b21dd-125">See also</span></span>

- [<span data-ttu-id="b21dd-126">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="b21dd-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)


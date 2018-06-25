---
title: FreeBusyAccessLevel (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a287b9c3-7fb6-4f2f-a8dc-15d4bc32394c
description: FreeBusyAccessLevel 要素は、FreeBusyAccessLevel プロパティを表します。 FreeBusyAccessLevel 要素は、内部使用のみ。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: c978608982a2795af1683b4b2121435a02149935
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760598"
---
# <a name="freebusyaccesslevel-soap"></a><span data-ttu-id="c6a34-105">FreeBusyAccessLevel (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c6a34-105">FreeBusyAccessLevel (SOAP)</span></span>

<span data-ttu-id="c6a34-106">**FreeBusyAccessLevel**要素は、 **FreeBusyAccessLevel**プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="c6a34-106">The **FreeBusyAccessLevel** element represents the **FreeBusyAccessLevel** property.</span></span> <span data-ttu-id="c6a34-107">**FreeBusyAccessLevel**要素は、内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="c6a34-107">The **FreeBusyAccessLevel** element is for internal use only.</span></span> <span data-ttu-id="c6a34-108">クライアントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="c6a34-108">This element is not used by clients.</span></span> 
  
```XML
<FreeBusyAccessLevel/>
```

 <span data-ttu-id="c6a34-109">**string**</span><span class="sxs-lookup"><span data-stu-id="c6a34-109">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c6a34-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c6a34-110">Attributes and elements</span></span>

<span data-ttu-id="c6a34-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c6a34-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6a34-112">属性</span><span class="sxs-lookup"><span data-stu-id="c6a34-112">Attributes</span></span>

<span data-ttu-id="c6a34-113">なし。</span><span class="sxs-lookup"><span data-stu-id="c6a34-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c6a34-114">子要素</span><span class="sxs-lookup"><span data-stu-id="c6a34-114">Child elements</span></span>

<span data-ttu-id="c6a34-115">なし。</span><span class="sxs-lookup"><span data-stu-id="c6a34-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c6a34-116">親要素</span><span class="sxs-lookup"><span data-stu-id="c6a34-116">Parent elements</span></span>

|<span data-ttu-id="c6a34-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="c6a34-117">**Element**</span></span>|<span data-ttu-id="c6a34-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="c6a34-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6a34-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c6a34-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="c6a34-120">1 つの組織の組織との関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="c6a34-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c6a34-121">備考</span><span class="sxs-lookup"><span data-stu-id="c6a34-121">Remarks</span></span>

<span data-ttu-id="c6a34-122">この要素は、応答で返される空き時間情報の詳細情報の最大量を指定し、外部で共有されている空き時間情報データのレベルを示します。</span><span class="sxs-lookup"><span data-stu-id="c6a34-122">This element specifies the maximum amount of free/busy detail that will be returned in the response and indicates the level of free/busy data that is externally shared.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="c6a34-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="c6a34-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6a34-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="c6a34-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="c6a34-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c6a34-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c6a34-126">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="c6a34-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="c6a34-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c6a34-127">Validation File</span></span>  <br/> |<span data-ttu-id="c6a34-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c6a34-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c6a34-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c6a34-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="c6a34-130">True</span><span class="sxs-lookup"><span data-stu-id="c6a34-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c6a34-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="c6a34-131">See also</span></span>



[<span data-ttu-id="c6a34-132">GetOrganizationRelationshipSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c6a34-132">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)


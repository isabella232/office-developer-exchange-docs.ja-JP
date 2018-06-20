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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760598"
---
# <a name="freebusyaccesslevel-soap"></a><span data-ttu-id="72d97-105">FreeBusyAccessLevel (SOAP)</span><span class="sxs-lookup"><span data-stu-id="72d97-105">FreeBusyAccessLevel (SOAP)</span></span>

<span data-ttu-id="72d97-106">**FreeBusyAccessLevel**要素は、 **FreeBusyAccessLevel**プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="72d97-106">The **FreeBusyAccessLevel** element represents the **FreeBusyAccessLevel** property.</span></span> <span data-ttu-id="72d97-107">**FreeBusyAccessLevel**要素は、内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="72d97-107">The **FreeBusyAccessLevel** element is for internal use only.</span></span> <span data-ttu-id="72d97-108">クライアントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="72d97-108">This element is not used by clients.</span></span> 
  
```XML
<FreeBusyAccessLevel/>
```

 <span data-ttu-id="72d97-109">**string**</span><span class="sxs-lookup"><span data-stu-id="72d97-109">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="72d97-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="72d97-110">Attributes and elements</span></span>

<span data-ttu-id="72d97-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="72d97-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72d97-112">属性</span><span class="sxs-lookup"><span data-stu-id="72d97-112">Attributes</span></span>

<span data-ttu-id="72d97-113">なし。</span><span class="sxs-lookup"><span data-stu-id="72d97-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="72d97-114">子要素</span><span class="sxs-lookup"><span data-stu-id="72d97-114">Child elements</span></span>

<span data-ttu-id="72d97-115">なし。</span><span class="sxs-lookup"><span data-stu-id="72d97-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="72d97-116">親要素</span><span class="sxs-lookup"><span data-stu-id="72d97-116">Parent elements</span></span>

|<span data-ttu-id="72d97-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="72d97-117">**Element**</span></span>|<span data-ttu-id="72d97-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="72d97-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72d97-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="72d97-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="72d97-120">1 つの組織の組織との関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="72d97-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="72d97-121">備考</span><span class="sxs-lookup"><span data-stu-id="72d97-121">Remarks</span></span>

<span data-ttu-id="72d97-122">この要素は、応答で返される空き時間情報の詳細情報の最大量を指定し、外部で共有されている空き時間情報データのレベルを示します。</span><span class="sxs-lookup"><span data-stu-id="72d97-122">This element specifies the maximum amount of free/busy detail that will be returned in the response and indicates the level of free/busy data that is externally shared.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="72d97-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="72d97-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72d97-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="72d97-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="72d97-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="72d97-125">Schema Name</span></span>  <br/> |<span data-ttu-id="72d97-126">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="72d97-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="72d97-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="72d97-127">Validation File</span></span>  <br/> |<span data-ttu-id="72d97-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="72d97-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="72d97-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="72d97-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="72d97-130">True</span><span class="sxs-lookup"><span data-stu-id="72d97-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="72d97-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="72d97-131">See also</span></span>



[<span data-ttu-id="72d97-132">GetOrganizationRelationshipSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="72d97-132">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)


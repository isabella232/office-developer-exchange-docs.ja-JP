---
title: TargetApplicationUri (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e13c0edd-2ab1-49bb-a993-54a8db2dfbb9
description: TargetApplicationUri 要素は、ターゲット アプリケーションの URI を定義します。 TargetApplicationUri 要素は、内部使用のみ。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: fa401d4c1e8c1460804f116d840fe21129957852
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839645"
---
# <a name="targetapplicationuri-soap"></a><span data-ttu-id="7ca3d-105">TargetApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7ca3d-105">TargetApplicationUri (SOAP)</span></span>

<span data-ttu-id="7ca3d-106">**TargetApplicationUri**要素は、ターゲット アプリケーションの URI を定義します。</span><span class="sxs-lookup"><span data-stu-id="7ca3d-106">The **TargetApplicationUri** element defines the target application URI.</span></span> <span data-ttu-id="7ca3d-107">**TargetApplicationUri**要素は、内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="7ca3d-107">The **TargetApplicationUri** element is for internal use only.</span></span> <span data-ttu-id="7ca3d-108">クライアントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="7ca3d-108">This element is not used by clients.</span></span> 
  
```XML
<TargetApplicationUri/>
```

 <span data-ttu-id="7ca3d-109">**anyURI**</span><span class="sxs-lookup"><span data-stu-id="7ca3d-109">**anyURI**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7ca3d-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7ca3d-110">Attributes and elements</span></span>

<span data-ttu-id="7ca3d-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7ca3d-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ca3d-112">属性</span><span class="sxs-lookup"><span data-stu-id="7ca3d-112">Attributes</span></span>

<span data-ttu-id="7ca3d-113">なし。</span><span class="sxs-lookup"><span data-stu-id="7ca3d-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7ca3d-114">子要素</span><span class="sxs-lookup"><span data-stu-id="7ca3d-114">Child elements</span></span>

<span data-ttu-id="7ca3d-115">なし。</span><span class="sxs-lookup"><span data-stu-id="7ca3d-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7ca3d-116">親要素</span><span class="sxs-lookup"><span data-stu-id="7ca3d-116">Parent elements</span></span>

|<span data-ttu-id="7ca3d-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="7ca3d-117">**Element**</span></span>|<span data-ttu-id="7ca3d-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="7ca3d-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ca3d-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7ca3d-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="7ca3d-120">1 つの組織の組織との関係の一覧を表します</span><span class="sxs-lookup"><span data-stu-id="7ca3d-120">Represents a list of organization relationships for a single organization</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7ca3d-121">備考</span><span class="sxs-lookup"><span data-stu-id="7ca3d-121">Remarks</span></span>

<span data-ttu-id="7ca3d-122">この要素は、対象の外部組織の URI を定義します。</span><span class="sxs-lookup"><span data-stu-id="7ca3d-122">This element defines the target URI of the external organization.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ca3d-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="7ca3d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ca3d-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="7ca3d-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="7ca3d-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7ca3d-125">Schema Name</span></span>  <br/> |<span data-ttu-id="7ca3d-126">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="7ca3d-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="7ca3d-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7ca3d-127">Validation File</span></span>  <br/> |<span data-ttu-id="7ca3d-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7ca3d-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7ca3d-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7ca3d-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="7ca3d-130">True</span><span class="sxs-lookup"><span data-stu-id="7ca3d-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ca3d-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="7ca3d-131">See also</span></span>



[<span data-ttu-id="7ca3d-132">GetOrganizationRelationshipSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7ca3d-132">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)


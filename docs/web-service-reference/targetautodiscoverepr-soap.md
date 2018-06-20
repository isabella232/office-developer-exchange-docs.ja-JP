---
title: TargetAutodiscoverEpr (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: fdb9cc7a-cf0a-431b-9f6f-5f1db1792db7
description: TargetAutodiscoverEpr 要素は、TargetAutodiscoverEpr プロパティを表します。 TargetAutodiscoverEpr 要素は、内部使用のみ。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: 0b28444727e21a98925b6d1062bcbbac62c68981
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839646"
---
# <a name="targetautodiscoverepr-soap"></a><span data-ttu-id="8286b-105">TargetAutodiscoverEpr (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8286b-105">TargetAutodiscoverEpr (SOAP)</span></span>

<span data-ttu-id="8286b-106">**TargetAutodiscoverEpr**要素は、 **TargetAutodiscoverEpr**プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="8286b-106">The **TargetAutodiscoverEpr** element represents the **TargetAutodiscoverEpr** property.</span></span> <span data-ttu-id="8286b-107">**TargetAutodiscoverEpr**要素は、内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="8286b-107">The **TargetAutodiscoverEpr** element is for internal use only.</span></span> <span data-ttu-id="8286b-108">クライアントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="8286b-108">This element is not used by clients.</span></span> 
  
```XML
<TargetAutodiscoverEpr/>
```

 <span data-ttu-id="8286b-109">**anyURI**</span><span class="sxs-lookup"><span data-stu-id="8286b-109">**anyURI**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8286b-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8286b-110">Attributes and elements</span></span>

<span data-ttu-id="8286b-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8286b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8286b-112">属性</span><span class="sxs-lookup"><span data-stu-id="8286b-112">Attributes</span></span>

<span data-ttu-id="8286b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="8286b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8286b-114">子要素</span><span class="sxs-lookup"><span data-stu-id="8286b-114">Child elements</span></span>

<span data-ttu-id="8286b-115">なし。</span><span class="sxs-lookup"><span data-stu-id="8286b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8286b-116">親要素</span><span class="sxs-lookup"><span data-stu-id="8286b-116">Parent elements</span></span>

|<span data-ttu-id="8286b-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="8286b-117">**Element**</span></span>|<span data-ttu-id="8286b-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="8286b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8286b-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8286b-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="8286b-120">1 つの組織の組織との関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="8286b-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8286b-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8286b-121">Text value</span></span>

<span data-ttu-id="8286b-122">この要素のテキスト値は、組織の関係の統一リソース識別子 (URI) です。</span><span class="sxs-lookup"><span data-stu-id="8286b-122">The text value for this element is a uniform resource identifier (URI) for the organization relationship.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8286b-123">備考</span><span class="sxs-lookup"><span data-stu-id="8286b-123">Remarks</span></span>

<span data-ttu-id="8286b-124">この要素は、外部組織のサーバーの自動検出 URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="8286b-124">This element specifies the Autodiscover URL of the server for the external organization.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="8286b-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="8286b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8286b-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="8286b-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="8286b-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8286b-127">Schema Name</span></span>  <br/> |<span data-ttu-id="8286b-128">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="8286b-128">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="8286b-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8286b-129">Validation File</span></span>  <br/> |<span data-ttu-id="8286b-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8286b-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8286b-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8286b-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="8286b-132">True</span><span class="sxs-lookup"><span data-stu-id="8286b-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8286b-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="8286b-133">See also</span></span>



[<span data-ttu-id="8286b-134">GetOrganizationRelationshipSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8286b-134">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)


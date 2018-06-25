---
title: TargetSharingEpr (SOAP)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0115a740-9264-4e57-a410-197bb39e6c81
description: TargetSharingEpr 要素は、TargetSharingEpr プロパティを表します。 TargetSharingEpr 要素は、内部使用のみ。
ms.openlocfilehash: 272133d4d8f6db260f37e2c6977be20f81fdc535
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839647"
---
# <a name="targetsharingepr-soap"></a><span data-ttu-id="4b4b0-104">TargetSharingEpr (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4b4b0-104">TargetSharingEpr (SOAP)</span></span>
 
<span data-ttu-id="4b4b0-105">**TargetSharingEpr**要素は、 **TargetSharingEpr**プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="4b4b0-105">The **TargetSharingEpr** element represents the **TargetSharingEpr** property.</span></span> <span data-ttu-id="4b4b0-106">**TargetSharingEpr**要素は、内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="4b4b0-106">The **TargetSharingEpr** element is for internal use only.</span></span> <span data-ttu-id="4b4b0-107">クライアントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="4b4b0-107">This element is not used by clients.</span></span> 
  
```XML
<TargetSharingEpr/>
```

<span data-ttu-id="4b4b0-108">**anyURI**</span><span class="sxs-lookup"><span data-stu-id="4b4b0-108">**anyURI**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4b4b0-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4b4b0-109">Attributes and elements</span></span>

<span data-ttu-id="4b4b0-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4b4b0-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b4b0-111">属性</span><span class="sxs-lookup"><span data-stu-id="4b4b0-111">Attributes</span></span>

<span data-ttu-id="4b4b0-112">なし。</span><span class="sxs-lookup"><span data-stu-id="4b4b0-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b4b0-113">子要素</span><span class="sxs-lookup"><span data-stu-id="4b4b0-113">Child elements</span></span>

<span data-ttu-id="4b4b0-114">なし。</span><span class="sxs-lookup"><span data-stu-id="4b4b0-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4b4b0-115">親要素</span><span class="sxs-lookup"><span data-stu-id="4b4b0-115">Parent elements</span></span>

|<span data-ttu-id="4b4b0-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="4b4b0-116">**Element**</span></span>|<span data-ttu-id="4b4b0-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="4b4b0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b4b0-118">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4b4b0-118">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="4b4b0-119">1 つの組織の組織との関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="4b4b0-119">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4b4b0-120">備考</span><span class="sxs-lookup"><span data-stu-id="4b4b0-120">Remarks</span></span>

<span data-ttu-id="4b4b0-121">この要素は、外部の組織に対して、対象サーバーの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="4b4b0-121">This element specifies the URL of the target server for the external organization.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="4b4b0-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="4b4b0-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b4b0-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="4b4b0-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="4b4b0-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4b4b0-124">Schema Name</span></span>  <br/> |<span data-ttu-id="4b4b0-125">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="4b4b0-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="4b4b0-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4b4b0-126">Validation File</span></span>  <br/> |<span data-ttu-id="4b4b0-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4b4b0-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4b4b0-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4b4b0-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="4b4b0-129">True</span><span class="sxs-lookup"><span data-stu-id="4b4b0-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4b4b0-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="4b4b0-130">See also</span></span>

- [<span data-ttu-id="4b4b0-131">GetOrganizationRelationshipSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4b4b0-131">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)


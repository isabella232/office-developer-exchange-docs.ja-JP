---
title: DeliveryReportEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ab522bc-40ea-4e43-aa57-6d2562db35e9
description: DeliveryReportEnabled 要素は、DeliveryReportEnabled() フラグを表します。 DeliveryReportEnabled 要素は、内部使用のみ。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: 089256a5f75ad92a4f11c5aaf3d175382eeee456
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760007"
---
# <a name="deliveryreportenabled-soap"></a><span data-ttu-id="9073f-105">DeliveryReportEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9073f-105">DeliveryReportEnabled (SOAP)</span></span>

<span data-ttu-id="9073f-106">**DeliveryReportEnabled**要素は、 **DeliveryReportEnabled()** フラグを表します。</span><span class="sxs-lookup"><span data-stu-id="9073f-106">The **DeliveryReportEnabled** element represents the **DeliveryReportEnabled()** flag.</span></span> <span data-ttu-id="9073f-107">**DeliveryReportEnabled**要素は、内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="9073f-107">The **DeliveryReportEnabled** element is for internal use only.</span></span> <span data-ttu-id="9073f-108">クライアントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="9073f-108">This element is not used by clients.</span></span> 
  
```XML
<DeliveryReportEnabled>true | false</DeliveryReportEnabled>
```

 <span data-ttu-id="9073f-109">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="9073f-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9073f-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9073f-110">Attributes and elements</span></span>

<span data-ttu-id="9073f-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9073f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9073f-112">属性</span><span class="sxs-lookup"><span data-stu-id="9073f-112">Attributes</span></span>

<span data-ttu-id="9073f-113">なし。</span><span class="sxs-lookup"><span data-stu-id="9073f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9073f-114">子要素</span><span class="sxs-lookup"><span data-stu-id="9073f-114">Child elements</span></span>

<span data-ttu-id="9073f-115">なし。</span><span class="sxs-lookup"><span data-stu-id="9073f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9073f-116">親要素</span><span class="sxs-lookup"><span data-stu-id="9073f-116">Parent elements</span></span>

|<span data-ttu-id="9073f-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="9073f-117">**Element**</span></span>|<span data-ttu-id="9073f-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="9073f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9073f-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9073f-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="9073f-120">1 つの組織の組織との関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="9073f-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9073f-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9073f-121">Text value</span></span>

<span data-ttu-id="9073f-122">DeliveryReportEnabled 要素のテキスト値は、組織内のユーザーからの配信レポートを使用できることを示します。</span><span class="sxs-lookup"><span data-stu-id="9073f-122">A text value of true for the DeliveryReportEnabled element indicates that the delivery reports from users in the organization can be used.</span></span> <span data-ttu-id="9073f-123">False の値は、配信レポートを抑制する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="9073f-123">A value of false indicates that the delivery reports should suppressed.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9073f-124">備考</span><span class="sxs-lookup"><span data-stu-id="9073f-124">Remarks</span></span>

<span data-ttu-id="9073f-125">許可またはサーバーからの配信レポートを抑制するには、この要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="9073f-125">Use this element to allow or suppress delivery reports from the server.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9073f-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="9073f-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9073f-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="9073f-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="9073f-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9073f-128">Schema Name</span></span>  <br/> |<span data-ttu-id="9073f-129">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="9073f-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="9073f-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9073f-130">Validation File</span></span>  <br/> |<span data-ttu-id="9073f-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9073f-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9073f-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9073f-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="9073f-133">True</span><span class="sxs-lookup"><span data-stu-id="9073f-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9073f-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="9073f-134">See also</span></span>

- [<span data-ttu-id="9073f-135">GetOrganizationRelationshipSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9073f-135">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)


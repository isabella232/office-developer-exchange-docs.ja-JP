---
title: DeliveryReportEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ab522bc-40ea-4e43-aa57-6d2562db35e9
description: DeliveryReportEnabled 要素は、DeliveryReportEnabled () フラグを表します。 DeliveryReportEnabled 要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: 2a163b3e6ceaa169cc8f76f395b7d501419a31ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458475"
---
# <a name="deliveryreportenabled-soap"></a><span data-ttu-id="d4126-105">DeliveryReportEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4126-105">DeliveryReportEnabled (SOAP)</span></span>

<span data-ttu-id="d4126-106">**Deliveryreportenabled**要素は、 **deliveryreportenabled ()** フラグを表します。</span><span class="sxs-lookup"><span data-stu-id="d4126-106">The **DeliveryReportEnabled** element represents the **DeliveryReportEnabled()** flag.</span></span> <span data-ttu-id="d4126-107">**Deliveryreportenabled**要素は、内部使用のみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="d4126-107">The **DeliveryReportEnabled** element is for internal use only.</span></span> <span data-ttu-id="d4126-108">この要素はクライアントによって使用されません。</span><span class="sxs-lookup"><span data-stu-id="d4126-108">This element is not used by clients.</span></span> 
  
```XML
<DeliveryReportEnabled>true | false</DeliveryReportEnabled>
```

 <span data-ttu-id="d4126-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d4126-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4126-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d4126-110">Attributes and elements</span></span>

<span data-ttu-id="d4126-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d4126-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4126-112">属性</span><span class="sxs-lookup"><span data-stu-id="d4126-112">Attributes</span></span>

<span data-ttu-id="d4126-113">なし。</span><span class="sxs-lookup"><span data-stu-id="d4126-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4126-114">子要素</span><span class="sxs-lookup"><span data-stu-id="d4126-114">Child elements</span></span>

<span data-ttu-id="d4126-115">なし。</span><span class="sxs-lookup"><span data-stu-id="d4126-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d4126-116">親要素</span><span class="sxs-lookup"><span data-stu-id="d4126-116">Parent elements</span></span>

|<span data-ttu-id="d4126-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="d4126-117">**Element**</span></span>|<span data-ttu-id="d4126-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="d4126-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4126-119">組織のリレーションシップ設定 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4126-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="d4126-120">1つの組織の組織上の関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="d4126-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d4126-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d4126-121">Text value</span></span>

<span data-ttu-id="d4126-122">DeliveryReportEnabled 要素のテキスト値が true の場合は、組織内のユーザーからの配信レポートを使用できることを示します。</span><span class="sxs-lookup"><span data-stu-id="d4126-122">A text value of true for the DeliveryReportEnabled element indicates that the delivery reports from users in the organization can be used.</span></span> <span data-ttu-id="d4126-123">値が false の場合は、配信レポートを抑制する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="d4126-123">A value of false indicates that the delivery reports should suppressed.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d4126-124">注釈</span><span class="sxs-lookup"><span data-stu-id="d4126-124">Remarks</span></span>

<span data-ttu-id="d4126-125">この要素を使用して、サーバーからの配信レポートを許可または抑制します。</span><span class="sxs-lookup"><span data-stu-id="d4126-125">Use this element to allow or suppress delivery reports from the server.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4126-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d4126-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4126-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="d4126-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d4126-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d4126-128">Schema Name</span></span>  <br/> |<span data-ttu-id="d4126-129">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="d4126-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d4126-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d4126-130">Validation File</span></span>  <br/> |<span data-ttu-id="d4126-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d4126-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d4126-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d4126-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4126-133">正しい</span><span class="sxs-lookup"><span data-stu-id="d4126-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4126-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="d4126-134">See also</span></span>

- [<span data-ttu-id="d4126-135">Get組織の Relationshipsettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4126-135">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)


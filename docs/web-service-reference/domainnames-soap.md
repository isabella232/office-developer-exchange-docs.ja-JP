---
title: DomainNames (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 79ffc3f9-25c4-40b5-84ce-09a3c5f892fa
description: DomainNames 要素は、ドメイン名のコレクションを表します。 DomainNames 要素では、内部でのみ使用します。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: 45d256f3d5a57028a04572ad67d4be0786ca39e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760147"
---
# <a name="domainnames-soap"></a><span data-ttu-id="efaf3-105">DomainNames (SOAP)</span><span class="sxs-lookup"><span data-stu-id="efaf3-105">DomainNames (SOAP)</span></span>

<span data-ttu-id="efaf3-106">**DomainNames**要素は、ドメイン名のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="efaf3-106">The **DomainNames** element represents the domain names collection.</span></span> <span data-ttu-id="efaf3-107">**DomainNames**要素では、内部でのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="efaf3-107">The **DomainNames** element is for internal use only.</span></span> <span data-ttu-id="efaf3-108">クライアントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="efaf3-108">This element is not used by clients.</span></span> 
  
```XML
<DomainNames>
    <Domains/>
</DomainNames>
```

 <span data-ttu-id="efaf3-109">**DomainNames**</span><span class="sxs-lookup"><span data-stu-id="efaf3-109">**DomainNames**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="efaf3-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="efaf3-110">Attributes and elements</span></span>

<span data-ttu-id="efaf3-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="efaf3-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="efaf3-112">属性</span><span class="sxs-lookup"><span data-stu-id="efaf3-112">Attributes</span></span>

<span data-ttu-id="efaf3-113">なし。</span><span class="sxs-lookup"><span data-stu-id="efaf3-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="efaf3-114">子要素</span><span class="sxs-lookup"><span data-stu-id="efaf3-114">Child elements</span></span>

|<span data-ttu-id="efaf3-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="efaf3-115">**Element**</span></span>|<span data-ttu-id="efaf3-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="efaf3-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="efaf3-117">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="efaf3-117">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="efaf3-118">[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)、 [GetFederationInformation の操作 (SOAP)](getfederationinformation-operation-soap.md)、または[GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)から返されるドメインのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="efaf3-118">Represents a collection of domains that are returned from the [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md), or the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="efaf3-119">親要素</span><span class="sxs-lookup"><span data-stu-id="efaf3-119">Parent elements</span></span>

|<span data-ttu-id="efaf3-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="efaf3-120">**Element**</span></span>|<span data-ttu-id="efaf3-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="efaf3-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="efaf3-122">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="efaf3-122">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="efaf3-123">1 つの組織の組織との関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="efaf3-123">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="efaf3-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="efaf3-124">Text value</span></span>

<span data-ttu-id="efaf3-125">なし。</span><span class="sxs-lookup"><span data-stu-id="efaf3-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="efaf3-126">備考</span><span class="sxs-lookup"><span data-stu-id="efaf3-126">Remarks</span></span>

<span data-ttu-id="efaf3-127">この要素は、外部の組織の SMTP ドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="efaf3-127">This element represents the SMTP domains of the external organizations.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="efaf3-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="efaf3-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="efaf3-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="efaf3-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="efaf3-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="efaf3-130">Schema Name</span></span>  <br/> |<span data-ttu-id="efaf3-131">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="efaf3-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="efaf3-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="efaf3-132">Validation File</span></span>  <br/> |<span data-ttu-id="efaf3-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="efaf3-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="efaf3-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="efaf3-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="efaf3-135">True</span><span class="sxs-lookup"><span data-stu-id="efaf3-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="efaf3-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="efaf3-136">See also</span></span>

- [<span data-ttu-id="efaf3-137">GetOrganizationRelationshipSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="efaf3-137">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)


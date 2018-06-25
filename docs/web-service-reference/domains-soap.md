---
title: ドメイン (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5f81d1b7-c6a4-456f-9935-13d04a3d92d7
description: ドメイン要素は、GetDomainSettings 操作 (SOAP)、(SOAP)、GetFederationInformation の操作で、組織がフェデレーションには、ドメインまたは組織と関係を持つドメインで返されるドメインのコレクションを表しますGetOrganizationRelationshipSettings 操作 (SOAP) によって返されます。
ms.openlocfilehash: 7a21a3a09516de2d1c38021ca3ccd2161d9cdd1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760156"
---
# <a name="domains-soap"></a><span data-ttu-id="e7e78-103">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e7e78-103">Domains (SOAP)</span></span>

<span data-ttu-id="e7e78-104">**ドメイン**要素は、 [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)、組織は、 [GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)でフェデレーション ドメインまたはドメインに返されるドメインのコレクションを表しますが組織の関係[(SOAP) の GetOrganizationRelationshipSettings 操作](getorganizationrelationshipsettings-operation-soap.md)によって返される。</span><span class="sxs-lookup"><span data-stu-id="e7e78-104">The **Domains** element represents the domain collection that is returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), the domains that the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md), or the domains with an organization relationship as returned by [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span></span>
  
```XML
<Domains>
   <Domain/>
</Domains>
```

 <span data-ttu-id="e7e78-105">**ドメイン**</span><span class="sxs-lookup"><span data-stu-id="e7e78-105">**Domains**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7e78-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e7e78-106">Attributes and elements</span></span>

<span data-ttu-id="e7e78-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e7e78-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7e78-108">属性</span><span class="sxs-lookup"><span data-stu-id="e7e78-108">Attributes</span></span>

<span data-ttu-id="e7e78-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e7e78-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e7e78-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e7e78-110">Child elements</span></span>

|<span data-ttu-id="e7e78-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="e7e78-111">**Element**</span></span>|<span data-ttu-id="e7e78-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e7e78-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7e78-113">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e7e78-113">Domain (SOAP)</span></span>](domain-soap.md) <br/> |<span data-ttu-id="e7e78-114">1 つのドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="e7e78-114">Represents a single domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e7e78-115">親要素</span><span class="sxs-lookup"><span data-stu-id="e7e78-115">Parent elements</span></span>

|<span data-ttu-id="e7e78-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="e7e78-116">**Element**</span></span>|<span data-ttu-id="e7e78-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="e7e78-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7e78-118">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e7e78-118">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md) <br/> |<span data-ttu-id="e7e78-119">[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)要求を表します。</span><span class="sxs-lookup"><span data-stu-id="e7e78-119">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="e7e78-120">応答 (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e7e78-120">Response (GetFederationInformation) (SOAP)</span></span>](response-getfederationinformationsoap.md) <br/> |<span data-ttu-id="e7e78-121">[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)応答の情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e7e78-121">Contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response information.</span></span>  <br/> |
|[<span data-ttu-id="e7e78-122">GetOrganizationRelationshipSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e7e78-122">GetOrganizationRelationshipSettingsRequest (SOAP)</span></span>](getorganizationrelationshipsettingsrequest-soap.md) <br/> |<span data-ttu-id="e7e78-123">[GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)要求を表します。</span><span class="sxs-lookup"><span data-stu-id="e7e78-123">Represents a [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e7e78-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e7e78-124">Text value</span></span>

<span data-ttu-id="e7e78-125">なし。</span><span class="sxs-lookup"><span data-stu-id="e7e78-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7e78-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="e7e78-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7e78-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="e7e78-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="e7e78-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e7e78-128">Schema Name</span></span>  <br/> |<span data-ttu-id="e7e78-129">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="e7e78-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="e7e78-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e7e78-130">Validation File</span></span>  <br/> |<span data-ttu-id="e7e78-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e7e78-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e7e78-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e7e78-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="e7e78-133">True</span><span class="sxs-lookup"><span data-stu-id="e7e78-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e7e78-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="e7e78-134">See also</span></span>

- [<span data-ttu-id="e7e78-135">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e7e78-135">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md)  
- [<span data-ttu-id="e7e78-136">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e7e78-136">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md)


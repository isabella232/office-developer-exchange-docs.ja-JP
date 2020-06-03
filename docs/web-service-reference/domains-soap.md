---
title: Domains (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5f81d1b7-c6a4-456f-9935-13d04a3d92d7
description: Domains 要素は、GetDomainSettings 操作 (SOAP) で返されるドメインコレクション、組織が GetFederationInformation 操作 (SOAP) に対してフェデレーションされているドメイン、または Getruleaction Relationshipsettings 操作 (SOAP) によって返される組織上の関係を持つドメインに相当します。
ms.openlocfilehash: c56fb72841776c0060c1300b52b2f6a06b1ec0ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526306"
---
# <a name="domains-soap"></a><span data-ttu-id="7d57e-103">Domains (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7d57e-103">Domains (SOAP)</span></span>

<span data-ttu-id="7d57e-104">**Domains**要素は、 [getdomainsettings 操作 (soap)](getdomainsettings-operation-soap.md)で返されるドメインコレクション、組織が[GetFederationInformation 操作 (soap)](getfederationinformation-operation-soap.md)に対してフェデレーションされているドメイン、または[getruleaction relationshipsettings 操作 (soap)](getorganizationrelationshipsettings-operation-soap.md)によって返される組織上の関係を持つドメインに相当します。</span><span class="sxs-lookup"><span data-stu-id="7d57e-104">The **Domains** element represents the domain collection that is returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), the domains that the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md), or the domains with an organization relationship as returned by [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span></span>
  
```XML
<Domains>
   <Domain/>
</Domains>
```

 <span data-ttu-id="7d57e-105">**ドメイン**</span><span class="sxs-lookup"><span data-stu-id="7d57e-105">**Domains**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7d57e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7d57e-106">Attributes and elements</span></span>

<span data-ttu-id="7d57e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7d57e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d57e-108">属性</span><span class="sxs-lookup"><span data-stu-id="7d57e-108">Attributes</span></span>

<span data-ttu-id="7d57e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7d57e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d57e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7d57e-110">Child elements</span></span>

|<span data-ttu-id="7d57e-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="7d57e-111">**Element**</span></span>|<span data-ttu-id="7d57e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7d57e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d57e-113">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7d57e-113">Domain (SOAP)</span></span>](domain-soap.md) <br/> |<span data-ttu-id="7d57e-114">単一のドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="7d57e-114">Represents a single domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7d57e-115">親要素</span><span class="sxs-lookup"><span data-stu-id="7d57e-115">Parent elements</span></span>

|<span data-ttu-id="7d57e-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="7d57e-116">**Element**</span></span>|<span data-ttu-id="7d57e-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="7d57e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d57e-118">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7d57e-118">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md) <br/> |<span data-ttu-id="7d57e-119">[Getdomainsettings 操作 (SOAP)](getdomainsettings-operation-soap.md)要求を表します。</span><span class="sxs-lookup"><span data-stu-id="7d57e-119">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="7d57e-120">Response (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7d57e-120">Response (GetFederationInformation) (SOAP)</span></span>](response-getfederationinformationsoap.md) <br/> |<span data-ttu-id="7d57e-121">[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)応答情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="7d57e-121">Contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response information.</span></span>  <br/> |
|[<span data-ttu-id="7d57e-122">Get組織の Relationshipsettingsrequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7d57e-122">GetOrganizationRelationshipSettingsRequest (SOAP)</span></span>](getorganizationrelationshipsettingsrequest-soap.md) <br/> |<span data-ttu-id="7d57e-123">[Get組織の設定操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)要求を表します。</span><span class="sxs-lookup"><span data-stu-id="7d57e-123">Represents a [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7d57e-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7d57e-124">Text value</span></span>

<span data-ttu-id="7d57e-125">なし。</span><span class="sxs-lookup"><span data-stu-id="7d57e-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d57e-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7d57e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d57e-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="7d57e-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="7d57e-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7d57e-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7d57e-129">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="7d57e-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="7d57e-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7d57e-130">Validation File</span></span>  <br/> |<span data-ttu-id="7d57e-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7d57e-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7d57e-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7d57e-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7d57e-133">正しい</span><span class="sxs-lookup"><span data-stu-id="7d57e-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d57e-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="7d57e-134">See also</span></span>

- [<span data-ttu-id="7d57e-135">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7d57e-135">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md)  
- [<span data-ttu-id="7d57e-136">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7d57e-136">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md)


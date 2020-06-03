---
title: DomainNames (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 79ffc3f9-25c4-40b5-84ce-09a3c5f892fa
description: DomainNames 要素は、ドメイン名のコレクションを表します。 DomainNames 要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: 0b425b3cd4c0e7cb2427920d61feb04010a3b123
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458419"
---
# <a name="domainnames-soap"></a><span data-ttu-id="c9be5-105">DomainNames (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c9be5-105">DomainNames (SOAP)</span></span>

<span data-ttu-id="c9be5-106">**Domainnames**要素は、ドメイン名のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="c9be5-106">The **DomainNames** element represents the domain names collection.</span></span> <span data-ttu-id="c9be5-107">**Domainnames**要素は、内部使用のみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="c9be5-107">The **DomainNames** element is for internal use only.</span></span> <span data-ttu-id="c9be5-108">この要素はクライアントによって使用されません。</span><span class="sxs-lookup"><span data-stu-id="c9be5-108">This element is not used by clients.</span></span> 
  
```XML
<DomainNames>
    <Domains/>
</DomainNames>
```

 <span data-ttu-id="c9be5-109">**DomainNames**</span><span class="sxs-lookup"><span data-stu-id="c9be5-109">**DomainNames**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9be5-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c9be5-110">Attributes and elements</span></span>

<span data-ttu-id="c9be5-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c9be5-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9be5-112">属性</span><span class="sxs-lookup"><span data-stu-id="c9be5-112">Attributes</span></span>

<span data-ttu-id="c9be5-113">なし。</span><span class="sxs-lookup"><span data-stu-id="c9be5-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9be5-114">子要素</span><span class="sxs-lookup"><span data-stu-id="c9be5-114">Child elements</span></span>

|<span data-ttu-id="c9be5-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="c9be5-115">**Element**</span></span>|<span data-ttu-id="c9be5-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="c9be5-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9be5-117">Domains (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c9be5-117">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="c9be5-118">[Getdomainsettings 操作 (soap](getdomainsettings-operation-soap.md))、 [GETFEDERATIONINFORMATION operation (soap)](getfederationinformation-operation-soap.md)、または[getruleaction relationshipsettings 操作 (soap)](getorganizationrelationshipsettings-operation-soap.md)から返されるドメインのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="c9be5-118">Represents a collection of domains that are returned from the [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md), or the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c9be5-119">親要素</span><span class="sxs-lookup"><span data-stu-id="c9be5-119">Parent elements</span></span>

|<span data-ttu-id="c9be5-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="c9be5-120">**Element**</span></span>|<span data-ttu-id="c9be5-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="c9be5-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9be5-122">組織のリレーションシップ設定 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c9be5-122">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="c9be5-123">1つの組織の組織上の関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="c9be5-123">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c9be5-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c9be5-124">Text value</span></span>

<span data-ttu-id="c9be5-125">なし。</span><span class="sxs-lookup"><span data-stu-id="c9be5-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c9be5-126">注釈</span><span class="sxs-lookup"><span data-stu-id="c9be5-126">Remarks</span></span>

<span data-ttu-id="c9be5-127">この要素は、外部組織の SMTP ドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="c9be5-127">This element represents the SMTP domains of the external organizations.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9be5-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c9be5-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9be5-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="c9be5-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="c9be5-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c9be5-130">Schema Name</span></span>  <br/> |<span data-ttu-id="c9be5-131">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="c9be5-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="c9be5-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c9be5-132">Validation File</span></span>  <br/> |<span data-ttu-id="c9be5-133">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c9be5-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c9be5-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c9be5-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="c9be5-135">正しい</span><span class="sxs-lookup"><span data-stu-id="c9be5-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9be5-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="c9be5-136">See also</span></span>

- [<span data-ttu-id="c9be5-137">Get組織の Relationshipsettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c9be5-137">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)


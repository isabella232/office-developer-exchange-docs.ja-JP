---
title: 要求 (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 3ea026fc-74f1-4118-86ae-908ed4f82a4b
description: 要求要素には、ドメインの設定を取得する要求が含まれています。
ms.openlocfilehash: 71a6072d476fd665dad8b0c0fe388a40db56e059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833135"
---
# <a name="request-getdomainsettings-soap"></a><span data-ttu-id="1a723-103">要求 (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1a723-103">Request (GetDomainSettings) (SOAP)</span></span>

<span data-ttu-id="1a723-104">**要求**要素には、ドメインの設定を取得する要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1a723-104">The **Request** element contains a request to return domain settings.</span></span> 
  
```xml
<Request>
   <Domains/>
   <RequestedSettings/>
</Request>
```

 <span data-ttu-id="1a723-105">**GetDomainSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="1a723-105">**GetDomainSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a723-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1a723-106">Attributes and elements</span></span>

<span data-ttu-id="1a723-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1a723-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a723-108">属性</span><span class="sxs-lookup"><span data-stu-id="1a723-108">Attributes</span></span>

<span data-ttu-id="1a723-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1a723-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a723-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1a723-110">Child elements</span></span>

|<span data-ttu-id="1a723-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="1a723-111">**Element**</span></span>|<span data-ttu-id="1a723-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1a723-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a723-113">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1a723-113">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="1a723-114">構成が[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)で返されるドメインまたは組織は、 [GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)でフェデレーション ドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="1a723-114">Represents the domains the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) or the domains the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md).</span></span>  <br/> |
|[<span data-ttu-id="1a723-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1a723-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="1a723-116">要求された構成設定の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1a723-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1a723-117">親要素</span><span class="sxs-lookup"><span data-stu-id="1a723-117">Parent elements</span></span>

|<span data-ttu-id="1a723-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="1a723-118">**Element**</span></span>|<span data-ttu-id="1a723-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="1a723-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a723-120">GetDomainSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1a723-120">GetDomainSettingsRequestMessage (SOAP)</span></span>](getdomainsettingsrequestmessage-soap.md) <br/> |<span data-ttu-id="1a723-121">[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)要求を表します。</span><span class="sxs-lookup"><span data-stu-id="1a723-121">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md)request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1a723-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1a723-122">Text value</span></span>

<span data-ttu-id="1a723-123">なし。</span><span class="sxs-lookup"><span data-stu-id="1a723-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a723-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="1a723-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a723-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="1a723-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="1a723-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1a723-126">Schema Name</span></span>  <br/> |<span data-ttu-id="1a723-127">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="1a723-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="1a723-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1a723-128">Validation File</span></span>  <br/> |<span data-ttu-id="1a723-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1a723-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1a723-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1a723-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="1a723-131">True</span><span class="sxs-lookup"><span data-stu-id="1a723-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a723-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="1a723-132">See also</span></span>



[<span data-ttu-id="1a723-133">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1a723-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)


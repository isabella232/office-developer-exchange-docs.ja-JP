---
title: DomainResponses (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: d9c7fd91-22cd-4c72-a841-25cb9d415e0c
description: DomainResponses 要素には、要求された各ドメインの設定の応答の配列が含まれています。
ms.openlocfilehash: 77a3efc1605337ab436f6aea2b61a67f22e4f8ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760155"
---
# <a name="domainresponses-soap"></a><span data-ttu-id="76a8c-103">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="76a8c-103">DomainResponses (SOAP)</span></span>

<span data-ttu-id="76a8c-104">**DomainResponses**要素には、要求された各ドメインの設定の応答の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="76a8c-104">The **DomainResponses** element contains an array of responses for each requested domain's settings.</span></span> 
  
```XML
<DomainResponses>
   <DomainResponse/>
</DomainResponses>
```

 <span data-ttu-id="76a8c-105">**ArrayOfDomainResponse**</span><span class="sxs-lookup"><span data-stu-id="76a8c-105">**ArrayOfDomainResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="76a8c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="76a8c-106">Attributes and elements</span></span>

<span data-ttu-id="76a8c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="76a8c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76a8c-108">属性</span><span class="sxs-lookup"><span data-stu-id="76a8c-108">Attributes</span></span>

<span data-ttu-id="76a8c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="76a8c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="76a8c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="76a8c-110">Child elements</span></span>

|<span data-ttu-id="76a8c-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="76a8c-111">**Element**</span></span>|<span data-ttu-id="76a8c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="76a8c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76a8c-113">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="76a8c-113">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="76a8c-114">指定したドメインの指定された設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="76a8c-114">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="76a8c-115">親要素</span><span class="sxs-lookup"><span data-stu-id="76a8c-115">Parent elements</span></span>

|<span data-ttu-id="76a8c-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="76a8c-116">**Element**</span></span>|<span data-ttu-id="76a8c-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="76a8c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76a8c-118">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="76a8c-118">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="76a8c-119">ドメインの[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)要求への応答を表し、ドメインの設定を返します。</span><span class="sxs-lookup"><span data-stu-id="76a8c-119">Represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request for a domain, and returns the domain settings.</span></span>  <br/> |
|[<span data-ttu-id="76a8c-120">応答 (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="76a8c-120">Response (GetDomainSettings) (SOAP)</span></span>](response-getdomainsettingssoap.md) <br/> |<span data-ttu-id="76a8c-121">個々 のドメインの[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)呼び出しへの応答を表します。</span><span class="sxs-lookup"><span data-stu-id="76a8c-121">Represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="76a8c-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="76a8c-122">Text value</span></span>

<span data-ttu-id="76a8c-123">なし。</span><span class="sxs-lookup"><span data-stu-id="76a8c-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76a8c-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="76a8c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76a8c-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="76a8c-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="76a8c-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="76a8c-126">Schema Name</span></span>  <br/> |<span data-ttu-id="76a8c-127">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="76a8c-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="76a8c-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="76a8c-128">Validation File</span></span>  <br/> |<span data-ttu-id="76a8c-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="76a8c-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="76a8c-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="76a8c-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="76a8c-131">True</span><span class="sxs-lookup"><span data-stu-id="76a8c-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76a8c-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="76a8c-132">See also</span></span>

- [<span data-ttu-id="76a8c-133">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="76a8c-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)


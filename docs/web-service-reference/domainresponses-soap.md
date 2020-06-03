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
description: DomainResponses 要素には、要求された各ドメインの設定に対する応答の配列が含まれています。
ms.openlocfilehash: 2c76b9691fe88657a65130ef6829e5af64380d95
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526320"
---
# <a name="domainresponses-soap"></a><span data-ttu-id="20b4f-103">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="20b4f-103">DomainResponses (SOAP)</span></span>

<span data-ttu-id="20b4f-104">**Domainresponses**要素には、要求された各ドメインの設定に対する応答の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="20b4f-104">The **DomainResponses** element contains an array of responses for each requested domain's settings.</span></span> 
  
```XML
<DomainResponses>
   <DomainResponse/>
</DomainResponses>
```

 <span data-ttu-id="20b4f-105">**ArrayOfDomainResponse**</span><span class="sxs-lookup"><span data-stu-id="20b4f-105">**ArrayOfDomainResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20b4f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="20b4f-106">Attributes and elements</span></span>

<span data-ttu-id="20b4f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="20b4f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20b4f-108">属性</span><span class="sxs-lookup"><span data-stu-id="20b4f-108">Attributes</span></span>

<span data-ttu-id="20b4f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="20b4f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20b4f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="20b4f-110">Child elements</span></span>

|<span data-ttu-id="20b4f-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="20b4f-111">**Element**</span></span>|<span data-ttu-id="20b4f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="20b4f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20b4f-113">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="20b4f-113">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="20b4f-114">指定したドメインに対して要求された設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="20b4f-114">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="20b4f-115">親要素</span><span class="sxs-lookup"><span data-stu-id="20b4f-115">Parent elements</span></span>

|<span data-ttu-id="20b4f-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="20b4f-116">**Element**</span></span>|<span data-ttu-id="20b4f-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="20b4f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20b4f-118">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="20b4f-118">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="20b4f-119">ドメインの[Getdomainsettings operation (SOAP)](getdomainsettings-operation-soap.md)要求に対する応答を表し、ドメインの設定を返します。</span><span class="sxs-lookup"><span data-stu-id="20b4f-119">Represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request for a domain, and returns the domain settings.</span></span>  <br/> |
|[<span data-ttu-id="20b4f-120">Response (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="20b4f-120">Response (GetDomainSettings) (SOAP)</span></span>](response-getdomainsettingssoap.md) <br/> |<span data-ttu-id="20b4f-121">個々のドメインに対する[Getdomainsettings operation (SOAP)](getdomainsettings-operation-soap.md)呼び出しへの応答を表します。</span><span class="sxs-lookup"><span data-stu-id="20b4f-121">Represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="20b4f-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="20b4f-122">Text value</span></span>

<span data-ttu-id="20b4f-123">なし。</span><span class="sxs-lookup"><span data-stu-id="20b4f-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20b4f-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="20b4f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20b4f-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="20b4f-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="20b4f-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="20b4f-126">Schema Name</span></span>  <br/> |<span data-ttu-id="20b4f-127">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="20b4f-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="20b4f-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="20b4f-128">Validation File</span></span>  <br/> |<span data-ttu-id="20b4f-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="20b4f-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="20b4f-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="20b4f-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="20b4f-131">正しい</span><span class="sxs-lookup"><span data-stu-id="20b4f-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="20b4f-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="20b4f-132">See also</span></span>

- [<span data-ttu-id="20b4f-133">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="20b4f-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)


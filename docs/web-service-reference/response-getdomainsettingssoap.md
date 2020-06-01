---
title: Response (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a5b052df-93bd-4fe1-ac30-83de9a3dfcd7
description: Response 要素は、個々のドメインに対する GetDomainSettings 呼び出しへの応答を表します。
ms.openlocfilehash: 67fe7aea4533058fa0df972e49a2069749dc258b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455584"
---
# <a name="response-getdomainsettings-soap"></a><span data-ttu-id="92dbe-103">Response (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="92dbe-103">Response (GetDomainSettings) (SOAP)</span></span>

<span data-ttu-id="92dbe-104">**Response**要素は、個々のドメインに対する**getdomainsettings**呼び出しへの応答を表します。</span><span class="sxs-lookup"><span data-stu-id="92dbe-104">The **Response** element represents the response to a **GetDomainSettings** call for an individual domain.</span></span> 
  
```XML
<Response>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</Response>
```

 <span data-ttu-id="92dbe-105">**GetDomainSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="92dbe-105">**GetDomainSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92dbe-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="92dbe-106">Attributes and elements</span></span>

<span data-ttu-id="92dbe-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="92dbe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92dbe-108">属性</span><span class="sxs-lookup"><span data-stu-id="92dbe-108">Attributes</span></span>

<span data-ttu-id="92dbe-109">なし。</span><span class="sxs-lookup"><span data-stu-id="92dbe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="92dbe-110">子要素</span><span class="sxs-lookup"><span data-stu-id="92dbe-110">Child elements</span></span>

|<span data-ttu-id="92dbe-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="92dbe-111">**Element**</span></span>|<span data-ttu-id="92dbe-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="92dbe-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92dbe-113">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="92dbe-113">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="92dbe-114">**Getdomainsettings**要求で要求された各ドメインに対する応答を含みます。</span><span class="sxs-lookup"><span data-stu-id="92dbe-114">Contains the response for each domain requested in a **GetDomainSettings** request.</span></span>  <br/> |
|[<span data-ttu-id="92dbe-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="92dbe-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="92dbe-116">応答に関連付けられているエラーコードが含まれます (該当する場合)。</span><span class="sxs-lookup"><span data-stu-id="92dbe-116">Contains the error code that is associated with the response, if applicable.</span></span>  <br/> |
|[<span data-ttu-id="92dbe-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="92dbe-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="92dbe-118">応答に関連付けられているエラーメッセージ (該当する場合) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="92dbe-118">Contains the error message that is associated with the response, if applicable.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="92dbe-119">親要素</span><span class="sxs-lookup"><span data-stu-id="92dbe-119">Parent elements</span></span>

|<span data-ttu-id="92dbe-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="92dbe-120">**Element**</span></span>|<span data-ttu-id="92dbe-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="92dbe-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92dbe-122">GetDomainSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="92dbe-122">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="92dbe-123">発信者にドメインの構成設定を返します。</span><span class="sxs-lookup"><span data-stu-id="92dbe-123">Returns to the caller the domain configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="92dbe-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="92dbe-124">Text value</span></span>

<span data-ttu-id="92dbe-125">なし。</span><span class="sxs-lookup"><span data-stu-id="92dbe-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92dbe-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="92dbe-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92dbe-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="92dbe-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="92dbe-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="92dbe-128">Schema Name</span></span>  <br/> |<span data-ttu-id="92dbe-129">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="92dbe-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="92dbe-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="92dbe-130">Validation File</span></span>  <br/> |<span data-ttu-id="92dbe-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="92dbe-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="92dbe-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="92dbe-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="92dbe-133">正しい</span><span class="sxs-lookup"><span data-stu-id="92dbe-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92dbe-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="92dbe-134">See also</span></span>



[<span data-ttu-id="92dbe-135">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="92dbe-135">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)


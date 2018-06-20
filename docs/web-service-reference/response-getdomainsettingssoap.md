---
title: 応答 (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a5b052df-93bd-4fe1-ac30-83de9a3dfcd7
description: 応答要素は、個々 のドメインの GetDomainSettings 呼び出しへの応答を表します。
ms.openlocfilehash: 316d77104894cf5ed9121e7dab1c38646765c948
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833169"
---
# <a name="response-getdomainsettings-soap"></a><span data-ttu-id="5a272-103">応答 (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5a272-103">Response (GetDomainSettings) (SOAP)</span></span>

<span data-ttu-id="5a272-104">**応答**要素は、個々 のドメインの**GetDomainSettings**呼び出しへの応答を表します。</span><span class="sxs-lookup"><span data-stu-id="5a272-104">The **Response** element represents the response to a **GetDomainSettings** call for an individual domain.</span></span> 
  
```XML
<Response>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</Response>
```

 <span data-ttu-id="5a272-105">**GetDomainSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="5a272-105">**GetDomainSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a272-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5a272-106">Attributes and elements</span></span>

<span data-ttu-id="5a272-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5a272-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a272-108">属性</span><span class="sxs-lookup"><span data-stu-id="5a272-108">Attributes</span></span>

<span data-ttu-id="5a272-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5a272-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a272-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5a272-110">Child elements</span></span>

|<span data-ttu-id="5a272-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="5a272-111">**Element**</span></span>|<span data-ttu-id="5a272-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5a272-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a272-113">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5a272-113">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="5a272-114">**GetDomainSettings**要求で要求された各ドメインへの応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a272-114">Contains the response for each domain requested in a **GetDomainSettings** request.</span></span>  <br/> |
|[<span data-ttu-id="5a272-115">エラー コード (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5a272-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="5a272-116">該当する場合、応答に関連付けられているエラー コードが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a272-116">Contains the error code that is associated with the response, if applicable.</span></span>  <br/> |
|[<span data-ttu-id="5a272-117">エラー メッセージ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5a272-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="5a272-118">該当する場合、応答に関連付けられているエラー メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a272-118">Contains the error message that is associated with the response, if applicable.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5a272-119">親要素</span><span class="sxs-lookup"><span data-stu-id="5a272-119">Parent elements</span></span>

|<span data-ttu-id="5a272-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="5a272-120">**Element**</span></span>|<span data-ttu-id="5a272-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="5a272-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a272-122">GetDomainSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5a272-122">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="5a272-123">呼び出し元に、ドメイン構成設定を返します。</span><span class="sxs-lookup"><span data-stu-id="5a272-123">Returns to the caller the domain configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5a272-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5a272-124">Text value</span></span>

<span data-ttu-id="5a272-125">なし。</span><span class="sxs-lookup"><span data-stu-id="5a272-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a272-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="5a272-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a272-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="5a272-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="5a272-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5a272-128">Schema Name</span></span>  <br/> |<span data-ttu-id="5a272-129">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="5a272-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="5a272-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5a272-130">Validation File</span></span>  <br/> |<span data-ttu-id="5a272-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5a272-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5a272-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5a272-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="5a272-133">True</span><span class="sxs-lookup"><span data-stu-id="5a272-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a272-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="5a272-134">See also</span></span>



[<span data-ttu-id="5a272-135">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5a272-135">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)


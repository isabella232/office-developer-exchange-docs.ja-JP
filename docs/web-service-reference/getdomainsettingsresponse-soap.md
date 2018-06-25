---
title: GetDomainSettingsResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 43ebd17b-3a70-4878-9254-97a4c2c87b77
description: GetDomainSettingsResponse 要素は、ドメインの設定を返す GetDomainSettings 操作 (SOAP) への応答を表します。
ms.openlocfilehash: c4984c2c6c532fcbd45c1a75733e578f6d9491fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760700"
---
# <a name="getdomainsettingsresponse-soap"></a><span data-ttu-id="3ea6e-103">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3ea6e-103">GetDomainSettingsResponse (SOAP)</span></span>

<span data-ttu-id="3ea6e-104">**GetDomainSettingsResponse**要素は、 [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)、ドメインの設定を返す応答を表します。</span><span class="sxs-lookup"><span data-stu-id="3ea6e-104">The **GetDomainSettingsResponse** element represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), which returns the domain settings.</span></span>
  
```XML
<GetDomainSettingsResponse>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</GetDomainSettingsResponse>
```

 <span data-ttu-id="3ea6e-105">**GetDomainSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="3ea6e-105">**GetDomainSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3ea6e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3ea6e-106">Attributes and elements</span></span>

<span data-ttu-id="3ea6e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3ea6e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3ea6e-108">属性</span><span class="sxs-lookup"><span data-stu-id="3ea6e-108">Attributes</span></span>

<span data-ttu-id="3ea6e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3ea6e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3ea6e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3ea6e-110">Child elements</span></span>

|<span data-ttu-id="3ea6e-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="3ea6e-111">**Element**</span></span>|<span data-ttu-id="3ea6e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3ea6e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3ea6e-113">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3ea6e-113">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="3ea6e-114">要求された各ドメインの設定の応答の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3ea6e-114">Contains an array of responses for each requested domain's settings.</span></span>  <br/> |
|[<span data-ttu-id="3ea6e-115">エラー コード (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3ea6e-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="3ea6e-116">自動検出サービスによって返されるエラー コードを表します。</span><span class="sxs-lookup"><span data-stu-id="3ea6e-116">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="3ea6e-117">エラー メッセージ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3ea6e-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="3ea6e-118">自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="3ea6e-118">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3ea6e-119">親要素</span><span class="sxs-lookup"><span data-stu-id="3ea6e-119">Parent elements</span></span>

<span data-ttu-id="3ea6e-120">なし。</span><span class="sxs-lookup"><span data-stu-id="3ea6e-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3ea6e-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3ea6e-121">Text value</span></span>

<span data-ttu-id="3ea6e-122">なし。</span><span class="sxs-lookup"><span data-stu-id="3ea6e-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3ea6e-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="3ea6e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3ea6e-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="3ea6e-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="3ea6e-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3ea6e-125">Schema Name</span></span>  <br/> |<span data-ttu-id="3ea6e-126">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="3ea6e-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="3ea6e-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3ea6e-127">Validation File</span></span>  <br/> |<span data-ttu-id="3ea6e-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3ea6e-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3ea6e-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3ea6e-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="3ea6e-130">True</span><span class="sxs-lookup"><span data-stu-id="3ea6e-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3ea6e-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="3ea6e-131">See also</span></span>



[<span data-ttu-id="3ea6e-132">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3ea6e-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)


---
title: Response (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ca48a4b3-5006-4bb7-973e-d9137ce67e16
description: Response 要素には、GetFederationInformation operation (SOAP) 応答情報が含まれています。
ms.openlocfilehash: 0b9a2c518b968faa6ef86b7c1f544eac40f8e5c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530587"
---
# <a name="response-getfederationinformation-soap"></a><span data-ttu-id="3baed-103">Response (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3baed-103">Response (GetFederationInformation) (SOAP)</span></span>

<span data-ttu-id="3baed-104">**Response**要素には、 [GETFEDERATIONINFORMATION operation (SOAP)](getfederationinformation-operation-soap.md)応答情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3baed-104">The **Response** element contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response information.</span></span> 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <ApplicationUri/>
   <Domains/>
</Response>
```

 <span data-ttu-id="3baed-105">**GetFederationInformationResponse**</span><span class="sxs-lookup"><span data-stu-id="3baed-105">**GetFederationInformationResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3baed-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3baed-106">Attributes and elements</span></span>

<span data-ttu-id="3baed-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3baed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3baed-108">属性</span><span class="sxs-lookup"><span data-stu-id="3baed-108">Attributes</span></span>

<span data-ttu-id="3baed-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3baed-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3baed-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3baed-110">Child elements</span></span>

|<span data-ttu-id="3baed-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="3baed-111">**Element**</span></span>|<span data-ttu-id="3baed-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3baed-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3baed-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3baed-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="3baed-114">自動検出サービスによって返されるエラーコードを表します。</span><span class="sxs-lookup"><span data-stu-id="3baed-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="3baed-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3baed-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="3baed-116">自動検出サービスによって返されるエラーコードに関連付けられているメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="3baed-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="3baed-117">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3baed-117">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md) <br/> |<span data-ttu-id="3baed-118">アプリケーションの場所を定義します。</span><span class="sxs-lookup"><span data-stu-id="3baed-118">Defines the location of an application.</span></span>  <br/> |
|[<span data-ttu-id="3baed-119">Domains (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3baed-119">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="3baed-120">は、 [Getdomainsettings 操作 (soap)](getdomainsettings-operation-soap.md)で返される構成、または組織が[GETFEDERATIONINFORMATION 操作 (soap)](getfederationinformation-operation-soap.md)でフェデレーションしたドメインのドメインコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="3baed-120">Represents the domain collection the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), or the domains that the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3baed-121">親要素</span><span class="sxs-lookup"><span data-stu-id="3baed-121">Parent elements</span></span>

|<span data-ttu-id="3baed-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="3baed-122">**Element**</span></span>|<span data-ttu-id="3baed-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="3baed-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3baed-124">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3baed-124">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md) <br/> |<span data-ttu-id="3baed-125">[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="3baed-125">Defines a response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3baed-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3baed-126">Text value</span></span>

<span data-ttu-id="3baed-127">なし。</span><span class="sxs-lookup"><span data-stu-id="3baed-127">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3baed-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3baed-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3baed-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="3baed-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="3baed-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3baed-130">Schema Name</span></span>  <br/> |<span data-ttu-id="3baed-131">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="3baed-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="3baed-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3baed-132">Validation File</span></span>  <br/> |<span data-ttu-id="3baed-133">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3baed-133">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3baed-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3baed-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="3baed-135">正しい</span><span class="sxs-lookup"><span data-stu-id="3baed-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3baed-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="3baed-136">See also</span></span>



[<span data-ttu-id="3baed-137">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3baed-137">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)


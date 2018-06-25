---
title: 応答 (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ca48a4b3-5006-4bb7-973e-d9137ce67e16
description: 応答要素には、GetFederationInformation (SOAP) の操作の応答の情報が含まれています。
ms.openlocfilehash: 946cba56d7503a0e20ec59640f4f1258c00a844e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833171"
---
# <a name="response-getfederationinformation-soap"></a><span data-ttu-id="70f73-103">応答 (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="70f73-103">Response (GetFederationInformation) (SOAP)</span></span>

<span data-ttu-id="70f73-104">**応答**要素には、 [GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)応答の情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="70f73-104">The **Response** element contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response information.</span></span> 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <ApplicationUri/>
   <Domains/>
</Response>
```

 <span data-ttu-id="70f73-105">**GetFederationInformationResponse**</span><span class="sxs-lookup"><span data-stu-id="70f73-105">**GetFederationInformationResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70f73-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="70f73-106">Attributes and elements</span></span>

<span data-ttu-id="70f73-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="70f73-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70f73-108">属性</span><span class="sxs-lookup"><span data-stu-id="70f73-108">Attributes</span></span>

<span data-ttu-id="70f73-109">なし。</span><span class="sxs-lookup"><span data-stu-id="70f73-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70f73-110">子要素</span><span class="sxs-lookup"><span data-stu-id="70f73-110">Child elements</span></span>

|<span data-ttu-id="70f73-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="70f73-111">**Element**</span></span>|<span data-ttu-id="70f73-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="70f73-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70f73-113">エラー コード (SOAP)</span><span class="sxs-lookup"><span data-stu-id="70f73-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="70f73-114">自動検出サービスによって返されるエラー コードを表します。</span><span class="sxs-lookup"><span data-stu-id="70f73-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="70f73-115">エラー メッセージ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="70f73-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="70f73-116">自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="70f73-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="70f73-117">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="70f73-117">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md) <br/> |<span data-ttu-id="70f73-118">アプリケーションの場所を定義します。</span><span class="sxs-lookup"><span data-stu-id="70f73-118">Defines the location of an application.</span></span>  <br/> |
|[<span data-ttu-id="70f73-119">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="70f73-119">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="70f73-120">で[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)、または組織は、 [GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)でフェデレーション ドメインの構成が返されるドメインのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="70f73-120">Represents the domain collection the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), or the domains that the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="70f73-121">親要素</span><span class="sxs-lookup"><span data-stu-id="70f73-121">Parent elements</span></span>

|<span data-ttu-id="70f73-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="70f73-122">**Element**</span></span>|<span data-ttu-id="70f73-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="70f73-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70f73-124">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="70f73-124">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md) <br/> |<span data-ttu-id="70f73-125">[GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="70f73-125">Defines a response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="70f73-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="70f73-126">Text value</span></span>

<span data-ttu-id="70f73-127">なし。</span><span class="sxs-lookup"><span data-stu-id="70f73-127">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70f73-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="70f73-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70f73-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="70f73-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="70f73-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="70f73-130">Schema Name</span></span>  <br/> |<span data-ttu-id="70f73-131">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="70f73-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="70f73-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="70f73-132">Validation File</span></span>  <br/> |<span data-ttu-id="70f73-133">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="70f73-133">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="70f73-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="70f73-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="70f73-135">True</span><span class="sxs-lookup"><span data-stu-id="70f73-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="70f73-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="70f73-136">See also</span></span>



[<span data-ttu-id="70f73-137">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="70f73-137">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)


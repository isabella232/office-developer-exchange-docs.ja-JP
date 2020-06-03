---
title: GetFederationInformationResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2033c14f-dcc8-43c2-9fd9-a51946ec7055
description: GetFederationInformationResponse 要素には、GetFederationInformation 操作 (SOAP) 応答が含まれています。
ms.openlocfilehash: c9e65a2b1759946b8493b3c730f08df6fe353fd8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460044"
---
# <a name="getfederationinformationresponse-soap"></a><span data-ttu-id="538d7-103">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="538d7-103">GetFederationInformationResponse (SOAP)</span></span>

<span data-ttu-id="538d7-104">**GetFederationInformationResponse**要素には、 [GETFEDERATIONINFORMATION 操作 (SOAP)](getfederationinformation-operation-soap.md)応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="538d7-104">The **GetFederationInformationResponse** element contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response.</span></span> 
  
```XML
<GetFederationInformationResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <TokenIssuers/>
   <ApplicationUri/>
   <Domains/>
</GetFederationInformationResponse>
```

 <span data-ttu-id="538d7-105">**GetFederationInformationResponse**</span><span class="sxs-lookup"><span data-stu-id="538d7-105">**GetFederationInformationResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="538d7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="538d7-106">Attributes and elements</span></span>

<span data-ttu-id="538d7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="538d7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="538d7-108">属性</span><span class="sxs-lookup"><span data-stu-id="538d7-108">Attributes</span></span>

<span data-ttu-id="538d7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="538d7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="538d7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="538d7-110">Child elements</span></span>

|<span data-ttu-id="538d7-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="538d7-111">**Element**</span></span>|<span data-ttu-id="538d7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="538d7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="538d7-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="538d7-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="538d7-114">自動検出サービスによって返されるエラーコードを表します。</span><span class="sxs-lookup"><span data-stu-id="538d7-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="538d7-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="538d7-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="538d7-116">自動検出サービスによって返されるエラーコードに関連付けられているメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="538d7-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="538d7-117">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="538d7-117">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md) <br/> |<span data-ttu-id="538d7-118">アプリケーションの場所を定義します。</span><span class="sxs-lookup"><span data-stu-id="538d7-118">Defines the location of an application.</span></span>  <br/> |
|[<span data-ttu-id="538d7-119">TokenIssuers 者 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="538d7-119">TokenIssuers (SOAP)</span></span>](tokenissuers-soap.md) <br/> |<span data-ttu-id="538d7-120">セキュリティトークンサービスの識別子とエンドポイントを含むセキュリティトークンのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="538d7-120">Represents a collection of security tokens, which contain security token service identifiers and endpoints.</span></span>  <br/> |
|[<span data-ttu-id="538d7-121">Domains (SOAP)</span><span class="sxs-lookup"><span data-stu-id="538d7-121">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="538d7-122">[Getdomainsettings 操作 (soap)](getdomainsettings-operation-soap.md)の**getdomainsettings**操作または組織が[GetFederationInformation operation (soap)](getfederationinformation-operation-soap.md) **GetFederationInformation**操作でフェデレーションを行ったドメインを表します。.</span><span class="sxs-lookup"><span data-stu-id="538d7-122">Represents the domains the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** operation or the domains the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) **GetFederationInformation** operation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="538d7-123">親要素</span><span class="sxs-lookup"><span data-stu-id="538d7-123">Parent elements</span></span>

<span data-ttu-id="538d7-124">なし。</span><span class="sxs-lookup"><span data-stu-id="538d7-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="538d7-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="538d7-125">Text value</span></span>

<span data-ttu-id="538d7-126">なし。</span><span class="sxs-lookup"><span data-stu-id="538d7-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="538d7-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="538d7-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="538d7-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="538d7-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="538d7-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="538d7-129">Schema Name</span></span>  <br/> |<span data-ttu-id="538d7-130">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="538d7-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="538d7-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="538d7-131">Validation File</span></span>  <br/> |<span data-ttu-id="538d7-132">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="538d7-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="538d7-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="538d7-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="538d7-134">正しい</span><span class="sxs-lookup"><span data-stu-id="538d7-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="538d7-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="538d7-135">See also</span></span>



[<span data-ttu-id="538d7-136">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="538d7-136">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)


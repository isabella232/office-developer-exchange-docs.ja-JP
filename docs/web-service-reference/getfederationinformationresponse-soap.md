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
description: GetFederationInformationResponse 要素には、GetFederationInformation (SOAP) の操作の応答が含まれています。
ms.openlocfilehash: 28b002b45968278ad4c7160b4eed29721422646d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760730"
---
# <a name="getfederationinformationresponse-soap"></a><span data-ttu-id="b134c-103">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b134c-103">GetFederationInformationResponse (SOAP)</span></span>

<span data-ttu-id="b134c-104">**GetFederationInformationResponse**要素には、 [GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)の応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b134c-104">The **GetFederationInformationResponse** element contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response.</span></span> 
  
```XML
<GetFederationInformationResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <TokenIssuers/>
   <ApplicationUri/>
   <Domains/>
</GetFederationInformationResponse>
```

 <span data-ttu-id="b134c-105">**GetFederationInformationResponse**</span><span class="sxs-lookup"><span data-stu-id="b134c-105">**GetFederationInformationResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b134c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b134c-106">Attributes and elements</span></span>

<span data-ttu-id="b134c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b134c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b134c-108">属性</span><span class="sxs-lookup"><span data-stu-id="b134c-108">Attributes</span></span>

<span data-ttu-id="b134c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b134c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b134c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b134c-110">Child elements</span></span>

|<span data-ttu-id="b134c-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="b134c-111">**Element**</span></span>|<span data-ttu-id="b134c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b134c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b134c-113">エラー コード (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b134c-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="b134c-114">自動検出サービスによって返されるエラー コードを表します。</span><span class="sxs-lookup"><span data-stu-id="b134c-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="b134c-115">エラー メッセージ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b134c-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="b134c-116">自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="b134c-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="b134c-117">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b134c-117">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md) <br/> |<span data-ttu-id="b134c-118">アプリケーションの場所を定義します。</span><span class="sxs-lookup"><span data-stu-id="b134c-118">Defines the location of an application.</span></span>  <br/> |
|[<span data-ttu-id="b134c-119">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b134c-119">TokenIssuers (SOAP)</span></span>](tokenissuers-soap.md) <br/> |<span data-ttu-id="b134c-120">セキュリティ トークン サービスの識別子は、エンドポイントが含まれているは、セキュリティ トークンのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="b134c-120">Represents a collection of security tokens, which contain security token service identifiers and endpoints.</span></span>  <br/> |
|[<span data-ttu-id="b134c-121">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b134c-121">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="b134c-122">構成が[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings**の操作で返されるドメインまたは組織は、 [GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)でフェデレーション ドメインを表す**GetFederationInformation**操作です。</span><span class="sxs-lookup"><span data-stu-id="b134c-122">Represents the domains the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** operation or the domains the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) **GetFederationInformation** operation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b134c-123">親要素</span><span class="sxs-lookup"><span data-stu-id="b134c-123">Parent elements</span></span>

<span data-ttu-id="b134c-124">なし。</span><span class="sxs-lookup"><span data-stu-id="b134c-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b134c-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b134c-125">Text value</span></span>

<span data-ttu-id="b134c-126">なし。</span><span class="sxs-lookup"><span data-stu-id="b134c-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b134c-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="b134c-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b134c-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="b134c-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="b134c-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b134c-129">Schema Name</span></span>  <br/> |<span data-ttu-id="b134c-130">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="b134c-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="b134c-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b134c-131">Validation File</span></span>  <br/> |<span data-ttu-id="b134c-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b134c-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b134c-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b134c-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="b134c-134">True</span><span class="sxs-lookup"><span data-stu-id="b134c-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b134c-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="b134c-135">See also</span></span>



[<span data-ttu-id="b134c-136">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b134c-136">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)


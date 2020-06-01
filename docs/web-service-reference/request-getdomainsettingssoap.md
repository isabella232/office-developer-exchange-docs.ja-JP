---
title: Request (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 3ea026fc-74f1-4118-86ae-908ed4f82a4b
description: Request 要素には、ドメイン設定を返す要求が含まれています。
ms.openlocfilehash: c5f666102be8aaeee001a23706732e9e6c44b560
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459589"
---
# <a name="request-getdomainsettings-soap"></a><span data-ttu-id="a24bb-103">Request (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a24bb-103">Request (GetDomainSettings) (SOAP)</span></span>

<span data-ttu-id="a24bb-104">**Request**要素には、ドメイン設定を返す要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a24bb-104">The **Request** element contains a request to return domain settings.</span></span> 
  
```xml
<Request>
   <Domains/>
   <RequestedSettings/>
</Request>
```

 <span data-ttu-id="a24bb-105">**GetDomainSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="a24bb-105">**GetDomainSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a24bb-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a24bb-106">Attributes and elements</span></span>

<span data-ttu-id="a24bb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a24bb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a24bb-108">属性</span><span class="sxs-lookup"><span data-stu-id="a24bb-108">Attributes</span></span>

<span data-ttu-id="a24bb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a24bb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a24bb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a24bb-110">Child elements</span></span>

|<span data-ttu-id="a24bb-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="a24bb-111">**Element**</span></span>|<span data-ttu-id="a24bb-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a24bb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a24bb-113">Domains (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a24bb-113">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="a24bb-114">[Getdomainsettings 操作 (soap)](getdomainsettings-operation-soap.md)または組織の[GETFEDERATIONINFORMATION 操作 (soap)](getfederationinformation-operation-soap.md)でフェデレーションされているドメインで、その構成が返されるドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="a24bb-114">Represents the domains the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) or the domains the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md).</span></span>  <br/> |
|[<span data-ttu-id="a24bb-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a24bb-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="a24bb-116">要求された構成設定の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a24bb-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a24bb-117">親要素</span><span class="sxs-lookup"><span data-stu-id="a24bb-117">Parent elements</span></span>

|<span data-ttu-id="a24bb-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="a24bb-118">**Element**</span></span>|<span data-ttu-id="a24bb-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="a24bb-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a24bb-120">GetDomainSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a24bb-120">GetDomainSettingsRequestMessage (SOAP)</span></span>](getdomainsettingsrequestmessage-soap.md) <br/> |<span data-ttu-id="a24bb-121">[Getdomainsettings 操作 (SOAP)](getdomainsettings-operation-soap.md)要求を表します。</span><span class="sxs-lookup"><span data-stu-id="a24bb-121">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md)request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a24bb-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a24bb-122">Text value</span></span>

<span data-ttu-id="a24bb-123">なし。</span><span class="sxs-lookup"><span data-stu-id="a24bb-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a24bb-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a24bb-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a24bb-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="a24bb-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="a24bb-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a24bb-126">Schema Name</span></span>  <br/> |<span data-ttu-id="a24bb-127">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="a24bb-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="a24bb-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a24bb-128">Validation File</span></span>  <br/> |<span data-ttu-id="a24bb-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a24bb-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a24bb-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a24bb-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="a24bb-131">正しい</span><span class="sxs-lookup"><span data-stu-id="a24bb-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a24bb-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="a24bb-132">See also</span></span>



[<span data-ttu-id="a24bb-133">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a24bb-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)


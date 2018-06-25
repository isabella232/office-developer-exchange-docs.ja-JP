---
title: DomainSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f3d37f5a-c9ea-4ed9-a011-94d33bda64d1
description: DomainSettings 要素は、自動検出要求の送信、または、自動検出応答によって返されるドメインの設定を表します。
ms.openlocfilehash: 961051399dc8babd8cba6eeaf43456071d0f40a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760166"
---
# <a name="domainsettings-soap"></a><span data-ttu-id="5cbcf-103">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5cbcf-103">DomainSettings (SOAP)</span></span>

<span data-ttu-id="5cbcf-104">**DomainSettings**要素は、自動検出要求の送信、または、自動検出応答によって返されるドメインの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="5cbcf-104">The **DomainSettings** element represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span> 
  
```XML
<DomainSettings>
   <DomainSetting/>
</DomainSettings>
```

 <span data-ttu-id="5cbcf-105">**DomainSettings**</span><span class="sxs-lookup"><span data-stu-id="5cbcf-105">**DomainSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5cbcf-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5cbcf-106">Attributes and elements</span></span>

<span data-ttu-id="5cbcf-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5cbcf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5cbcf-108">属性</span><span class="sxs-lookup"><span data-stu-id="5cbcf-108">Attributes</span></span>

<span data-ttu-id="5cbcf-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5cbcf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5cbcf-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5cbcf-110">Child elements</span></span>

|<span data-ttu-id="5cbcf-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="5cbcf-111">**Element**</span></span>|<span data-ttu-id="5cbcf-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5cbcf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5cbcf-113">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5cbcf-113">DomainSetting (SOAP)</span></span>](domainsetting-soap.md) <br/> |<span data-ttu-id="5cbcf-114">[GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)要求によって返されるドメインの設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5cbcf-114">Contains domain settings that are returned by a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5cbcf-115">親要素</span><span class="sxs-lookup"><span data-stu-id="5cbcf-115">Parent elements</span></span>

|<span data-ttu-id="5cbcf-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="5cbcf-116">**Element**</span></span>|<span data-ttu-id="5cbcf-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="5cbcf-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5cbcf-118">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5cbcf-118">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="5cbcf-119">指定したドメインの指定された設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5cbcf-119">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5cbcf-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5cbcf-120">Text value</span></span>

<span data-ttu-id="5cbcf-121">なし。</span><span class="sxs-lookup"><span data-stu-id="5cbcf-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5cbcf-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="5cbcf-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5cbcf-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="5cbcf-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="5cbcf-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5cbcf-124">Schema Name</span></span>  <br/> |<span data-ttu-id="5cbcf-125">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="5cbcf-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="5cbcf-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5cbcf-126">Validation File</span></span>  <br/> |<span data-ttu-id="5cbcf-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5cbcf-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5cbcf-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5cbcf-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="5cbcf-129">True</span><span class="sxs-lookup"><span data-stu-id="5cbcf-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5cbcf-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="5cbcf-130">See also</span></span>

- [<span data-ttu-id="5cbcf-131">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5cbcf-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)


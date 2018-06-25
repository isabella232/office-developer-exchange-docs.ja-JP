---
title: ドメイン (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 849629a0-0467-422f-88f6-3b8a95c17bba
description: ドメイン要素は、GetFederationInformation 応答内のフェデレーション ドメインが含まれています。 または、対象の構成の設定が GetDomainSettings の要求で要求されたドメインが含まれています。
ms.openlocfilehash: 411ca866800322ef06eeecc2ab92adc6f711917c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760145"
---
# <a name="domain-soap"></a><span data-ttu-id="33efb-103">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33efb-103">Domain (SOAP)</span></span>

<span data-ttu-id="33efb-104">**ドメイン**要素は、 **GetFederationInformation**応答内のフェデレーション ドメインが含まれています。 または、対象の構成の設定が**GetDomainSettings**の要求で要求されたドメインが含まれています。</span><span class="sxs-lookup"><span data-stu-id="33efb-104">The **Domain** element contains a federated domain in a **GetFederationInformation** response or contains a domain the configuration settings for which are requested in a **GetDomainSettings** request.</span></span> 
  
```XML
<Domain/> 
```

 <span data-ttu-id="33efb-105">**string**</span><span class="sxs-lookup"><span data-stu-id="33efb-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33efb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="33efb-106">Attributes and elements</span></span>

<span data-ttu-id="33efb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="33efb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33efb-108">属性</span><span class="sxs-lookup"><span data-stu-id="33efb-108">Attributes</span></span>

<span data-ttu-id="33efb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="33efb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33efb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="33efb-110">Child elements</span></span>

<span data-ttu-id="33efb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="33efb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="33efb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="33efb-112">Parent elements</span></span>

|<span data-ttu-id="33efb-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="33efb-113">**Element**</span></span>|<span data-ttu-id="33efb-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="33efb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33efb-115">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33efb-115">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="33efb-116">対象の構成の設定が**GetDomainSettings**の操作で返されるドメインまたは組織は、 **GetFederationInformation**の操作でフェデレーション ドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="33efb-116">Represents the domains the configuration settings for which are returned in a **GetDomainSettings** operation or the domains that the organization has federated in a **GetFederationInformation** operation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="33efb-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="33efb-117">Text value</span></span>

<span data-ttu-id="33efb-118">**ドメイン**要素のテキスト値は、ドメイン名を表します。</span><span class="sxs-lookup"><span data-stu-id="33efb-118">The text value of the **Domain** element represents a domain name.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="33efb-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="33efb-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33efb-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="33efb-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="33efb-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="33efb-121">Schema Name</span></span>  <br/> |<span data-ttu-id="33efb-122">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="33efb-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="33efb-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="33efb-123">Validation File</span></span>  <br/> |<span data-ttu-id="33efb-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="33efb-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="33efb-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="33efb-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="33efb-126">True</span><span class="sxs-lookup"><span data-stu-id="33efb-126">True</span></span>  <br/> |
   


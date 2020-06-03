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
description: ドメイン要素には、GetFederationInformation 応答のフェデレーションドメインが含まれているか、または GetDomainSettings 要求で要求される構成設定がドメインに含まれています。
ms.openlocfilehash: f90c608ee1fc3356a227bca6411eaeff0c1e8b22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456984"
---
# <a name="domain-soap"></a><span data-ttu-id="dc1a6-103">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dc1a6-103">Domain (SOAP)</span></span>

<span data-ttu-id="dc1a6-104">**ドメイン**要素には、 **GetFederationInformation**応答のフェデレーションドメインが含まれているか、または**getdomainsettings**要求で要求される構成設定がドメインに含まれています。</span><span class="sxs-lookup"><span data-stu-id="dc1a6-104">The **Domain** element contains a federated domain in a **GetFederationInformation** response or contains a domain the configuration settings for which are requested in a **GetDomainSettings** request.</span></span> 
  
```XML
<Domain/> 
```

 <span data-ttu-id="dc1a6-105">**string**</span><span class="sxs-lookup"><span data-stu-id="dc1a6-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dc1a6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="dc1a6-106">Attributes and elements</span></span>

<span data-ttu-id="dc1a6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dc1a6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc1a6-108">属性</span><span class="sxs-lookup"><span data-stu-id="dc1a6-108">Attributes</span></span>

<span data-ttu-id="dc1a6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dc1a6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc1a6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dc1a6-110">Child elements</span></span>

<span data-ttu-id="dc1a6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="dc1a6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dc1a6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="dc1a6-112">Parent elements</span></span>

|<span data-ttu-id="dc1a6-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="dc1a6-113">**Element**</span></span>|<span data-ttu-id="dc1a6-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="dc1a6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc1a6-115">Domains (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dc1a6-115">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="dc1a6-116">**Getdomainsettings**操作または組織が**GetFederationInformation**操作でフェデレーションしたドメインで返される構成設定のドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="dc1a6-116">Represents the domains the configuration settings for which are returned in a **GetDomainSettings** operation or the domains that the organization has federated in a **GetFederationInformation** operation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dc1a6-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="dc1a6-117">Text value</span></span>

<span data-ttu-id="dc1a6-118">**Domain**要素のテキスト値は、ドメイン名を表します。</span><span class="sxs-lookup"><span data-stu-id="dc1a6-118">The text value of the **Domain** element represents a domain name.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="dc1a6-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="dc1a6-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc1a6-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="dc1a6-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="dc1a6-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dc1a6-121">Schema Name</span></span>  <br/> |<span data-ttu-id="dc1a6-122">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="dc1a6-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="dc1a6-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dc1a6-123">Validation File</span></span>  <br/> |<span data-ttu-id="dc1a6-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="dc1a6-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dc1a6-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dc1a6-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="dc1a6-126">はい</span><span class="sxs-lookup"><span data-stu-id="dc1a6-126">True</span></span>  <br/> |
   


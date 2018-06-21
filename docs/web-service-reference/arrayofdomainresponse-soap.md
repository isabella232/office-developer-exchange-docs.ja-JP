---
title: ArrayOfDomainResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6dbd9221-e019-4981-bcdb-ea370331f407
description: ArrayOfDomainResponse 要素には、要求された各ドメインの設定の応答の配列が含まれています。
ms.openlocfilehash: 7dec7f4e3df2fd0d7d1fcd4f08bc74a2b432af1b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/21/2018
ms.locfileid: "19759439"
---
# <a name="arrayofdomainresponse-soap"></a><span data-ttu-id="9ca78-103">ArrayOfDomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ca78-103">ArrayOfDomainResponse (SOAP)</span></span>

<span data-ttu-id="9ca78-104">**ArrayOfDomainResponse**要素には、要求された各ドメインの設定の応答の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ca78-104">The **ArrayOfDomainResponse** element contains an array of responses for each requested domain's settings.</span></span> 
  
```XML
<ArrayOfDomainResponse>
   <DomainResponse/>
</ArrayOfDomainResponse>
```

 <span data-ttu-id="9ca78-105">**ArrayOfDomainResponse**</span><span class="sxs-lookup"><span data-stu-id="9ca78-105">**ArrayOfDomainResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ca78-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9ca78-106">Attributes and elements</span></span>

<span data-ttu-id="9ca78-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9ca78-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ca78-108">属性</span><span class="sxs-lookup"><span data-stu-id="9ca78-108">Attributes</span></span>

<span data-ttu-id="9ca78-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9ca78-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ca78-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9ca78-110">Child elements</span></span>

|<span data-ttu-id="9ca78-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="9ca78-111">**Element**</span></span>|<span data-ttu-id="9ca78-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ca78-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ca78-113">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ca78-113">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="9ca78-114">指定したドメインの指定された設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ca78-114">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9ca78-115">親要素</span><span class="sxs-lookup"><span data-stu-id="9ca78-115">Parent elements</span></span>

<span data-ttu-id="9ca78-116">なし。</span><span class="sxs-lookup"><span data-stu-id="9ca78-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="9ca78-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9ca78-117">Text value</span></span>

<span data-ttu-id="9ca78-118">なし。</span><span class="sxs-lookup"><span data-stu-id="9ca78-118">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ca78-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="9ca78-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ca78-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="9ca78-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="9ca78-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9ca78-121">Schema Name</span></span>  <br/> |<span data-ttu-id="9ca78-122">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="9ca78-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="9ca78-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9ca78-123">Validation File</span></span>  <br/> |<span data-ttu-id="9ca78-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9ca78-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9ca78-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9ca78-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ca78-126">True</span><span class="sxs-lookup"><span data-stu-id="9ca78-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ca78-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="9ca78-127">See also</span></span>

- [<span data-ttu-id="9ca78-128">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ca78-128">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)


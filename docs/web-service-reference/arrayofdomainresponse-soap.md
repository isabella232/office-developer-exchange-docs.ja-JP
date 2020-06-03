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
description: ArrayOfDomainResponse 要素には、要求された各ドメインの設定に対する応答の配列が含まれています。
ms.openlocfilehash: 382a62ed14e7015c2a25f06b6f9cfc1be4f9e66b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466018"
---
# <a name="arrayofdomainresponse-soap"></a><span data-ttu-id="a7cf2-103">ArrayOfDomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a7cf2-103">ArrayOfDomainResponse (SOAP)</span></span>

<span data-ttu-id="a7cf2-104">**Arrayofdomainresponse**要素には、要求された各ドメインの設定に対する応答の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a7cf2-104">The **ArrayOfDomainResponse** element contains an array of responses for each requested domain's settings.</span></span> 
  
```XML
<ArrayOfDomainResponse>
   <DomainResponse/>
</ArrayOfDomainResponse>
```

 <span data-ttu-id="a7cf2-105">**ArrayOfDomainResponse**</span><span class="sxs-lookup"><span data-stu-id="a7cf2-105">**ArrayOfDomainResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a7cf2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a7cf2-106">Attributes and elements</span></span>

<span data-ttu-id="a7cf2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a7cf2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7cf2-108">属性</span><span class="sxs-lookup"><span data-stu-id="a7cf2-108">Attributes</span></span>

<span data-ttu-id="a7cf2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a7cf2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a7cf2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a7cf2-110">Child elements</span></span>

|<span data-ttu-id="a7cf2-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="a7cf2-111">**Element**</span></span>|<span data-ttu-id="a7cf2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a7cf2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7cf2-113">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a7cf2-113">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="a7cf2-114">指定したドメインに対して要求された設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a7cf2-114">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a7cf2-115">親要素</span><span class="sxs-lookup"><span data-stu-id="a7cf2-115">Parent elements</span></span>

<span data-ttu-id="a7cf2-116">なし。</span><span class="sxs-lookup"><span data-stu-id="a7cf2-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a7cf2-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a7cf2-117">Text value</span></span>

<span data-ttu-id="a7cf2-118">なし。</span><span class="sxs-lookup"><span data-stu-id="a7cf2-118">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7cf2-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a7cf2-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7cf2-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="a7cf2-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="a7cf2-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a7cf2-121">Schema Name</span></span>  <br/> |<span data-ttu-id="a7cf2-122">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="a7cf2-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="a7cf2-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a7cf2-123">Validation File</span></span>  <br/> |<span data-ttu-id="a7cf2-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a7cf2-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a7cf2-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a7cf2-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="a7cf2-126">正しい</span><span class="sxs-lookup"><span data-stu-id="a7cf2-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a7cf2-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="a7cf2-127">See also</span></span>

- [<span data-ttu-id="a7cf2-128">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a7cf2-128">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)


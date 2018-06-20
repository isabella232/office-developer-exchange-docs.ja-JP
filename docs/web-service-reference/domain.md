---
title: ドメイン
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Domain
api_type:
- schema
ms.assetid: 7e45a061-856f-4b44-b053-a7c4d5ad569e
description: ドメイン要素は、1 つの SMTP ドメインを識別します。
ms.openlocfilehash: 78eb1edfd347a513b84b9c15d143d76425041e85
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760148"
---
# <a name="domain"></a><span data-ttu-id="7caf8-103">ドメイン</span><span class="sxs-lookup"><span data-stu-id="7caf8-103">Domain</span></span>

<span data-ttu-id="7caf8-104">**ドメイン**要素は、1 つの SMTP ドメインを識別します。</span><span class="sxs-lookup"><span data-stu-id="7caf8-104">The **Domain** element identifies a single SMTP domain.</span></span> 
  
```xml
<Domain Name="" IncludeSubdomains="" />
```

 <span data-ttu-id="7caf8-105">**StmpDomain**</span><span class="sxs-lookup"><span data-stu-id="7caf8-105">**StmpDomain**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7caf8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7caf8-106">Attributes and elements</span></span>

<span data-ttu-id="7caf8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7caf8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7caf8-108">属性</span><span class="sxs-lookup"><span data-stu-id="7caf8-108">Attributes</span></span>

|<span data-ttu-id="7caf8-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="7caf8-109">**Attribute**</span></span>|<span data-ttu-id="7caf8-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="7caf8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7caf8-111">名前</span><span class="sxs-lookup"><span data-stu-id="7caf8-111">Name</span></span>  <br/> |<span data-ttu-id="7caf8-112">ドメインの名前を識別します。</span><span class="sxs-lookup"><span data-stu-id="7caf8-112">Identifies the name of a domain.</span></span> <span data-ttu-id="7caf8-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="7caf8-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="7caf8-114">IncludeSubdomains</span><span class="sxs-lookup"><span data-stu-id="7caf8-114">IncludeSubdomains</span></span>  <br/> |<span data-ttu-id="7caf8-115">**Name**属性によって識別されるドメインのサブドメインを内部に考慮がかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7caf8-115">Indicates whether subdomains of the domain identified by the **Name** attribute are considered internal.</span></span> <span data-ttu-id="7caf8-116">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="7caf8-116">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7caf8-117">子要素</span><span class="sxs-lookup"><span data-stu-id="7caf8-117">Child elements</span></span>

<span data-ttu-id="7caf8-118">なし。</span><span class="sxs-lookup"><span data-stu-id="7caf8-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7caf8-119">親要素</span><span class="sxs-lookup"><span data-stu-id="7caf8-119">Parent elements</span></span>

|<span data-ttu-id="7caf8-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="7caf8-120">**Element**</span></span>|<span data-ttu-id="7caf8-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="7caf8-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7caf8-122">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="7caf8-122">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="7caf8-123">組織の内部の SMTP ドメインのリストを識別します。</span><span class="sxs-lookup"><span data-stu-id="7caf8-123">Identifies the list of internal SMTP domains of the organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7caf8-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7caf8-124">Text value</span></span>

<span data-ttu-id="7caf8-125">なし。</span><span class="sxs-lookup"><span data-stu-id="7caf8-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7caf8-126">備考</span><span class="sxs-lookup"><span data-stu-id="7caf8-126">Remarks</span></span>

<span data-ttu-id="7caf8-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7caf8-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7caf8-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="7caf8-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7caf8-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="7caf8-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7caf8-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7caf8-130">Schema Name</span></span>  <br/> |<span data-ttu-id="7caf8-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7caf8-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="7caf8-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7caf8-132">Validation File</span></span>  <br/> |<span data-ttu-id="7caf8-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7caf8-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7caf8-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7caf8-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="7caf8-135">False</span><span class="sxs-lookup"><span data-stu-id="7caf8-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7caf8-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="7caf8-136">See also</span></span>

- [<span data-ttu-id="7caf8-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7caf8-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


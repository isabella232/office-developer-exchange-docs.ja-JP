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
description: Domain 要素は、1つの SMTP ドメインを識別します。
ms.openlocfilehash: 3bf8e132b5fa588171ac4f3c095692bc68394663
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461332"
---
# <a name="domain"></a><span data-ttu-id="27f5a-103">ドメイン</span><span class="sxs-lookup"><span data-stu-id="27f5a-103">Domain</span></span>

<span data-ttu-id="27f5a-104">**Domain**要素は、1つの SMTP ドメインを識別します。</span><span class="sxs-lookup"><span data-stu-id="27f5a-104">The **Domain** element identifies a single SMTP domain.</span></span> 
  
```xml
<Domain Name="" IncludeSubdomains="" />
```

 <span data-ttu-id="27f5a-105">**StmpDomain**</span><span class="sxs-lookup"><span data-stu-id="27f5a-105">**StmpDomain**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27f5a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="27f5a-106">Attributes and elements</span></span>

<span data-ttu-id="27f5a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="27f5a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27f5a-108">属性</span><span class="sxs-lookup"><span data-stu-id="27f5a-108">Attributes</span></span>

|<span data-ttu-id="27f5a-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="27f5a-109">**Attribute**</span></span>|<span data-ttu-id="27f5a-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="27f5a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="27f5a-111">名前</span><span class="sxs-lookup"><span data-stu-id="27f5a-111">Name</span></span>  <br/> |<span data-ttu-id="27f5a-112">ドメインの名前を識別します。</span><span class="sxs-lookup"><span data-stu-id="27f5a-112">Identifies the name of a domain.</span></span> <span data-ttu-id="27f5a-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="27f5a-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="27f5a-114">IncludeSubdomains</span><span class="sxs-lookup"><span data-stu-id="27f5a-114">IncludeSubdomains</span></span>  <br/> |<span data-ttu-id="27f5a-115">**Name**属性によって識別されるドメインのサブドメインが内部と見なされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27f5a-115">Indicates whether subdomains of the domain identified by the **Name** attribute are considered internal.</span></span> <span data-ttu-id="27f5a-116">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="27f5a-116">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="27f5a-117">子要素</span><span class="sxs-lookup"><span data-stu-id="27f5a-117">Child elements</span></span>

<span data-ttu-id="27f5a-118">なし。</span><span class="sxs-lookup"><span data-stu-id="27f5a-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="27f5a-119">親要素</span><span class="sxs-lookup"><span data-stu-id="27f5a-119">Parent elements</span></span>

|<span data-ttu-id="27f5a-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="27f5a-120">**Element**</span></span>|<span data-ttu-id="27f5a-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="27f5a-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27f5a-122">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="27f5a-122">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="27f5a-123">組織の内部 SMTP ドメインのリストを識別します。</span><span class="sxs-lookup"><span data-stu-id="27f5a-123">Identifies the list of internal SMTP domains of the organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="27f5a-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="27f5a-124">Text value</span></span>

<span data-ttu-id="27f5a-125">なし。</span><span class="sxs-lookup"><span data-stu-id="27f5a-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="27f5a-126">注釈</span><span class="sxs-lookup"><span data-stu-id="27f5a-126">Remarks</span></span>

<span data-ttu-id="27f5a-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="27f5a-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27f5a-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="27f5a-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27f5a-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="27f5a-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="27f5a-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="27f5a-130">Schema Name</span></span>  <br/> |<span data-ttu-id="27f5a-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="27f5a-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="27f5a-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="27f5a-132">Validation File</span></span>  <br/> |<span data-ttu-id="27f5a-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="27f5a-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="27f5a-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="27f5a-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="27f5a-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="27f5a-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27f5a-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="27f5a-136">See also</span></span>

- [<span data-ttu-id="27f5a-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="27f5a-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


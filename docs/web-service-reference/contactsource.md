---
title: ContactSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactSource
api_type:
- schema
ms.assetid: 500b0423-864e-4cde-a39b-6b5b06d1aa6a
description: ContactSource 要素は、連絡先が Exchange ストアまたは Active Directory ドメインサービス (AD DS) に配置されているかどうかを表します。
ms.openlocfilehash: 5447dedf199c5ad6b944aa33e6dca03e83a3c340
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462711"
---
# <a name="contactsource"></a><span data-ttu-id="dc61c-103">ContactSource</span><span class="sxs-lookup"><span data-stu-id="dc61c-103">ContactSource</span></span>

<span data-ttu-id="dc61c-104">**Contactsource**要素は、連絡先が Exchange ストアまたは Active Directory ドメインサービス (AD DS) に配置されているかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="dc61c-104">The **ContactSource** element describes whether the contact is located in the Exchange store or Active Directory Domain Services (AD DS).</span></span> 
  
```xml
<ContactSource/>
```

 <span data-ttu-id="dc61c-105">**ContactSourceType**</span><span class="sxs-lookup"><span data-stu-id="dc61c-105">**ContactSourceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dc61c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="dc61c-106">Attributes and elements</span></span>

<span data-ttu-id="dc61c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dc61c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc61c-108">属性</span><span class="sxs-lookup"><span data-stu-id="dc61c-108">Attributes</span></span>

<span data-ttu-id="dc61c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dc61c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc61c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dc61c-110">Child elements</span></span>

<span data-ttu-id="dc61c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="dc61c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dc61c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="dc61c-112">Parent elements</span></span>

|<span data-ttu-id="dc61c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="dc61c-113">**Element**</span></span>|<span data-ttu-id="dc61c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="dc61c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc61c-115">連絡先</span><span class="sxs-lookup"><span data-stu-id="dc61c-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="dc61c-116">Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="dc61c-116">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="dc61c-117">DistributionList</span><span class="sxs-lookup"><span data-stu-id="dc61c-117">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="dc61c-118">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="dc61c-118">Represents a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dc61c-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="dc61c-119">Text value</span></span>

<span data-ttu-id="dc61c-120">この要素に使用できる値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="dc61c-120">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="dc61c-121">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="dc61c-121">ActiveDirectory</span></span>
    
- <span data-ttu-id="dc61c-122">ストア</span><span class="sxs-lookup"><span data-stu-id="dc61c-122">Store</span></span>
    
## <a name="remarks"></a><span data-ttu-id="dc61c-123">注釈</span><span class="sxs-lookup"><span data-stu-id="dc61c-123">Remarks</span></span>

<span data-ttu-id="dc61c-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="dc61c-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc61c-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="dc61c-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc61c-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="dc61c-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dc61c-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dc61c-127">Schema name</span></span>  <br/> |<span data-ttu-id="dc61c-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="dc61c-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="dc61c-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dc61c-129">Validation file</span></span>  <br/> |<span data-ttu-id="dc61c-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="dc61c-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dc61c-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="dc61c-131">Can be empty</span></span>  <br/> |<span data-ttu-id="dc61c-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="dc61c-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc61c-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="dc61c-133">See also</span></span>



- [<span data-ttu-id="dc61c-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="dc61c-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


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
description: ContactSource 要素は、連絡先が Exchange ストアまたは Active Directory ドメイン サービス (AD DS) 内にあるかどうかについて説明します。
ms.openlocfilehash: a82b766fc81b9397fc707415ea82e2f2d63d952d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759683"
---
# <a name="contactsource"></a><span data-ttu-id="52bf9-103">ContactSource</span><span class="sxs-lookup"><span data-stu-id="52bf9-103">ContactSource</span></span>

<span data-ttu-id="52bf9-104">**ContactSource**要素は、連絡先が Exchange ストアまたは Active Directory ドメイン サービス (AD DS) 内にあるかどうかについて説明します。</span><span class="sxs-lookup"><span data-stu-id="52bf9-104">The **ContactSource** element describes whether the contact is located in the Exchange store or Active Directory Domain Services (AD DS).</span></span> 
  
```xml
<ContactSource/>
```

 <span data-ttu-id="52bf9-105">**ContactSourceType**</span><span class="sxs-lookup"><span data-stu-id="52bf9-105">**ContactSourceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="52bf9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="52bf9-106">Attributes and elements</span></span>

<span data-ttu-id="52bf9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="52bf9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="52bf9-108">属性</span><span class="sxs-lookup"><span data-stu-id="52bf9-108">Attributes</span></span>

<span data-ttu-id="52bf9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="52bf9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="52bf9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="52bf9-110">Child elements</span></span>

<span data-ttu-id="52bf9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="52bf9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="52bf9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="52bf9-112">Parent elements</span></span>

|<span data-ttu-id="52bf9-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="52bf9-113">**Element**</span></span>|<span data-ttu-id="52bf9-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="52bf9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52bf9-115">Contact</span><span class="sxs-lookup"><span data-stu-id="52bf9-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="52bf9-116">Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="52bf9-116">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="52bf9-117">DistributionList</span><span class="sxs-lookup"><span data-stu-id="52bf9-117">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="52bf9-118">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="52bf9-118">Represents a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="52bf9-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="52bf9-119">Text value</span></span>

<span data-ttu-id="52bf9-120">以下は、この要素の有効な値です。</span><span class="sxs-lookup"><span data-stu-id="52bf9-120">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="52bf9-121">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="52bf9-121">ActiveDirectory</span></span>
    
- <span data-ttu-id="52bf9-122">ストア</span><span class="sxs-lookup"><span data-stu-id="52bf9-122">Store</span></span>
    
## <a name="remarks"></a><span data-ttu-id="52bf9-123">備考</span><span class="sxs-lookup"><span data-stu-id="52bf9-123">Remarks</span></span>

<span data-ttu-id="52bf9-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="52bf9-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="52bf9-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="52bf9-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="52bf9-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="52bf9-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="52bf9-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="52bf9-127">Schema name</span></span>  <br/> |<span data-ttu-id="52bf9-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="52bf9-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="52bf9-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="52bf9-129">Validation file</span></span>  <br/> |<span data-ttu-id="52bf9-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="52bf9-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="52bf9-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="52bf9-131">Can be empty</span></span>  <br/> |<span data-ttu-id="52bf9-132">False</span><span class="sxs-lookup"><span data-stu-id="52bf9-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="52bf9-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="52bf9-133">See also</span></span>



- [<span data-ttu-id="52bf9-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="52bf9-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


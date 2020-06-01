---
title: 条件 (RestrictionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4fdb373e-bf1b-4cb0-bbfb-444c6c6cec50
description: Condition 要素は、FindItem または FindConversation 操作の検索の終了を識別するために使用される条件を指定します。
ms.openlocfilehash: 00c5b5e615ed9b253c79dae9dc2b89c797853089
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463938"
---
# <a name="condition-restrictiontype"></a><span data-ttu-id="d2879-103">条件 (RestrictionType)</span><span class="sxs-lookup"><span data-stu-id="d2879-103">Condition (RestrictionType)</span></span>

<span data-ttu-id="d2879-104">**Condition**要素は、 **FindItem**または**findconversation**操作の検索の終了を識別するために使用される条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="d2879-104">The **Condition** element specifies the condition that is used to identify the end of a search for a **FindItem** or a **FindConversation** operation.</span></span> 
  
```XML
<Condition>
    <SearchExpression></SearchExpression>
</Condition>
```

 <span data-ttu-id="d2879-105">**RestrictionType**</span><span class="sxs-lookup"><span data-stu-id="d2879-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2879-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d2879-106">Attributes and elements</span></span>

<span data-ttu-id="d2879-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d2879-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2879-108">属性</span><span class="sxs-lookup"><span data-stu-id="d2879-108">Attributes</span></span>

<span data-ttu-id="d2879-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d2879-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2879-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d2879-110">Child elements</span></span>

|<span data-ttu-id="d2879-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d2879-111">**Element**</span></span>|<span data-ttu-id="d2879-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2879-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2879-113">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="d2879-113">SearchExpression</span></span>](searchexpression.md) <br/> |<span data-ttu-id="d2879-114">制限内の代替要素を表す抽象要素。</span><span class="sxs-lookup"><span data-stu-id="d2879-114">Abstract element that represents the substituted element within a restriction.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d2879-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d2879-115">Parent elements</span></span>

|<span data-ttu-id="d2879-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="d2879-116">**Element**</span></span>|<span data-ttu-id="d2879-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2879-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2879-118">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="d2879-118">SeekToConditionPageItemView</span></span>](seektoconditionpageitemview.md) <br/> |<span data-ttu-id="d2879-119">検索の終了を識別するために使用される条件、検索の開始インデックス、返される最大エントリ、および**FindItem**または**findconversation**操作の検索方向を識別します。</span><span class="sxs-lookup"><span data-stu-id="d2879-119">Identifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or a **FindConversation** operation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d2879-120">注釈</span><span class="sxs-lookup"><span data-stu-id="d2879-120">Remarks</span></span>

<span data-ttu-id="d2879-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d2879-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d2879-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d2879-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2879-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d2879-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2879-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="d2879-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d2879-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d2879-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d2879-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="d2879-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="d2879-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d2879-127">Validation File</span></span>  <br/> |<span data-ttu-id="d2879-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d2879-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d2879-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d2879-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d2879-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="d2879-130">See also</span></span>



- [<span data-ttu-id="d2879-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d2879-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: 条件 (RestrictionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4fdb373e-bf1b-4cb0-bbfb-444c6c6cec50
description: 条件要素は、FindItem または FindConversation 操作の検索の終了を識別するために使用される条件を指定します。
ms.openlocfilehash: 513fc21be52a90698f1c292d6d20d7cdaab07371
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759646"
---
# <a name="condition-restrictiontype"></a><span data-ttu-id="e1584-103">条件 (RestrictionType)</span><span class="sxs-lookup"><span data-stu-id="e1584-103">Condition (RestrictionType)</span></span>

<span data-ttu-id="e1584-104">**条件**要素ではの**FindItem**または**FindConversation**操作の検索の終了を識別するために使用される条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1584-104">The **Condition** element specifies the condition that is used to identify the end of a search for a **FindItem** or a **FindConversation** operation.</span></span> 
  
```XML
<Condition>
    <SearchExpression></SearchExpression>
</Condition>
```

 <span data-ttu-id="e1584-105">**RestrictionType**</span><span class="sxs-lookup"><span data-stu-id="e1584-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1584-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e1584-106">Attributes and elements</span></span>

<span data-ttu-id="e1584-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e1584-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1584-108">属性</span><span class="sxs-lookup"><span data-stu-id="e1584-108">Attributes</span></span>

<span data-ttu-id="e1584-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e1584-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1584-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e1584-110">Child elements</span></span>

|<span data-ttu-id="e1584-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="e1584-111">**Element**</span></span>|<span data-ttu-id="e1584-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e1584-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1584-113">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="e1584-113">SearchExpression</span></span>](searchexpression.md) <br/> |<span data-ttu-id="e1584-114">制限内の代替要素を表す抽象型の要素です。</span><span class="sxs-lookup"><span data-stu-id="e1584-114">Abstract element that represents the substituted element within a restriction.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e1584-115">親要素</span><span class="sxs-lookup"><span data-stu-id="e1584-115">Parent elements</span></span>

|<span data-ttu-id="e1584-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="e1584-116">**Element**</span></span>|<span data-ttu-id="e1584-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="e1584-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1584-118">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="e1584-118">SeekToConditionPageItemView</span></span>](seektoconditionpageitemview.md) <br/> |<span data-ttu-id="e1584-119">の**FindItem**または**FindConversation**操作の検索の終了、検索、戻るには、最大のエントリ、および検索方向の開始インデックスを識別するために使用される条件を識別します。</span><span class="sxs-lookup"><span data-stu-id="e1584-119">Identifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or a **FindConversation** operation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e1584-120">備考</span><span class="sxs-lookup"><span data-stu-id="e1584-120">Remarks</span></span>

<span data-ttu-id="e1584-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e1584-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e1584-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e1584-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1584-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="e1584-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1584-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="e1584-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e1584-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e1584-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e1584-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="e1584-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="e1584-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e1584-127">Validation File</span></span>  <br/> |<span data-ttu-id="e1584-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="e1584-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e1584-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e1584-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e1584-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="e1584-130">See also</span></span>



- [<span data-ttu-id="e1584-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e1584-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


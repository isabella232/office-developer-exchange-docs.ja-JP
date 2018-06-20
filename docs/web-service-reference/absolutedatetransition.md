---
title: AbsoluteDateTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteDateTransition
api_type:
- schema
ms.assetid: 8f5731eb-bed0-45bf-ba89-4aaf20c34a39
description: AbsoluteDateTransition 要素は、特定の日付と、特定の時刻に表示されるタイム ゾーンの移行を表します。
ms.openlocfilehash: 1e9e5f3f2269814a82b827efe46c71a172e21348
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759266"
---
# <a name="absolutedatetransition"></a><span data-ttu-id="2cdab-103">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="2cdab-103">AbsoluteDateTransition</span></span>

<span data-ttu-id="2cdab-104">**AbsoluteDateTransition**要素は、特定の日付と、特定の時刻に表示されるタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="2cdab-104">The **AbsoluteDateTransition** element represents a time zone transition that occurs on a specific date and at a specific time.</span></span> 
  
```xml
<AbsoluteDateTransition>
   <To/>
   <DateTime/>
</AbsoluteDateTransition>
```

<span data-ttu-id="2cdab-105">**AbsoluteDateTransitionType**</span><span class="sxs-lookup"><span data-stu-id="2cdab-105">**AbsoluteDateTransitionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2cdab-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2cdab-106">Attributes and elements</span></span>

<span data-ttu-id="2cdab-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2cdab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2cdab-108">属性</span><span class="sxs-lookup"><span data-stu-id="2cdab-108">Attributes</span></span>

<span data-ttu-id="2cdab-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2cdab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2cdab-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2cdab-110">Child elements</span></span>

|<span data-ttu-id="2cdab-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="2cdab-111">**Element**</span></span>|<span data-ttu-id="2cdab-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2cdab-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cdab-113">To</span><span class="sxs-lookup"><span data-stu-id="2cdab-113">To</span></span>](to.md) <br/> |<span data-ttu-id="2cdab-114">[TransitionsGroup](transitionsgroup.md)タイム ゾーンの移行の対象となる[期間](period.md)を指定します。</span><span class="sxs-lookup"><span data-stu-id="2cdab-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="2cdab-115">DateTime</span><span class="sxs-lookup"><span data-stu-id="2cdab-115">DateTime</span></span>](datetime.md) <br/> |<span data-ttu-id="2cdab-116">日付とタイム ゾーンの切り替えが発生する時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="2cdab-116">Represents the date and time at which the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2cdab-117">親要素</span><span class="sxs-lookup"><span data-stu-id="2cdab-117">Parent elements</span></span>

|<span data-ttu-id="2cdab-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="2cdab-118">**Element**</span></span>|<span data-ttu-id="2cdab-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="2cdab-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cdab-120">遷移</span><span class="sxs-lookup"><span data-stu-id="2cdab-120">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="2cdab-121">タイム ゾーンの切り替え効果のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="2cdab-121">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="2cdab-122">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="2cdab-122">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="2cdab-123">タイム ゾーンの切り替え効果のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="2cdab-123">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2cdab-124">備考</span><span class="sxs-lookup"><span data-stu-id="2cdab-124">Remarks</span></span>

<span data-ttu-id="2cdab-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2cdab-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2cdab-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="2cdab-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2cdab-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="2cdab-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2cdab-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2cdab-128">Schema Name</span></span>  <br/> |<span data-ttu-id="2cdab-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="2cdab-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="2cdab-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2cdab-130">Validation File</span></span>  <br/> |<span data-ttu-id="2cdab-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2cdab-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2cdab-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2cdab-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="2cdab-133">False</span><span class="sxs-lookup"><span data-stu-id="2cdab-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2cdab-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="2cdab-134">See also</span></span>

- [<span data-ttu-id="2cdab-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2cdab-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


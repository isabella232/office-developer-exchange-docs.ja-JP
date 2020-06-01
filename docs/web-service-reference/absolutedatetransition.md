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
description: AbsoluteDateTransition 要素は、特定の日付に特定の時刻に実行されるタイムゾーンの切り替えを表します。
ms.openlocfilehash: 514464f69c3be5496aedbe184848ef9ed9f296b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461724"
---
# <a name="absolutedatetransition"></a><span data-ttu-id="77c99-103">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="77c99-103">AbsoluteDateTransition</span></span>

<span data-ttu-id="77c99-104">**AbsoluteDateTransition**要素は、特定の日付に特定の時刻に実行されるタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="77c99-104">The **AbsoluteDateTransition** element represents a time zone transition that occurs on a specific date and at a specific time.</span></span> 
  
```xml
<AbsoluteDateTransition>
   <To/>
   <DateTime/>
</AbsoluteDateTransition>
```

<span data-ttu-id="77c99-105">**AbsoluteDateTransitionType**</span><span class="sxs-lookup"><span data-stu-id="77c99-105">**AbsoluteDateTransitionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="77c99-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="77c99-106">Attributes and elements</span></span>

<span data-ttu-id="77c99-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="77c99-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77c99-108">属性</span><span class="sxs-lookup"><span data-stu-id="77c99-108">Attributes</span></span>

<span data-ttu-id="77c99-109">なし。</span><span class="sxs-lookup"><span data-stu-id="77c99-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="77c99-110">子要素</span><span class="sxs-lookup"><span data-stu-id="77c99-110">Child elements</span></span>

|<span data-ttu-id="77c99-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="77c99-111">**Element**</span></span>|<span data-ttu-id="77c99-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="77c99-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77c99-113">To</span><span class="sxs-lookup"><span data-stu-id="77c99-113">To</span></span>](to.md) <br/> |<span data-ttu-id="77c99-114">タイムゾーンの遷移のターゲットである[期間](period.md)[または時間を指定](transitionsgroup.md)します。</span><span class="sxs-lookup"><span data-stu-id="77c99-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="77c99-115">DateTime</span><span class="sxs-lookup"><span data-stu-id="77c99-115">DateTime</span></span>](datetime.md) <br/> |<span data-ttu-id="77c99-116">タイムゾーンの切り替えが行われる日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="77c99-116">Represents the date and time at which the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="77c99-117">親要素</span><span class="sxs-lookup"><span data-stu-id="77c99-117">Parent elements</span></span>

|<span data-ttu-id="77c99-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="77c99-118">**Element**</span></span>|<span data-ttu-id="77c99-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="77c99-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77c99-120">切り替わる</span><span class="sxs-lookup"><span data-stu-id="77c99-120">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="77c99-121">タイムゾーンの遷移のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="77c99-121">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="77c99-122">遷移 Tionsgroup</span><span class="sxs-lookup"><span data-stu-id="77c99-122">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="77c99-123">タイムゾーンの遷移のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="77c99-123">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="77c99-124">注釈</span><span class="sxs-lookup"><span data-stu-id="77c99-124">Remarks</span></span>

<span data-ttu-id="77c99-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="77c99-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77c99-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="77c99-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77c99-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="77c99-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="77c99-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="77c99-128">Schema Name</span></span>  <br/> |<span data-ttu-id="77c99-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="77c99-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="77c99-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="77c99-130">Validation File</span></span>  <br/> |<span data-ttu-id="77c99-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="77c99-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="77c99-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="77c99-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="77c99-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="77c99-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77c99-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="77c99-134">See also</span></span>

- [<span data-ttu-id="77c99-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="77c99-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


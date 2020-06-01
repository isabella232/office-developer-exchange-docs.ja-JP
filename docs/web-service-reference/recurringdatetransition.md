---
title: RecurringDateTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringDateTransition
api_type:
- schema
ms.assetid: 52fe1e05-3c50-40a1-8752-5c3c64c9f1ed
description: RecurringDateTransition 要素は、年ごとに特定の日付に発生するタイムゾーンの切り替えを表します。
ms.openlocfilehash: 2acbd3afb50a92d4e4f3d7b552eecb36fe59be8b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461577"
---
# <a name="recurringdatetransition"></a><span data-ttu-id="f2be1-103">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="f2be1-103">RecurringDateTransition</span></span>

<span data-ttu-id="f2be1-104">**RecurringDateTransition**要素は、年ごとに特定の日付に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="f2be1-104">The **RecurringDateTransition** element represents a time zone transition that occurs on a specific date each year.</span></span> 
  
```xml
<RecurringDateTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <Day/>
</RecurringDateTransition>
```

 <span data-ttu-id="f2be1-105">**RecurringDateTransitionType**</span><span class="sxs-lookup"><span data-stu-id="f2be1-105">**RecurringDateTransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2be1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f2be1-106">Attributes and elements</span></span>

<span data-ttu-id="f2be1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f2be1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2be1-108">属性</span><span class="sxs-lookup"><span data-stu-id="f2be1-108">Attributes</span></span>

<span data-ttu-id="f2be1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f2be1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2be1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f2be1-110">Child elements</span></span>

|<span data-ttu-id="f2be1-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="f2be1-111">**Element**</span></span>|<span data-ttu-id="f2be1-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f2be1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2be1-113">To</span><span class="sxs-lookup"><span data-stu-id="f2be1-113">To</span></span>](to.md) <br/> |<span data-ttu-id="f2be1-114">タイムゾーンの遷移のターゲットである[期間](period.md)[または時間を指定](transitionsgroup.md)します。</span><span class="sxs-lookup"><span data-stu-id="f2be1-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="f2be1-115">TimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2be1-115">TimeOffset</span></span>](timeoffset.md) <br/> |<span data-ttu-id="f2be1-116">タイムゾーンの切り替えについて、世界協定時刻 (UTC) からの時間オフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="f2be1-116">Represents the duration offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="f2be1-117">月 (タイムゾーン切り替え)</span><span class="sxs-lookup"><span data-stu-id="f2be1-117">Month (Time Zone Transition)</span></span>](month-time-zone-transition.md) <br/> |<span data-ttu-id="f2be1-118">タイムゾーンの切り替えが行われる月を表します。</span><span class="sxs-lookup"><span data-stu-id="f2be1-118">Represents the month in which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="f2be1-119">Day</span><span class="sxs-lookup"><span data-stu-id="f2be1-119">Day</span></span>](day.md) <br/> |<span data-ttu-id="f2be1-120">タイムゾーンの切り替えが発生する月の日付を表します。</span><span class="sxs-lookup"><span data-stu-id="f2be1-120">Represents the day of the month on which the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f2be1-121">親要素</span><span class="sxs-lookup"><span data-stu-id="f2be1-121">Parent elements</span></span>

|<span data-ttu-id="f2be1-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="f2be1-122">**Element**</span></span>|<span data-ttu-id="f2be1-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="f2be1-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2be1-124">切り替わる</span><span class="sxs-lookup"><span data-stu-id="f2be1-124">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="f2be1-125">タイムゾーンの遷移のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="f2be1-125">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="f2be1-126">遷移 Tionsgroup</span><span class="sxs-lookup"><span data-stu-id="f2be1-126">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="f2be1-127">タイムゾーンの遷移のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="f2be1-127">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f2be1-128">注釈</span><span class="sxs-lookup"><span data-stu-id="f2be1-128">Remarks</span></span>

<span data-ttu-id="f2be1-129">[RecurringDateTransition](recurringdatetransition.md)要素によって表される可能性があるタイムゾーンの遷移の例としては、毎年3月15日に発生する遷移があります。</span><span class="sxs-lookup"><span data-stu-id="f2be1-129">An example of a time zone transition that could be represented by the [RecurringDateTransition](recurringdatetransition.md) element is a transition that occurs on March 15 each year.</span></span> 
  
<span data-ttu-id="f2be1-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f2be1-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2be1-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f2be1-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2be1-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="f2be1-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f2be1-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f2be1-133">Schema Name</span></span>  <br/> |<span data-ttu-id="f2be1-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f2be1-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="f2be1-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f2be1-135">Validation File</span></span>  <br/> |<span data-ttu-id="f2be1-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f2be1-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f2be1-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f2be1-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="f2be1-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="f2be1-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2be1-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="f2be1-139">See also</span></span>



- [<span data-ttu-id="f2be1-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f2be1-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


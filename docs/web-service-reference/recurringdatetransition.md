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
description: RecurringDateTransition 要素は、毎年特定の日に発生するタイム ゾーンの移行を表します。
ms.openlocfilehash: 7cd8f3452a744e0c9a98fd3698dffb9ed8721a6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833014"
---
# <a name="recurringdatetransition"></a><span data-ttu-id="7cac7-103">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="7cac7-103">RecurringDateTransition</span></span>

<span data-ttu-id="7cac7-104">**RecurringDateTransition**要素は、毎年特定の日に発生するタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="7cac7-104">The **RecurringDateTransition** element represents a time zone transition that occurs on a specific date each year.</span></span> 
  
```xml
<RecurringDateTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <Day/>
</RecurringDateTransition>
```

 <span data-ttu-id="7cac7-105">**RecurringDateTransitionType**</span><span class="sxs-lookup"><span data-stu-id="7cac7-105">**RecurringDateTransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7cac7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7cac7-106">Attributes and elements</span></span>

<span data-ttu-id="7cac7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7cac7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7cac7-108">属性</span><span class="sxs-lookup"><span data-stu-id="7cac7-108">Attributes</span></span>

<span data-ttu-id="7cac7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7cac7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7cac7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7cac7-110">Child elements</span></span>

|<span data-ttu-id="7cac7-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="7cac7-111">**Element**</span></span>|<span data-ttu-id="7cac7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7cac7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cac7-113">To</span><span class="sxs-lookup"><span data-stu-id="7cac7-113">To</span></span>](to.md) <br/> |<span data-ttu-id="7cac7-114">[TransitionsGroup](transitionsgroup.md)タイム ゾーンの移行の対象となる[期間](period.md)を指定します。</span><span class="sxs-lookup"><span data-stu-id="7cac7-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="7cac7-115">TimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cac7-115">TimeOffset</span></span>](timeoffset.md) <br/> |<span data-ttu-id="7cac7-116">タイム ゾーンの移行の世界協定時刻 (UTC) からの期間のオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="7cac7-116">Represents the duration offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="7cac7-117">月 (タイム ゾーンの切り替え)</span><span class="sxs-lookup"><span data-stu-id="7cac7-117">Month (Time Zone Transition)</span></span>](month-time-zone-transition.md) <br/> |<span data-ttu-id="7cac7-118">タイム ゾーンの切り替えが発生する月を表します。</span><span class="sxs-lookup"><span data-stu-id="7cac7-118">Represents the month in which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="7cac7-119">日</span><span class="sxs-lookup"><span data-stu-id="7cac7-119">Day</span></span>](day.md) <br/> |<span data-ttu-id="7cac7-120">タイム ゾーンの切り替えが発生する月の日を表します。</span><span class="sxs-lookup"><span data-stu-id="7cac7-120">Represents the day of the month on which the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7cac7-121">親要素</span><span class="sxs-lookup"><span data-stu-id="7cac7-121">Parent elements</span></span>

|<span data-ttu-id="7cac7-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="7cac7-122">**Element**</span></span>|<span data-ttu-id="7cac7-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="7cac7-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cac7-124">遷移</span><span class="sxs-lookup"><span data-stu-id="7cac7-124">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="7cac7-125">タイム ゾーンの切り替え効果のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="7cac7-125">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="7cac7-126">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="7cac7-126">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="7cac7-127">タイム ゾーンの切り替え効果のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="7cac7-127">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7cac7-128">備考</span><span class="sxs-lookup"><span data-stu-id="7cac7-128">Remarks</span></span>

<span data-ttu-id="7cac7-129">[RecurringDateTransition](recurringdatetransition.md)要素によって表すことができるタイム ゾーンの切り替えの例としては毎年 3 月 15 日に移行します。</span><span class="sxs-lookup"><span data-stu-id="7cac7-129">An example of a time zone transition that could be represented by the [RecurringDateTransition](recurringdatetransition.md) element is a transition that occurs on March 15 each year.</span></span> 
  
<span data-ttu-id="7cac7-130">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7cac7-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7cac7-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="7cac7-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7cac7-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="7cac7-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7cac7-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7cac7-133">Schema Name</span></span>  <br/> |<span data-ttu-id="7cac7-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7cac7-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="7cac7-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7cac7-135">Validation File</span></span>  <br/> |<span data-ttu-id="7cac7-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7cac7-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7cac7-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7cac7-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="7cac7-138">False</span><span class="sxs-lookup"><span data-stu-id="7cac7-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7cac7-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="7cac7-139">See also</span></span>



- [<span data-ttu-id="7cac7-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7cac7-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


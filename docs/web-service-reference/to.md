---
title: To
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- To
api_type:
- schema
ms.assetid: d14e46da-14bd-4a33-a78e-8ee314d9c1d8
description: 要素では、タイム ゾーンの移行のターゲットを指定します。 ターゲットは、タイム ゾーンの期間またはタイム ゾーンの切り替え効果のグループのいずれかです。
ms.openlocfilehash: dc7df8ed3ddd6a9b4222ffab4c2b47b00ee4ba0c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839706"
---
# <a name="to"></a><span data-ttu-id="10dec-104">To</span><span class="sxs-lookup"><span data-stu-id="10dec-104">To</span></span>

<span data-ttu-id="10dec-105">要素**へ**は、タイム ゾーンの移行のターゲットを指定します。</span><span class="sxs-lookup"><span data-stu-id="10dec-105">The **To** element specifies the target of the time zone transition.</span></span> <span data-ttu-id="10dec-106">ターゲットは、タイム ゾーンの期間またはタイム ゾーンの切り替え効果のグループのいずれかです。</span><span class="sxs-lookup"><span data-stu-id="10dec-106">The target is either a time zone period or a group of time zone transitions.</span></span> 
  
```xml
<To Kind=""/>
```

 <span data-ttu-id="10dec-107">**TransitionTargetType**</span><span class="sxs-lookup"><span data-stu-id="10dec-107">**TransitionTargetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="10dec-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="10dec-108">Attributes and elements</span></span>

<span data-ttu-id="10dec-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="10dec-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="10dec-110">属性</span><span class="sxs-lookup"><span data-stu-id="10dec-110">Attributes</span></span>

|<span data-ttu-id="10dec-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="10dec-111">**Attribute**</span></span>|<span data-ttu-id="10dec-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="10dec-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="10dec-113">種類</span><span class="sxs-lookup"><span data-stu-id="10dec-113">Kind</span></span>  <br/> |<span data-ttu-id="10dec-114">タイム ゾーンの移行のターゲットがタイム ゾーンの期間であるかどうか、またはタイム ゾーンの切り替え効果のグループのことを示します。</span><span class="sxs-lookup"><span data-stu-id="10dec-114">Indicates whether the time zone transition target is a time zone period or of a group of time zone transitions.</span></span>  <br/> |
   
#### <a name="kind-attribute-values"></a><span data-ttu-id="10dec-115">Kind 属性値</span><span class="sxs-lookup"><span data-stu-id="10dec-115">Kind attribute values</span></span>

|<span data-ttu-id="10dec-116">**値**</span><span class="sxs-lookup"><span data-stu-id="10dec-116">**Value**</span></span>|<span data-ttu-id="10dec-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="10dec-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="10dec-118">ピリオド</span><span class="sxs-lookup"><span data-stu-id="10dec-118">Period</span></span>  <br/> |<span data-ttu-id="10dec-119">タイム ゾーンの移行の対象には、タイム ゾーンの期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="10dec-119">Specifies that the time zone transition target is a time zone period.</span></span>  <br/> |
|<span data-ttu-id="10dec-120">グループ</span><span class="sxs-lookup"><span data-stu-id="10dec-120">Group</span></span>  <br/> |<span data-ttu-id="10dec-121">タイム ゾーンの移行の対象には、タイム ゾーンの切り替え効果のグループを指定します。</span><span class="sxs-lookup"><span data-stu-id="10dec-121">Specifies that the time zone transition target is a group of time zone transitions.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="10dec-122">子要素</span><span class="sxs-lookup"><span data-stu-id="10dec-122">Child elements</span></span>

<span data-ttu-id="10dec-123">なし。</span><span class="sxs-lookup"><span data-stu-id="10dec-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="10dec-124">親要素</span><span class="sxs-lookup"><span data-stu-id="10dec-124">Parent elements</span></span>

|<span data-ttu-id="10dec-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="10dec-125">**Element**</span></span>|<span data-ttu-id="10dec-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="10dec-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10dec-127">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="10dec-127">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="10dec-128">特定の日付と、特定の時刻に表示されるタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="10dec-128">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="10dec-129">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="10dec-129">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="10dec-130">毎年同じ日に発生するタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="10dec-130">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="10dec-131">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="10dec-131">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="10dec-132">年の指定された日に発生するタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="10dec-132">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
|[<span data-ttu-id="10dec-133">Transition</span><span class="sxs-lookup"><span data-stu-id="10dec-133">Transition</span></span>](transition.md) <br/> |<span data-ttu-id="10dec-134">タイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="10dec-134">Represents a time zone transition.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="10dec-135">テキスト値</span><span class="sxs-lookup"><span data-stu-id="10dec-135">Text value</span></span>

<span data-ttu-id="10dec-136">テキスト値は、[期間](period.md)またはタイム ゾーンの移行の対象である[TransitionsGroup](transitionsgroup.md)の一意の識別子を指定する文字列です。</span><span class="sxs-lookup"><span data-stu-id="10dec-136">The text value is a string that specifies the unique identifier of the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="10dec-137">備考</span><span class="sxs-lookup"><span data-stu-id="10dec-137">Remarks</span></span>

<span data-ttu-id="10dec-138">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="10dec-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="10dec-139">要素情報</span><span class="sxs-lookup"><span data-stu-id="10dec-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="10dec-140">名前空間</span><span class="sxs-lookup"><span data-stu-id="10dec-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="10dec-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="10dec-141">Schema Name</span></span>  <br/> |<span data-ttu-id="10dec-142">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="10dec-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="10dec-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="10dec-143">Validation File</span></span>  <br/> |<span data-ttu-id="10dec-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="10dec-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="10dec-145">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="10dec-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="10dec-146">False</span><span class="sxs-lookup"><span data-stu-id="10dec-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="10dec-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="10dec-147">See also</span></span>



- [<span data-ttu-id="10dec-148">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="10dec-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


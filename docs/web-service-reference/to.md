---
title: 宛先
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
description: To 要素は、タイムゾーン遷移のターゲットを指定します。 目標は、タイムゾーンの期間またはタイムゾーンの移行のグループのいずれかです。
ms.openlocfilehash: 8cce700eedd64035f2e21be4db6b517f3f85d98d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468797"
---
# <a name="to"></a><span data-ttu-id="99164-104">宛先</span><span class="sxs-lookup"><span data-stu-id="99164-104">To</span></span>

<span data-ttu-id="99164-105">**To**要素は、タイムゾーン遷移のターゲットを指定します。</span><span class="sxs-lookup"><span data-stu-id="99164-105">The **To** element specifies the target of the time zone transition.</span></span> <span data-ttu-id="99164-106">目標は、タイムゾーンの期間またはタイムゾーンの移行のグループのいずれかです。</span><span class="sxs-lookup"><span data-stu-id="99164-106">The target is either a time zone period or a group of time zone transitions.</span></span> 
  
```xml
<To Kind=""/>
```

 <span data-ttu-id="99164-107">**遷移 Tiontargettype**</span><span class="sxs-lookup"><span data-stu-id="99164-107">**TransitionTargetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="99164-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="99164-108">Attributes and elements</span></span>

<span data-ttu-id="99164-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="99164-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99164-110">属性</span><span class="sxs-lookup"><span data-stu-id="99164-110">Attributes</span></span>

|<span data-ttu-id="99164-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="99164-111">**Attribute**</span></span>|<span data-ttu-id="99164-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="99164-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="99164-113">Kind</span><span class="sxs-lookup"><span data-stu-id="99164-113">Kind</span></span>  <br/> |<span data-ttu-id="99164-114">タイムゾーンの移行対象がタイムゾーンの期間であるか、またはタイムゾーンの切り替えのグループであるかを示します。</span><span class="sxs-lookup"><span data-stu-id="99164-114">Indicates whether the time zone transition target is a time zone period or of a group of time zone transitions.</span></span>  <br/> |
   
#### <a name="kind-attribute-values"></a><span data-ttu-id="99164-115">Kind 属性値</span><span class="sxs-lookup"><span data-stu-id="99164-115">Kind attribute values</span></span>

|<span data-ttu-id="99164-116">**値**</span><span class="sxs-lookup"><span data-stu-id="99164-116">**Value**</span></span>|<span data-ttu-id="99164-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="99164-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="99164-118">ピリオド</span><span class="sxs-lookup"><span data-stu-id="99164-118">Period</span></span>  <br/> |<span data-ttu-id="99164-119">タイムゾーンの移行ターゲットがタイムゾーンの期間であることを指定します。</span><span class="sxs-lookup"><span data-stu-id="99164-119">Specifies that the time zone transition target is a time zone period.</span></span>  <br/> |
|<span data-ttu-id="99164-120">Group</span><span class="sxs-lookup"><span data-stu-id="99164-120">Group</span></span>  <br/> |<span data-ttu-id="99164-121">タイムゾーンの移行ターゲットが、タイムゾーン遷移のグループであることを指定します。</span><span class="sxs-lookup"><span data-stu-id="99164-121">Specifies that the time zone transition target is a group of time zone transitions.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="99164-122">子要素</span><span class="sxs-lookup"><span data-stu-id="99164-122">Child elements</span></span>

<span data-ttu-id="99164-123">なし。</span><span class="sxs-lookup"><span data-stu-id="99164-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="99164-124">親要素</span><span class="sxs-lookup"><span data-stu-id="99164-124">Parent elements</span></span>

|<span data-ttu-id="99164-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="99164-125">**Element**</span></span>|<span data-ttu-id="99164-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="99164-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99164-127">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="99164-127">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="99164-128">特定の日付および特定の時刻に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="99164-128">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="99164-129">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="99164-129">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="99164-130">毎年同じ日に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="99164-130">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="99164-131">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="99164-131">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="99164-132">指定した日に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="99164-132">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
|[<span data-ttu-id="99164-133">Transition</span><span class="sxs-lookup"><span data-stu-id="99164-133">Transition</span></span>](transition.md) <br/> |<span data-ttu-id="99164-134">タイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="99164-134">Represents a time zone transition.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="99164-135">テキスト値</span><span class="sxs-lookup"><span data-stu-id="99164-135">Text value</span></span>

<span data-ttu-id="99164-136">テキスト値は、期間または時間帯遷移のターゲットである[期間](period.md)または[推移 tionsgroup](transitionsgroup.md)の一意の識別子を指定する文字列です。</span><span class="sxs-lookup"><span data-stu-id="99164-136">The text value is a string that specifies the unique identifier of the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="99164-137">注釈</span><span class="sxs-lookup"><span data-stu-id="99164-137">Remarks</span></span>

<span data-ttu-id="99164-138">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="99164-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="99164-139">要素の情報</span><span class="sxs-lookup"><span data-stu-id="99164-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="99164-140">名前空間</span><span class="sxs-lookup"><span data-stu-id="99164-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="99164-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="99164-141">Schema Name</span></span>  <br/> |<span data-ttu-id="99164-142">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="99164-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="99164-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="99164-143">Validation File</span></span>  <br/> |<span data-ttu-id="99164-144">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="99164-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="99164-145">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="99164-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="99164-146">正しくない</span><span class="sxs-lookup"><span data-stu-id="99164-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="99164-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="99164-147">See also</span></span>



- [<span data-ttu-id="99164-148">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="99164-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


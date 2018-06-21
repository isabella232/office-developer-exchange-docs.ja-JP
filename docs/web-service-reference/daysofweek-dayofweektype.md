---
title: DaysOfWeek (DayOfWeekType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DaysOfWeek
api_type:
- schema
ms.assetid: ba8f990d-d37d-403d-b31f-55e5208c8ad5
description: DaysOfWeek 要素では、項目の定期的なパターンで使用されている週の日について説明します。
ms.openlocfilehash: a7afb0aeb650284739d559164f06590fc5266c57
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/21/2018
ms.locfileid: "19759946"
---
# <a name="daysofweek-dayofweektype"></a><span data-ttu-id="6bcdf-103">DaysOfWeek (DayOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="6bcdf-103">DaysOfWeek (DayOfWeekType)</span></span>

<span data-ttu-id="6bcdf-104">**DaysOfWeek**要素では、項目の定期的なパターンで使用されている週の日について説明します。</span><span class="sxs-lookup"><span data-stu-id="6bcdf-104">The **DaysOfWeek** element describes days of the week that are used in item recurrence patterns.</span></span> 
  
```xml
<DaysOfWeek/>
```

<span data-ttu-id="6bcdf-105">**DayOfWeekType**</span><span class="sxs-lookup"><span data-stu-id="6bcdf-105">**DayOfWeekType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6bcdf-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6bcdf-106">Attributes and elements</span></span>

<span data-ttu-id="6bcdf-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6bcdf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6bcdf-108">属性</span><span class="sxs-lookup"><span data-stu-id="6bcdf-108">Attributes</span></span>

<span data-ttu-id="6bcdf-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6bcdf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6bcdf-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6bcdf-110">Child elements</span></span>

<span data-ttu-id="6bcdf-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6bcdf-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6bcdf-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6bcdf-112">Parent elements</span></span>

|<span data-ttu-id="6bcdf-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6bcdf-113">**Element**</span></span>|<span data-ttu-id="6bcdf-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6bcdf-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6bcdf-115">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="6bcdf-115">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="6bcdf-116">相対年間の定期的なパターンをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="6bcdf-116">Describes a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="6bcdf-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="6bcdf-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="6bcdf-118">相対的な毎月の定期的なパターンをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="6bcdf-118">Describes a relative monthly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6bcdf-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6bcdf-119">Text value</span></span>

<span data-ttu-id="6bcdf-120">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="6bcdf-120">A text value is required.</span></span> <span data-ttu-id="6bcdf-121">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="6bcdf-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="6bcdf-122">日曜日</span><span class="sxs-lookup"><span data-stu-id="6bcdf-122">Sunday</span></span>    
- <span data-ttu-id="6bcdf-123">月曜日</span><span class="sxs-lookup"><span data-stu-id="6bcdf-123">Monday</span></span>    
- <span data-ttu-id="6bcdf-124">火曜日</span><span class="sxs-lookup"><span data-stu-id="6bcdf-124">Tuesday</span></span>   
- <span data-ttu-id="6bcdf-125">水曜日</span><span class="sxs-lookup"><span data-stu-id="6bcdf-125">Wednesday</span></span>    
- <span data-ttu-id="6bcdf-126">木曜日</span><span class="sxs-lookup"><span data-stu-id="6bcdf-126">Thursday</span></span>    
- <span data-ttu-id="6bcdf-127">金曜日</span><span class="sxs-lookup"><span data-stu-id="6bcdf-127">Friday</span></span>    
- <span data-ttu-id="6bcdf-128">土曜日</span><span class="sxs-lookup"><span data-stu-id="6bcdf-128">Saturday</span></span>    
- <span data-ttu-id="6bcdf-129">(、TimeChangePatternTypes では使用されません) の日</span><span class="sxs-lookup"><span data-stu-id="6bcdf-129">Day (not used in the TimeChangePatternTypes)</span></span>    
- <span data-ttu-id="6bcdf-130">(、TimeChangePatternTypes では使用されません) の平日</span><span class="sxs-lookup"><span data-stu-id="6bcdf-130">Weekday (not used in the TimeChangePatternTypes)</span></span>    
- <span data-ttu-id="6bcdf-131">(、TimeChangePatternTypes では使用されません) WeekendDay</span><span class="sxs-lookup"><span data-stu-id="6bcdf-131">WeekendDay (not used in the TimeChangePatternTypes)</span></span>
    
## <a name="remarks"></a><span data-ttu-id="6bcdf-132">備考</span><span class="sxs-lookup"><span data-stu-id="6bcdf-132">Remarks</span></span>

<span data-ttu-id="6bcdf-133">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6bcdf-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6bcdf-134">要素情報</span><span class="sxs-lookup"><span data-stu-id="6bcdf-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6bcdf-135">名前空間</span><span class="sxs-lookup"><span data-stu-id="6bcdf-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6bcdf-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6bcdf-136">Schema Name</span></span>  <br/> |<span data-ttu-id="6bcdf-137">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6bcdf-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="6bcdf-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6bcdf-138">Validation File</span></span>  <br/> |<span data-ttu-id="6bcdf-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6bcdf-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6bcdf-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6bcdf-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="6bcdf-141">False</span><span class="sxs-lookup"><span data-stu-id="6bcdf-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6bcdf-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="6bcdf-142">See also</span></span>

- [<span data-ttu-id="6bcdf-143">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6bcdf-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


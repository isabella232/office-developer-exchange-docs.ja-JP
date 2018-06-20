---
title: DaysOfWeek (DaysOfWeekType)
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
ms.assetid: c56f997d-28f3-4590-97b0-cb71f016dbe4
description: DaysOfWeek 要素では、項目の定期的なパターンで使用されている週の日について説明します。
ms.openlocfilehash: 0b730ff5a7bc9aa6b324fc080022d056c5342296
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759945"
---
# <a name="daysofweek-daysofweektype"></a><span data-ttu-id="67f9b-103">DaysOfWeek (DaysOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="67f9b-103">DaysOfWeek (DaysOfWeekType)</span></span>

<span data-ttu-id="67f9b-104">**DaysOfWeek**要素では、項目の定期的なパターンで使用されている週の日について説明します。</span><span class="sxs-lookup"><span data-stu-id="67f9b-104">The **DaysOfWeek** element describes days of the week that are used in item recurrence patterns.</span></span> 
  
```XML
<DaysOfWeek/>
```

<span data-ttu-id="67f9b-105">**DaysOfWeekType**</span><span class="sxs-lookup"><span data-stu-id="67f9b-105">**DaysOfWeekType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="67f9b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="67f9b-106">Attributes and elements</span></span>

<span data-ttu-id="67f9b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="67f9b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="67f9b-108">属性</span><span class="sxs-lookup"><span data-stu-id="67f9b-108">Attributes</span></span>

<span data-ttu-id="67f9b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="67f9b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="67f9b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="67f9b-110">Child elements</span></span>

<span data-ttu-id="67f9b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="67f9b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="67f9b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="67f9b-112">Parent elements</span></span>

|<span data-ttu-id="67f9b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="67f9b-113">**Element**</span></span>|<span data-ttu-id="67f9b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="67f9b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67f9b-115">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="67f9b-115">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="67f9b-116">毎週の定期的なパターンをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="67f9b-116">Describes a weekly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="67f9b-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="67f9b-117">Text value</span></span>

<span data-ttu-id="67f9b-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="67f9b-118">A text value is required.</span></span> <span data-ttu-id="67f9b-119">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="67f9b-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="67f9b-120">日曜日</span><span class="sxs-lookup"><span data-stu-id="67f9b-120">Sunday</span></span>    
- <span data-ttu-id="67f9b-121">月曜日</span><span class="sxs-lookup"><span data-stu-id="67f9b-121">Monday</span></span>    
- <span data-ttu-id="67f9b-122">火曜日</span><span class="sxs-lookup"><span data-stu-id="67f9b-122">Tuesday</span></span>    
- <span data-ttu-id="67f9b-123">水曜日</span><span class="sxs-lookup"><span data-stu-id="67f9b-123">Wednesday</span></span>    
- <span data-ttu-id="67f9b-124">木曜日</span><span class="sxs-lookup"><span data-stu-id="67f9b-124">Thursday</span></span>    
- <span data-ttu-id="67f9b-125">金曜日</span><span class="sxs-lookup"><span data-stu-id="67f9b-125">Friday</span></span>    
- <span data-ttu-id="67f9b-126">土曜日</span><span class="sxs-lookup"><span data-stu-id="67f9b-126">Saturday</span></span>    
- <span data-ttu-id="67f9b-127">(この値は毎週の定期的なパターンに対して有効ではありません) の日</span><span class="sxs-lookup"><span data-stu-id="67f9b-127">Day (this value is not valid for a weekly recurrence pattern)</span></span>    
- <span data-ttu-id="67f9b-128">(この値は毎週の定期的なパターンに対して有効ではありません) の平日</span><span class="sxs-lookup"><span data-stu-id="67f9b-128">Weekday (this value is not valid for a weekly recurrence pattern)</span></span>    
- <span data-ttu-id="67f9b-129">(この値は毎週の定期的なパターンに対して有効ではありません) WeekendDay</span><span class="sxs-lookup"><span data-stu-id="67f9b-129">WeekendDay (this value is not valid for a weekly recurrence pattern)</span></span>
    
<span data-ttu-id="67f9b-130">毎週の定期的なパターンでは、複数の値を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="67f9b-130">A weekly recurrence pattern can contain multiple values.</span></span> <span data-ttu-id="67f9b-131">値は、空白文字で区切られます。</span><span class="sxs-lookup"><span data-stu-id="67f9b-131">Values are separated by a space character.</span></span> <span data-ttu-id="67f9b-132">たとえば、火曜日と木曜日の毎週、テキスト値に「火曜日木曜日」です。</span><span class="sxs-lookup"><span data-stu-id="67f9b-132">For example, for a weekly recurrence on Tuesdays and Thursdays, the text value will be "Tuesday Thursday".</span></span>
  
## <a name="remarks"></a><span data-ttu-id="67f9b-133">備考</span><span class="sxs-lookup"><span data-stu-id="67f9b-133">Remarks</span></span>

<span data-ttu-id="67f9b-134">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="67f9b-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="67f9b-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="67f9b-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67f9b-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="67f9b-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="67f9b-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="67f9b-137">Schema Name</span></span>  <br/> |<span data-ttu-id="67f9b-138">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="67f9b-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="67f9b-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="67f9b-139">Validation File</span></span>  <br/> |<span data-ttu-id="67f9b-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="67f9b-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="67f9b-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="67f9b-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="67f9b-142">False</span><span class="sxs-lookup"><span data-stu-id="67f9b-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="67f9b-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="67f9b-143">See also</span></span>

- [<span data-ttu-id="67f9b-144">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="67f9b-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


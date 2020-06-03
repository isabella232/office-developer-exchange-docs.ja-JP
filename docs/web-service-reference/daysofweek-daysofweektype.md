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
description: DaysOfWeek 要素は、アイテムの定期的なパターンで使用される曜日を表します。
ms.openlocfilehash: 3036cbe3f93ff87b9a4d5dc7bf164e3e952b06fd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463721"
---
# <a name="daysofweek-daysofweektype"></a><span data-ttu-id="80c41-103">DaysOfWeek (DaysOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="80c41-103">DaysOfWeek (DaysOfWeekType)</span></span>

<span data-ttu-id="80c41-104">**DaysOfWeek**要素は、アイテムの定期的なパターンで使用される曜日を表します。</span><span class="sxs-lookup"><span data-stu-id="80c41-104">The **DaysOfWeek** element describes days of the week that are used in item recurrence patterns.</span></span> 
  
```XML
<DaysOfWeek/>
```

<span data-ttu-id="80c41-105">**DaysOfWeekType**</span><span class="sxs-lookup"><span data-stu-id="80c41-105">**DaysOfWeekType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="80c41-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="80c41-106">Attributes and elements</span></span>

<span data-ttu-id="80c41-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="80c41-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80c41-108">属性</span><span class="sxs-lookup"><span data-stu-id="80c41-108">Attributes</span></span>

<span data-ttu-id="80c41-109">なし。</span><span class="sxs-lookup"><span data-stu-id="80c41-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80c41-110">子要素</span><span class="sxs-lookup"><span data-stu-id="80c41-110">Child elements</span></span>

<span data-ttu-id="80c41-111">なし。</span><span class="sxs-lookup"><span data-stu-id="80c41-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="80c41-112">親要素</span><span class="sxs-lookup"><span data-stu-id="80c41-112">Parent elements</span></span>

|<span data-ttu-id="80c41-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="80c41-113">**Element**</span></span>|<span data-ttu-id="80c41-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="80c41-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80c41-115">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="80c41-115">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="80c41-116">週単位の定期的なパターンを記述します。</span><span class="sxs-lookup"><span data-stu-id="80c41-116">Describes a weekly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="80c41-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="80c41-117">Text value</span></span>

<span data-ttu-id="80c41-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="80c41-118">A text value is required.</span></span> <span data-ttu-id="80c41-119">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="80c41-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="80c41-120">日曜日</span><span class="sxs-lookup"><span data-stu-id="80c41-120">Sunday</span></span>    
- <span data-ttu-id="80c41-121">月曜日</span><span class="sxs-lookup"><span data-stu-id="80c41-121">Monday</span></span>    
- <span data-ttu-id="80c41-122">火曜日</span><span class="sxs-lookup"><span data-stu-id="80c41-122">Tuesday</span></span>    
- <span data-ttu-id="80c41-123">水曜日</span><span class="sxs-lookup"><span data-stu-id="80c41-123">Wednesday</span></span>    
- <span data-ttu-id="80c41-124">木曜日</span><span class="sxs-lookup"><span data-stu-id="80c41-124">Thursday</span></span>    
- <span data-ttu-id="80c41-125">金曜日</span><span class="sxs-lookup"><span data-stu-id="80c41-125">Friday</span></span>    
- <span data-ttu-id="80c41-126">土曜日</span><span class="sxs-lookup"><span data-stu-id="80c41-126">Saturday</span></span>    
- <span data-ttu-id="80c41-127">Day (この値は、週単位の定期的なパターンに対しては無効です)</span><span class="sxs-lookup"><span data-stu-id="80c41-127">Day (this value is not valid for a weekly recurrence pattern)</span></span>    
- <span data-ttu-id="80c41-128">Weekday (この値は、週単位の定期的なパターンに対しては無効です)</span><span class="sxs-lookup"><span data-stu-id="80c41-128">Weekday (this value is not valid for a weekly recurrence pattern)</span></span>    
- <span data-ttu-id="80c41-129">WeekendDay (この値は、週単位の定期的なパターンに対しては無効です)</span><span class="sxs-lookup"><span data-stu-id="80c41-129">WeekendDay (this value is not valid for a weekly recurrence pattern)</span></span>
    
<span data-ttu-id="80c41-130">週単位の定期的なパターンでは、複数の値を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="80c41-130">A weekly recurrence pattern can contain multiple values.</span></span> <span data-ttu-id="80c41-131">値は空白文字で区切られます。</span><span class="sxs-lookup"><span data-stu-id="80c41-131">Values are separated by a space character.</span></span> <span data-ttu-id="80c41-132">たとえば、火曜日と木曜日の週単位の定期的な予定の場合、テキスト値は "火曜日木曜日" になります。</span><span class="sxs-lookup"><span data-stu-id="80c41-132">For example, for a weekly recurrence on Tuesdays and Thursdays, the text value will be "Tuesday Thursday".</span></span>
  
## <a name="remarks"></a><span data-ttu-id="80c41-133">注釈</span><span class="sxs-lookup"><span data-stu-id="80c41-133">Remarks</span></span>

<span data-ttu-id="80c41-134">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="80c41-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="80c41-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="80c41-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80c41-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="80c41-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="80c41-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="80c41-137">Schema Name</span></span>  <br/> |<span data-ttu-id="80c41-138">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="80c41-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="80c41-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="80c41-139">Validation File</span></span>  <br/> |<span data-ttu-id="80c41-140">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="80c41-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="80c41-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="80c41-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="80c41-142">正しくない</span><span class="sxs-lookup"><span data-stu-id="80c41-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="80c41-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="80c41-143">See also</span></span>

- [<span data-ttu-id="80c41-144">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="80c41-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


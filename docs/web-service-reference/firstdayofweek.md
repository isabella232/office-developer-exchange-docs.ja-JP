---
title: FirstDayOfWeek
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FirstDayOfWeek
api_type:
- schema
ms.assetid: d6cf1bd3-a19b-4d5f-9e25-8e337a4939e0
description: FirstDayOfWeek の要素では、週の最初の日を指定します。
ms.openlocfilehash: 99858d17213d077ce7c51ad1c746588f2f3939a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760544"
---
# <a name="firstdayofweek"></a><span data-ttu-id="ef3bc-103">FirstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="ef3bc-103">FirstDayOfWeek</span></span>

<span data-ttu-id="ef3bc-104">**FirstDayOfWeek**の要素では、週の最初の日を指定します。</span><span class="sxs-lookup"><span data-stu-id="ef3bc-104">The **FirstDayOfWeek** element specifies the first day of the week.</span></span> 
  
```XML
<FirstDayOfWeek> Sunday | Monday | Tuesday | Wednesday | Thursday | Friday | Saturday</FirstDayOfWeek>
```

 <span data-ttu-id="ef3bc-105">**DayOfWeekType**</span><span class="sxs-lookup"><span data-stu-id="ef3bc-105">**DayOfWeekType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ef3bc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ef3bc-106">Attributes and elements</span></span>

<span data-ttu-id="ef3bc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ef3bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef3bc-108">属性</span><span class="sxs-lookup"><span data-stu-id="ef3bc-108">Attributes</span></span>

<span data-ttu-id="ef3bc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ef3bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ef3bc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ef3bc-110">Child elements</span></span>

<span data-ttu-id="ef3bc-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ef3bc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ef3bc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ef3bc-112">Parent elements</span></span>

|<span data-ttu-id="ef3bc-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ef3bc-113">**Element**</span></span>|<span data-ttu-id="ef3bc-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ef3bc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef3bc-115">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="ef3bc-115">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="ef3bc-116">毎週の定期的なパターンをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="ef3bc-116">Describes a weekly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ef3bc-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ef3bc-117">Text value</span></span>

<span data-ttu-id="ef3bc-118">**FirstDayOfWeek**要素のテキスト値は、週の曜日が週の最初の日として使用されることを示します。</span><span class="sxs-lookup"><span data-stu-id="ef3bc-118">The text value of the **FirstDayOfWeek** element indicates which day of the week is used as the first day of the week.</span></span> <span data-ttu-id="ef3bc-119">可能なテキスト値は、次のように。</span><span class="sxs-lookup"><span data-stu-id="ef3bc-119">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="ef3bc-120">日曜日</span><span class="sxs-lookup"><span data-stu-id="ef3bc-120">Sunday</span></span>
    
- <span data-ttu-id="ef3bc-121">月曜日</span><span class="sxs-lookup"><span data-stu-id="ef3bc-121">Monday</span></span>
    
- <span data-ttu-id="ef3bc-122">火曜日</span><span class="sxs-lookup"><span data-stu-id="ef3bc-122">Tuesday</span></span>
    
- <span data-ttu-id="ef3bc-123">水曜日</span><span class="sxs-lookup"><span data-stu-id="ef3bc-123">Wednesday</span></span>
    
- <span data-ttu-id="ef3bc-124">木曜日</span><span class="sxs-lookup"><span data-stu-id="ef3bc-124">Thursday</span></span>
    
- <span data-ttu-id="ef3bc-125">金曜日</span><span class="sxs-lookup"><span data-stu-id="ef3bc-125">Friday</span></span>
    
- <span data-ttu-id="ef3bc-126">土曜日</span><span class="sxs-lookup"><span data-stu-id="ef3bc-126">Saturday</span></span>
    
## <a name="remarks"></a><span data-ttu-id="ef3bc-127">備考</span><span class="sxs-lookup"><span data-stu-id="ef3bc-127">Remarks</span></span>

<span data-ttu-id="ef3bc-128">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="ef3bc-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ef3bc-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="ef3bc-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef3bc-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="ef3bc-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ef3bc-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ef3bc-131">Schema Name</span></span>  <br/> |<span data-ttu-id="ef3bc-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ef3bc-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="ef3bc-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ef3bc-133">Validation File</span></span>  <br/> |<span data-ttu-id="ef3bc-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ef3bc-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ef3bc-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ef3bc-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="ef3bc-136">False</span><span class="sxs-lookup"><span data-stu-id="ef3bc-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ef3bc-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="ef3bc-137">See also</span></span>



- [<span data-ttu-id="ef3bc-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ef3bc-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


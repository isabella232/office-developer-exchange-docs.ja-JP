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
description: FirstDayOfWeek 要素は、週の最初の曜日を指定します。
ms.openlocfilehash: 1b4aee8e1ce2548cd6b0047623b0bcda47ad316b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530973"
---
# <a name="firstdayofweek"></a><span data-ttu-id="16462-103">FirstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="16462-103">FirstDayOfWeek</span></span>

<span data-ttu-id="16462-104">**FirstDayOfWeek**要素は、週の最初の曜日を指定します。</span><span class="sxs-lookup"><span data-stu-id="16462-104">The **FirstDayOfWeek** element specifies the first day of the week.</span></span> 
  
```XML
<FirstDayOfWeek> Sunday | Monday | Tuesday | Wednesday | Thursday | Friday | Saturday</FirstDayOfWeek>
```

 <span data-ttu-id="16462-105">**DayOfWeekType**</span><span class="sxs-lookup"><span data-stu-id="16462-105">**DayOfWeekType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="16462-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="16462-106">Attributes and elements</span></span>

<span data-ttu-id="16462-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="16462-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16462-108">属性</span><span class="sxs-lookup"><span data-stu-id="16462-108">Attributes</span></span>

<span data-ttu-id="16462-109">なし。</span><span class="sxs-lookup"><span data-stu-id="16462-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="16462-110">子要素</span><span class="sxs-lookup"><span data-stu-id="16462-110">Child elements</span></span>

<span data-ttu-id="16462-111">なし。</span><span class="sxs-lookup"><span data-stu-id="16462-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="16462-112">親要素</span><span class="sxs-lookup"><span data-stu-id="16462-112">Parent elements</span></span>

|<span data-ttu-id="16462-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="16462-113">**Element**</span></span>|<span data-ttu-id="16462-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="16462-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16462-115">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="16462-115">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="16462-116">週単位の定期的なパターンを記述します。</span><span class="sxs-lookup"><span data-stu-id="16462-116">Describes a weekly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="16462-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="16462-117">Text value</span></span>

<span data-ttu-id="16462-118">**FirstDayOfWeek**要素のテキスト値は、週の最初の曜日として使用される曜日を示します。</span><span class="sxs-lookup"><span data-stu-id="16462-118">The text value of the **FirstDayOfWeek** element indicates which day of the week is used as the first day of the week.</span></span> <span data-ttu-id="16462-119">可能なテキスト値を次に示します。</span><span class="sxs-lookup"><span data-stu-id="16462-119">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="16462-120">日曜日</span><span class="sxs-lookup"><span data-stu-id="16462-120">Sunday</span></span>
    
- <span data-ttu-id="16462-121">月曜日</span><span class="sxs-lookup"><span data-stu-id="16462-121">Monday</span></span>
    
- <span data-ttu-id="16462-122">火曜日</span><span class="sxs-lookup"><span data-stu-id="16462-122">Tuesday</span></span>
    
- <span data-ttu-id="16462-123">水曜日</span><span class="sxs-lookup"><span data-stu-id="16462-123">Wednesday</span></span>
    
- <span data-ttu-id="16462-124">木曜日</span><span class="sxs-lookup"><span data-stu-id="16462-124">Thursday</span></span>
    
- <span data-ttu-id="16462-125">金曜日</span><span class="sxs-lookup"><span data-stu-id="16462-125">Friday</span></span>
    
- <span data-ttu-id="16462-126">土曜日</span><span class="sxs-lookup"><span data-stu-id="16462-126">Saturday</span></span>
    
## <a name="remarks"></a><span data-ttu-id="16462-127">注釈</span><span class="sxs-lookup"><span data-stu-id="16462-127">Remarks</span></span>

<span data-ttu-id="16462-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="16462-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="16462-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="16462-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16462-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="16462-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="16462-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="16462-131">Schema Name</span></span>  <br/> |<span data-ttu-id="16462-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="16462-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="16462-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="16462-133">Validation File</span></span>  <br/> |<span data-ttu-id="16462-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="16462-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="16462-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="16462-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="16462-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="16462-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="16462-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="16462-137">See also</span></span>



- [<span data-ttu-id="16462-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="16462-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


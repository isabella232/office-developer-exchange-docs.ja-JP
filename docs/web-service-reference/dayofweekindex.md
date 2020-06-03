---
title: DayOfWeekIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeekIndex
api_type:
- schema
ms.assetid: 82420338-a1f7-4887-b338-b2d93b2c2bf1
description: DayOfWeekIndex 要素は、相対的な定期的なパターンで使用される月の週を示します。
ms.openlocfilehash: c9235d83a944f9c8883439dd2adf190b88977f16
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529211"
---
# <a name="dayofweekindex"></a><span data-ttu-id="27529-103">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="27529-103">DayOfWeekIndex</span></span>

<span data-ttu-id="27529-104">**DayOfWeekIndex**要素は、相対的な定期的なパターンで使用される月の週を示します。</span><span class="sxs-lookup"><span data-stu-id="27529-104">The **DayOfWeekIndex** element describes which week in a month is used in a relative recurrence pattern.</span></span> 
  
```xml
<DayOfWeekIndex/>
```

<span data-ttu-id="27529-105">**DayOfWeekIndexType**</span><span class="sxs-lookup"><span data-stu-id="27529-105">**DayOfWeekIndexType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="27529-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="27529-106">Attributes and elements</span></span>

<span data-ttu-id="27529-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="27529-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27529-108">属性</span><span class="sxs-lookup"><span data-stu-id="27529-108">Attributes</span></span>

<span data-ttu-id="27529-109">なし。</span><span class="sxs-lookup"><span data-stu-id="27529-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27529-110">子要素</span><span class="sxs-lookup"><span data-stu-id="27529-110">Child elements</span></span>

<span data-ttu-id="27529-111">なし。</span><span class="sxs-lookup"><span data-stu-id="27529-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="27529-112">親要素</span><span class="sxs-lookup"><span data-stu-id="27529-112">Parent elements</span></span>

|<span data-ttu-id="27529-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="27529-113">**Element**</span></span>|<span data-ttu-id="27529-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="27529-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27529-115">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="27529-115">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="27529-116">相対的な年単位の定期的なパターンを記述します。</span><span class="sxs-lookup"><span data-stu-id="27529-116">Describes a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="27529-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="27529-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="27529-118">相対的な月単位の定期的なパターンを記述します。</span><span class="sxs-lookup"><span data-stu-id="27529-118">Describes a relative monthly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="27529-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="27529-119">Text value</span></span>

<span data-ttu-id="27529-120">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="27529-120">A text value is required.</span></span> <span data-ttu-id="27529-121">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="27529-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="27529-122">第 1</span><span class="sxs-lookup"><span data-stu-id="27529-122">First</span></span>    
- <span data-ttu-id="27529-123">秒</span><span class="sxs-lookup"><span data-stu-id="27529-123">Second</span></span>    
- <span data-ttu-id="27529-124">第 3</span><span class="sxs-lookup"><span data-stu-id="27529-124">Third</span></span>    
- <span data-ttu-id="27529-125">第 4</span><span class="sxs-lookup"><span data-stu-id="27529-125">Fourth</span></span>    
- <span data-ttu-id="27529-126">末尾</span><span class="sxs-lookup"><span data-stu-id="27529-126">Last</span></span>
    
## <a name="remarks"></a><span data-ttu-id="27529-127">注釈</span><span class="sxs-lookup"><span data-stu-id="27529-127">Remarks</span></span>

<span data-ttu-id="27529-128">たとえば、月の第2月曜日は、その月の第3週に発生する場合があります。</span><span class="sxs-lookup"><span data-stu-id="27529-128">For example, the second Monday of a month may occur in the third week of that month.</span></span> <span data-ttu-id="27529-129">1か月の金曜日に開始する場合、その月の最初の週には数日だけが含まれ、月曜日は含まれません。</span><span class="sxs-lookup"><span data-stu-id="27529-129">If a month starts on a Friday, the first week of the month only contains a few days and does not contain a Monday.</span></span> <span data-ttu-id="27529-130">そのため、最初の月曜日は2週間以内に実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="27529-130">Therefore, the first Monday would have to occur in the second week.</span></span>
  
<span data-ttu-id="27529-131">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="27529-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27529-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="27529-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27529-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="27529-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="27529-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="27529-134">Schema name</span></span>  <br/> |<span data-ttu-id="27529-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="27529-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="27529-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="27529-136">Validation file</span></span>  <br/> |<span data-ttu-id="27529-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="27529-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="27529-138">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="27529-138">Can be empty</span></span>  <br/> |<span data-ttu-id="27529-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="27529-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27529-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="27529-140">See also</span></span>

- [<span data-ttu-id="27529-141">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="27529-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


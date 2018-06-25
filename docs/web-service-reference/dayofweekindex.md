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
description: DayOfWeekIndex 要素は、1 か月の週が相対的な定期的なパターンの使用について説明します。
ms.openlocfilehash: 4987685d0c3cefdfad4f5be1368776a5b859bf94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759941"
---
# <a name="dayofweekindex"></a><span data-ttu-id="378fe-103">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="378fe-103">DayOfWeekIndex</span></span>

<span data-ttu-id="378fe-104">**DayOfWeekIndex**要素は、1 か月の週が相対的な定期的なパターンの使用について説明します。</span><span class="sxs-lookup"><span data-stu-id="378fe-104">The **DayOfWeekIndex** element describes which week in a month is used in a relative recurrence pattern.</span></span> 
  
```xml
<DayOfWeekIndex/>
```

<span data-ttu-id="378fe-105">**DayOfWeekIndexType**</span><span class="sxs-lookup"><span data-stu-id="378fe-105">**DayOfWeekIndexType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="378fe-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="378fe-106">Attributes and elements</span></span>

<span data-ttu-id="378fe-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="378fe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="378fe-108">属性</span><span class="sxs-lookup"><span data-stu-id="378fe-108">Attributes</span></span>

<span data-ttu-id="378fe-109">なし。</span><span class="sxs-lookup"><span data-stu-id="378fe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="378fe-110">子要素</span><span class="sxs-lookup"><span data-stu-id="378fe-110">Child elements</span></span>

<span data-ttu-id="378fe-111">なし。</span><span class="sxs-lookup"><span data-stu-id="378fe-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="378fe-112">親要素</span><span class="sxs-lookup"><span data-stu-id="378fe-112">Parent elements</span></span>

|<span data-ttu-id="378fe-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="378fe-113">**Element**</span></span>|<span data-ttu-id="378fe-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="378fe-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="378fe-115">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="378fe-115">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="378fe-116">相対年間の定期的なパターンをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="378fe-116">Describes a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="378fe-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="378fe-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="378fe-118">相対的な毎月の定期的なパターンをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="378fe-118">Describes a relative monthly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="378fe-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="378fe-119">Text value</span></span>

<span data-ttu-id="378fe-120">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="378fe-120">A text value is required.</span></span> <span data-ttu-id="378fe-121">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="378fe-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="378fe-122">第 1</span><span class="sxs-lookup"><span data-stu-id="378fe-122">First</span></span>    
- <span data-ttu-id="378fe-123">第 2</span><span class="sxs-lookup"><span data-stu-id="378fe-123">Second</span></span>    
- <span data-ttu-id="378fe-124">第 3</span><span class="sxs-lookup"><span data-stu-id="378fe-124">Third</span></span>    
- <span data-ttu-id="378fe-125">第 4</span><span class="sxs-lookup"><span data-stu-id="378fe-125">Fourth</span></span>    
- <span data-ttu-id="378fe-126">末尾</span><span class="sxs-lookup"><span data-stu-id="378fe-126">Last</span></span>
    
## <a name="remarks"></a><span data-ttu-id="378fe-127">備考</span><span class="sxs-lookup"><span data-stu-id="378fe-127">Remarks</span></span>

<span data-ttu-id="378fe-128">たとえば、その月の第 3 週に 1 か月の第 2 月曜日に発生します。</span><span class="sxs-lookup"><span data-stu-id="378fe-128">For example, the second Monday of a month may occur in the third week of that month.</span></span> <span data-ttu-id="378fe-129">1 か月は、金曜日に起動する場合、月の最初の週、いくつかの日が含まれています、だけ月曜日が含まれていません。</span><span class="sxs-lookup"><span data-stu-id="378fe-129">If a month starts on a Friday, the first week of the month only contains a few days and does not contain a Monday.</span></span> <span data-ttu-id="378fe-130">したがって、第 1 月曜日は、第 2 週に発生する必要があります。</span><span class="sxs-lookup"><span data-stu-id="378fe-130">Therefore, the first Monday would have to occur in the second week.</span></span>
  
<span data-ttu-id="378fe-131">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="378fe-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="378fe-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="378fe-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="378fe-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="378fe-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="378fe-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="378fe-134">Schema name</span></span>  <br/> |<span data-ttu-id="378fe-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="378fe-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="378fe-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="378fe-136">Validation file</span></span>  <br/> |<span data-ttu-id="378fe-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="378fe-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="378fe-138">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="378fe-138">Can be empty</span></span>  <br/> |<span data-ttu-id="378fe-139">False</span><span class="sxs-lookup"><span data-stu-id="378fe-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="378fe-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="378fe-140">See also</span></span>

- [<span data-ttu-id="378fe-141">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="378fe-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


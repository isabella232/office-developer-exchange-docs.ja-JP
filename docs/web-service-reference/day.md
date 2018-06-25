---
title: 日
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Day
api_type:
- schema
ms.assetid: d3b2dc66-486a-41d1-bff3-606f0bf92715
description: Day 要素では、タイム ゾーンの切り替えが発生する月の 1 日を表します。
ms.openlocfilehash: 01d1bf7833a89c0bb9a2b1af95ec8dfc627336d9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759930"
---
# <a name="day"></a><span data-ttu-id="3404d-103">日</span><span class="sxs-lookup"><span data-stu-id="3404d-103">Day</span></span>

<span data-ttu-id="3404d-104">**Day**要素では、タイム ゾーンの切り替えが発生する月の 1 日を表します。</span><span class="sxs-lookup"><span data-stu-id="3404d-104">The **Day** element represents the day of the month on which the time zone transition occurs.</span></span> 
  
```xml
<Day/>
```

<span data-ttu-id="3404d-105">**int**</span><span class="sxs-lookup"><span data-stu-id="3404d-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3404d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3404d-106">Attributes and elements</span></span>

<span data-ttu-id="3404d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3404d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3404d-108">属性</span><span class="sxs-lookup"><span data-stu-id="3404d-108">Attributes</span></span>

<span data-ttu-id="3404d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3404d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3404d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3404d-110">Child elements</span></span>

<span data-ttu-id="3404d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3404d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3404d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3404d-112">Parent elements</span></span>

|<span data-ttu-id="3404d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="3404d-113">**Element**</span></span>|<span data-ttu-id="3404d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3404d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3404d-115">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="3404d-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="3404d-116">毎年特定の日に発生するタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="3404d-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3404d-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3404d-117">Text value</span></span>

<span data-ttu-id="3404d-118">**日付**要素のテキスト値は、タイム ゾーンの切り替えが発生する月の日付を表す整数です。</span><span class="sxs-lookup"><span data-stu-id="3404d-118">The text value of the **Day** element is an integer that represents the day of the month on which the time zone transition occurs.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3404d-119">備考</span><span class="sxs-lookup"><span data-stu-id="3404d-119">Remarks</span></span>

<span data-ttu-id="3404d-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3404d-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3404d-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="3404d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3404d-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="3404d-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3404d-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3404d-123">Schema Name</span></span>  <br/> |<span data-ttu-id="3404d-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="3404d-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="3404d-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3404d-125">Validation File</span></span>  <br/> |<span data-ttu-id="3404d-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3404d-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3404d-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3404d-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="3404d-128">False</span><span class="sxs-lookup"><span data-stu-id="3404d-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3404d-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="3404d-129">See also</span></span>

- [<span data-ttu-id="3404d-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3404d-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: DayOfMonth
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfMonth
api_type:
- schema
ms.assetid: 09b7504e-08d8-42f9-88cc-a2a37a2e2b8b
description: DayOfMonth 要素では、定期的なアイテムに発生する月の日について説明します。
ms.openlocfilehash: 0d0d95849a2562e06b88872b2857cc5e6ca67af3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759932"
---
# <a name="dayofmonth"></a><span data-ttu-id="f2e83-103">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="f2e83-103">DayOfMonth</span></span>

<span data-ttu-id="f2e83-104">**DayOfMonth**要素では、定期的なアイテムに発生する月の日について説明します。</span><span class="sxs-lookup"><span data-stu-id="f2e83-104">The **DayOfMonth** element describes the day in a month that a recurring item occurs.</span></span> 
  
```xml
<DayOfMonth/>
```

<span data-ttu-id="f2e83-105">**int**</span><span class="sxs-lookup"><span data-stu-id="f2e83-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f2e83-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f2e83-106">Attributes and elements</span></span>

<span data-ttu-id="f2e83-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f2e83-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2e83-108">属性</span><span class="sxs-lookup"><span data-stu-id="f2e83-108">Attributes</span></span>

<span data-ttu-id="f2e83-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f2e83-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2e83-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f2e83-110">Child elements</span></span>

<span data-ttu-id="f2e83-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f2e83-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f2e83-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f2e83-112">Parent elements</span></span>

|<span data-ttu-id="f2e83-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f2e83-113">**Element**</span></span>|<span data-ttu-id="f2e83-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f2e83-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2e83-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="f2e83-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="f2e83-116">1 年ごと。</span><span class="sxs-lookup"><span data-stu-id="f2e83-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="f2e83-117">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="f2e83-117">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="f2e83-118">1 か月ごと。</span><span class="sxs-lookup"><span data-stu-id="f2e83-118">Represents a monthly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f2e83-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f2e83-119">Text value</span></span>

<span data-ttu-id="f2e83-120">1 ~ 31 の範囲の整数値を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="f2e83-120">A text value that represents an integer in the range of 1 to 31 is required.</span></span> <span data-ttu-id="f2e83-121">特定の月のこの値が大きい場合、月の日数よりも、月の最後の日と見なされます。</span><span class="sxs-lookup"><span data-stu-id="f2e83-121">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f2e83-122">備考</span><span class="sxs-lookup"><span data-stu-id="f2e83-122">Remarks</span></span>

<span data-ttu-id="f2e83-123">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f2e83-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2e83-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="f2e83-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2e83-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="f2e83-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f2e83-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f2e83-126">Schema name</span></span>  <br/> |<span data-ttu-id="f2e83-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f2e83-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="f2e83-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f2e83-128">Validation file</span></span>  <br/> |<span data-ttu-id="f2e83-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f2e83-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f2e83-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f2e83-130">Can be empty</span></span>  <br/> |<span data-ttu-id="f2e83-131">False</span><span class="sxs-lookup"><span data-stu-id="f2e83-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2e83-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="f2e83-132">See also</span></span>

- [<span data-ttu-id="f2e83-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f2e83-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


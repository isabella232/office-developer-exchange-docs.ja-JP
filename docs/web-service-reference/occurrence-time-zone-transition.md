---
title: 発生 (タイム ゾーンの切り替え)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Occurrence
api_type:
- schema
ms.assetid: 5c1142b1-c51f-42e1-bbb2-57e00cad0fdb
description: 見つかった要素では、タイム ゾーンの切り替えが発生する月の週の日の発生を表します。
ms.openlocfilehash: bc5160480cc6881bb9d724aa61323f5717d1f2fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832636"
---
# <a name="occurrence-time-zone-transition"></a><span data-ttu-id="a4c6c-103">発生 (タイム ゾーンの切り替え)</span><span class="sxs-lookup"><span data-stu-id="a4c6c-103">Occurrence (Time Zone Transition)</span></span>

<span data-ttu-id="a4c6c-104">**見つかった**要素では、タイム ゾーンの切り替えが発生する月の週の日の発生を表します。</span><span class="sxs-lookup"><span data-stu-id="a4c6c-104">The **Occurrence** element represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span> 
  
```xml
<Occurrence/>
```

<span data-ttu-id="a4c6c-105">**int**</span><span class="sxs-lookup"><span data-stu-id="a4c6c-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a4c6c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a4c6c-106">Attributes and elements</span></span>

<span data-ttu-id="a4c6c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a4c6c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4c6c-108">属性</span><span class="sxs-lookup"><span data-stu-id="a4c6c-108">Attributes</span></span>

<span data-ttu-id="a4c6c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a4c6c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a4c6c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a4c6c-110">Child elements</span></span>

<span data-ttu-id="a4c6c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a4c6c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a4c6c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a4c6c-112">Parent elements</span></span>

|<span data-ttu-id="a4c6c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a4c6c-113">**Element**</span></span>|<span data-ttu-id="a4c6c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a4c6c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a4c6c-115">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="a4c6c-115">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="a4c6c-116">毎年同じ日に発生するタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="a4c6c-116">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a4c6c-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a4c6c-117">Text value</span></span>

<span data-ttu-id="a4c6c-118">テキスト値は、タイム ゾーンの切り替えが発生する月の週の日の発生を表す整数です。</span><span class="sxs-lookup"><span data-stu-id="a4c6c-118">The text value is an integer that represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span> <span data-ttu-id="a4c6c-119">次の表は、可能な値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="a4c6c-119">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="a4c6c-120">**値**</span><span class="sxs-lookup"><span data-stu-id="a4c6c-120">**Value**</span></span>|<span data-ttu-id="a4c6c-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="a4c6c-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a4c6c-122">1</span><span class="sxs-lookup"><span data-stu-id="a4c6c-122">1</span></span>  <br/> |<span data-ttu-id="a4c6c-123">指定した曜日、月の最初から最初に出現します。</span><span class="sxs-lookup"><span data-stu-id="a4c6c-123">The first occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="a4c6c-124">2</span><span class="sxs-lookup"><span data-stu-id="a4c6c-124">2</span></span>  <br/> |<span data-ttu-id="a4c6c-125">指定した曜日、月の最初からの 2 つ目の発生。</span><span class="sxs-lookup"><span data-stu-id="a4c6c-125">The second occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="a4c6c-126">3</span><span class="sxs-lookup"><span data-stu-id="a4c6c-126">3</span></span>  <br/> |<span data-ttu-id="a4c6c-127">指定した曜日、月の最初からの 3 つ目の発生。</span><span class="sxs-lookup"><span data-stu-id="a4c6c-127">The third occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="a4c6c-128">4</span><span class="sxs-lookup"><span data-stu-id="a4c6c-128">4</span></span>  <br/> |<span data-ttu-id="a4c6c-129">指定した曜日、月の最初からの 4 番目の発生。</span><span class="sxs-lookup"><span data-stu-id="a4c6c-129">The fourth occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="a4c6c-130">-1</span><span class="sxs-lookup"><span data-stu-id="a4c6c-130">-1</span></span>  <br/> |<span data-ttu-id="a4c6c-131">指定した曜日、月の最後から最初に出現します。</span><span class="sxs-lookup"><span data-stu-id="a4c6c-131">The first occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="a4c6c-132">-2</span><span class="sxs-lookup"><span data-stu-id="a4c6c-132">-2</span></span>  <br/> |<span data-ttu-id="a4c6c-133">指定した曜日、月の最後からの 2 つ目の発生。</span><span class="sxs-lookup"><span data-stu-id="a4c6c-133">The second occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="a4c6c-134">-3</span><span class="sxs-lookup"><span data-stu-id="a4c6c-134">-3</span></span>  <br/> |<span data-ttu-id="a4c6c-135">指定した曜日、月の最後からの 3 つ目の発生。</span><span class="sxs-lookup"><span data-stu-id="a4c6c-135">The third occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="a4c6c-136">-4</span><span class="sxs-lookup"><span data-stu-id="a4c6c-136">-4</span></span>  <br/> |<span data-ttu-id="a4c6c-137">指定した曜日、月の最後からの 4 番目の発生。</span><span class="sxs-lookup"><span data-stu-id="a4c6c-137">The fourth occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a4c6c-138">備考</span><span class="sxs-lookup"><span data-stu-id="a4c6c-138">Remarks</span></span>

<span data-ttu-id="a4c6c-139">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a4c6c-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4c6c-140">要素情報</span><span class="sxs-lookup"><span data-stu-id="a4c6c-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4c6c-141">名前空間</span><span class="sxs-lookup"><span data-stu-id="a4c6c-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a4c6c-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a4c6c-142">Schema Name</span></span>  <br/> |<span data-ttu-id="a4c6c-143">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a4c6c-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="a4c6c-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a4c6c-144">Validation File</span></span>  <br/> |<span data-ttu-id="a4c6c-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a4c6c-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a4c6c-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a4c6c-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="a4c6c-147">False</span><span class="sxs-lookup"><span data-stu-id="a4c6c-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a4c6c-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="a4c6c-148">See also</span></span>

- [<span data-ttu-id="a4c6c-149">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a4c6c-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


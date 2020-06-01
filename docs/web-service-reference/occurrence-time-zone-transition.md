---
title: 発生 (タイムゾーンの切り替え)
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
description: オカレンスリンク要素は、タイムゾーンの切り替えが行われる月の曜日の発生を表します。
ms.openlocfilehash: 846f6b22f43bcda07b9408d768d0845a5acfe668
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467978"
---
# <a name="occurrence-time-zone-transition"></a><span data-ttu-id="63c82-103">発生 (タイムゾーンの切り替え)</span><span class="sxs-lookup"><span data-stu-id="63c82-103">Occurrence (Time Zone Transition)</span></span>

<span data-ttu-id="63c82-104">**オカレンスリンク**要素は、タイムゾーンの切り替えが行われる月の曜日の発生を表します。</span><span class="sxs-lookup"><span data-stu-id="63c82-104">The **Occurrence** element represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span> 
  
```xml
<Occurrence/>
```

<span data-ttu-id="63c82-105">**int**</span><span class="sxs-lookup"><span data-stu-id="63c82-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="63c82-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="63c82-106">Attributes and elements</span></span>

<span data-ttu-id="63c82-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="63c82-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63c82-108">属性</span><span class="sxs-lookup"><span data-stu-id="63c82-108">Attributes</span></span>

<span data-ttu-id="63c82-109">なし。</span><span class="sxs-lookup"><span data-stu-id="63c82-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63c82-110">子要素</span><span class="sxs-lookup"><span data-stu-id="63c82-110">Child elements</span></span>

<span data-ttu-id="63c82-111">なし。</span><span class="sxs-lookup"><span data-stu-id="63c82-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="63c82-112">親要素</span><span class="sxs-lookup"><span data-stu-id="63c82-112">Parent elements</span></span>

|<span data-ttu-id="63c82-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="63c82-113">**Element**</span></span>|<span data-ttu-id="63c82-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="63c82-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63c82-115">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="63c82-115">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="63c82-116">毎年同じ日に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="63c82-116">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="63c82-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="63c82-117">Text value</span></span>

<span data-ttu-id="63c82-118">Text 値は、タイムゾーンの切り替えが行われる月の曜日の発生を表す整数です。</span><span class="sxs-lookup"><span data-stu-id="63c82-118">The text value is an integer that represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span> <span data-ttu-id="63c82-119">次の表に、使用可能な値を示します。</span><span class="sxs-lookup"><span data-stu-id="63c82-119">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="63c82-120">**値**</span><span class="sxs-lookup"><span data-stu-id="63c82-120">**Value**</span></span>|<span data-ttu-id="63c82-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="63c82-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="63c82-122">1-d</span><span class="sxs-lookup"><span data-stu-id="63c82-122">1</span></span>  <br/> |<span data-ttu-id="63c82-123">月の最初から指定された曜日の最初の出現。</span><span class="sxs-lookup"><span data-stu-id="63c82-123">The first occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="63c82-124">pbm-2</span><span class="sxs-lookup"><span data-stu-id="63c82-124">2</span></span>  <br/> |<span data-ttu-id="63c82-125">月の最初から指定された曜日の2回目の出現。</span><span class="sxs-lookup"><span data-stu-id="63c82-125">The second occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="63c82-126">1/3</span><span class="sxs-lookup"><span data-stu-id="63c82-126">3</span></span>  <br/> |<span data-ttu-id="63c82-127">月の最初から指定された曜日の3番目の出現。</span><span class="sxs-lookup"><span data-stu-id="63c82-127">The third occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="63c82-128">4 </span><span class="sxs-lookup"><span data-stu-id="63c82-128">4</span></span>  <br/> |<span data-ttu-id="63c82-129">月の最初の曜日の、指定された曜日の4番目の出現。</span><span class="sxs-lookup"><span data-stu-id="63c82-129">The fourth occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="63c82-130">-1</span><span class="sxs-lookup"><span data-stu-id="63c82-130">-1</span></span>  <br/> |<span data-ttu-id="63c82-131">月の終わりから、指定された曜日の最初の出現。</span><span class="sxs-lookup"><span data-stu-id="63c82-131">The first occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="63c82-132">-2</span><span class="sxs-lookup"><span data-stu-id="63c82-132">-2</span></span>  <br/> |<span data-ttu-id="63c82-133">月の終わりから、指定された曜日の2回目の出現。</span><span class="sxs-lookup"><span data-stu-id="63c82-133">The second occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="63c82-134">-3</span><span class="sxs-lookup"><span data-stu-id="63c82-134">-3</span></span>  <br/> |<span data-ttu-id="63c82-135">月の終わりから、指定された曜日の3番目の出現。</span><span class="sxs-lookup"><span data-stu-id="63c82-135">The third occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="63c82-136">-4</span><span class="sxs-lookup"><span data-stu-id="63c82-136">-4</span></span>  <br/> |<span data-ttu-id="63c82-137">月の終わりから、指定された曜日の4番目の出現。</span><span class="sxs-lookup"><span data-stu-id="63c82-137">The fourth occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="63c82-138">注釈</span><span class="sxs-lookup"><span data-stu-id="63c82-138">Remarks</span></span>

<span data-ttu-id="63c82-139">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="63c82-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63c82-140">要素の情報</span><span class="sxs-lookup"><span data-stu-id="63c82-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63c82-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="63c82-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="63c82-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="63c82-142">Schema Name</span></span>  <br/> |<span data-ttu-id="63c82-143">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="63c82-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="63c82-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="63c82-144">Validation File</span></span>  <br/> |<span data-ttu-id="63c82-145">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="63c82-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="63c82-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="63c82-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="63c82-147">正しくない</span><span class="sxs-lookup"><span data-stu-id="63c82-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63c82-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="63c82-148">See also</span></span>

- [<span data-ttu-id="63c82-149">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="63c82-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


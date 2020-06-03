---
title: End
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- End
api_type:
- schema
ms.assetid: 72329821-32ff-495d-b6e5-fdc011003c2e
description: End 要素は、期間の終わりを表します。
ms.openlocfilehash: d36f555d2ac9c0c1d82053029720ec17a53f2d92
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456144"
---
# <a name="end"></a><span data-ttu-id="3fe2e-103">End</span><span class="sxs-lookup"><span data-stu-id="3fe2e-103">End</span></span>

<span data-ttu-id="3fe2e-104">**End**要素は、期間の終わりを表します。</span><span class="sxs-lookup"><span data-stu-id="3fe2e-104">The **End** element represents the end of a duration.</span></span> 
  
```xml
<End/>
```

 <span data-ttu-id="3fe2e-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="3fe2e-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3fe2e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3fe2e-106">Attributes and elements</span></span>

<span data-ttu-id="3fe2e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3fe2e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3fe2e-108">属性</span><span class="sxs-lookup"><span data-stu-id="3fe2e-108">Attributes</span></span>

<span data-ttu-id="3fe2e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3fe2e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3fe2e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3fe2e-110">Child elements</span></span>

<span data-ttu-id="3fe2e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3fe2e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3fe2e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3fe2e-112">Parent elements</span></span>

|<span data-ttu-id="3fe2e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="3fe2e-113">**Element**</span></span>|<span data-ttu-id="3fe2e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3fe2e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3fe2e-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="3fe2e-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="3fe2e-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="3fe2e-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3fe2e-117">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="3fe2e-117">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="3fe2e-118">定期的な予定表アイテムの最初の出現を表します。</span><span class="sxs-lookup"><span data-stu-id="3fe2e-118">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3fe2e-119">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="3fe2e-119">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="3fe2e-120">定期的な予定表アイテムの最後の発生を表します。</span><span class="sxs-lookup"><span data-stu-id="3fe2e-120">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3fe2e-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="3fe2e-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="3fe2e-122">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="3fe2e-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3fe2e-123">発生</span><span class="sxs-lookup"><span data-stu-id="3fe2e-123">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="3fe2e-124">定期的な予定表アイテムの1つの変更されたアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="3fe2e-124">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3fe2e-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3fe2e-125">Text value</span></span>

<span data-ttu-id="3fe2e-126">テキスト値は、期間の終わりを表します。</span><span class="sxs-lookup"><span data-stu-id="3fe2e-126">The text value represents the end of a duration.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3fe2e-127">注釈</span><span class="sxs-lookup"><span data-stu-id="3fe2e-127">Remarks</span></span>

<span data-ttu-id="3fe2e-128">UpdateItem 操作は、Exchange ストアアイテムの[開始](start.md)時刻と**終了**時刻を設定できます。</span><span class="sxs-lookup"><span data-stu-id="3fe2e-128">The UpdateItem operation can set the [Start](start.md) and **End** time of an Exchange store item.</span></span> <span data-ttu-id="3fe2e-129">UpdateItem 要求では、**終了**時刻を設定することなく、[開始](start.md)時刻を設定できます。</span><span class="sxs-lookup"><span data-stu-id="3fe2e-129">In an UpdateItem request, you can set the [Start](start.md) time without also setting the **End** time.</span></span> <span data-ttu-id="3fe2e-130">これにより、[開始](start.md)時刻が**終了**時刻よりも後の場合にエラーが発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="3fe2e-130">This can cause an error if the [Start](start.md) time is later than the **End** time.</span></span> <span data-ttu-id="3fe2e-131">時間を保持するためにその[開始](start.md)時刻が変更された場合、クライアントアプリケーションは**終了**時刻を調整する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="3fe2e-131">Be aware that client applications must perform adjustments to the **End** time when that [Start](start.md) time is changed in order to preserve the duration.</span></span> 
  
 <span data-ttu-id="3fe2e-132">**メモ**定期的なマスターアイテムの[開始](start.md)日と**終了**日に、最初に週単位の定期的なパターンと同じ日付が設定されていない場合は、タイムゾーンのオフセット情報は失われます。</span><span class="sxs-lookup"><span data-stu-id="3fe2e-132">**Note** The time zone offset information is lost if the [Start](start.md) and **End** dates of the recurring master item do not have a date that is equal to the first occurrence of a weekly recurrence pattern.</span></span> 
  
<span data-ttu-id="3fe2e-133">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="3fe2e-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3fe2e-134">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3fe2e-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3fe2e-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="3fe2e-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3fe2e-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3fe2e-136">Schema Name</span></span>  <br/> |<span data-ttu-id="3fe2e-137">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="3fe2e-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="3fe2e-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3fe2e-138">Validation File</span></span>  <br/> |<span data-ttu-id="3fe2e-139">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="3fe2e-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3fe2e-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3fe2e-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="3fe2e-141">正しくない</span><span class="sxs-lookup"><span data-stu-id="3fe2e-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3fe2e-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="3fe2e-142">See also</span></span>



[<span data-ttu-id="3fe2e-143">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="3fe2e-143">WeeklyRecurrence</span></span>](weeklyrecurrence.md)
  
 <span data-ttu-id="3fe2e-144">**End**</span><span class="sxs-lookup"><span data-stu-id="3fe2e-144">**End**</span></span>


- [<span data-ttu-id="3fe2e-145">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3fe2e-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


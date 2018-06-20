---
title: 終了
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
description: 末尾の要素は、期間の終了を表します。
ms.openlocfilehash: 90eea4fc545fae083e5675225665e517b502ba6f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760284"
---
# <a name="end"></a><span data-ttu-id="ca582-103">終了</span><span class="sxs-lookup"><span data-stu-id="ca582-103">End</span></span>

<span data-ttu-id="ca582-104">**末尾**の要素は、期間の終了を表します。</span><span class="sxs-lookup"><span data-stu-id="ca582-104">The **End** element represents the end of a duration.</span></span> 
  
```xml
<End/>
```

 <span data-ttu-id="ca582-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="ca582-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ca582-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ca582-106">Attributes and elements</span></span>

<span data-ttu-id="ca582-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ca582-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ca582-108">属性</span><span class="sxs-lookup"><span data-stu-id="ca582-108">Attributes</span></span>

<span data-ttu-id="ca582-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ca582-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ca582-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ca582-110">Child elements</span></span>

<span data-ttu-id="ca582-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ca582-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ca582-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ca582-112">Parent elements</span></span>

|<span data-ttu-id="ca582-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ca582-113">**Element**</span></span>|<span data-ttu-id="ca582-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ca582-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca582-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="ca582-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ca582-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="ca582-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ca582-117">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="ca582-117">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="ca582-118">定期的な予定表アイテムが最初に見つかった位置を表します。</span><span class="sxs-lookup"><span data-stu-id="ca582-118">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ca582-119">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="ca582-119">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="ca582-120">定期的な予定表アイテムが最後に見つかった位置を表します。</span><span class="sxs-lookup"><span data-stu-id="ca582-120">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ca582-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ca582-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ca582-122">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="ca582-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ca582-123">出現</span><span class="sxs-lookup"><span data-stu-id="ca582-123">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="ca582-124">定期的な予定表アイテムの 1 つの変更されたアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="ca582-124">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ca582-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ca582-125">Text value</span></span>

<span data-ttu-id="ca582-126">テキスト値は、期間の終了を表します。</span><span class="sxs-lookup"><span data-stu-id="ca582-126">The text value represents the end of a duration.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ca582-127">備考</span><span class="sxs-lookup"><span data-stu-id="ca582-127">Remarks</span></span>

<span data-ttu-id="ca582-128">UpdateItem 操作は、Exchange ストアの項目の[開始](start.md)と**終了**時間を設定できます。</span><span class="sxs-lookup"><span data-stu-id="ca582-128">The UpdateItem operation can set the [Start](start.md) and **End** time of an Exchange store item.</span></span> <span data-ttu-id="ca582-129">UpdateItem 要求では、**終了**時刻を設定せず、[開始](start.md)時刻を設定できます。</span><span class="sxs-lookup"><span data-stu-id="ca582-129">In an UpdateItem request, you can set the [Start](start.md) time without also setting the **End** time.</span></span> <span data-ttu-id="ca582-130">[開始](start.md)時刻は**終了**時刻より後の場合は、エラーが発生することができます。</span><span class="sxs-lookup"><span data-stu-id="ca582-130">This can cause an error if the [Start](start.md) time is later than the **End** time.</span></span> <span data-ttu-id="ca582-131">クライアント アプリケーションが、期間を保持するために[開始](start.md)時間を変更するときの**終了**時刻の調整を行う必要があることに注意します。</span><span class="sxs-lookup"><span data-stu-id="ca582-131">Be aware that client applications must perform adjustments to the **End** time when that [Start](start.md) time is changed in order to preserve the duration.</span></span> 
  
 <span data-ttu-id="ca582-132">**メモ**定期的なマスター アイテムの[開始](start.md)と**終了**日が毎週の定期的なパターンの 1 番目の日付があるない場合、タイム ゾーン オフセット情報は失われます。</span><span class="sxs-lookup"><span data-stu-id="ca582-132">**Note** The time zone offset information is lost if the [Start](start.md) and **End** dates of the recurring master item do not have a date that is equal to the first occurrence of a weekly recurrence pattern.</span></span> 
  
<span data-ttu-id="ca582-133">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="ca582-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ca582-134">要素情報</span><span class="sxs-lookup"><span data-stu-id="ca582-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ca582-135">名前空間</span><span class="sxs-lookup"><span data-stu-id="ca582-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ca582-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ca582-136">Schema Name</span></span>  <br/> |<span data-ttu-id="ca582-137">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ca582-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="ca582-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ca582-138">Validation File</span></span>  <br/> |<span data-ttu-id="ca582-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ca582-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ca582-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ca582-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="ca582-141">False</span><span class="sxs-lookup"><span data-stu-id="ca582-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ca582-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="ca582-142">See also</span></span>



[<span data-ttu-id="ca582-143">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="ca582-143">WeeklyRecurrence</span></span>](weeklyrecurrence.md)
  
 <span data-ttu-id="ca582-144">**End**</span><span class="sxs-lookup"><span data-stu-id="ca582-144">**End**</span></span>


- [<span data-ttu-id="ca582-145">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ca582-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


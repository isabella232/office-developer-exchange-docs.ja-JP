---
title: 標準
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Standard
api_type:
- schema
ms.assetid: d598f0a6-e296-423f-8ce5-3da57cfd8189
description: 標準的な要素では、日付と時刻が変更されたとき夏時間から標準時間への時間を表します。
ms.openlocfilehash: 1c9be4cf35773583078bc8e16ddf44433d3ad98c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833536"
---
# <a name="standard"></a><span data-ttu-id="cce04-103">標準</span><span class="sxs-lookup"><span data-stu-id="cce04-103">Standard</span></span>

<span data-ttu-id="cce04-104">**標準的な**要素では、日付と時刻が変更されたとき夏時間から標準時間への時間を表します。</span><span class="sxs-lookup"><span data-stu-id="cce04-104">The **Standard** element represents the date and time when the time changes from daylight saving time to standard time.</span></span> 
  
```xml
<Standard TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Standard>
```

 <span data-ttu-id="cce04-105">**TimeChangeType**</span><span class="sxs-lookup"><span data-stu-id="cce04-105">**TimeChangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cce04-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cce04-106">Attributes and elements</span></span>

<span data-ttu-id="cce04-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cce04-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cce04-108">属性</span><span class="sxs-lookup"><span data-stu-id="cce04-108">Attributes</span></span>

|<span data-ttu-id="cce04-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="cce04-109">**Attribute**</span></span>|<span data-ttu-id="cce04-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="cce04-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cce04-111">**TimeZoneName**</span><span class="sxs-lookup"><span data-stu-id="cce04-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="cce04-112">タイム ゾーンの名前について説明します。</span><span class="sxs-lookup"><span data-stu-id="cce04-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="cce04-113">子要素</span><span class="sxs-lookup"><span data-stu-id="cce04-113">Child elements</span></span>

|<span data-ttu-id="cce04-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="cce04-114">**Element**</span></span>|<span data-ttu-id="cce04-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="cce04-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cce04-116">Offset</span><span class="sxs-lookup"><span data-stu-id="cce04-116">Offset</span></span>](offset.md) <br/> |<span data-ttu-id="cce04-117">[BaseOffset](baseoffset.md)からのオフセットを示します。</span><span class="sxs-lookup"><span data-stu-id="cce04-117">Describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="cce04-118">**BaseOffset**要素とは、**オフセット**要素は、時間が標準時か夏時間かどうかを識別します。</span><span class="sxs-lookup"><span data-stu-id="cce04-118">Together with the **BaseOffset** element, the **Offset** element identifies whether the time is standard time or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="cce04-119">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="cce04-119">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="cce04-120">タイム ゾーンの移行日の相対的な年間の定期的なパターンを説明します。</span><span class="sxs-lookup"><span data-stu-id="cce04-120">Describes a relative yearly recurrence pattern for a time zone transition date.</span></span>  <br/> |
|[<span data-ttu-id="cce04-121">AbsoluteDate</span><span class="sxs-lookup"><span data-stu-id="cce04-121">AbsoluteDate</span></span>](absolutedate.md) <br/> |<span data-ttu-id="cce04-122">標準時間または夏時間から標準時から時間が変更されたときの日付を表します。</span><span class="sxs-lookup"><span data-stu-id="cce04-122">Represents the date when the time changes from standard time or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="cce04-123">時間 (TimeChangeType)</span><span class="sxs-lookup"><span data-stu-id="cce04-123">Time (TimeChangeType)</span></span>](time-timechangetype.md) <br/> |<span data-ttu-id="cce04-124">標準時と夏時間との間の時間が変更されたときの時間について説明します。</span><span class="sxs-lookup"><span data-stu-id="cce04-124">Describes the time when the time changes between standard time and daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cce04-125">親要素</span><span class="sxs-lookup"><span data-stu-id="cce04-125">Parent elements</span></span>

|<span data-ttu-id="cce04-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="cce04-126">**Element**</span></span>|<span data-ttu-id="cce04-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="cce04-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cce04-128">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="cce04-128">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="cce04-129">会議がホストされている場所のタイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="cce04-129">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cce04-130">備考</span><span class="sxs-lookup"><span data-stu-id="cce04-130">Remarks</span></span>

<span data-ttu-id="cce04-131">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="cce04-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cce04-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="cce04-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cce04-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="cce04-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cce04-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cce04-134">Schema Name</span></span>  <br/> |<span data-ttu-id="cce04-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="cce04-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="cce04-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cce04-136">Validation File</span></span>  <br/> |<span data-ttu-id="cce04-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cce04-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cce04-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cce04-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="cce04-139">False</span><span class="sxs-lookup"><span data-stu-id="cce04-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cce04-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="cce04-140">See also</span></span>



- [<span data-ttu-id="cce04-141">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="cce04-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: (夏時間)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Daylight
api_type:
- schema
ms.assetid: ea400839-fba8-4a5e-a5d1-9b677afc0ff9
description: 夏時間の要素では、日付と時刻が変更されたとき標準時間から夏時間への時間を表します。
ms.openlocfilehash: cdb6ed305f1d77a73b952f8c659991f3b2a8df7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759931"
---
# <a name="daylight"></a><span data-ttu-id="a89ac-103">(夏時間)</span><span class="sxs-lookup"><span data-stu-id="a89ac-103">Daylight</span></span>

<span data-ttu-id="a89ac-104">**夏時間**の要素では、日付と時刻が変更されたとき標準時間から夏時間への時間を表します。</span><span class="sxs-lookup"><span data-stu-id="a89ac-104">The **Daylight** element represents the date and time when the time changes from standard time to daylight saving time.</span></span> 
  
```xml
<Daylight TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Daylight>
```

```xml
<Daylight TimeZoneName="">
   <Offset/>
   <AbsoluteDate/>
   <Time/>
</Daylight>
```

<span data-ttu-id="a89ac-105">**TimeChangeType**</span><span class="sxs-lookup"><span data-stu-id="a89ac-105">**TimeChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a89ac-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a89ac-106">Attributes and elements</span></span>

<span data-ttu-id="a89ac-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a89ac-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a89ac-108">属性</span><span class="sxs-lookup"><span data-stu-id="a89ac-108">Attributes</span></span>

|<span data-ttu-id="a89ac-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="a89ac-109">**Attribute**</span></span>|<span data-ttu-id="a89ac-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="a89ac-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a89ac-111">**TimeZoneName**</span><span class="sxs-lookup"><span data-stu-id="a89ac-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="a89ac-112">タイム ゾーンの名前について説明します。</span><span class="sxs-lookup"><span data-stu-id="a89ac-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a89ac-113">子要素</span><span class="sxs-lookup"><span data-stu-id="a89ac-113">Child elements</span></span>

|<span data-ttu-id="a89ac-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="a89ac-114">**Element**</span></span>|<span data-ttu-id="a89ac-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="a89ac-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a89ac-116">Offset</span><span class="sxs-lookup"><span data-stu-id="a89ac-116">Offset</span></span>](offset.md) <br/> |<span data-ttu-id="a89ac-117">[BaseOffset](baseoffset.md)からのオフセットを示します。</span><span class="sxs-lookup"><span data-stu-id="a89ac-117">Describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="a89ac-118">このオフセットだけでなく相手のベースは、標準的なことがあるかどうか、または夏時間から標準時、時間を識別します。</span><span class="sxs-lookup"><span data-stu-id="a89ac-118">The base offset in addition to this offset identifies the time according to whether it is standard or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="a89ac-119">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="a89ac-119">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="a89ac-120">相対年間定期的なパターンをタイム ゾーンの移行の日付形式のパターンについて説明します。</span><span class="sxs-lookup"><span data-stu-id="a89ac-120">Describes a relative yearly recurrence pattern for a time zone transition date pattern.</span></span>  <br/> |
|[<span data-ttu-id="a89ac-121">AbsoluteDate</span><span class="sxs-lookup"><span data-stu-id="a89ac-121">AbsoluteDate</span></span>](absolutedate.md) <br/> |<span data-ttu-id="a89ac-122">標準または夏時間から標準時から時間が変更されたときの日付を表します。</span><span class="sxs-lookup"><span data-stu-id="a89ac-122">Represents the date when the time changes from standard or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="a89ac-123">時間 (TimeChangeType)</span><span class="sxs-lookup"><span data-stu-id="a89ac-123">Time (TimeChangeType)</span></span>](time-timechangetype.md) <br/> |<span data-ttu-id="a89ac-124">標準時と夏時間との間の時間が変更されたときの時間について説明します。</span><span class="sxs-lookup"><span data-stu-id="a89ac-124">Describes the time when the time changes between standard time and daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a89ac-125">親要素</span><span class="sxs-lookup"><span data-stu-id="a89ac-125">Parent elements</span></span>

|<span data-ttu-id="a89ac-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="a89ac-126">**Element**</span></span>|<span data-ttu-id="a89ac-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="a89ac-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a89ac-128">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="a89ac-128">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="a89ac-129">会議がホストされている場所のタイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="a89ac-129">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a89ac-130">備考</span><span class="sxs-lookup"><span data-stu-id="a89ac-130">Remarks</span></span>

<span data-ttu-id="a89ac-131">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a89ac-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a89ac-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="a89ac-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a89ac-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="a89ac-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a89ac-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a89ac-134">Schema Name</span></span>  <br/> |<span data-ttu-id="a89ac-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a89ac-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="a89ac-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a89ac-136">Validation File</span></span>  <br/> |<span data-ttu-id="a89ac-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a89ac-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a89ac-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a89ac-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="a89ac-139">False</span><span class="sxs-lookup"><span data-stu-id="a89ac-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a89ac-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="a89ac-140">See also</span></span>

- [<span data-ttu-id="a89ac-141">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a89ac-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


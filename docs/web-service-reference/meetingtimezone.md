---
title: MeetingTimeZone
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingTimeZone
api_type:
- schema
ms.assetid: 413b47d9-8126-462c-9a4f-4e771a5e8889
description: Meeting Timezone 要素は、会議がホストされている場所のタイムゾーンを表します。
ms.openlocfilehash: aef4ac4e7571ded6920cbaf90e2895d421068f55
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465472"
---
# <a name="meetingtimezone"></a><span data-ttu-id="c0303-103">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="c0303-103">MeetingTimeZone</span></span>

<span data-ttu-id="c0303-104">Meeting **timezone**要素は、会議がホストされている場所のタイムゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="c0303-104">The **MeetingTimeZone** element represents the time zone of the location where the meeting is hosted.</span></span> 
  
```xml
<MeetingTimeZone>
   <BaseOffset/>
   <Standard/>
   <Daylight/>
</MeetingTimeZone>
```

 <span data-ttu-id="c0303-105">**TimeZoneType**</span><span class="sxs-lookup"><span data-stu-id="c0303-105">**TimeZoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c0303-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c0303-106">Attributes and elements</span></span>

<span data-ttu-id="c0303-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c0303-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0303-108">属性</span><span class="sxs-lookup"><span data-stu-id="c0303-108">Attributes</span></span>

|<span data-ttu-id="c0303-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="c0303-109">**Attribute**</span></span>|<span data-ttu-id="c0303-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="c0303-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c0303-111">**TimeZoneName**</span><span class="sxs-lookup"><span data-stu-id="c0303-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="c0303-112">タイムゾーンの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="c0303-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c0303-113">子要素</span><span class="sxs-lookup"><span data-stu-id="c0303-113">Child elements</span></span>

|<span data-ttu-id="c0303-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="c0303-114">**Element**</span></span>|<span data-ttu-id="c0303-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="c0303-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0303-116">BaseOffset</span><span class="sxs-lookup"><span data-stu-id="c0303-116">BaseOffset</span></span>](baseoffset.md) <br/> |<span data-ttu-id="c0303-117">現在のタイムゾーンの UTC からの時間オフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="c0303-117">Represents the hourly offset from UTC for the current time zone.</span></span>  <br/> |
|[<span data-ttu-id="c0303-118">Standard</span><span class="sxs-lookup"><span data-stu-id="c0303-118">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="c0303-119">夏時間から標準時までの時刻が変更された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="c0303-119">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="c0303-120">日光</span><span class="sxs-lookup"><span data-stu-id="c0303-120">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="c0303-121">時刻が標準時から夏時間に変更された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="c0303-121">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c0303-122">親要素</span><span class="sxs-lookup"><span data-stu-id="c0303-122">Parent elements</span></span>

|<span data-ttu-id="c0303-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="c0303-123">**Element**</span></span>|<span data-ttu-id="c0303-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="c0303-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0303-125">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="c0303-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c0303-126">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c0303-126">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c0303-127">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c0303-127">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c0303-128">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="c0303-128">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c0303-129">注釈</span><span class="sxs-lookup"><span data-stu-id="c0303-129">Remarks</span></span>

<span data-ttu-id="c0303-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c0303-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0303-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c0303-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0303-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="c0303-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c0303-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c0303-133">Schema Name</span></span>  <br/> |<span data-ttu-id="c0303-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c0303-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="c0303-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c0303-135">Validation File</span></span>  <br/> |<span data-ttu-id="c0303-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c0303-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c0303-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c0303-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="c0303-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="c0303-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c0303-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="c0303-139">See also</span></span>



- [<span data-ttu-id="c0303-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c0303-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


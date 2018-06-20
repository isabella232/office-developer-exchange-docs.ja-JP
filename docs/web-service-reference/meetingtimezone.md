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
description: MeetingTimeZone 要素は、会議をホストしている場所のタイム ゾーンを表します。
ms.openlocfilehash: ce014ac6d8841e451927a94049cb4e8860886fdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832440"
---
# <a name="meetingtimezone"></a><span data-ttu-id="7a8ea-103">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="7a8ea-103">MeetingTimeZone</span></span>

<span data-ttu-id="7a8ea-104">**MeetingTimeZone**要素は、会議をホストしている場所のタイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="7a8ea-104">The **MeetingTimeZone** element represents the time zone of the location where the meeting is hosted.</span></span> 
  
```xml
<MeetingTimeZone>
   <BaseOffset/>
   <Standard/>
   <Daylight/>
</MeetingTimeZone>
```

 <span data-ttu-id="7a8ea-105">**TimeZoneType**</span><span class="sxs-lookup"><span data-stu-id="7a8ea-105">**TimeZoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a8ea-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7a8ea-106">Attributes and elements</span></span>

<span data-ttu-id="7a8ea-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7a8ea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a8ea-108">属性</span><span class="sxs-lookup"><span data-stu-id="7a8ea-108">Attributes</span></span>

|<span data-ttu-id="7a8ea-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="7a8ea-109">**Attribute**</span></span>|<span data-ttu-id="7a8ea-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="7a8ea-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7a8ea-111">**TimeZoneName**</span><span class="sxs-lookup"><span data-stu-id="7a8ea-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="7a8ea-112">タイム ゾーンの名前について説明します。</span><span class="sxs-lookup"><span data-stu-id="7a8ea-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7a8ea-113">子要素</span><span class="sxs-lookup"><span data-stu-id="7a8ea-113">Child elements</span></span>

|<span data-ttu-id="7a8ea-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="7a8ea-114">**Element**</span></span>|<span data-ttu-id="7a8ea-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="7a8ea-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a8ea-116">BaseOffset</span><span class="sxs-lookup"><span data-stu-id="7a8ea-116">BaseOffset</span></span>](baseoffset.md) <br/> |<span data-ttu-id="7a8ea-117">時間単位の現在のタイム ゾーンの UTC からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="7a8ea-117">Represents the hourly offset from UTC for the current time zone.</span></span>  <br/> |
|[<span data-ttu-id="7a8ea-118">Standard</span><span class="sxs-lookup"><span data-stu-id="7a8ea-118">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="7a8ea-119">日付と時刻が変更されたとき夏時間から標準時間への時間を表します。</span><span class="sxs-lookup"><span data-stu-id="7a8ea-119">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="7a8ea-120">(夏時間)</span><span class="sxs-lookup"><span data-stu-id="7a8ea-120">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="7a8ea-121">日付と時刻が変更されたとき標準時間から夏時間への時間を表します。</span><span class="sxs-lookup"><span data-stu-id="7a8ea-121">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7a8ea-122">親要素</span><span class="sxs-lookup"><span data-stu-id="7a8ea-122">Parent elements</span></span>

|<span data-ttu-id="7a8ea-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="7a8ea-123">**Element**</span></span>|<span data-ttu-id="7a8ea-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="7a8ea-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a8ea-125">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="7a8ea-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="7a8ea-126">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="7a8ea-126">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7a8ea-127">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="7a8ea-127">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="7a8ea-128">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="7a8ea-128">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7a8ea-129">備考</span><span class="sxs-lookup"><span data-stu-id="7a8ea-129">Remarks</span></span>

<span data-ttu-id="7a8ea-130">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="7a8ea-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a8ea-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="7a8ea-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a8ea-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="7a8ea-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7a8ea-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7a8ea-133">Schema Name</span></span>  <br/> |<span data-ttu-id="7a8ea-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7a8ea-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="7a8ea-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7a8ea-135">Validation File</span></span>  <br/> |<span data-ttu-id="7a8ea-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7a8ea-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7a8ea-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7a8ea-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="7a8ea-138">False</span><span class="sxs-lookup"><span data-stu-id="7a8ea-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a8ea-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="7a8ea-139">See also</span></span>



- [<span data-ttu-id="7a8ea-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7a8ea-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


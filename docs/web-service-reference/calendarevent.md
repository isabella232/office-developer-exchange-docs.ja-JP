---
title: CalendarEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEvent
api_type:
- schema
ms.assetid: 91958c01-1fcb-4ac0-8601-5e5b434c988a
description: CalendarEvent 要素は、固有の予定表アイテムの出現を表します。
ms.openlocfilehash: 8bf37c907ed726e33dd2b1eff9add5d6235704da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459077"
---
# <a name="calendarevent"></a><span data-ttu-id="b50ce-103">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="b50ce-103">CalendarEvent</span></span>

<span data-ttu-id="b50ce-104">**CalendarEvent**要素は、固有の予定表アイテムの出現を表します。</span><span class="sxs-lookup"><span data-stu-id="b50ce-104">The **CalendarEvent** element represents a unique calendar item occurrence.</span></span> 
  
[<span data-ttu-id="b50ce-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b50ce-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="b50ce-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="b50ce-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="b50ce-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="b50ce-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="b50ce-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="b50ce-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="b50ce-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="b50ce-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="b50ce-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="b50ce-110">CalendarEvent</span></span>](calendarevent.md)
  
```xml
<CalendarEvent>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
   <BusyType>...</BusyType>
   <CalendarEventDetails>...</CalendarEventDetails>
</CalendarEvent>
```

 <span data-ttu-id="b50ce-111">**CalendarEvent**</span><span class="sxs-lookup"><span data-stu-id="b50ce-111">**CalendarEvent**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b50ce-112">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b50ce-112">Attributes and elements</span></span>

<span data-ttu-id="b50ce-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b50ce-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b50ce-114">属性</span><span class="sxs-lookup"><span data-stu-id="b50ce-114">Attributes</span></span>

<span data-ttu-id="b50ce-115">なし。</span><span class="sxs-lookup"><span data-stu-id="b50ce-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b50ce-116">子要素</span><span class="sxs-lookup"><span data-stu-id="b50ce-116">Child elements</span></span>

|<span data-ttu-id="b50ce-117">**Element**</span><span class="sxs-lookup"><span data-stu-id="b50ce-117">**Element**</span></span>|<span data-ttu-id="b50ce-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="b50ce-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b50ce-119">StartTime</span><span class="sxs-lookup"><span data-stu-id="b50ce-119">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="b50ce-120">予定表イベントの開始を表します。</span><span class="sxs-lookup"><span data-stu-id="b50ce-120">Represents the start of a calendar event.</span></span> <span data-ttu-id="b50ce-121">これは必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="b50ce-121">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="b50ce-122">EndTime</span><span class="sxs-lookup"><span data-stu-id="b50ce-122">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="b50ce-123">予定表イベントの終了を表します。</span><span class="sxs-lookup"><span data-stu-id="b50ce-123">Represents the end of a calendar event.</span></span> <span data-ttu-id="b50ce-124">これは必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="b50ce-124">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="b50ce-125">BusyType</span><span class="sxs-lookup"><span data-stu-id="b50ce-125">BusyType</span></span>](busytype.md) <br/> |<span data-ttu-id="b50ce-126">予定表イベントの空き時間状態セットを表します。</span><span class="sxs-lookup"><span data-stu-id="b50ce-126">Represents the free/busy status set for a calendar event.</span></span> <span data-ttu-id="b50ce-127">これは必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="b50ce-127">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="b50ce-128">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="b50ce-128">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="b50ce-129">予定表イベントに関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="b50ce-129">Provides additional information for a calendar event.</span></span> <span data-ttu-id="b50ce-130">これはオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="b50ce-130">This is an optional child element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b50ce-131">親要素</span><span class="sxs-lookup"><span data-stu-id="b50ce-131">Parent elements</span></span>

|<span data-ttu-id="b50ce-132">**要素**</span><span class="sxs-lookup"><span data-stu-id="b50ce-132">**Element**</span></span>|<span data-ttu-id="b50ce-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="b50ce-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b50ce-134">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="b50ce-134">CalendarEventArray</span></span>](calendareventarray.md) <br/> |<span data-ttu-id="b50ce-135">要求されたユーザーの空き時間情報を表す、一連の一意な予定表アイテムの繰り返しを含みます。</span><span class="sxs-lookup"><span data-stu-id="b50ce-135">Contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span>  <br/> <span data-ttu-id="b50ce-136">この要素の XPath 2.0 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b50ce-136">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b50ce-137">注釈</span><span class="sxs-lookup"><span data-stu-id="b50ce-137">Remarks</span></span>

<span data-ttu-id="b50ce-138">予定および会議の時刻は、クライアントのタイムゾーンで返されます。</span><span class="sxs-lookup"><span data-stu-id="b50ce-138">The appointment and meeting times are returned in the time zone of the client.</span></span> <span data-ttu-id="b50ce-139">すべての子要素が発生する順序で一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="b50ce-139">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="b50ce-140">この要素によって提供される詳細レベルは、リクエスターに付与されるアクセス許可によって異なります。</span><span class="sxs-lookup"><span data-stu-id="b50ce-140">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="b50ce-141">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b50ce-141">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b50ce-142">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b50ce-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b50ce-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="b50ce-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b50ce-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b50ce-144">Schema Name</span></span>  <br/> |<span data-ttu-id="b50ce-145">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b50ce-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="b50ce-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b50ce-146">Validation File</span></span>  <br/> |<span data-ttu-id="b50ce-147">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b50ce-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b50ce-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b50ce-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="b50ce-149">正しくない</span><span class="sxs-lookup"><span data-stu-id="b50ce-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b50ce-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="b50ce-150">See also</span></span>



[<span data-ttu-id="b50ce-151">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="b50ce-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="b50ce-152">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b50ce-152">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="b50ce-153">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="b50ce-153">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


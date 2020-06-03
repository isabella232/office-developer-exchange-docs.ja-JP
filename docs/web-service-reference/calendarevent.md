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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459077"
---
# <a name="calendarevent"></a><span data-ttu-id="f5cc0-103">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="f5cc0-103">CalendarEvent</span></span>

<span data-ttu-id="f5cc0-104">**CalendarEvent**要素は、固有の予定表アイテムの出現を表します。</span><span class="sxs-lookup"><span data-stu-id="f5cc0-104">The **CalendarEvent** element represents a unique calendar item occurrence.</span></span> 
  
[<span data-ttu-id="f5cc0-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f5cc0-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="f5cc0-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="f5cc0-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="f5cc0-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="f5cc0-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="f5cc0-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="f5cc0-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="f5cc0-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="f5cc0-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="f5cc0-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="f5cc0-110">CalendarEvent</span></span>](calendarevent.md)
  
```xml
<CalendarEvent>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
   <BusyType>...</BusyType>
   <CalendarEventDetails>...</CalendarEventDetails>
</CalendarEvent>
```

 <span data-ttu-id="f5cc0-111">**CalendarEvent**</span><span class="sxs-lookup"><span data-stu-id="f5cc0-111">**CalendarEvent**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f5cc0-112">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f5cc0-112">Attributes and elements</span></span>

<span data-ttu-id="f5cc0-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f5cc0-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f5cc0-114">属性</span><span class="sxs-lookup"><span data-stu-id="f5cc0-114">Attributes</span></span>

<span data-ttu-id="f5cc0-115">なし。</span><span class="sxs-lookup"><span data-stu-id="f5cc0-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f5cc0-116">子要素</span><span class="sxs-lookup"><span data-stu-id="f5cc0-116">Child elements</span></span>

|<span data-ttu-id="f5cc0-117">**Element**</span><span class="sxs-lookup"><span data-stu-id="f5cc0-117">**Element**</span></span>|<span data-ttu-id="f5cc0-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="f5cc0-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5cc0-119">StartTime</span><span class="sxs-lookup"><span data-stu-id="f5cc0-119">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="f5cc0-120">予定表イベントの開始を表します。</span><span class="sxs-lookup"><span data-stu-id="f5cc0-120">Represents the start of a calendar event.</span></span> <span data-ttu-id="f5cc0-121">これは必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="f5cc0-121">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="f5cc0-122">EndTime</span><span class="sxs-lookup"><span data-stu-id="f5cc0-122">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="f5cc0-123">予定表イベントの終了を表します。</span><span class="sxs-lookup"><span data-stu-id="f5cc0-123">Represents the end of a calendar event.</span></span> <span data-ttu-id="f5cc0-124">これは必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="f5cc0-124">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="f5cc0-125">BusyType</span><span class="sxs-lookup"><span data-stu-id="f5cc0-125">BusyType</span></span>](busytype.md) <br/> |<span data-ttu-id="f5cc0-126">予定表イベントの空き時間状態セットを表します。</span><span class="sxs-lookup"><span data-stu-id="f5cc0-126">Represents the free/busy status set for a calendar event.</span></span> <span data-ttu-id="f5cc0-127">これは必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="f5cc0-127">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="f5cc0-128">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="f5cc0-128">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="f5cc0-129">予定表イベントに関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="f5cc0-129">Provides additional information for a calendar event.</span></span> <span data-ttu-id="f5cc0-130">これはオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="f5cc0-130">This is an optional child element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f5cc0-131">親要素</span><span class="sxs-lookup"><span data-stu-id="f5cc0-131">Parent elements</span></span>

|<span data-ttu-id="f5cc0-132">**要素**</span><span class="sxs-lookup"><span data-stu-id="f5cc0-132">**Element**</span></span>|<span data-ttu-id="f5cc0-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="f5cc0-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5cc0-134">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="f5cc0-134">CalendarEventArray</span></span>](calendareventarray.md) <br/> |<span data-ttu-id="f5cc0-135">要求されたユーザーの空き時間情報を表す、一連の一意な予定表アイテムの繰り返しを含みます。</span><span class="sxs-lookup"><span data-stu-id="f5cc0-135">Contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span>  <br/> <span data-ttu-id="f5cc0-136">この要素の XPath 2.0 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f5cc0-136">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f5cc0-137">注釈</span><span class="sxs-lookup"><span data-stu-id="f5cc0-137">Remarks</span></span>

<span data-ttu-id="f5cc0-138">予定および会議の時刻は、クライアントのタイムゾーンで返されます。</span><span class="sxs-lookup"><span data-stu-id="f5cc0-138">The appointment and meeting times are returned in the time zone of the client.</span></span> <span data-ttu-id="f5cc0-139">すべての子要素が発生する順序で一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="f5cc0-139">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="f5cc0-140">この要素によって提供される詳細レベルは、リクエスターに付与されるアクセス許可によって異なります。</span><span class="sxs-lookup"><span data-stu-id="f5cc0-140">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="f5cc0-141">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f5cc0-141">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f5cc0-142">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f5cc0-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f5cc0-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="f5cc0-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f5cc0-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f5cc0-144">Schema Name</span></span>  <br/> |<span data-ttu-id="f5cc0-145">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f5cc0-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="f5cc0-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f5cc0-146">Validation File</span></span>  <br/> |<span data-ttu-id="f5cc0-147">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f5cc0-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f5cc0-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f5cc0-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="f5cc0-149">正しくない</span><span class="sxs-lookup"><span data-stu-id="f5cc0-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f5cc0-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="f5cc0-150">See also</span></span>



[<span data-ttu-id="f5cc0-151">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="f5cc0-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="f5cc0-152">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f5cc0-152">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="f5cc0-153">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="f5cc0-153">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


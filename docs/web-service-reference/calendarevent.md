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
description: CalendarEvent 要素は、一意の予定表アイテムの出現を表します。
ms.openlocfilehash: f7fff7ba511ca12813dd4c2d694e89c97589ba31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759579"
---
# <a name="calendarevent"></a><span data-ttu-id="cf2bc-103">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="cf2bc-103">CalendarEvent</span></span>

<span data-ttu-id="cf2bc-104">**CalendarEvent**要素は、一意の予定表アイテムの出現を表します。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-104">The **CalendarEvent** element represents a unique calendar item occurrence.</span></span> 
  
[<span data-ttu-id="cf2bc-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="cf2bc-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="cf2bc-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="cf2bc-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="cf2bc-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="cf2bc-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="cf2bc-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="cf2bc-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="cf2bc-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="cf2bc-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="cf2bc-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="cf2bc-110">CalendarEvent</span></span>](calendarevent.md)
  
```xml
<CalendarEvent>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
   <BusyType>...</BusyType>
   <CalendarEventDetails>...</CalendarEventDetails>
</CalendarEvent>
```

 <span data-ttu-id="cf2bc-111">**CalendarEvent**</span><span class="sxs-lookup"><span data-stu-id="cf2bc-111">**CalendarEvent**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf2bc-112">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cf2bc-112">Attributes and elements</span></span>

<span data-ttu-id="cf2bc-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf2bc-114">属性</span><span class="sxs-lookup"><span data-stu-id="cf2bc-114">Attributes</span></span>

<span data-ttu-id="cf2bc-115">なし。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf2bc-116">子要素</span><span class="sxs-lookup"><span data-stu-id="cf2bc-116">Child elements</span></span>

|<span data-ttu-id="cf2bc-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="cf2bc-117">**Element**</span></span>|<span data-ttu-id="cf2bc-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="cf2bc-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf2bc-119">開始時刻</span><span class="sxs-lookup"><span data-stu-id="cf2bc-119">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="cf2bc-120">予定表イベントの開始を表します。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-120">Represents the start of a calendar event.</span></span> <span data-ttu-id="cf2bc-121">これは、必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-121">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="cf2bc-122">終了時刻</span><span class="sxs-lookup"><span data-stu-id="cf2bc-122">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="cf2bc-123">予定表のイベントの終了を表します。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-123">Represents the end of a calendar event.</span></span> <span data-ttu-id="cf2bc-124">これは、必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-124">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="cf2bc-125">BusyType</span><span class="sxs-lookup"><span data-stu-id="cf2bc-125">BusyType</span></span>](busytype.md) <br/> |<span data-ttu-id="cf2bc-126">予定表イベントの空き時間情報の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-126">Represents the free/busy status set for a calendar event.</span></span> <span data-ttu-id="cf2bc-127">これは、必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-127">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="cf2bc-128">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="cf2bc-128">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="cf2bc-129">カレンダー イベントの追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-129">Provides additional information for a calendar event.</span></span> <span data-ttu-id="cf2bc-130">これは、省略可能な子要素です。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-130">This is an optional child element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cf2bc-131">親要素</span><span class="sxs-lookup"><span data-stu-id="cf2bc-131">Parent elements</span></span>

|<span data-ttu-id="cf2bc-132">**要素**</span><span class="sxs-lookup"><span data-stu-id="cf2bc-132">**Element**</span></span>|<span data-ttu-id="cf2bc-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="cf2bc-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf2bc-134">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="cf2bc-134">CalendarEventArray</span></span>](calendareventarray.md) <br/> |<span data-ttu-id="cf2bc-135">要求されたユーザーの可用性を表す一意の予定表アイテムの出現回数のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-135">Contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span>  <br/> <span data-ttu-id="cf2bc-136">この要素への XPath 2.0 の式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-136">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cf2bc-137">備考</span><span class="sxs-lookup"><span data-stu-id="cf2bc-137">Remarks</span></span>

<span data-ttu-id="cf2bc-138">クライアントのタイム ゾーンでは、予定と会議の時刻が返されます。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-138">The appointment and meeting times are returned in the time zone of the client.</span></span> <span data-ttu-id="cf2bc-139">発生したシーケンスは、すべての子要素の一覧です。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-139">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="cf2bc-140">この要素によって提供される詳細のレベルは、要求側に付与するアクセス許可に依存します。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-140">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="cf2bc-141">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-141">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf2bc-142">要素情報</span><span class="sxs-lookup"><span data-stu-id="cf2bc-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf2bc-143">名前空間</span><span class="sxs-lookup"><span data-stu-id="cf2bc-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cf2bc-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cf2bc-144">Schema Name</span></span>  <br/> |<span data-ttu-id="cf2bc-145">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="cf2bc-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="cf2bc-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cf2bc-146">Validation File</span></span>  <br/> |<span data-ttu-id="cf2bc-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cf2bc-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cf2bc-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cf2bc-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf2bc-149">False</span><span class="sxs-lookup"><span data-stu-id="cf2bc-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf2bc-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="cf2bc-150">See also</span></span>



[<span data-ttu-id="cf2bc-151">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="cf2bc-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="cf2bc-152">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="cf2bc-152">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="cf2bc-153">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="cf2bc-153">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


---
title: CalendarEventDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEventDetails
api_type:
- schema
ms.assetid: 2dca0192-b91b-4154-aa09-84da74e875e9
description: CalendarEventDetails 要素は、予定表のイベントに関する追加情報を提供します。
ms.openlocfilehash: 8df4f3ed4f66c7dcba00e1f0c5b0c383075da0a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759581"
---
# <a name="calendareventdetails"></a><span data-ttu-id="1ba6a-103">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="1ba6a-103">CalendarEventDetails</span></span>

<span data-ttu-id="1ba6a-104">**CalendarEventDetails**要素は、予定表のイベントに関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-104">The **CalendarEventDetails** element provides additional information about a calendar event.</span></span> 
  
[<span data-ttu-id="1ba6a-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1ba6a-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="1ba6a-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="1ba6a-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="1ba6a-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="1ba6a-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="1ba6a-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="1ba6a-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="1ba6a-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="1ba6a-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="1ba6a-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="1ba6a-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="1ba6a-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="1ba6a-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
```xml
<CalendarEventDetails>
   <ID/>
   <Subject/>
   <Location/>
   <IsMeeting/>
   <IsRecurring/>
   <IsException/>
   <IsReminderSet/>
   <IsPrivate/>
</CalendarEventDetails>
```

 <span data-ttu-id="1ba6a-112">**CalendarEventDetails**</span><span class="sxs-lookup"><span data-stu-id="1ba6a-112">**CalendarEventDetails**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ba6a-113">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1ba6a-113">Attributes and elements</span></span>

<span data-ttu-id="1ba6a-114">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ba6a-115">属性</span><span class="sxs-lookup"><span data-stu-id="1ba6a-115">Attributes</span></span>

<span data-ttu-id="1ba6a-116">なし。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1ba6a-117">子要素</span><span class="sxs-lookup"><span data-stu-id="1ba6a-117">Child elements</span></span>

|<span data-ttu-id="1ba6a-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="1ba6a-118">**Element**</span></span>|<span data-ttu-id="1ba6a-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ba6a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ba6a-120">ID</span><span class="sxs-lookup"><span data-stu-id="1ba6a-120">ID</span></span>](id.md) <br/> |<span data-ttu-id="1ba6a-121">予定表アイテムのエントリ ID を表します。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-121">Represents the entry ID of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="1ba6a-122">件名 (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="1ba6a-122">Subject (CalendarEventDetails)</span></span>](subject-calendareventdetails.md) <br/> |<span data-ttu-id="1ba6a-123">予定表アイテムの件名を表します。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-123">Represents the subject of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="1ba6a-124">場所 (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="1ba6a-124">Location (CalendarEventDetails)</span></span>](location-calendareventdetails.md) <br/> |<span data-ttu-id="1ba6a-125">予定表アイテムの [場所] フィールドを表します。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-125">Represents the location field of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="1ba6a-126">IsMeeting (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="1ba6a-126">IsMeeting (CalendarEventDetails)</span></span>](ismeeting-calendareventdetails.md) <br/> |<span data-ttu-id="1ba6a-127">予定表のイベントは、会議または予定かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-127">Indicates whether the calendar event is a meeting or an appointment.</span></span>  <br/> |
|[<span data-ttu-id="1ba6a-128">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="1ba6a-128">IsRecurring (CalendarEventDetails)</span></span>](isrecurring-calendareventdetails.md) <br/> |<span data-ttu-id="1ba6a-129">予定表のイベントが定期的な予定表アイテムまたは単一の予定表アイテムのインスタンスであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-129">Indicates whether the calendar event is an instance of a recurring calendar item or a single calendar item.</span></span>  <br/> |
|[<span data-ttu-id="1ba6a-130">IsException</span><span class="sxs-lookup"><span data-stu-id="1ba6a-130">IsException</span></span>](isexception.md) <br/> |<span data-ttu-id="1ba6a-131">マスターから定期的な予定表アイテムのインスタンスが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-131">Indicates whether an instance of a recurring calendar item is changed from the master.</span></span>  <br/> |
|[<span data-ttu-id="1ba6a-132">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="1ba6a-132">IsReminderSet</span></span>](isreminderset.md) <br/> |<span data-ttu-id="1ba6a-133">カレンダー イベントのアラームが設定されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-133">Indicates whether a reminder has been set for the calendar event.</span></span>  <br/> |
|[<span data-ttu-id="1ba6a-134">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="1ba6a-134">IsPrivate</span></span>](isprivate.md) <br/> |<span data-ttu-id="1ba6a-135">予定表アイテムがプライベートかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-135">Indicates whether the calendar item is private.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1ba6a-136">親要素</span><span class="sxs-lookup"><span data-stu-id="1ba6a-136">Parent elements</span></span>

|<span data-ttu-id="1ba6a-137">**要素**</span><span class="sxs-lookup"><span data-stu-id="1ba6a-137">**Element**</span></span>|<span data-ttu-id="1ba6a-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ba6a-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ba6a-139">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="1ba6a-139">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="1ba6a-140">独自の予定表アイテムの出現を表します。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-140">Represents a unique calendar item occurrence.</span></span>  <br/> <span data-ttu-id="1ba6a-141">この要素への XPath 2.0 の式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-141">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1ba6a-142">備考</span><span class="sxs-lookup"><span data-stu-id="1ba6a-142">Remarks</span></span>

<span data-ttu-id="1ba6a-143">発生したシーケンスは、すべての子要素の一覧です。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-143">All the child elements are listed in the sequence in which they occur.</span></span> 
  
<span data-ttu-id="1ba6a-144">[IsPrivate](isprivate.md)要素が**true**の場合は、 [CalendarEventDetails](calendareventdetails.md)要素内の他のすべての要素は、応答で返されません。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-144">If the [IsPrivate](isprivate.md) element is **true**, all the other elements in the [CalendarEventDetails](calendareventdetails.md) element are not returned in the response.</span></span> 
  
<span data-ttu-id="1ba6a-145">GetUserAvailability 操作では、呼び出し元は、ターゲット ユーザーの予定表の読み取りアクセス権を持っていない限り、呼び出し元の詳細な情報は返されません。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-145">The GetUserAvailability operation does not return detailed caller information unless the caller has read access on the target user's calendar.</span></span> <span data-ttu-id="1ba6a-146">Exchange 管理シェルを使用してアクセス許可を設定することができます。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-146">You can set access permissions by using the Exchange Management Shell.</span></span>
  
<span data-ttu-id="1ba6a-147">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ba6a-148">要素情報</span><span class="sxs-lookup"><span data-stu-id="1ba6a-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ba6a-149">名前空間</span><span class="sxs-lookup"><span data-stu-id="1ba6a-149">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1ba6a-150">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1ba6a-150">Schema Name</span></span>  <br/> |<span data-ttu-id="1ba6a-151">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1ba6a-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="1ba6a-152">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1ba6a-152">Validation File</span></span>  <br/> |<span data-ttu-id="1ba6a-153">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1ba6a-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1ba6a-154">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1ba6a-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="1ba6a-155">False</span><span class="sxs-lookup"><span data-stu-id="1ba6a-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ba6a-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="1ba6a-156">See also</span></span>



[<span data-ttu-id="1ba6a-157">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="1ba6a-157">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="1ba6a-158">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1ba6a-158">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="1ba6a-159">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="1ba6a-159">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


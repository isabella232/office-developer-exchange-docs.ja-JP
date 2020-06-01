---
title: IsMeeting (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeeting
api_type:
- schema
ms.assetid: dd6900e4-e4a3-471a-909d-7240ebec501b
description: IsMeeting 要素は、予定表イベントが会議と予定のどちらであるかを示します。
ms.openlocfilehash: b75dfba203177d6451f3847bf8d1f68014612e1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465997"
---
# <a name="ismeeting-calendareventdetails"></a><span data-ttu-id="7ebdd-103">IsMeeting (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="7ebdd-103">IsMeeting (CalendarEventDetails)</span></span>

<span data-ttu-id="7ebdd-104">**Ismeeting**要素は、予定表イベントが会議と予定のどちらであるかを示します。</span><span class="sxs-lookup"><span data-stu-id="7ebdd-104">The **IsMeeting** element indicates whether the calendar event is a meeting or an appointment.</span></span> 
  
[<span data-ttu-id="7ebdd-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7ebdd-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="7ebdd-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="7ebdd-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="7ebdd-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="7ebdd-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="7ebdd-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="7ebdd-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="7ebdd-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="7ebdd-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="7ebdd-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="7ebdd-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="7ebdd-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="7ebdd-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="7ebdd-112">IsMeeting (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="7ebdd-112">IsMeeting (CalendarEventDetails)</span></span>](ismeeting-calendareventdetails.md)
  
```xml
<IsMeeting>true or false</IsMeeting>
```

 <span data-ttu-id="7ebdd-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="7ebdd-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7ebdd-114">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7ebdd-114">Attributes and elements</span></span>

<span data-ttu-id="7ebdd-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7ebdd-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ebdd-116">属性</span><span class="sxs-lookup"><span data-stu-id="7ebdd-116">Attributes</span></span>

<span data-ttu-id="7ebdd-117">なし。</span><span class="sxs-lookup"><span data-stu-id="7ebdd-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7ebdd-118">子要素</span><span class="sxs-lookup"><span data-stu-id="7ebdd-118">Child elements</span></span>

<span data-ttu-id="7ebdd-119">なし。</span><span class="sxs-lookup"><span data-stu-id="7ebdd-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7ebdd-120">親要素</span><span class="sxs-lookup"><span data-stu-id="7ebdd-120">Parent elements</span></span>

|<span data-ttu-id="7ebdd-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="7ebdd-121">**Element**</span></span>|<span data-ttu-id="7ebdd-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="7ebdd-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ebdd-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="7ebdd-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="7ebdd-124">予定表イベントに関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="7ebdd-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="7ebdd-125">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ebdd-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7ebdd-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7ebdd-126">Text value</span></span>

<span data-ttu-id="7ebdd-127">この要素が応答で返される場合は、テキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="7ebdd-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="7ebdd-128">この要素は、 [CalendarEventDetails](calendareventdetails.md)要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="7ebdd-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7ebdd-129">注釈</span><span class="sxs-lookup"><span data-stu-id="7ebdd-129">Remarks</span></span>

<span data-ttu-id="7ebdd-130">会議と予定の違いは、会議は出席者を含む予定表アイテムであるということです。予定は出席者を含まない予定表アイテムです。</span><span class="sxs-lookup"><span data-stu-id="7ebdd-130">The difference between a meeting and an appointment is that a meeting is a calendar item that includes attendees; an appointment is a calendar item that does not include attendees.</span></span>
  
<span data-ttu-id="7ebdd-131">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7ebdd-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ebdd-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7ebdd-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ebdd-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="7ebdd-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7ebdd-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7ebdd-134">Schema Name</span></span>  <br/> |<span data-ttu-id="7ebdd-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7ebdd-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="7ebdd-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7ebdd-136">Validation File</span></span>  <br/> |<span data-ttu-id="7ebdd-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7ebdd-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7ebdd-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7ebdd-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="7ebdd-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="7ebdd-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ebdd-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="7ebdd-140">See also</span></span>



[<span data-ttu-id="7ebdd-141">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="7ebdd-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="7ebdd-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7ebdd-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="7ebdd-143">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="7ebdd-143">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


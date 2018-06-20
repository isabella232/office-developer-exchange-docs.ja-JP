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
description: IsMeeting 要素は、予定表のイベントは、会議または予定かどうかを示します。
ms.openlocfilehash: f3f6e0cc5fbfe29e5a818d69794cbaf5b6855962
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832046"
---
# <a name="ismeeting-calendareventdetails"></a><span data-ttu-id="b1a43-103">IsMeeting (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="b1a43-103">IsMeeting (CalendarEventDetails)</span></span>

<span data-ttu-id="b1a43-104">**IsMeeting**要素は、予定表のイベントは、会議または予定かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b1a43-104">The **IsMeeting** element indicates whether the calendar event is a meeting or an appointment.</span></span> 
  
[<span data-ttu-id="b1a43-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b1a43-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="b1a43-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="b1a43-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="b1a43-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="b1a43-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="b1a43-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="b1a43-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="b1a43-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="b1a43-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="b1a43-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="b1a43-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="b1a43-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="b1a43-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="b1a43-112">IsMeeting (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="b1a43-112">IsMeeting (CalendarEventDetails)</span></span>](ismeeting-calendareventdetails.md)
  
```xml
<IsMeeting>true or false</IsMeeting>
```

 <span data-ttu-id="b1a43-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="b1a43-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b1a43-114">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b1a43-114">Attributes and elements</span></span>

<span data-ttu-id="b1a43-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b1a43-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b1a43-116">属性</span><span class="sxs-lookup"><span data-stu-id="b1a43-116">Attributes</span></span>

<span data-ttu-id="b1a43-117">なし。</span><span class="sxs-lookup"><span data-stu-id="b1a43-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b1a43-118">子要素</span><span class="sxs-lookup"><span data-stu-id="b1a43-118">Child elements</span></span>

<span data-ttu-id="b1a43-119">なし。</span><span class="sxs-lookup"><span data-stu-id="b1a43-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b1a43-120">親要素</span><span class="sxs-lookup"><span data-stu-id="b1a43-120">Parent elements</span></span>

|<span data-ttu-id="b1a43-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="b1a43-121">**Element**</span></span>|<span data-ttu-id="b1a43-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="b1a43-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b1a43-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="b1a43-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="b1a43-124">カレンダー イベントの追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="b1a43-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="b1a43-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="b1a43-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b1a43-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b1a43-126">Text value</span></span>

<span data-ttu-id="b1a43-127">テキスト値は、この要素が応答で返された場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="b1a43-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="b1a43-128">[CalendarEventDetails](calendareventdetails.md)要素を使用する場合、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="b1a43-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b1a43-129">備考</span><span class="sxs-lookup"><span data-stu-id="b1a43-129">Remarks</span></span>

<span data-ttu-id="b1a43-130">会議と予定の違いは、会議の出席者を含む予定表アイテムであります。予定は、予定表アイテムの出席者が含まれていないです。</span><span class="sxs-lookup"><span data-stu-id="b1a43-130">The difference between a meeting and an appointment is that a meeting is a calendar item that includes attendees; an appointment is a calendar item that does not include attendees.</span></span>
  
<span data-ttu-id="b1a43-131">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="b1a43-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b1a43-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="b1a43-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b1a43-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="b1a43-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b1a43-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b1a43-134">Schema Name</span></span>  <br/> |<span data-ttu-id="b1a43-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b1a43-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="b1a43-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b1a43-136">Validation File</span></span>  <br/> |<span data-ttu-id="b1a43-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b1a43-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b1a43-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b1a43-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="b1a43-139">False</span><span class="sxs-lookup"><span data-stu-id="b1a43-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b1a43-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="b1a43-140">See also</span></span>



[<span data-ttu-id="b1a43-141">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="b1a43-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="b1a43-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b1a43-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="b1a43-143">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="b1a43-143">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


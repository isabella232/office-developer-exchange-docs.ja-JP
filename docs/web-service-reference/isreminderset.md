---
title: IsReminderSet
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsReminderSet
api_type:
- schema
ms.assetid: 6aea4cb7-ca14-4949-8e7f-660b565f6556
description: IsReminderSet 要素は、カレンダー イベントのアラームが設定されているかどうかを示します。
ms.openlocfilehash: 589178072baca652bff2779e64a212fb90478247
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832100"
---
# <a name="isreminderset"></a><span data-ttu-id="0f77f-103">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="0f77f-103">IsReminderSet</span></span>

<span data-ttu-id="0f77f-104">**IsReminderSet**要素は、カレンダー イベントのアラームが設定されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0f77f-104">The **IsReminderSet** element indicates whether a reminder has been set for the calendar event.</span></span> 
  
[<span data-ttu-id="0f77f-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="0f77f-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="0f77f-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="0f77f-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="0f77f-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="0f77f-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="0f77f-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="0f77f-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="0f77f-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="0f77f-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="0f77f-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="0f77f-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="0f77f-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="0f77f-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="0f77f-112">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="0f77f-112">IsReminderSet</span></span>](isreminderset.md)
  
```xml
<IsReminderSet>true or false</IsReminderSet>
```

 <span data-ttu-id="0f77f-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="0f77f-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0f77f-114">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0f77f-114">Attributes and elements</span></span>

<span data-ttu-id="0f77f-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0f77f-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f77f-116">属性</span><span class="sxs-lookup"><span data-stu-id="0f77f-116">Attributes</span></span>

<span data-ttu-id="0f77f-117">なし。</span><span class="sxs-lookup"><span data-stu-id="0f77f-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0f77f-118">子要素</span><span class="sxs-lookup"><span data-stu-id="0f77f-118">Child elements</span></span>

<span data-ttu-id="0f77f-119">なし。</span><span class="sxs-lookup"><span data-stu-id="0f77f-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0f77f-120">親要素</span><span class="sxs-lookup"><span data-stu-id="0f77f-120">Parent elements</span></span>

|<span data-ttu-id="0f77f-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="0f77f-121">**Element**</span></span>|<span data-ttu-id="0f77f-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="0f77f-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f77f-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="0f77f-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="0f77f-124">予定表のイベントに関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="0f77f-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="0f77f-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="0f77f-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0f77f-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0f77f-126">Text value</span></span>

<span data-ttu-id="0f77f-127">テキスト値は、この要素が応答で返された場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="0f77f-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="0f77f-128">[IsPrivate](isprivate.md)要素が**true**に設定しない限り、 [CalendarEventDetails](calendareventdetails.md)要素を使用する場合、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f77f-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used unless the [IsPrivate](isprivate.md) element is set to **true**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0f77f-129">備考</span><span class="sxs-lookup"><span data-stu-id="0f77f-129">Remarks</span></span>

<span data-ttu-id="0f77f-130">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="0f77f-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0f77f-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="0f77f-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f77f-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="0f77f-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0f77f-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0f77f-133">Schema Name</span></span>  <br/> |<span data-ttu-id="0f77f-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="0f77f-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="0f77f-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0f77f-135">Validation File</span></span>  <br/> |<span data-ttu-id="0f77f-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0f77f-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0f77f-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0f77f-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="0f77f-138">False</span><span class="sxs-lookup"><span data-stu-id="0f77f-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0f77f-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="0f77f-139">See also</span></span>



[<span data-ttu-id="0f77f-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="0f77f-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="0f77f-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="0f77f-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="0f77f-142">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="0f77f-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


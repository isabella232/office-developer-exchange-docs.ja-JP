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
description: IsReminderSet 要素は、予定表イベントにアラームが設定されているかどうかを示します。
ms.openlocfilehash: e2f5fa072b549bdaf636a15313e7dfe72172f768
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460338"
---
# <a name="isreminderset"></a><span data-ttu-id="7bc25-103">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="7bc25-103">IsReminderSet</span></span>

<span data-ttu-id="7bc25-104">**IsReminderSet**要素は、予定表イベントにアラームが設定されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7bc25-104">The **IsReminderSet** element indicates whether a reminder has been set for the calendar event.</span></span> 
  
[<span data-ttu-id="7bc25-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7bc25-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="7bc25-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="7bc25-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="7bc25-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="7bc25-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="7bc25-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="7bc25-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="7bc25-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="7bc25-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="7bc25-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="7bc25-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="7bc25-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="7bc25-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="7bc25-112">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="7bc25-112">IsReminderSet</span></span>](isreminderset.md)
  
```xml
<IsReminderSet>true or false</IsReminderSet>
```

 <span data-ttu-id="7bc25-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="7bc25-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7bc25-114">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7bc25-114">Attributes and elements</span></span>

<span data-ttu-id="7bc25-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7bc25-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7bc25-116">属性</span><span class="sxs-lookup"><span data-stu-id="7bc25-116">Attributes</span></span>

<span data-ttu-id="7bc25-117">なし。</span><span class="sxs-lookup"><span data-stu-id="7bc25-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7bc25-118">子要素</span><span class="sxs-lookup"><span data-stu-id="7bc25-118">Child elements</span></span>

<span data-ttu-id="7bc25-119">なし。</span><span class="sxs-lookup"><span data-stu-id="7bc25-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7bc25-120">親要素</span><span class="sxs-lookup"><span data-stu-id="7bc25-120">Parent elements</span></span>

|<span data-ttu-id="7bc25-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="7bc25-121">**Element**</span></span>|<span data-ttu-id="7bc25-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="7bc25-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7bc25-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="7bc25-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="7bc25-124">予定表イベントに関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="7bc25-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="7bc25-125">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7bc25-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7bc25-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7bc25-126">Text value</span></span>

<span data-ttu-id="7bc25-127">この要素が応答で返される場合は、テキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="7bc25-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="7bc25-128">この要素は、 [IsPrivate](isprivate.md)要素が**true**に設定されていない限り、 [CalendarEventDetails](calendareventdetails.md)要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="7bc25-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used unless the [IsPrivate](isprivate.md) element is set to **true**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7bc25-129">注釈</span><span class="sxs-lookup"><span data-stu-id="7bc25-129">Remarks</span></span>

<span data-ttu-id="7bc25-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7bc25-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7bc25-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7bc25-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7bc25-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="7bc25-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7bc25-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7bc25-133">Schema Name</span></span>  <br/> |<span data-ttu-id="7bc25-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7bc25-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="7bc25-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7bc25-135">Validation File</span></span>  <br/> |<span data-ttu-id="7bc25-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7bc25-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7bc25-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7bc25-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="7bc25-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="7bc25-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7bc25-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="7bc25-139">See also</span></span>



[<span data-ttu-id="7bc25-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="7bc25-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="7bc25-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7bc25-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="7bc25-142">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="7bc25-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


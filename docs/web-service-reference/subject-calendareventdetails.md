---
title: Subject (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subject
api_type:
- schema
ms.assetid: 05e955b5-8e90-4043-b06b-6ce523eaed9b
description: Subject 要素は、予定表アイテムの件名を表します。
ms.openlocfilehash: 268e5fa4bb8d02d83154267fc8e475c6d2b7c31c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463056"
---
# <a name="subject-calendareventdetails"></a><span data-ttu-id="3122a-103">Subject (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="3122a-103">Subject (CalendarEventDetails)</span></span>

<span data-ttu-id="3122a-104">**Subject**要素は、予定表アイテムの件名を表します。</span><span class="sxs-lookup"><span data-stu-id="3122a-104">The **Subject** element represents the subject of a calendar item.</span></span> 
  
[<span data-ttu-id="3122a-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="3122a-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="3122a-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="3122a-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="3122a-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="3122a-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="3122a-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="3122a-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="3122a-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="3122a-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="3122a-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="3122a-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="3122a-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="3122a-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="3122a-112">Subject (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="3122a-112">Subject (CalendarEventDetails)</span></span>](subject-calendareventdetails.md)
  
```xml
<Subject/>
```

 <span data-ttu-id="3122a-113">**string**</span><span class="sxs-lookup"><span data-stu-id="3122a-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3122a-114">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3122a-114">Attributes and elements</span></span>

<span data-ttu-id="3122a-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3122a-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3122a-116">属性</span><span class="sxs-lookup"><span data-stu-id="3122a-116">Attributes</span></span>

<span data-ttu-id="3122a-117">なし。</span><span class="sxs-lookup"><span data-stu-id="3122a-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3122a-118">子要素</span><span class="sxs-lookup"><span data-stu-id="3122a-118">Child elements</span></span>

<span data-ttu-id="3122a-119">なし。</span><span class="sxs-lookup"><span data-stu-id="3122a-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3122a-120">親要素</span><span class="sxs-lookup"><span data-stu-id="3122a-120">Parent elements</span></span>

|<span data-ttu-id="3122a-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="3122a-121">**Element**</span></span>|<span data-ttu-id="3122a-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="3122a-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3122a-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="3122a-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="3122a-124">予定表イベントに関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="3122a-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="3122a-125">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3122a-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3122a-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3122a-126">Text value</span></span>

<span data-ttu-id="3122a-127">この要素が応答で返される場合は、テキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="3122a-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="3122a-128">[IsPrivate](isprivate.md)要素の値が**true**に等しい場合、この要素は返されません。</span><span class="sxs-lookup"><span data-stu-id="3122a-128">This element will not be returned if the [IsPrivate](isprivate.md) element value is equal to **true**.</span></span> <span data-ttu-id="3122a-129">この要素には、空の文字列を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="3122a-129">This element can contain an empty string.</span></span> <span data-ttu-id="3122a-130">[CalendarEventDetails](calendareventdetails.md)要素が使用されている場合、この要素は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="3122a-130">This element is optional if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3122a-131">注釈</span><span class="sxs-lookup"><span data-stu-id="3122a-131">Remarks</span></span>

<span data-ttu-id="3122a-132">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="3122a-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3122a-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3122a-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3122a-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="3122a-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3122a-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3122a-135">Schema Name</span></span>  <br/> |<span data-ttu-id="3122a-136">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="3122a-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="3122a-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3122a-137">Validation File</span></span>  <br/> |<span data-ttu-id="3122a-138">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="3122a-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3122a-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3122a-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="3122a-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="3122a-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3122a-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="3122a-141">See also</span></span>



[<span data-ttu-id="3122a-142">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="3122a-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="3122a-143">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="3122a-143">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="3122a-144">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="3122a-144">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


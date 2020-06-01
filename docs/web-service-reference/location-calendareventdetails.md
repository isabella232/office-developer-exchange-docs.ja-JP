---
title: 場所 (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Location
api_type:
- schema
ms.assetid: 883cce6e-66b8-4dbc-935c-83ef5100a953
description: Location 要素は、予定表アイテムの "場所" フィールドを表します。
ms.openlocfilehash: 4a590c315d2211ce9128305a514e68f1c785596c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467999"
---
# <a name="location-calendareventdetails"></a><span data-ttu-id="a3f05-103">場所 (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="a3f05-103">Location (CalendarEventDetails)</span></span>

<span data-ttu-id="a3f05-104">**Location**要素は、予定表アイテムの "場所" フィールドを表します。</span><span class="sxs-lookup"><span data-stu-id="a3f05-104">The **Location** element represents the location field of the calendar item.</span></span> 
  
[<span data-ttu-id="a3f05-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a3f05-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="a3f05-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="a3f05-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="a3f05-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="a3f05-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="a3f05-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="a3f05-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="a3f05-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="a3f05-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="a3f05-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="a3f05-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="a3f05-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="a3f05-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="a3f05-112">場所 (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="a3f05-112">Location (CalendarEventDetails)</span></span>](location-calendareventdetails.md)
  
```xml
<Location/>
```

 <span data-ttu-id="a3f05-113">**string**</span><span class="sxs-lookup"><span data-stu-id="a3f05-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a3f05-114">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a3f05-114">Attributes and elements</span></span>

<span data-ttu-id="a3f05-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a3f05-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3f05-116">属性</span><span class="sxs-lookup"><span data-stu-id="a3f05-116">Attributes</span></span>

<span data-ttu-id="a3f05-117">なし。</span><span class="sxs-lookup"><span data-stu-id="a3f05-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3f05-118">子要素</span><span class="sxs-lookup"><span data-stu-id="a3f05-118">Child elements</span></span>

<span data-ttu-id="a3f05-119">なし。</span><span class="sxs-lookup"><span data-stu-id="a3f05-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a3f05-120">親要素</span><span class="sxs-lookup"><span data-stu-id="a3f05-120">Parent elements</span></span>

|<span data-ttu-id="a3f05-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="a3f05-121">**Element**</span></span>|<span data-ttu-id="a3f05-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="a3f05-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3f05-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="a3f05-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="a3f05-124">予定表イベントに関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="a3f05-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="a3f05-125">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a3f05-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a3f05-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a3f05-126">Text value</span></span>

<span data-ttu-id="a3f05-127">この要素が応答で返される場合は、テキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3f05-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="a3f05-128">この要素には、空の文字列を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a3f05-128">This element can contain an empty string.</span></span> <span data-ttu-id="a3f05-129">[CalendarEventDetails](calendareventdetails.md)要素が使用されている場合、この要素は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="a3f05-129">This element is optional if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a3f05-130">注釈</span><span class="sxs-lookup"><span data-stu-id="a3f05-130">Remarks</span></span>

<span data-ttu-id="a3f05-131">この要素は、MAPI という名前の PR_Location プロパティにマップします。</span><span class="sxs-lookup"><span data-stu-id="a3f05-131">This element maps to a PR_Location MAPI named property.</span></span>
  
<span data-ttu-id="a3f05-132">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a3f05-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3f05-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a3f05-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3f05-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="a3f05-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a3f05-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a3f05-135">Schema Name</span></span>  <br/> |<span data-ttu-id="a3f05-136">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a3f05-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="a3f05-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a3f05-137">Validation File</span></span>  <br/> |<span data-ttu-id="a3f05-138">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a3f05-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a3f05-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a3f05-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="a3f05-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="a3f05-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a3f05-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="a3f05-141">See also</span></span>



[<span data-ttu-id="a3f05-142">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="a3f05-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="a3f05-143">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a3f05-143">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="a3f05-144">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="a3f05-144">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


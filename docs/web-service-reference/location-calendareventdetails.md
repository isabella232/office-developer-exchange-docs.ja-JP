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
description: Location 要素では、予定表アイテムの [場所] フィールドを表します。
ms.openlocfilehash: 3678bd94851633fcca9817c020106670b57d110c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832245"
---
# <a name="location-calendareventdetails"></a><span data-ttu-id="32308-103">場所 (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="32308-103">Location (CalendarEventDetails)</span></span>

<span data-ttu-id="32308-104">**Location**要素では、予定表アイテムの [場所] フィールドを表します。</span><span class="sxs-lookup"><span data-stu-id="32308-104">The **Location** element represents the location field of the calendar item.</span></span> 
  
[<span data-ttu-id="32308-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="32308-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="32308-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="32308-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="32308-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="32308-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="32308-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="32308-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="32308-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="32308-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="32308-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="32308-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="32308-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="32308-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="32308-112">場所 (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="32308-112">Location (CalendarEventDetails)</span></span>](location-calendareventdetails.md)
  
```xml
<Location/>
```

 <span data-ttu-id="32308-113">**string**</span><span class="sxs-lookup"><span data-stu-id="32308-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32308-114">属性および要素</span><span class="sxs-lookup"><span data-stu-id="32308-114">Attributes and elements</span></span>

<span data-ttu-id="32308-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="32308-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32308-116">属性</span><span class="sxs-lookup"><span data-stu-id="32308-116">Attributes</span></span>

<span data-ttu-id="32308-117">なし。</span><span class="sxs-lookup"><span data-stu-id="32308-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="32308-118">子要素</span><span class="sxs-lookup"><span data-stu-id="32308-118">Child elements</span></span>

<span data-ttu-id="32308-119">なし。</span><span class="sxs-lookup"><span data-stu-id="32308-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="32308-120">親要素</span><span class="sxs-lookup"><span data-stu-id="32308-120">Parent elements</span></span>

|<span data-ttu-id="32308-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="32308-121">**Element**</span></span>|<span data-ttu-id="32308-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="32308-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32308-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="32308-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="32308-124">カレンダー イベントの追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="32308-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="32308-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="32308-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="32308-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="32308-126">Text value</span></span>

<span data-ttu-id="32308-127">テキスト値は、この要素が応答で返された場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="32308-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="32308-128">この要素は、空の文字列を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="32308-128">This element can contain an empty string.</span></span> <span data-ttu-id="32308-129">[CalendarEventDetails](calendareventdetails.md)要素を使用する場合、この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="32308-129">This element is optional if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="32308-130">備考</span><span class="sxs-lookup"><span data-stu-id="32308-130">Remarks</span></span>

<span data-ttu-id="32308-131">この要素は、PR_Location の MAPI 名前付きプロパティにマップします。</span><span class="sxs-lookup"><span data-stu-id="32308-131">This element maps to a PR_Location MAPI named property.</span></span>
  
<span data-ttu-id="32308-132">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="32308-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="32308-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="32308-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32308-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="32308-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="32308-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="32308-135">Schema Name</span></span>  <br/> |<span data-ttu-id="32308-136">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="32308-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="32308-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="32308-137">Validation File</span></span>  <br/> |<span data-ttu-id="32308-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="32308-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="32308-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="32308-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="32308-140">False</span><span class="sxs-lookup"><span data-stu-id="32308-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32308-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="32308-141">See also</span></span>



[<span data-ttu-id="32308-142">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="32308-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="32308-143">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="32308-143">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="32308-144">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="32308-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


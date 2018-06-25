---
title: BusyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BusyType
api_type:
- schema
ms.assetid: 26d4fae0-8c78-4705-b5e8-d6033712c41e
description: BusyType 要素は、空き/予約済み状態の設定の予定表のイベントを表します。
ms.openlocfilehash: 6484bc70c6a05084e5d2bc1738b575fbebe4c132
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759577"
---
# <a name="busytype"></a><span data-ttu-id="afab0-103">BusyType</span><span class="sxs-lookup"><span data-stu-id="afab0-103">BusyType</span></span>

<span data-ttu-id="afab0-104">**BusyType**要素は、空き/予約済み状態の設定の予定表のイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="afab0-104">The **BusyType** element represents the free/busy status set for a calendar event.</span></span> 
  
```xml
<BusyType>Free or Tentative or Busy or OOF or NoData</BusyType>
```

 <span data-ttu-id="afab0-105">**BusyType**</span><span class="sxs-lookup"><span data-stu-id="afab0-105">**BusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="afab0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="afab0-106">Attributes and elements</span></span>

<span data-ttu-id="afab0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="afab0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="afab0-108">属性</span><span class="sxs-lookup"><span data-stu-id="afab0-108">Attributes</span></span>

<span data-ttu-id="afab0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="afab0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="afab0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="afab0-110">Child elements</span></span>

<span data-ttu-id="afab0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="afab0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="afab0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="afab0-112">Parent elements</span></span>

|<span data-ttu-id="afab0-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="afab0-113">**Element**</span></span>|<span data-ttu-id="afab0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="afab0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afab0-115">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="afab0-115">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md) <br/> |<span data-ttu-id="afab0-116">推奨される会議の時刻と同時に発生するタイム ・ ウィンドウのユーザーまたは連絡先の空き時間状況が含まれています。</span><span class="sxs-lookup"><span data-stu-id="afab0-116">Contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time.</span></span>  <br/> <span data-ttu-id="afab0-117">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="afab0-117">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/IndividualAttendeeConflictData` <br/> |
|[<span data-ttu-id="afab0-118">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="afab0-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="afab0-119">独自の予定表アイテムの出現を表します。</span><span class="sxs-lookup"><span data-stu-id="afab0-119">Represents a unique calendar item occurrence.</span></span>  <br/> <span data-ttu-id="afab0-120">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="afab0-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="afab0-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="afab0-121">Text value</span></span>

<span data-ttu-id="afab0-122">テキスト値は、この要素の必要があります。</span><span class="sxs-lookup"><span data-stu-id="afab0-122">A text value is required for this element.</span></span> <span data-ttu-id="afab0-123">値は、文字列型です。</span><span class="sxs-lookup"><span data-stu-id="afab0-123">The value is a string type.</span></span> <span data-ttu-id="afab0-124">[BusyType](busytype.md)要素の値は、次のように。</span><span class="sxs-lookup"><span data-stu-id="afab0-124">The following are the possible values for the [BusyType](busytype.md) element:</span></span> 
  
- <span data-ttu-id="afab0-125">Free</span><span class="sxs-lookup"><span data-stu-id="afab0-125">Free</span></span>
    
- <span data-ttu-id="afab0-126">Tentative</span><span class="sxs-lookup"><span data-stu-id="afab0-126">Tentative</span></span>
    
- <span data-ttu-id="afab0-127">Busy</span><span class="sxs-lookup"><span data-stu-id="afab0-127">Busy</span></span>
    
- <span data-ttu-id="afab0-128">不在時</span><span class="sxs-lookup"><span data-stu-id="afab0-128">OOF</span></span>
    
- <span data-ttu-id="afab0-129">NoData</span><span class="sxs-lookup"><span data-stu-id="afab0-129">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="afab0-130">備考</span><span class="sxs-lookup"><span data-stu-id="afab0-130">Remarks</span></span>

<span data-ttu-id="afab0-131">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="afab0-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="afab0-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="afab0-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="afab0-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="afab0-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="afab0-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="afab0-134">Schema Name</span></span>  <br/> |<span data-ttu-id="afab0-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="afab0-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="afab0-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="afab0-136">Validation File</span></span>  <br/> |<span data-ttu-id="afab0-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="afab0-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="afab0-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="afab0-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="afab0-139">False</span><span class="sxs-lookup"><span data-stu-id="afab0-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="afab0-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="afab0-140">See also</span></span>



[<span data-ttu-id="afab0-141">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="afab0-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="afab0-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="afab0-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="afab0-143">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="afab0-143">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


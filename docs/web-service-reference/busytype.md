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
description: BusyType 要素は、予定表イベントの空き時間状態セットを表します。
ms.openlocfilehash: 7c2d18c21156a8603d3caeeb796a56c5d8afcba5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459084"
---
# <a name="busytype"></a><span data-ttu-id="b490f-103">BusyType</span><span class="sxs-lookup"><span data-stu-id="b490f-103">BusyType</span></span>

<span data-ttu-id="b490f-104">**BusyType**要素は、予定表イベントの空き時間状態セットを表します。</span><span class="sxs-lookup"><span data-stu-id="b490f-104">The **BusyType** element represents the free/busy status set for a calendar event.</span></span> 
  
```xml
<BusyType>Free or Tentative or Busy or OOF or NoData</BusyType>
```

 <span data-ttu-id="b490f-105">**BusyType**</span><span class="sxs-lookup"><span data-stu-id="b490f-105">**BusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b490f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b490f-106">Attributes and elements</span></span>

<span data-ttu-id="b490f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b490f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b490f-108">属性</span><span class="sxs-lookup"><span data-stu-id="b490f-108">Attributes</span></span>

<span data-ttu-id="b490f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b490f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b490f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b490f-110">Child elements</span></span>

<span data-ttu-id="b490f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b490f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b490f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b490f-112">Parent elements</span></span>

|<span data-ttu-id="b490f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b490f-113">**Element**</span></span>|<span data-ttu-id="b490f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b490f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b490f-115">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="b490f-115">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md) <br/> |<span data-ttu-id="b490f-116">会議の提案時刻と同時に発生する時間枠のユーザーまたは連絡先の空き時間状態を格納します。</span><span class="sxs-lookup"><span data-stu-id="b490f-116">Contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time.</span></span>  <br/> <span data-ttu-id="b490f-117">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b490f-117">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/IndividualAttendeeConflictData` <br/> |
|[<span data-ttu-id="b490f-118">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="b490f-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="b490f-119">一意の予定表アイテムの出現を表します。</span><span class="sxs-lookup"><span data-stu-id="b490f-119">Represents a unique calendar item occurrence.</span></span>  <br/> <span data-ttu-id="b490f-120">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b490f-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b490f-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b490f-121">Text value</span></span>

<span data-ttu-id="b490f-122">この要素にはテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="b490f-122">A text value is required for this element.</span></span> <span data-ttu-id="b490f-123">値は文字列型です。</span><span class="sxs-lookup"><span data-stu-id="b490f-123">The value is a string type.</span></span> <span data-ttu-id="b490f-124">[BusyType](busytype.md)要素に使用できる値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="b490f-124">The following are the possible values for the [BusyType](busytype.md) element:</span></span> 
  
- <span data-ttu-id="b490f-125">空き</span><span class="sxs-lookup"><span data-stu-id="b490f-125">Free</span></span>
    
- <span data-ttu-id="b490f-126">仮の予定</span><span class="sxs-lookup"><span data-stu-id="b490f-126">Tentative</span></span>
    
- <span data-ttu-id="b490f-127">多忙</span><span class="sxs-lookup"><span data-stu-id="b490f-127">Busy</span></span>
    
- <span data-ttu-id="b490f-128">OOF</span><span class="sxs-lookup"><span data-stu-id="b490f-128">OOF</span></span>
    
- <span data-ttu-id="b490f-129">NoData</span><span class="sxs-lookup"><span data-stu-id="b490f-129">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="b490f-130">注釈</span><span class="sxs-lookup"><span data-stu-id="b490f-130">Remarks</span></span>

<span data-ttu-id="b490f-131">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b490f-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b490f-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b490f-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b490f-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="b490f-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b490f-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b490f-134">Schema Name</span></span>  <br/> |<span data-ttu-id="b490f-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b490f-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="b490f-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b490f-136">Validation File</span></span>  <br/> |<span data-ttu-id="b490f-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b490f-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b490f-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b490f-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="b490f-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="b490f-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b490f-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="b490f-140">See also</span></span>



[<span data-ttu-id="b490f-141">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="b490f-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="b490f-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b490f-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="b490f-143">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="b490f-143">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


---
title: IndividualAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndividualAttendeeConflictData
api_type:
- schema
ms.assetid: d45d3c34-abe1-40da-afd3-23bc5c3ef474
description: IndividualAttendeeConflictData 要素には、ユーザーのまたは提案の要素で提案された会議の時刻と同時に発生するタイム ・ ウィンドウの連絡先の空き/予約済みの状態を識別します。
ms.openlocfilehash: 0bd164e08a6f3685415452b7c82a4220cf69d792
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831930"
---
# <a name="individualattendeeconflictdata"></a><span data-ttu-id="72bdf-103">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="72bdf-103">IndividualAttendeeConflictData</span></span>

<span data-ttu-id="72bdf-104">**IndividualAttendeeConflictData**要素には、ユーザーのまたは[提案](suggestion.md)の要素で提案された会議の時刻と同時に発生するタイム ・ ウィンドウの連絡先の空き/予約済みの状態を識別します。</span><span class="sxs-lookup"><span data-stu-id="72bdf-104">The **IndividualAttendeeConflictData** element contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span> 
  
[<span data-ttu-id="72bdf-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="72bdf-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="72bdf-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="72bdf-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="72bdf-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="72bdf-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="72bdf-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="72bdf-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="72bdf-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="72bdf-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="72bdf-110">提案</span><span class="sxs-lookup"><span data-stu-id="72bdf-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="72bdf-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="72bdf-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="72bdf-112">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="72bdf-112">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md)
  
```xml
<IndividualAttendeeConflictData>
   <BusyType>...</BusyType>
</IndividualAttendeeConflictData>
```

 <span data-ttu-id="72bdf-113">**IndividualAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="72bdf-113">**IndividualAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="72bdf-114">属性および要素</span><span class="sxs-lookup"><span data-stu-id="72bdf-114">Attributes and elements</span></span>

<span data-ttu-id="72bdf-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="72bdf-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72bdf-116">属性</span><span class="sxs-lookup"><span data-stu-id="72bdf-116">Attributes</span></span>

<span data-ttu-id="72bdf-117">なし。</span><span class="sxs-lookup"><span data-stu-id="72bdf-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="72bdf-118">子要素</span><span class="sxs-lookup"><span data-stu-id="72bdf-118">Child elements</span></span>

|<span data-ttu-id="72bdf-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="72bdf-119">**Element**</span></span>|<span data-ttu-id="72bdf-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="72bdf-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72bdf-121">BusyType</span><span class="sxs-lookup"><span data-stu-id="72bdf-121">BusyType</span></span>](busytype.md) <br/> |<span data-ttu-id="72bdf-122">提案された会議の時間のユーザーの空き/予約済み状態を表します。</span><span class="sxs-lookup"><span data-stu-id="72bdf-122">Represents the free/busy status of a user for a suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="72bdf-123">親要素</span><span class="sxs-lookup"><span data-stu-id="72bdf-123">Parent elements</span></span>

|<span data-ttu-id="72bdf-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="72bdf-124">**Element**</span></span>|<span data-ttu-id="72bdf-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="72bdf-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72bdf-126">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="72bdf-126">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="72bdf-127">[GetUserAvailabilityRequest](getuseravailabilityrequest.md)で特定の出席者に対して競合データの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="72bdf-127">Contains an array of conflict data for attendees identified in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span></span>  <br/> <span data-ttu-id="72bdf-128">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="72bdf-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="72bdf-129">備考</span><span class="sxs-lookup"><span data-stu-id="72bdf-129">Remarks</span></span>

<span data-ttu-id="72bdf-130">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="72bdf-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="72bdf-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="72bdf-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72bdf-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="72bdf-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="72bdf-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="72bdf-133">Schema Name</span></span>  <br/> |<span data-ttu-id="72bdf-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="72bdf-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="72bdf-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="72bdf-135">Validation File</span></span>  <br/> |<span data-ttu-id="72bdf-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="72bdf-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="72bdf-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="72bdf-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="72bdf-138">False</span><span class="sxs-lookup"><span data-stu-id="72bdf-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="72bdf-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="72bdf-139">See also</span></span>



[<span data-ttu-id="72bdf-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="72bdf-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="72bdf-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="72bdf-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="72bdf-142">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="72bdf-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


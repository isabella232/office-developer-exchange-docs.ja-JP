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
description: IndividualAttendeeConflictData 要素には、提案要素で特定された会議の時間と同時に発生する時間枠のユーザーまたは連絡先の空き時間情報が含まれています。
ms.openlocfilehash: 55210230259b78e5ed9c4f0744aae003cf2e7ae5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459315"
---
# <a name="individualattendeeconflictdata"></a><span data-ttu-id="b0dc1-103">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="b0dc1-103">IndividualAttendeeConflictData</span></span>

<span data-ttu-id="b0dc1-104">**IndividualAttendeeConflictData**要素には、[提案](suggestion.md)要素で特定された会議の時間と同時に発生する時間枠のユーザーまたは連絡先の空き時間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0dc1-104">The **IndividualAttendeeConflictData** element contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span> 
  
[<span data-ttu-id="b0dc1-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b0dc1-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="b0dc1-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="b0dc1-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="b0dc1-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="b0dc1-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="b0dc1-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="b0dc1-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="b0dc1-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="b0dc1-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="b0dc1-110">提案</span><span class="sxs-lookup"><span data-stu-id="b0dc1-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="b0dc1-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="b0dc1-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="b0dc1-112">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="b0dc1-112">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md)
  
```xml
<IndividualAttendeeConflictData>
   <BusyType>...</BusyType>
</IndividualAttendeeConflictData>
```

 <span data-ttu-id="b0dc1-113">**IndividualAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="b0dc1-113">**IndividualAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0dc1-114">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b0dc1-114">Attributes and elements</span></span>

<span data-ttu-id="b0dc1-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b0dc1-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0dc1-116">属性</span><span class="sxs-lookup"><span data-stu-id="b0dc1-116">Attributes</span></span>

<span data-ttu-id="b0dc1-117">なし。</span><span class="sxs-lookup"><span data-stu-id="b0dc1-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0dc1-118">子要素</span><span class="sxs-lookup"><span data-stu-id="b0dc1-118">Child elements</span></span>

|<span data-ttu-id="b0dc1-119">**Element**</span><span class="sxs-lookup"><span data-stu-id="b0dc1-119">**Element**</span></span>|<span data-ttu-id="b0dc1-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0dc1-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0dc1-121">BusyType</span><span class="sxs-lookup"><span data-stu-id="b0dc1-121">BusyType</span></span>](busytype.md) <br/> |<span data-ttu-id="b0dc1-122">提案された会議の時間のユーザーの空き時間情報を表します。</span><span class="sxs-lookup"><span data-stu-id="b0dc1-122">Represents the free/busy status of a user for a suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0dc1-123">親要素</span><span class="sxs-lookup"><span data-stu-id="b0dc1-123">Parent elements</span></span>

|<span data-ttu-id="b0dc1-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="b0dc1-124">**Element**</span></span>|<span data-ttu-id="b0dc1-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0dc1-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0dc1-126">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="b0dc1-126">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="b0dc1-127">[GetUserAvailabilityRequest](getuseravailabilityrequest.md)で特定された参加者の競合データの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0dc1-127">Contains an array of conflict data for attendees identified in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span></span>  <br/> <span data-ttu-id="b0dc1-128">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b0dc1-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b0dc1-129">注釈</span><span class="sxs-lookup"><span data-stu-id="b0dc1-129">Remarks</span></span>

<span data-ttu-id="b0dc1-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b0dc1-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0dc1-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b0dc1-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0dc1-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="b0dc1-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b0dc1-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b0dc1-133">Schema Name</span></span>  <br/> |<span data-ttu-id="b0dc1-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b0dc1-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="b0dc1-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b0dc1-135">Validation File</span></span>  <br/> |<span data-ttu-id="b0dc1-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b0dc1-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b0dc1-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b0dc1-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0dc1-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="b0dc1-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0dc1-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="b0dc1-139">See also</span></span>



[<span data-ttu-id="b0dc1-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="b0dc1-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="b0dc1-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b0dc1-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="b0dc1-142">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="b0dc1-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


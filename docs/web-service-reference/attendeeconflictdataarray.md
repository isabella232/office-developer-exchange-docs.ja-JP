---
title: AttendeeConflictDataArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttendeeConflictDataArray
api_type:
- schema
ms.assetid: 1d758547-28c5-4649-8334-427480c282d6
description: AttendeeConflictDataArray 要素には、GetUserAvailability 操作で指定されたクエリを実行した出席者のための競合データの配列が含まれています。
ms.openlocfilehash: 169312b8a3d37c014ba58fbfe094d786b134fc90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759459"
---
# <a name="attendeeconflictdataarray"></a><span data-ttu-id="fd3cd-103">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="fd3cd-103">AttendeeConflictDataArray</span></span>

<span data-ttu-id="fd3cd-104">**AttendeeConflictDataArray**要素には、 [GetUserAvailability の操作](getuseravailability-operation.md)で指定されたクエリを実行した出席者のための競合データの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fd3cd-104">The **AttendeeConflictDataArray** element contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>
  
- [<span data-ttu-id="fd3cd-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="fd3cd-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
- [<span data-ttu-id="fd3cd-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="fd3cd-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
- [<span data-ttu-id="fd3cd-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="fd3cd-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
- [<span data-ttu-id="fd3cd-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="fd3cd-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
- [<span data-ttu-id="fd3cd-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="fd3cd-109">SuggestionArray</span></span>](suggestionarray.md)
  
- [<span data-ttu-id="fd3cd-110">提案</span><span class="sxs-lookup"><span data-stu-id="fd3cd-110">Suggestion</span></span>](suggestion.md)
  
- [<span data-ttu-id="fd3cd-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="fd3cd-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
```xml
<ArrayOfAttendeeConflictData>
   <UnknownAttendeeConflictData>...</UnknownAttendeeConflictData>
   <IndividualAttendeeConflictData>...</IndividualAttendeeConflictData>
   <TooBigGroupAttendeeConflictData>...</TooBigGroupAttendeeConflictData>
   <GroupAttendeeConflictData>...</GroupAttendeeConflictData>
</ArrayOfAttendeeConflictData>
```

 <span data-ttu-id="fd3cd-112">**ArrayOfAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="fd3cd-112">**ArrayOfAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd3cd-113">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fd3cd-113">Attributes and elements</span></span>

<span data-ttu-id="fd3cd-114">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fd3cd-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd3cd-115">属性</span><span class="sxs-lookup"><span data-stu-id="fd3cd-115">Attributes</span></span>

<span data-ttu-id="fd3cd-116">なし。</span><span class="sxs-lookup"><span data-stu-id="fd3cd-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd3cd-117">子要素</span><span class="sxs-lookup"><span data-stu-id="fd3cd-117">Child elements</span></span>

|<span data-ttu-id="fd3cd-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="fd3cd-118">**Element**</span></span>|<span data-ttu-id="fd3cd-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="fd3cd-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd3cd-120">UnknownAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="fd3cd-120">UnknownAttendeeConflictData</span></span>](unknownattendeeconflictdata.md) <br/> |<span data-ttu-id="fd3cd-121">解決できない出席者やユーザー、配布リスト、または取引先担当者ではない出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="fd3cd-121">Represents an unresolvable attendee or an attendee that is not a user, distribution list, or contact.</span></span>  <br/> |
|[<span data-ttu-id="fd3cd-122">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="fd3cd-122">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md) <br/> |<span data-ttu-id="fd3cd-123">示したと同時に発生するタイム ・ ウィンドウのユーザーまたは連絡先の空き時間状況が含まれています会議[提案](suggestion.md)の要素で指定された時刻。</span><span class="sxs-lookup"><span data-stu-id="fd3cd-123">Contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span>  <br/> |
|[<span data-ttu-id="fd3cd-124">TooBigGroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="fd3cd-124">TooBigGroupAttendeeConflictData</span></span>](toobiggroupattendeeconflictdata.md) <br/> |<span data-ttu-id="fd3cd-125">配布リストを展開するのには大きすぎるとして解決する出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="fd3cd-125">Represents an attendee that resolved as a distribution list that was too large to expand.</span></span>  <br/> |
|[<span data-ttu-id="fd3cd-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="fd3cd-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="fd3cd-127">可能なユーザー数、競合を持っているユーザーの数および提案された会議の配布リストの利用可能時間情報を持っていないユーザーの数についての集計の競合に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fd3cd-127">Contains aggregate conflict information about the number of users available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fd3cd-128">親要素</span><span class="sxs-lookup"><span data-stu-id="fd3cd-128">Parent elements</span></span>

|<span data-ttu-id="fd3cd-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="fd3cd-129">**Element**</span></span>|<span data-ttu-id="fd3cd-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="fd3cd-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd3cd-131">提案</span><span class="sxs-lookup"><span data-stu-id="fd3cd-131">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="fd3cd-132">単一会議の時間を提案します。</span><span class="sxs-lookup"><span data-stu-id="fd3cd-132">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="fd3cd-133">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="fd3cd-133">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fd3cd-134">備考</span><span class="sxs-lookup"><span data-stu-id="fd3cd-134">Remarks</span></span>

<span data-ttu-id="fd3cd-135">**AttendeeConflictDataArray**内の各要素の位置は、 [MailboxDataArray](mailboxdataarray.md)要素でクエリを実行した出席者の位置に対応します。</span><span class="sxs-lookup"><span data-stu-id="fd3cd-135">The position of each element in the **AttendeeConflictDataArray** corresponds to the position of the queried attendees in the [MailboxDataArray](mailboxdataarray.md) element.</span></span> <span data-ttu-id="fd3cd-136">各クエリを実行した出席者は、 **AttendeeConflictDataArray**の子要素の 1 つに対応しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="fd3cd-136">Each queried attendee must correspond to one of the **AttendeeConflictDataArray** child elements.</span></span> <span data-ttu-id="fd3cd-137">これらの要素は、[提案](suggestion.md)の要素で識別される候補の会議の時刻に 1 つの競合を表します。</span><span class="sxs-lookup"><span data-stu-id="fd3cd-137">These elements represent a single conflict with the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span> 
  
<span data-ttu-id="fd3cd-138">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="fd3cd-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd3cd-139">要素情報</span><span class="sxs-lookup"><span data-stu-id="fd3cd-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd3cd-140">名前空間</span><span class="sxs-lookup"><span data-stu-id="fd3cd-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fd3cd-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fd3cd-141">Schema Name</span></span>  <br/> |<span data-ttu-id="fd3cd-142">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="fd3cd-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="fd3cd-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fd3cd-143">Validation File</span></span>  <br/> |<span data-ttu-id="fd3cd-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fd3cd-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fd3cd-145">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fd3cd-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd3cd-146">False</span><span class="sxs-lookup"><span data-stu-id="fd3cd-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd3cd-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="fd3cd-147">See also</span></span>

- [<span data-ttu-id="fd3cd-148">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="fd3cd-148">GetUserAvailability operation</span></span>](getuseravailability-operation.md) 
- [<span data-ttu-id="fd3cd-149">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="fd3cd-149">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="fd3cd-150">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="fd3cd-150">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


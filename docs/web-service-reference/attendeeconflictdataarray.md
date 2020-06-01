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
description: AttendeeConflictDataArray 要素には、GetUserAvailability 操作で識別された、クエリを実行した出席者の競合データの配列が含まれています。
ms.openlocfilehash: 770e8c00ca248ec3562180dc9d3626fd5b58f4d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455801"
---
# <a name="attendeeconflictdataarray"></a><span data-ttu-id="51a5c-103">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="51a5c-103">AttendeeConflictDataArray</span></span>

<span data-ttu-id="51a5c-104">**AttendeeConflictDataArray**要素には、 [getuseravailability 操作](getuseravailability-operation.md)で識別された、クエリを実行した出席者の競合データの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="51a5c-104">The **AttendeeConflictDataArray** element contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>
  
- [<span data-ttu-id="51a5c-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="51a5c-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
- [<span data-ttu-id="51a5c-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="51a5c-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
- [<span data-ttu-id="51a5c-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="51a5c-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
- [<span data-ttu-id="51a5c-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="51a5c-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
- [<span data-ttu-id="51a5c-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="51a5c-109">SuggestionArray</span></span>](suggestionarray.md)
  
- [<span data-ttu-id="51a5c-110">提案</span><span class="sxs-lookup"><span data-stu-id="51a5c-110">Suggestion</span></span>](suggestion.md)
  
- [<span data-ttu-id="51a5c-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="51a5c-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
```xml
<ArrayOfAttendeeConflictData>
   <UnknownAttendeeConflictData>...</UnknownAttendeeConflictData>
   <IndividualAttendeeConflictData>...</IndividualAttendeeConflictData>
   <TooBigGroupAttendeeConflictData>...</TooBigGroupAttendeeConflictData>
   <GroupAttendeeConflictData>...</GroupAttendeeConflictData>
</ArrayOfAttendeeConflictData>
```

 <span data-ttu-id="51a5c-112">**ArrayOfAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="51a5c-112">**ArrayOfAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="51a5c-113">属性と要素</span><span class="sxs-lookup"><span data-stu-id="51a5c-113">Attributes and elements</span></span>

<span data-ttu-id="51a5c-114">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="51a5c-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="51a5c-115">属性</span><span class="sxs-lookup"><span data-stu-id="51a5c-115">Attributes</span></span>

<span data-ttu-id="51a5c-116">なし。</span><span class="sxs-lookup"><span data-stu-id="51a5c-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="51a5c-117">子要素</span><span class="sxs-lookup"><span data-stu-id="51a5c-117">Child elements</span></span>

|<span data-ttu-id="51a5c-118">**Element**</span><span class="sxs-lookup"><span data-stu-id="51a5c-118">**Element**</span></span>|<span data-ttu-id="51a5c-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="51a5c-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51a5c-120">UnknownAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="51a5c-120">UnknownAttendeeConflictData</span></span>](unknownattendeeconflictdata.md) <br/> |<span data-ttu-id="51a5c-121">非解決の出席者またはユーザー、配布リスト、または連絡先ではない出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="51a5c-121">Represents an unresolvable attendee or an attendee that is not a user, distribution list, or contact.</span></span>  <br/> |
|[<span data-ttu-id="51a5c-122">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="51a5c-122">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md) <br/> |<span data-ttu-id="51a5c-123">[提案](suggestion.md)要素で特定された会議の時間と同時に発生する時間枠のユーザーまたは連絡先の空き時間状態を格納します。</span><span class="sxs-lookup"><span data-stu-id="51a5c-123">Contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span>  <br/> |
|[<span data-ttu-id="51a5c-124">TooBigGroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="51a5c-124">TooBigGroupAttendeeConflictData</span></span>](toobiggroupattendeeconflictdata.md) <br/> |<span data-ttu-id="51a5c-125">展開するには大きすぎる配布リストとして解決された出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="51a5c-125">Represents an attendee that resolved as a distribution list that was too large to expand.</span></span>  <br/> |
|[<span data-ttu-id="51a5c-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="51a5c-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="51a5c-127">利用可能なユーザー数、競合しているユーザーの数、および推奨される会議時間の配布リストに空き時間情報を持たないユーザーの数についての集約競合情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="51a5c-127">Contains aggregate conflict information about the number of users available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="51a5c-128">親要素</span><span class="sxs-lookup"><span data-stu-id="51a5c-128">Parent elements</span></span>

|<span data-ttu-id="51a5c-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="51a5c-129">**Element**</span></span>|<span data-ttu-id="51a5c-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="51a5c-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51a5c-131">提案</span><span class="sxs-lookup"><span data-stu-id="51a5c-131">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="51a5c-132">1つの会議時間の提案を表します。</span><span class="sxs-lookup"><span data-stu-id="51a5c-132">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="51a5c-133">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="51a5c-133">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="51a5c-134">注釈</span><span class="sxs-lookup"><span data-stu-id="51a5c-134">Remarks</span></span>

<span data-ttu-id="51a5c-135">**AttendeeConflictDataArray**の各要素の位置は、 [MailboxDataArray](mailboxdataarray.md)要素の中でクエリを行った出席者の位置に対応します。</span><span class="sxs-lookup"><span data-stu-id="51a5c-135">The position of each element in the **AttendeeConflictDataArray** corresponds to the position of the queried attendees in the [MailboxDataArray](mailboxdataarray.md) element.</span></span> <span data-ttu-id="51a5c-136">クエリを行った各出席者は、 **AttendeeConflictDataArray**子要素のいずれかに対応している必要があります。</span><span class="sxs-lookup"><span data-stu-id="51a5c-136">Each queried attendee must correspond to one of the **AttendeeConflictDataArray** child elements.</span></span> <span data-ttu-id="51a5c-137">これらの要素は、[提案](suggestion.md)要素で特定された会議の推奨時間との単一の競合を表します。</span><span class="sxs-lookup"><span data-stu-id="51a5c-137">These elements represent a single conflict with the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span> 
  
<span data-ttu-id="51a5c-138">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="51a5c-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="51a5c-139">要素の情報</span><span class="sxs-lookup"><span data-stu-id="51a5c-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="51a5c-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="51a5c-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="51a5c-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="51a5c-141">Schema Name</span></span>  <br/> |<span data-ttu-id="51a5c-142">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="51a5c-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="51a5c-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="51a5c-143">Validation File</span></span>  <br/> |<span data-ttu-id="51a5c-144">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="51a5c-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="51a5c-145">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="51a5c-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="51a5c-146">正しくない</span><span class="sxs-lookup"><span data-stu-id="51a5c-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="51a5c-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="51a5c-147">See also</span></span>

- [<span data-ttu-id="51a5c-148">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="51a5c-148">GetUserAvailability operation</span></span>](getuseravailability-operation.md) 
- [<span data-ttu-id="51a5c-149">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="51a5c-149">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="51a5c-150">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="51a5c-150">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


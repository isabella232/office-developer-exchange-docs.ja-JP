---
title: GroupAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupAttendeeConflictData
api_type:
- schema
ms.assetid: fd8bf19a-298b-4135-93e8-ead3db7e1142
description: GroupAttendeeConflictData 要素には、使用可能なユーザー数、競合しているユーザーの数、および推奨される会議時間の配布リストの空き時間情報を持っていないユーザーの数についての集約競合情報が含まれています。
ms.openlocfilehash: c75a4e6f8fdff7fb2514f448350fee9f1acb9775
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462930"
---
# <a name="groupattendeeconflictdata"></a><span data-ttu-id="69002-103">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="69002-103">GroupAttendeeConflictData</span></span>

<span data-ttu-id="69002-104">**GroupAttendeeConflictData**要素には、使用可能なユーザー数、競合しているユーザーの数、および推奨される会議時間の配布リストの空き時間情報を持っていないユーザーの数についての集約競合情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="69002-104">The **GroupAttendeeConflictData** element contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span> 
  
- [<span data-ttu-id="69002-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="69002-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="69002-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="69002-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
- [<span data-ttu-id="69002-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="69002-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
- [<span data-ttu-id="69002-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="69002-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
- [<span data-ttu-id="69002-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="69002-109">SuggestionArray</span></span>](suggestionarray.md)
- [<span data-ttu-id="69002-110">提案</span><span class="sxs-lookup"><span data-stu-id="69002-110">Suggestion</span></span>](suggestion.md)
- [<span data-ttu-id="69002-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="69002-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
- [<span data-ttu-id="69002-112">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="69002-112">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
```xml
<GroupAttendeeConflictData>
   <NumberOfMembers>...</NumberOfMembers>
   <NumberOfMembersAvailable>...</NumberOfMembersAvailable>
   <NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
   <NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
</GroupAttendeeConflictData>
```

<span data-ttu-id="69002-113">**GroupAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="69002-113">**GroupAttendeeConflictData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="69002-114">属性と要素</span><span class="sxs-lookup"><span data-stu-id="69002-114">Attributes and elements</span></span>

<span data-ttu-id="69002-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="69002-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69002-116">属性</span><span class="sxs-lookup"><span data-stu-id="69002-116">Attributes</span></span>

<span data-ttu-id="69002-117">なし。</span><span class="sxs-lookup"><span data-stu-id="69002-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="69002-118">子要素</span><span class="sxs-lookup"><span data-stu-id="69002-118">Child elements</span></span>

|<span data-ttu-id="69002-119">**Element**</span><span class="sxs-lookup"><span data-stu-id="69002-119">**Element**</span></span>|<span data-ttu-id="69002-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="69002-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69002-121">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="69002-121">NumberOfMembers</span></span>](numberofmembers.md) <br/> |<span data-ttu-id="69002-122">配布リスト内のユーザー、リソース、ルームの数を表します。</span><span class="sxs-lookup"><span data-stu-id="69002-122">Represents the number of users, resources, and rooms in a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="69002-123">NumberOfMembersAvailable</span><span class="sxs-lookup"><span data-stu-id="69002-123">NumberOfMembersAvailable</span></span>](numberofmembersavailable.md) <br/> |<span data-ttu-id="69002-124">提案された会議の時間に使用できる配布リストのメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="69002-124">Represents the number of distribution list members who are available for a suggested meeting time.</span></span> <span data-ttu-id="69002-125">この要素は、状態が "**フリー**" であるメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="69002-125">This element represents members for whom the status is **Free**.</span></span>  <br/> |
|[<span data-ttu-id="69002-126">NumberOfMembersWithConflict</span><span class="sxs-lookup"><span data-stu-id="69002-126">NumberOfMembersWithConflict</span></span>](numberofmemberswithconflict.md) <br/> |<span data-ttu-id="69002-127">提案された会議時間と競合している配布リストメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="69002-127">Represents the number of distribution list members who have a conflict with a suggested meeting time.</span></span> <span data-ttu-id="69002-128">この要素は、**取り込み中**、 **OOF**、または**仮承諾**状態のメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="69002-128">This element represents members who have a **Busy**, **OOF**, or **Tentative** status.</span></span>  <br/> |
|[<span data-ttu-id="69002-129">NumberOfMembersWithNoData</span><span class="sxs-lookup"><span data-stu-id="69002-129">NumberOfMembersWithNoData</span></span>](numberofmemberswithnodata.md) <br/> |<span data-ttu-id="69002-130">公開されている空き時間情報データを持たないグループメンバーのうち、提案された会議の時刻と比較するものの数を表します。</span><span class="sxs-lookup"><span data-stu-id="69002-130">Represents the number of group members who do not have published free/busy data to compare to a suggested meeting time.</span></span> <span data-ttu-id="69002-131">この要素は、大きすぎる、またはデータの状態を持た**ない**メンバーを表す配布リストのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="69002-131">This element represents members of a distribution list that is too large or members who have **No Data** status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="69002-132">親要素</span><span class="sxs-lookup"><span data-stu-id="69002-132">Parent elements</span></span>

|<span data-ttu-id="69002-133">**要素**</span><span class="sxs-lookup"><span data-stu-id="69002-133">**Element**</span></span>|<span data-ttu-id="69002-134">**説明**</span><span class="sxs-lookup"><span data-stu-id="69002-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69002-135">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="69002-135">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="69002-136">[Getuseravailability 操作](getuseravailability-operation.md)で識別された、クエリを実行した出席者の競合データの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="69002-136">Contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/> <span data-ttu-id="69002-137">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="69002-137">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="69002-138">注釈</span><span class="sxs-lookup"><span data-stu-id="69002-138">Remarks</span></span>

<span data-ttu-id="69002-139">[GetUserAvailabilityRequest](getuseravailabilityrequest.md)内の出席者が配布リストに解決された場合、 **GroupAttendeeConflictData**要素は応答内に存在します。</span><span class="sxs-lookup"><span data-stu-id="69002-139">The **GroupAttendeeConflictData** element is present in the response when an attendee in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md) is resolved to a distribution list.</span></span> <span data-ttu-id="69002-140">**GroupAttendeeConflictData**要素は、配布リストのメンバーの3つの状態を示します。使用可能、競合している、またはデータがありません。</span><span class="sxs-lookup"><span data-stu-id="69002-140">The **GroupAttendeeConflictData** element identifies three states for members of a distribution list: available, conflicted, or no data.</span></span> <span data-ttu-id="69002-141">配布リストの展開は最大100のメンバーをサポートします。</span><span class="sxs-lookup"><span data-stu-id="69002-141">Distribution list expansion will support up to 100 members.</span></span> <span data-ttu-id="69002-142">そのため、 [numberofmembers](numberofmembers.md)要素には最大で100のメンバーを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="69002-142">Therefore, the [NumberOfMembers](numberofmembers.md) element can contain a maximum of 100 members.</span></span> <span data-ttu-id="69002-143">配布リストの展開は再帰的です。</span><span class="sxs-lookup"><span data-stu-id="69002-143">Distribution list expansion is recursive.</span></span> <span data-ttu-id="69002-144">配布リストに親メンバーシップの合計を100のメンバーまで展開する子配布リストが含まれている場合、子配布リストは展開されず、 [Numberofmemberswithnodata](numberofmemberswithnodata.md)要素数の1つのエントリとしてカウントされます。</span><span class="sxs-lookup"><span data-stu-id="69002-144">If a distribution list contains a child distribution list that expands the total parent membership to over 100 members, the child distribution list will not be expanded and will count as a single entry of the [NumberOfMembersWithNoData](numberofmemberswithnodata.md) element count.</span></span> <span data-ttu-id="69002-145">子配布リストを展開でき、親メンバーシップの合計が100を超えるメンバーに展開されていない場合は、そのメンバーシップが展開され、メンバー数が**GroupAttendeeConflictData**要素の子要素に追加されます。</span><span class="sxs-lookup"><span data-stu-id="69002-145">If a child distribution list can be expanded and the total parent membership does not expand to over 100 members, its membership is expanded and the member counts are added to the child elements of the **GroupAttendeeConflictData** element.</span></span> 
  
<span data-ttu-id="69002-146">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="69002-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69002-147">要素の情報</span><span class="sxs-lookup"><span data-stu-id="69002-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69002-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="69002-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="69002-149">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="69002-149">Schema Name</span></span>  <br/> |<span data-ttu-id="69002-150">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="69002-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="69002-151">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="69002-151">Validation File</span></span>  <br/> |<span data-ttu-id="69002-152">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="69002-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="69002-153">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="69002-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="69002-154">正しくない</span><span class="sxs-lookup"><span data-stu-id="69002-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69002-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="69002-155">See also</span></span>

- [<span data-ttu-id="69002-156">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="69002-156">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="69002-157">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="69002-157">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="69002-158">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="69002-158">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


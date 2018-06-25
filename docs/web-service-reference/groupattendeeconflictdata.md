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
description: GroupAttendeeConflictData 要素にはでの利用の競合を持っているユーザーの数と、配布に利用可能時間情報を持たないユーザーの数を一覧表示するユーザーの数についての集計の競合に関する情報が含まれます、ミーティング時間を提示します。
ms.openlocfilehash: 382b4d866c95de98bd444cd6226d71813889d4f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831757"
---
# <a name="groupattendeeconflictdata"></a><span data-ttu-id="d2e09-103">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="d2e09-103">GroupAttendeeConflictData</span></span>

<span data-ttu-id="d2e09-104">**GroupAttendeeConflictData**要素には、使用可能であるユーザーの数、競合を持っているユーザーの数および配布リストの利用可能時間情報を持っていないユーザーの数についての集計の競合に関する情報が含まれています。提案された会議の時間です。</span><span class="sxs-lookup"><span data-stu-id="d2e09-104">The **GroupAttendeeConflictData** element contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span> 
  
- [<span data-ttu-id="d2e09-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d2e09-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="d2e09-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="d2e09-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
- [<span data-ttu-id="d2e09-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="d2e09-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
- [<span data-ttu-id="d2e09-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="d2e09-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
- [<span data-ttu-id="d2e09-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="d2e09-109">SuggestionArray</span></span>](suggestionarray.md)
- [<span data-ttu-id="d2e09-110">提案</span><span class="sxs-lookup"><span data-stu-id="d2e09-110">Suggestion</span></span>](suggestion.md)
- [<span data-ttu-id="d2e09-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="d2e09-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
- [<span data-ttu-id="d2e09-112">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="d2e09-112">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
```xml
<GroupAttendeeConflictData>
   <NumberOfMembers>...</NumberOfMembers>
   <NumberOfMembersAvailable>...</NumberOfMembersAvailable>
   <NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
   <NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
</GroupAttendeeConflictData>
```

<span data-ttu-id="d2e09-113">**GroupAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="d2e09-113">**GroupAttendeeConflictData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d2e09-114">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d2e09-114">Attributes and elements</span></span>

<span data-ttu-id="d2e09-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d2e09-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2e09-116">属性</span><span class="sxs-lookup"><span data-stu-id="d2e09-116">Attributes</span></span>

<span data-ttu-id="d2e09-117">なし。</span><span class="sxs-lookup"><span data-stu-id="d2e09-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2e09-118">子要素</span><span class="sxs-lookup"><span data-stu-id="d2e09-118">Child elements</span></span>

|<span data-ttu-id="d2e09-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="d2e09-119">**Element**</span></span>|<span data-ttu-id="d2e09-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2e09-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2e09-121">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="d2e09-121">NumberOfMembers</span></span>](numberofmembers.md) <br/> |<span data-ttu-id="d2e09-122">ユーザー、リソース、およびパブリック フォルダーの配布リストの数を表します。</span><span class="sxs-lookup"><span data-stu-id="d2e09-122">Represents the number of users, resources, and rooms in a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="d2e09-123">NumberOfMembersAvailable</span><span class="sxs-lookup"><span data-stu-id="d2e09-123">NumberOfMembersAvailable</span></span>](numberofmembersavailable.md) <br/> |<span data-ttu-id="d2e09-124">提案された会議の時間を利用した配布リストのメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="d2e09-124">Represents the number of distribution list members who are available for a suggested meeting time.</span></span> <span data-ttu-id="d2e09-125">この要素は、対象となる状態は、**無料**のメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="d2e09-125">This element represents members for whom the status is **Free**.</span></span>  <br/> |
|[<span data-ttu-id="d2e09-126">NumberOfMembersWithConflict</span><span class="sxs-lookup"><span data-stu-id="d2e09-126">NumberOfMembersWithConflict</span></span>](numberofmemberswithconflict.md) <br/> |<span data-ttu-id="d2e09-127">提案された会議の時間との競合を持つ配布リストのメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="d2e09-127">Represents the number of distribution list members who have a conflict with a suggested meeting time.</span></span> <span data-ttu-id="d2e09-128">この要素では、**ビジー**、**不在時**、または**仮承諾**のステータスを持っているメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="d2e09-128">This element represents members who have a **Busy**, **OOF**, or **Tentative** status.</span></span>  <br/> |
|[<span data-ttu-id="d2e09-129">NumberOfMembersWithNoData</span><span class="sxs-lookup"><span data-stu-id="d2e09-129">NumberOfMembersWithNoData</span></span>](numberofmemberswithnodata.md) <br/> |<span data-ttu-id="d2e09-130">提案された会議の時間と比較するための空き/予約済みパブリッシュされたデータを持っていないグループ メンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="d2e09-130">Represents the number of group members who do not have published free/busy data to compare to a suggested meeting time.</span></span> <span data-ttu-id="d2e09-131">この要素は、メンバー配布リストが大きすぎるのか、**なしのデータ**のステータスを持っているメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="d2e09-131">This element represents members of a distribution list that is too large or members who have **No Data** status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d2e09-132">親要素</span><span class="sxs-lookup"><span data-stu-id="d2e09-132">Parent elements</span></span>

|<span data-ttu-id="d2e09-133">**要素**</span><span class="sxs-lookup"><span data-stu-id="d2e09-133">**Element**</span></span>|<span data-ttu-id="d2e09-134">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2e09-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2e09-135">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="d2e09-135">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="d2e09-136">[GetUserAvailability 操作](getuseravailability-operation.md)で指定されたクエリを実行した出席者のために競合データの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d2e09-136">Contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/> <span data-ttu-id="d2e09-137">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="d2e09-137">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d2e09-138">備考</span><span class="sxs-lookup"><span data-stu-id="d2e09-138">Remarks</span></span>

<span data-ttu-id="d2e09-139">**GroupAttendeeConflictData**要素は、 [GetUserAvailabilityRequest](getuseravailabilityrequest.md)の出席者が配布リストを解決するときの応答であります。</span><span class="sxs-lookup"><span data-stu-id="d2e09-139">The **GroupAttendeeConflictData** element is present in the response when an attendee in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md) is resolved to a distribution list.</span></span> <span data-ttu-id="d2e09-140">**GroupAttendeeConflictData**要素は、配布リストのメンバーの 3 つの状態を識別: 利用可能な競合した場合、またはデータがありません。</span><span class="sxs-lookup"><span data-stu-id="d2e09-140">The **GroupAttendeeConflictData** element identifies three states for members of a distribution list: available, conflicted, or no data.</span></span> <span data-ttu-id="d2e09-141">配布リストの展開では、最大 100 個のメンバーをサポートします。</span><span class="sxs-lookup"><span data-stu-id="d2e09-141">Distribution list expansion will support up to 100 members.</span></span> <span data-ttu-id="d2e09-142">したがって、 [NumberOfMembers](numberofmembers.md)要素は、最大 100 のメンバーを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="d2e09-142">Therefore, the [NumberOfMembers](numberofmembers.md) element can contain a maximum of 100 members.</span></span> <span data-ttu-id="d2e09-143">配布リストの展開は、再帰的です。</span><span class="sxs-lookup"><span data-stu-id="d2e09-143">Distribution list expansion is recursive.</span></span> <span data-ttu-id="d2e09-144">配布リストには、100 を超えるメンバーを親の合計のメンバーシップを展開する子の配布リストが含まれている、子の配布リストは展開されていないと、 [NumberOfMembersWithNoData](numberofmemberswithnodata.md)の要素数の 1 つのエントリとしてカウントされます。</span><span class="sxs-lookup"><span data-stu-id="d2e09-144">If a distribution list contains a child distribution list that expands the total parent membership to over 100 members, the child distribution list will not be expanded and will count as a single entry of the [NumberOfMembersWithNoData](numberofmemberswithnodata.md) element count.</span></span> <span data-ttu-id="d2e09-145">子の配布リストを展開することができます、100 を超えるメンバーを親の合計のメンバーシップを展開しない場合は、そのメンバーシップは展開し、メンバー数は、 **GroupAttendeeConflictData**要素の子要素に追加されます。</span><span class="sxs-lookup"><span data-stu-id="d2e09-145">If a child distribution list can be expanded and the total parent membership does not expand to over 100 members, its membership is expanded and the member counts are added to the child elements of the **GroupAttendeeConflictData** element.</span></span> 
  
<span data-ttu-id="d2e09-146">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="d2e09-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2e09-147">要素情報</span><span class="sxs-lookup"><span data-stu-id="d2e09-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2e09-148">名前空間</span><span class="sxs-lookup"><span data-stu-id="d2e09-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d2e09-149">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d2e09-149">Schema Name</span></span>  <br/> |<span data-ttu-id="d2e09-150">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d2e09-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="d2e09-151">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d2e09-151">Validation File</span></span>  <br/> |<span data-ttu-id="d2e09-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d2e09-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d2e09-153">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d2e09-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="d2e09-154">False</span><span class="sxs-lookup"><span data-stu-id="d2e09-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2e09-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="d2e09-155">See also</span></span>

- [<span data-ttu-id="d2e09-156">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="d2e09-156">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="d2e09-157">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d2e09-157">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="d2e09-158">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="d2e09-158">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


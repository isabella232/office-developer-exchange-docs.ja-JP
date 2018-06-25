---
title: NumberOfMembersWithNoData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfMembersWithNoData
api_type:
- schema
ms.assetid: 7ca9c57c-9519-442c-a9f4-dca2b0309716
description: NumberOfMembersWithNoData 要素は、提案された会議の時間と比較するための空き/予約済みパブリッシュされたデータを取得して、配布リストのメンバーの数を表します。 この要素は、メンバー配布リストが大きすぎるのか、なしのデータのステータスを持っているメンバーを表します。
ms.openlocfilehash: f73978df47bd8240dd5dabfbbf74523525e3270f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832637"
---
# <a name="numberofmemberswithnodata"></a><span data-ttu-id="bcbf9-104">NumberOfMembersWithNoData</span><span class="sxs-lookup"><span data-stu-id="bcbf9-104">NumberOfMembersWithNoData</span></span>

<span data-ttu-id="bcbf9-105">**NumberOfMembersWithNoData**要素は、提案された会議の時間と比較するための空き/予約済みパブリッシュされたデータを取得して、配布リストのメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="bcbf9-105">The **NumberOfMembersWithNoData** element represents the number of distribution list members who do not have published free/busy data to compare to a suggested meeting time.</span></span> <span data-ttu-id="bcbf9-106">この要素は、メンバー配布リストが大きすぎるのか、**なしのデータ**のステータスを持っているメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="bcbf9-106">This element represents members of a distribution list that is too large or members who have **No Data** status.</span></span> 
  
[<span data-ttu-id="bcbf9-107">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="bcbf9-107">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="bcbf9-108">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="bcbf9-108">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="bcbf9-109">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="bcbf9-109">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="bcbf9-110">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="bcbf9-110">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="bcbf9-111">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="bcbf9-111">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="bcbf9-112">提案</span><span class="sxs-lookup"><span data-stu-id="bcbf9-112">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="bcbf9-113">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="bcbf9-113">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="bcbf9-114">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="bcbf9-114">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="bcbf9-115">NumberOfMembersWithNoData</span><span class="sxs-lookup"><span data-stu-id="bcbf9-115">NumberOfMembersWithNoData</span></span>](numberofmemberswithnodata.md)
  
```xml
<NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
```

 <span data-ttu-id="bcbf9-116">**int**</span><span class="sxs-lookup"><span data-stu-id="bcbf9-116">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bcbf9-117">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bcbf9-117">Attributes and elements</span></span>

<span data-ttu-id="bcbf9-118">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bcbf9-118">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bcbf9-119">属性</span><span class="sxs-lookup"><span data-stu-id="bcbf9-119">Attributes</span></span>

<span data-ttu-id="bcbf9-120">なし。</span><span class="sxs-lookup"><span data-stu-id="bcbf9-120">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bcbf9-121">子要素</span><span class="sxs-lookup"><span data-stu-id="bcbf9-121">Child elements</span></span>

<span data-ttu-id="bcbf9-122">なし。</span><span class="sxs-lookup"><span data-stu-id="bcbf9-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bcbf9-123">親要素</span><span class="sxs-lookup"><span data-stu-id="bcbf9-123">Parent elements</span></span>

|<span data-ttu-id="bcbf9-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="bcbf9-124">**Element**</span></span>|<span data-ttu-id="bcbf9-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="bcbf9-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bcbf9-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="bcbf9-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="bcbf9-127">利用するユーザーの数、競合を持っているユーザーの数および提案された会議の配布リストの利用可能時間情報を持っていないユーザーの数についての集計の競合に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bcbf9-127">Contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="bcbf9-128">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="bcbf9-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bcbf9-129">備考</span><span class="sxs-lookup"><span data-stu-id="bcbf9-129">Remarks</span></span>

<span data-ttu-id="bcbf9-130">メールボックスを持っていないユーザー グループのメンバーは、配布リストのメンバーの予定表のデータを持っていないユーザーの例です。</span><span class="sxs-lookup"><span data-stu-id="bcbf9-130">A contact in a group who does not have a mailbox is an example of a distribution list member who does not have calendar data.</span></span> <span data-ttu-id="bcbf9-131">連絡先には、次の理由により**なしのデータ**の状態があります。</span><span class="sxs-lookup"><span data-stu-id="bcbf9-131">A contact may also have **No Data** status for the following reasons:</span></span> 
  
- <span data-ttu-id="bcbf9-132">アクセス許可が十分ではありません。</span><span class="sxs-lookup"><span data-stu-id="bcbf9-132">Permissions are insufficient.</span></span>
    
- <span data-ttu-id="bcbf9-133">展開するには、配布リストが大きすぎます。</span><span class="sxs-lookup"><span data-stu-id="bcbf9-133">The distribution list is too large to expand.</span></span>
    
- <span data-ttu-id="bcbf9-134">Active Directory ディレクトリ サービスでは使用できません。</span><span class="sxs-lookup"><span data-stu-id="bcbf9-134">The Active Directory directory service is unavailable.</span></span>
    
<span data-ttu-id="bcbf9-135">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="bcbf9-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bcbf9-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="bcbf9-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bcbf9-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="bcbf9-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bcbf9-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bcbf9-138">Schema Name</span></span>  <br/> |<span data-ttu-id="bcbf9-139">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="bcbf9-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="bcbf9-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bcbf9-140">Validation File</span></span>  <br/> |<span data-ttu-id="bcbf9-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bcbf9-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bcbf9-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bcbf9-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="bcbf9-143">False</span><span class="sxs-lookup"><span data-stu-id="bcbf9-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bcbf9-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="bcbf9-144">See also</span></span>



[<span data-ttu-id="bcbf9-145">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="bcbf9-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="bcbf9-146">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="bcbf9-146">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="bcbf9-147">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="bcbf9-147">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


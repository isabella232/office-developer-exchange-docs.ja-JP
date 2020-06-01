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
description: NumberOfMembersWithNoData 要素は、提案された会議時間と比較するために、公開された空き時間情報データを持たない配布リストメンバーの数を表します。 この要素は、大きすぎる、またはデータの状態を持たないメンバーを表す配布リストのメンバーを表します。
ms.openlocfilehash: df41adc14f4c35c0e24d0f3c54f74a63527859d6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462550"
---
# <a name="numberofmemberswithnodata"></a><span data-ttu-id="7c19f-104">NumberOfMembersWithNoData</span><span class="sxs-lookup"><span data-stu-id="7c19f-104">NumberOfMembersWithNoData</span></span>

<span data-ttu-id="7c19f-105">**Numberofmemberswithnodata**要素は、提案された会議時間と比較するために、公開された空き時間情報データを持たない配布リストメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="7c19f-105">The **NumberOfMembersWithNoData** element represents the number of distribution list members who do not have published free/busy data to compare to a suggested meeting time.</span></span> <span data-ttu-id="7c19f-106">この要素は、大きすぎる、またはデータの状態を持た**ない**メンバーを表す配布リストのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="7c19f-106">This element represents members of a distribution list that is too large or members who have **No Data** status.</span></span> 
  
[<span data-ttu-id="7c19f-107">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7c19f-107">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="7c19f-108">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="7c19f-108">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="7c19f-109">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="7c19f-109">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="7c19f-110">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="7c19f-110">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="7c19f-111">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="7c19f-111">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="7c19f-112">提案</span><span class="sxs-lookup"><span data-stu-id="7c19f-112">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="7c19f-113">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="7c19f-113">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="7c19f-114">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="7c19f-114">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="7c19f-115">NumberOfMembersWithNoData</span><span class="sxs-lookup"><span data-stu-id="7c19f-115">NumberOfMembersWithNoData</span></span>](numberofmemberswithnodata.md)
  
```xml
<NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
```

 <span data-ttu-id="7c19f-116">**int**</span><span class="sxs-lookup"><span data-stu-id="7c19f-116">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c19f-117">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7c19f-117">Attributes and elements</span></span>

<span data-ttu-id="7c19f-118">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7c19f-118">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c19f-119">属性</span><span class="sxs-lookup"><span data-stu-id="7c19f-119">Attributes</span></span>

<span data-ttu-id="7c19f-120">なし。</span><span class="sxs-lookup"><span data-stu-id="7c19f-120">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c19f-121">子要素</span><span class="sxs-lookup"><span data-stu-id="7c19f-121">Child elements</span></span>

<span data-ttu-id="7c19f-122">なし。</span><span class="sxs-lookup"><span data-stu-id="7c19f-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7c19f-123">親要素</span><span class="sxs-lookup"><span data-stu-id="7c19f-123">Parent elements</span></span>

|<span data-ttu-id="7c19f-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="7c19f-124">**Element**</span></span>|<span data-ttu-id="7c19f-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="7c19f-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c19f-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="7c19f-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="7c19f-127">利用可能なユーザーの数、競合しているユーザーの数、および提案された会議の時間について配布リストの空き時間情報を持っていないユーザーの数についての集約された競合情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="7c19f-127">Contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="7c19f-128">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7c19f-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7c19f-129">注釈</span><span class="sxs-lookup"><span data-stu-id="7c19f-129">Remarks</span></span>

<span data-ttu-id="7c19f-130">メールボックスを持たないグループの連絡先は、予定表データを持たない配布リストのメンバーの例です。</span><span class="sxs-lookup"><span data-stu-id="7c19f-130">A contact in a group who does not have a mailbox is an example of a distribution list member who does not have calendar data.</span></span> <span data-ttu-id="7c19f-131">また、次の理由により、連絡先は**データ**の状態を持たない場合があります。</span><span class="sxs-lookup"><span data-stu-id="7c19f-131">A contact may also have **No Data** status for the following reasons:</span></span> 
  
- <span data-ttu-id="7c19f-132">アクセス許可が不十分です。</span><span class="sxs-lookup"><span data-stu-id="7c19f-132">Permissions are insufficient.</span></span>
    
- <span data-ttu-id="7c19f-133">配布リストが大きすぎて展開できません。</span><span class="sxs-lookup"><span data-stu-id="7c19f-133">The distribution list is too large to expand.</span></span>
    
- <span data-ttu-id="7c19f-134">Active Directory ディレクトリサービスを使用できません。</span><span class="sxs-lookup"><span data-stu-id="7c19f-134">The Active Directory directory service is unavailable.</span></span>
    
<span data-ttu-id="7c19f-135">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7c19f-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c19f-136">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7c19f-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c19f-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="7c19f-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c19f-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7c19f-138">Schema Name</span></span>  <br/> |<span data-ttu-id="7c19f-139">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7c19f-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c19f-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7c19f-140">Validation File</span></span>  <br/> |<span data-ttu-id="7c19f-141">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7c19f-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c19f-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7c19f-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c19f-143">正しくない</span><span class="sxs-lookup"><span data-stu-id="7c19f-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c19f-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="7c19f-144">See also</span></span>



[<span data-ttu-id="7c19f-145">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="7c19f-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="7c19f-146">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7c19f-146">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="7c19f-147">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="7c19f-147">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


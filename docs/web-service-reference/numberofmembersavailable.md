---
title: NumberOfMembersAvailable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfMembersAvailable
api_type:
- schema
ms.assetid: e367a278-1622-4b65-955f-2d4b2fc6e4d7
description: NumberOfMembersAvailable 要素は、提案された会議の時間に使用できる配布リストのメンバーの数を表します。 この要素は、状態が "フリー" であるメンバーを表します。
ms.openlocfilehash: 947e1c133cc49fb7e322962e95e184fe77e09353
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462592"
---
# <a name="numberofmembersavailable"></a><span data-ttu-id="a5613-104">NumberOfMembersAvailable</span><span class="sxs-lookup"><span data-stu-id="a5613-104">NumberOfMembersAvailable</span></span>

<span data-ttu-id="a5613-105">**Numberofmembersavailable**要素は、提案された会議の時間に使用できる配布リストのメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="a5613-105">The **NumberOfMembersAvailable** element represents the number of distribution list members who are available for a suggested meeting time.</span></span> <span data-ttu-id="a5613-106">この要素は、状態が "**フリー**" であるメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="a5613-106">This element represents members for whom the status is **Free**.</span></span>
  
[<span data-ttu-id="a5613-107">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a5613-107">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="a5613-108">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="a5613-108">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="a5613-109">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="a5613-109">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="a5613-110">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="a5613-110">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="a5613-111">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="a5613-111">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="a5613-112">提案</span><span class="sxs-lookup"><span data-stu-id="a5613-112">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="a5613-113">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="a5613-113">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="a5613-114">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="a5613-114">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="a5613-115">NumberOfMembersAvailable</span><span class="sxs-lookup"><span data-stu-id="a5613-115">NumberOfMembersAvailable</span></span>](numberofmembersavailable.md)
  
```xml
<NumberOfMembersAvailable>...</NumberOfMembersAvailable>
```

 <span data-ttu-id="a5613-116">**int**</span><span class="sxs-lookup"><span data-stu-id="a5613-116">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a5613-117">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a5613-117">Attributes and elements</span></span>

<span data-ttu-id="a5613-118">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a5613-118">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5613-119">属性</span><span class="sxs-lookup"><span data-stu-id="a5613-119">Attributes</span></span>

<span data-ttu-id="a5613-120">なし。</span><span class="sxs-lookup"><span data-stu-id="a5613-120">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a5613-121">子要素</span><span class="sxs-lookup"><span data-stu-id="a5613-121">Child elements</span></span>

<span data-ttu-id="a5613-122">なし。</span><span class="sxs-lookup"><span data-stu-id="a5613-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a5613-123">親要素</span><span class="sxs-lookup"><span data-stu-id="a5613-123">Parent elements</span></span>

|<span data-ttu-id="a5613-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="a5613-124">**Element**</span></span>|<span data-ttu-id="a5613-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="a5613-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5613-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="a5613-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="a5613-127">利用可能なユーザーの数、競合しているユーザーの数、および提案された会議の時間について配布リストの空き時間情報を持っていないユーザーの数についての集約された競合情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="a5613-127">Contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="a5613-128">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a5613-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a5613-129">注釈</span><span class="sxs-lookup"><span data-stu-id="a5613-129">Remarks</span></span>

<span data-ttu-id="a5613-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a5613-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a5613-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a5613-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5613-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="a5613-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a5613-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a5613-133">Schema Name</span></span>  <br/> |<span data-ttu-id="a5613-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a5613-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="a5613-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a5613-135">Validation File</span></span>  <br/> |<span data-ttu-id="a5613-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a5613-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a5613-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a5613-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="a5613-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="a5613-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a5613-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="a5613-139">See also</span></span>



[<span data-ttu-id="a5613-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="a5613-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="a5613-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a5613-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="a5613-142">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="a5613-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


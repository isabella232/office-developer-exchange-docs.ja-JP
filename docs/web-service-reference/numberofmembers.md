---
title: NumberOfMembers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfMembers
api_type:
- schema
ms.assetid: 845fb877-de49-4e26-8885-6f026edd9ee9
description: NumberOfMembers 要素は、配布リスト内のユーザー、リソース、ルームの数を表します。
ms.openlocfilehash: c91087f42d806afb0a0d3d607cc84f14a1a6c1b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462599"
---
# <a name="numberofmembers"></a><span data-ttu-id="6d78c-103">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="6d78c-103">NumberOfMembers</span></span>

<span data-ttu-id="6d78c-104">**Numberofmembers**要素は、配布リスト内のユーザー、リソース、ルームの数を表します。</span><span class="sxs-lookup"><span data-stu-id="6d78c-104">The **NumberOfMembers** element represents the number of users, resources, and rooms in a distribution list.</span></span> 
  
[<span data-ttu-id="6d78c-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="6d78c-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="6d78c-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="6d78c-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="6d78c-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="6d78c-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="6d78c-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="6d78c-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="6d78c-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="6d78c-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="6d78c-110">提案</span><span class="sxs-lookup"><span data-stu-id="6d78c-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="6d78c-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="6d78c-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="6d78c-112">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="6d78c-112">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="6d78c-113">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="6d78c-113">NumberOfMembers</span></span>](numberofmembers.md)
  
```xml
<NumberOfMembers>...</NumberOfMembers>
```

 <span data-ttu-id="6d78c-114">**int**</span><span class="sxs-lookup"><span data-stu-id="6d78c-114">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d78c-115">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6d78c-115">Attributes and elements</span></span>

<span data-ttu-id="6d78c-116">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6d78c-116">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d78c-117">属性</span><span class="sxs-lookup"><span data-stu-id="6d78c-117">Attributes</span></span>

<span data-ttu-id="6d78c-118">なし。</span><span class="sxs-lookup"><span data-stu-id="6d78c-118">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d78c-119">子要素</span><span class="sxs-lookup"><span data-stu-id="6d78c-119">Child elements</span></span>

<span data-ttu-id="6d78c-120">なし。</span><span class="sxs-lookup"><span data-stu-id="6d78c-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6d78c-121">親要素</span><span class="sxs-lookup"><span data-stu-id="6d78c-121">Parent elements</span></span>

|<span data-ttu-id="6d78c-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="6d78c-122">**Element**</span></span>|<span data-ttu-id="6d78c-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="6d78c-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d78c-124">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="6d78c-124">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="6d78c-125">利用可能なユーザー数、競合しているユーザーの数、および推奨される会議時間の配布リストに空き時間情報を持たないユーザーの数についての集約競合情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="6d78c-125">Contains aggregate conflict information about the number of users available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="6d78c-126">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d78c-126">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6d78c-127">注釈</span><span class="sxs-lookup"><span data-stu-id="6d78c-127">Remarks</span></span>

<span data-ttu-id="6d78c-128">**Numberofmembers**要素の最大値は100です。</span><span class="sxs-lookup"><span data-stu-id="6d78c-128">The maximum value of the **NumberOfMembers** element is 100.</span></span> 
  
<span data-ttu-id="6d78c-129">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6d78c-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d78c-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6d78c-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d78c-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="6d78c-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6d78c-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6d78c-132">Schema Name</span></span>  <br/> |<span data-ttu-id="6d78c-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6d78c-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="6d78c-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6d78c-134">Validation File</span></span>  <br/> |<span data-ttu-id="6d78c-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6d78c-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6d78c-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6d78c-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="6d78c-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="6d78c-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6d78c-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="6d78c-138">See also</span></span>



[<span data-ttu-id="6d78c-139">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="6d78c-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="6d78c-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="6d78c-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="6d78c-141">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="6d78c-141">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


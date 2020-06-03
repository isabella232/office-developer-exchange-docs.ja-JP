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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462599"
---
# <a name="numberofmembers"></a><span data-ttu-id="acd9f-103">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="acd9f-103">NumberOfMembers</span></span>

<span data-ttu-id="acd9f-104">**Numberofmembers**要素は、配布リスト内のユーザー、リソース、ルームの数を表します。</span><span class="sxs-lookup"><span data-stu-id="acd9f-104">The **NumberOfMembers** element represents the number of users, resources, and rooms in a distribution list.</span></span> 
  
[<span data-ttu-id="acd9f-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="acd9f-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="acd9f-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="acd9f-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="acd9f-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="acd9f-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="acd9f-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="acd9f-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="acd9f-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="acd9f-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="acd9f-110">提案</span><span class="sxs-lookup"><span data-stu-id="acd9f-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="acd9f-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="acd9f-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="acd9f-112">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="acd9f-112">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="acd9f-113">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="acd9f-113">NumberOfMembers</span></span>](numberofmembers.md)
  
```xml
<NumberOfMembers>...</NumberOfMembers>
```

 <span data-ttu-id="acd9f-114">**int**</span><span class="sxs-lookup"><span data-stu-id="acd9f-114">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="acd9f-115">属性と要素</span><span class="sxs-lookup"><span data-stu-id="acd9f-115">Attributes and elements</span></span>

<span data-ttu-id="acd9f-116">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="acd9f-116">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="acd9f-117">属性</span><span class="sxs-lookup"><span data-stu-id="acd9f-117">Attributes</span></span>

<span data-ttu-id="acd9f-118">なし。</span><span class="sxs-lookup"><span data-stu-id="acd9f-118">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="acd9f-119">子要素</span><span class="sxs-lookup"><span data-stu-id="acd9f-119">Child elements</span></span>

<span data-ttu-id="acd9f-120">なし。</span><span class="sxs-lookup"><span data-stu-id="acd9f-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="acd9f-121">親要素</span><span class="sxs-lookup"><span data-stu-id="acd9f-121">Parent elements</span></span>

|<span data-ttu-id="acd9f-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="acd9f-122">**Element**</span></span>|<span data-ttu-id="acd9f-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="acd9f-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="acd9f-124">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="acd9f-124">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="acd9f-125">利用可能なユーザー数、競合しているユーザーの数、および推奨される会議時間の配布リストに空き時間情報を持たないユーザーの数についての集約競合情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="acd9f-125">Contains aggregate conflict information about the number of users available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="acd9f-126">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="acd9f-126">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="acd9f-127">注釈</span><span class="sxs-lookup"><span data-stu-id="acd9f-127">Remarks</span></span>

<span data-ttu-id="acd9f-128">**Numberofmembers**要素の最大値は100です。</span><span class="sxs-lookup"><span data-stu-id="acd9f-128">The maximum value of the **NumberOfMembers** element is 100.</span></span> 
  
<span data-ttu-id="acd9f-129">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="acd9f-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="acd9f-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="acd9f-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="acd9f-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="acd9f-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="acd9f-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="acd9f-132">Schema Name</span></span>  <br/> |<span data-ttu-id="acd9f-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="acd9f-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="acd9f-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="acd9f-134">Validation File</span></span>  <br/> |<span data-ttu-id="acd9f-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="acd9f-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="acd9f-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="acd9f-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="acd9f-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="acd9f-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="acd9f-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="acd9f-138">See also</span></span>



[<span data-ttu-id="acd9f-139">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="acd9f-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="acd9f-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="acd9f-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="acd9f-141">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="acd9f-141">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


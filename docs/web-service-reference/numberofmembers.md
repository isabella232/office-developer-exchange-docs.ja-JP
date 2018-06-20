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
description: NumberOfMembers 要素は、ユーザー、リソース、およびパブリック フォルダーの配布リストの数を表します。
ms.openlocfilehash: 9777660b1a54bfb5afb6e569ba1009a1654bdef3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832635"
---
# <a name="numberofmembers"></a><span data-ttu-id="045d1-103">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="045d1-103">NumberOfMembers</span></span>

<span data-ttu-id="045d1-104">**NumberOfMembers**要素は、ユーザー、リソース、およびパブリック フォルダーの配布リストの数を表します。</span><span class="sxs-lookup"><span data-stu-id="045d1-104">The **NumberOfMembers** element represents the number of users, resources, and rooms in a distribution list.</span></span> 
  
[<span data-ttu-id="045d1-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="045d1-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="045d1-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="045d1-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="045d1-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="045d1-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="045d1-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="045d1-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="045d1-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="045d1-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="045d1-110">提案</span><span class="sxs-lookup"><span data-stu-id="045d1-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="045d1-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="045d1-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="045d1-112">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="045d1-112">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="045d1-113">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="045d1-113">NumberOfMembers</span></span>](numberofmembers.md)
  
```xml
<NumberOfMembers>...</NumberOfMembers>
```

 <span data-ttu-id="045d1-114">**int**</span><span class="sxs-lookup"><span data-stu-id="045d1-114">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="045d1-115">属性および要素</span><span class="sxs-lookup"><span data-stu-id="045d1-115">Attributes and elements</span></span>

<span data-ttu-id="045d1-116">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="045d1-116">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="045d1-117">属性</span><span class="sxs-lookup"><span data-stu-id="045d1-117">Attributes</span></span>

<span data-ttu-id="045d1-118">なし。</span><span class="sxs-lookup"><span data-stu-id="045d1-118">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="045d1-119">子要素</span><span class="sxs-lookup"><span data-stu-id="045d1-119">Child elements</span></span>

<span data-ttu-id="045d1-120">なし。</span><span class="sxs-lookup"><span data-stu-id="045d1-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="045d1-121">親要素</span><span class="sxs-lookup"><span data-stu-id="045d1-121">Parent elements</span></span>

|<span data-ttu-id="045d1-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="045d1-122">**Element**</span></span>|<span data-ttu-id="045d1-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="045d1-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="045d1-124">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="045d1-124">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="045d1-125">可能なユーザー数、競合を持っているユーザーの数および提案された会議の配布リストの利用可能時間情報を持っていないユーザーの数についての集計の競合に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="045d1-125">Contains aggregate conflict information about the number of users available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="045d1-126">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="045d1-126">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="045d1-127">備考</span><span class="sxs-lookup"><span data-stu-id="045d1-127">Remarks</span></span>

<span data-ttu-id="045d1-128">**NumberOfMembers**要素の最大値は 100 です。</span><span class="sxs-lookup"><span data-stu-id="045d1-128">The maximum value of the **NumberOfMembers** element is 100.</span></span> 
  
<span data-ttu-id="045d1-129">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="045d1-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="045d1-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="045d1-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="045d1-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="045d1-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="045d1-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="045d1-132">Schema Name</span></span>  <br/> |<span data-ttu-id="045d1-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="045d1-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="045d1-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="045d1-134">Validation File</span></span>  <br/> |<span data-ttu-id="045d1-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="045d1-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="045d1-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="045d1-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="045d1-137">False</span><span class="sxs-lookup"><span data-stu-id="045d1-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="045d1-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="045d1-138">See also</span></span>



[<span data-ttu-id="045d1-139">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="045d1-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="045d1-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="045d1-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="045d1-141">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="045d1-141">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


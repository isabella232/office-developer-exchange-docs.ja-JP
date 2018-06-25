---
title: TooBigGroupAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TooBigGroupAttendeeConflictData
api_type:
- schema
ms.assetid: 1512428d-ce22-4da9-b1c1-446b4bcd0a21
description: TooBigGroupAttendeeConflictData 要素は、配布リストとして解決された出席者を表しますが、展開する配布リストが大きすぎます。
ms.openlocfilehash: 1137368d13cb5b88fd2a7866cadc6d69b783c75b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839740"
---
# <a name="toobiggroupattendeeconflictdata"></a><span data-ttu-id="1d038-103">TooBigGroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="1d038-103">TooBigGroupAttendeeConflictData</span></span>

<span data-ttu-id="1d038-104">**TooBigGroupAttendeeConflictData**要素は、配布リストとして解決された出席者を表しますが、展開する配布リストが大きすぎます。</span><span class="sxs-lookup"><span data-stu-id="1d038-104">The **TooBigGroupAttendeeConflictData** element represents an attendee that was resolved as a distribution list but the distribution list was too large to expand.</span></span> 
  
[<span data-ttu-id="1d038-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1d038-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="1d038-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="1d038-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="1d038-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="1d038-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="1d038-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="1d038-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="1d038-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="1d038-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="1d038-110">提案</span><span class="sxs-lookup"><span data-stu-id="1d038-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="1d038-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="1d038-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="1d038-112">TooBigGroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="1d038-112">TooBigGroupAttendeeConflictData</span></span>](toobiggroupattendeeconflictdata.md)
  
```xml
<TooBigGroupAttendeeConflictData/>
```

 <span data-ttu-id="1d038-113">**TooBigGroupAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="1d038-113">**TooBigGroupAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1d038-114">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1d038-114">Attributes and elements</span></span>

<span data-ttu-id="1d038-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1d038-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d038-116">属性</span><span class="sxs-lookup"><span data-stu-id="1d038-116">Attributes</span></span>

<span data-ttu-id="1d038-117">なし。</span><span class="sxs-lookup"><span data-stu-id="1d038-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1d038-118">子要素</span><span class="sxs-lookup"><span data-stu-id="1d038-118">Child elements</span></span>

<span data-ttu-id="1d038-119">なし。</span><span class="sxs-lookup"><span data-stu-id="1d038-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1d038-120">親要素</span><span class="sxs-lookup"><span data-stu-id="1d038-120">Parent elements</span></span>

|<span data-ttu-id="1d038-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="1d038-121">**Element**</span></span>|<span data-ttu-id="1d038-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="1d038-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d038-123">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="1d038-123">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="1d038-124">[GetUserAvailabilityRequest](getuseravailabilityrequest.md)で特定の出席者に対して競合データの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1d038-124">Contains an array of conflict data for attendees identified in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span></span>  <br/> <span data-ttu-id="1d038-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="1d038-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1d038-126">備考</span><span class="sxs-lookup"><span data-stu-id="1d038-126">Remarks</span></span>

<span data-ttu-id="1d038-127">100 を超えるメンバーを含む配布リストは展開できません。</span><span class="sxs-lookup"><span data-stu-id="1d038-127">Distribution lists that contain more than 100 members cannot be expanded.</span></span>
  
<span data-ttu-id="1d038-128">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="1d038-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1d038-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="1d038-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d038-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="1d038-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1d038-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1d038-131">Schema Name</span></span>  <br/> |<span data-ttu-id="1d038-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1d038-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="1d038-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1d038-133">Validation File</span></span>  <br/> |<span data-ttu-id="1d038-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1d038-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1d038-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1d038-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="1d038-136">False</span><span class="sxs-lookup"><span data-stu-id="1d038-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1d038-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="1d038-137">See also</span></span>



[<span data-ttu-id="1d038-138">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="1d038-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="1d038-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1d038-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="1d038-140">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="1d038-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


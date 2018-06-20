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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839740"
---
# <a name="toobiggroupattendeeconflictdata"></a><span data-ttu-id="fc4cf-103">TooBigGroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="fc4cf-103">TooBigGroupAttendeeConflictData</span></span>

<span data-ttu-id="fc4cf-104">**TooBigGroupAttendeeConflictData**要素は、配布リストとして解決された出席者を表しますが、展開する配布リストが大きすぎます。</span><span class="sxs-lookup"><span data-stu-id="fc4cf-104">The **TooBigGroupAttendeeConflictData** element represents an attendee that was resolved as a distribution list but the distribution list was too large to expand.</span></span> 
  
[<span data-ttu-id="fc4cf-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="fc4cf-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="fc4cf-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="fc4cf-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="fc4cf-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="fc4cf-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="fc4cf-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="fc4cf-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="fc4cf-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="fc4cf-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="fc4cf-110">提案</span><span class="sxs-lookup"><span data-stu-id="fc4cf-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="fc4cf-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="fc4cf-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="fc4cf-112">TooBigGroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="fc4cf-112">TooBigGroupAttendeeConflictData</span></span>](toobiggroupattendeeconflictdata.md)
  
```xml
<TooBigGroupAttendeeConflictData/>
```

 <span data-ttu-id="fc4cf-113">**TooBigGroupAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="fc4cf-113">**TooBigGroupAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc4cf-114">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fc4cf-114">Attributes and elements</span></span>

<span data-ttu-id="fc4cf-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fc4cf-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc4cf-116">属性</span><span class="sxs-lookup"><span data-stu-id="fc4cf-116">Attributes</span></span>

<span data-ttu-id="fc4cf-117">なし。</span><span class="sxs-lookup"><span data-stu-id="fc4cf-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc4cf-118">子要素</span><span class="sxs-lookup"><span data-stu-id="fc4cf-118">Child elements</span></span>

<span data-ttu-id="fc4cf-119">なし。</span><span class="sxs-lookup"><span data-stu-id="fc4cf-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fc4cf-120">親要素</span><span class="sxs-lookup"><span data-stu-id="fc4cf-120">Parent elements</span></span>

|<span data-ttu-id="fc4cf-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="fc4cf-121">**Element**</span></span>|<span data-ttu-id="fc4cf-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="fc4cf-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc4cf-123">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="fc4cf-123">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="fc4cf-124">[GetUserAvailabilityRequest](getuseravailabilityrequest.md)で特定の出席者に対して競合データの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fc4cf-124">Contains an array of conflict data for attendees identified in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span></span>  <br/> <span data-ttu-id="fc4cf-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="fc4cf-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fc4cf-126">備考</span><span class="sxs-lookup"><span data-stu-id="fc4cf-126">Remarks</span></span>

<span data-ttu-id="fc4cf-127">100 を超えるメンバーを含む配布リストは展開できません。</span><span class="sxs-lookup"><span data-stu-id="fc4cf-127">Distribution lists that contain more than 100 members cannot be expanded.</span></span>
  
<span data-ttu-id="fc4cf-128">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="fc4cf-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc4cf-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="fc4cf-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc4cf-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="fc4cf-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fc4cf-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fc4cf-131">Schema Name</span></span>  <br/> |<span data-ttu-id="fc4cf-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="fc4cf-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="fc4cf-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fc4cf-133">Validation File</span></span>  <br/> |<span data-ttu-id="fc4cf-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fc4cf-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fc4cf-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fc4cf-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc4cf-136">False</span><span class="sxs-lookup"><span data-stu-id="fc4cf-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc4cf-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="fc4cf-137">See also</span></span>



[<span data-ttu-id="fc4cf-138">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="fc4cf-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="fc4cf-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="fc4cf-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="fc4cf-140">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="fc4cf-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


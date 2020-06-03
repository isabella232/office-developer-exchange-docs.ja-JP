---
title: 提案
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Suggestion
api_type:
- schema
ms.assetid: 040a5c8f-b62f-4d1d-9d2c-dc3c5e01481f
description: 提案要素は、1つの会議提案を表します。
ms.openlocfilehash: 25821abd5463ddba86a487709c8d2f8d928a94cc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530381"
---
# <a name="suggestion"></a><span data-ttu-id="5b312-103">提案</span><span class="sxs-lookup"><span data-stu-id="5b312-103">Suggestion</span></span>

<span data-ttu-id="5b312-104">**提案**要素は、1つの会議提案を表します。</span><span class="sxs-lookup"><span data-stu-id="5b312-104">The **Suggestion** element represents a single meeting suggestion.</span></span> 
  
[<span data-ttu-id="5b312-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="5b312-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="5b312-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="5b312-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="5b312-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="5b312-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="5b312-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="5b312-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="5b312-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="5b312-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="5b312-110">提案</span><span class="sxs-lookup"><span data-stu-id="5b312-110">Suggestion</span></span>](suggestion.md)
  
```xml
<Suggestion>
   <MeetingTime>...</MeetingTime>
   <IsWorkTime>...</IsWorkTime>
   <SuggestionQuality>...</SuggestionQuality>
   <AttendeeConflictDataArray>...</AttendeeConflictDataArray>
</Suggestion>
```

 <span data-ttu-id="5b312-111">**提案**</span><span class="sxs-lookup"><span data-stu-id="5b312-111">**Suggestion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5b312-112">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5b312-112">Attributes and elements</span></span>

<span data-ttu-id="5b312-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5b312-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5b312-114">属性</span><span class="sxs-lookup"><span data-stu-id="5b312-114">Attributes</span></span>

<span data-ttu-id="5b312-115">なし。</span><span class="sxs-lookup"><span data-stu-id="5b312-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5b312-116">子要素</span><span class="sxs-lookup"><span data-stu-id="5b312-116">Child elements</span></span>

|<span data-ttu-id="5b312-117">**Element**</span><span class="sxs-lookup"><span data-stu-id="5b312-117">**Element**</span></span>|<span data-ttu-id="5b312-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="5b312-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b312-119">会議時間</span><span class="sxs-lookup"><span data-stu-id="5b312-119">MeetingTime</span></span>](meetingtime.md) <br/> |<span data-ttu-id="5b312-120">提案された会議の時間を表します。</span><span class="sxs-lookup"><span data-stu-id="5b312-120">Represents a suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="5b312-121">Iswork Time</span><span class="sxs-lookup"><span data-stu-id="5b312-121">IsWorkTime</span></span>](isworktime.md) <br/> |<span data-ttu-id="5b312-122">スケジュールされた作業時間に会議の提案時間が発生するかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="5b312-122">Represents whether the suggested meeting time occurs during scheduled work hours.</span></span>  <br/> |
|[<span data-ttu-id="5b312-123">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="5b312-123">SuggestionQuality</span></span>](suggestionquality.md) <br/> |<span data-ttu-id="5b312-124">提案された会議の時間の品質を表します。</span><span class="sxs-lookup"><span data-stu-id="5b312-124">Represents the quality of the suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="5b312-125">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="5b312-125">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="5b312-126">ユーザーとリソースの間の競合と、推奨される会議時間との間の競合を説明する情報の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5b312-126">Contains an array of information that describes conflicts between users and resources and the suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5b312-127">親要素</span><span class="sxs-lookup"><span data-stu-id="5b312-127">Parent elements</span></span>

|<span data-ttu-id="5b312-128">**要素**</span><span class="sxs-lookup"><span data-stu-id="5b312-128">**Element**</span></span>|<span data-ttu-id="5b312-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="5b312-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b312-130">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="5b312-130">SuggestionArray</span></span>](suggestionarray.md) <br/> |<span data-ttu-id="5b312-131">会議の提案時間の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="5b312-131">Contains an array of suggested meeting times.</span></span>  <br/> <span data-ttu-id="5b312-132">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5b312-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5b312-133">注釈</span><span class="sxs-lookup"><span data-stu-id="5b312-133">Remarks</span></span>

<span data-ttu-id="5b312-134">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5b312-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5b312-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5b312-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5b312-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="5b312-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5b312-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5b312-137">Schema Name</span></span>  <br/> |<span data-ttu-id="5b312-138">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="5b312-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="5b312-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5b312-139">Validation File</span></span>  <br/> |<span data-ttu-id="5b312-140">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="5b312-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5b312-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5b312-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="5b312-142">正しくない</span><span class="sxs-lookup"><span data-stu-id="5b312-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5b312-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="5b312-143">See also</span></span>



[<span data-ttu-id="5b312-144">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="5b312-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="5b312-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="5b312-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="5b312-146">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="5b312-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


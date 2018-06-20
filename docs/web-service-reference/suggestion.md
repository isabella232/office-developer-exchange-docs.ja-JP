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
description: 提案要素では、提案された 1 つの会議を表します。
ms.openlocfilehash: 24e2db1e0eabe35f7c971b0f1dbcbd333358f171
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839621"
---
# <a name="suggestion"></a><span data-ttu-id="7eb60-103">提案</span><span class="sxs-lookup"><span data-stu-id="7eb60-103">Suggestion</span></span>

<span data-ttu-id="7eb60-104">**提案**要素では、提案された 1 つの会議を表します。</span><span class="sxs-lookup"><span data-stu-id="7eb60-104">The **Suggestion** element represents a single meeting suggestion.</span></span> 
  
[<span data-ttu-id="7eb60-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7eb60-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="7eb60-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="7eb60-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="7eb60-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="7eb60-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="7eb60-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="7eb60-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="7eb60-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="7eb60-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="7eb60-110">提案</span><span class="sxs-lookup"><span data-stu-id="7eb60-110">Suggestion</span></span>](suggestion.md)
  
```xml
<Suggestion>
   <MeetingTime>...</MeetingTime>
   <IsWorkTime>...</IsWorkTime>
   <SuggestionQuality>...</SuggestionQuality>
   <AttendeeConflictDataArray>...</AttendeeConflictDataArray>
</Suggestion>
```

 <span data-ttu-id="7eb60-111">**提案**</span><span class="sxs-lookup"><span data-stu-id="7eb60-111">**Suggestion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7eb60-112">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7eb60-112">Attributes and elements</span></span>

<span data-ttu-id="7eb60-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7eb60-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7eb60-114">属性</span><span class="sxs-lookup"><span data-stu-id="7eb60-114">Attributes</span></span>

<span data-ttu-id="7eb60-115">なし。</span><span class="sxs-lookup"><span data-stu-id="7eb60-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7eb60-116">子要素</span><span class="sxs-lookup"><span data-stu-id="7eb60-116">Child elements</span></span>

|<span data-ttu-id="7eb60-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="7eb60-117">**Element**</span></span>|<span data-ttu-id="7eb60-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="7eb60-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7eb60-119">MeetingTime</span><span class="sxs-lookup"><span data-stu-id="7eb60-119">MeetingTime</span></span>](meetingtime.md) <br/> |<span data-ttu-id="7eb60-120">提案された会議の時間を表します。</span><span class="sxs-lookup"><span data-stu-id="7eb60-120">Represents a suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="7eb60-121">IsWorkTime</span><span class="sxs-lookup"><span data-stu-id="7eb60-121">IsWorkTime</span></span>](isworktime.md) <br/> |<span data-ttu-id="7eb60-122">提案された会議の時間がスケジュールされた作業時間中に発生するかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="7eb60-122">Represents whether the suggested meeting time occurs during scheduled work hours.</span></span>  <br/> |
|[<span data-ttu-id="7eb60-123">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="7eb60-123">SuggestionQuality</span></span>](suggestionquality.md) <br/> |<span data-ttu-id="7eb60-124">提案された会議の時間の品質を表します。</span><span class="sxs-lookup"><span data-stu-id="7eb60-124">Represents the quality of the suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="7eb60-125">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="7eb60-125">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="7eb60-126">ユーザーとリソース、および推奨される会議の時刻間の競合を説明する情報の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7eb60-126">Contains an array of information that describes conflicts between users and resources and the suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7eb60-127">親要素</span><span class="sxs-lookup"><span data-stu-id="7eb60-127">Parent elements</span></span>

|<span data-ttu-id="7eb60-128">**要素**</span><span class="sxs-lookup"><span data-stu-id="7eb60-128">**Element**</span></span>|<span data-ttu-id="7eb60-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="7eb60-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7eb60-130">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="7eb60-130">SuggestionArray</span></span>](suggestionarray.md) <br/> |<span data-ttu-id="7eb60-131">提案された会議の時間の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7eb60-131">Contains an array of suggested meeting times.</span></span>  <br/> <span data-ttu-id="7eb60-132">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="7eb60-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7eb60-133">備考</span><span class="sxs-lookup"><span data-stu-id="7eb60-133">Remarks</span></span>

<span data-ttu-id="7eb60-134">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="7eb60-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7eb60-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="7eb60-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7eb60-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="7eb60-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7eb60-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7eb60-137">Schema Name</span></span>  <br/> |<span data-ttu-id="7eb60-138">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7eb60-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="7eb60-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7eb60-139">Validation File</span></span>  <br/> |<span data-ttu-id="7eb60-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7eb60-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7eb60-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7eb60-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="7eb60-142">False</span><span class="sxs-lookup"><span data-stu-id="7eb60-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7eb60-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="7eb60-143">See also</span></span>



[<span data-ttu-id="7eb60-144">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="7eb60-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="7eb60-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7eb60-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="7eb60-146">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="7eb60-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


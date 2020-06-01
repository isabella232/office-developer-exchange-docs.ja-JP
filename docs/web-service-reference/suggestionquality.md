---
title: SuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionQuality
api_type:
- schema
ms.assetid: 734f1a58-adda-4830-973e-e84bf7b870d5
description: SuggestionQuality 要素は、提案された会議の時間の品質を表します。
ms.openlocfilehash: 3f8c15ccabd03687dc386a0328020cbc0bc802c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457978"
---
# <a name="suggestionquality"></a><span data-ttu-id="bb07a-103">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="bb07a-103">SuggestionQuality</span></span>

<span data-ttu-id="bb07a-104">**SuggestionQuality**要素は、提案された会議の時間の品質を表します。</span><span class="sxs-lookup"><span data-stu-id="bb07a-104">The **SuggestionQuality** element represents the quality of the suggested meeting time.</span></span> 
  
[<span data-ttu-id="bb07a-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="bb07a-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="bb07a-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="bb07a-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="bb07a-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="bb07a-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="bb07a-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="bb07a-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="bb07a-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="bb07a-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="bb07a-110">提案</span><span class="sxs-lookup"><span data-stu-id="bb07a-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="bb07a-111">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="bb07a-111">SuggestionQuality</span></span>](suggestionquality.md)
  
```xml
<SuggestionQuality>Excellent or Good or Fair or Poor</SuggestionQuality>
```

 <span data-ttu-id="bb07a-112">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="bb07a-112">**SuggestionQuality**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb07a-113">属性と要素</span><span class="sxs-lookup"><span data-stu-id="bb07a-113">Attributes and elements</span></span>

<span data-ttu-id="bb07a-114">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bb07a-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb07a-115">属性</span><span class="sxs-lookup"><span data-stu-id="bb07a-115">Attributes</span></span>

<span data-ttu-id="bb07a-116">なし。</span><span class="sxs-lookup"><span data-stu-id="bb07a-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bb07a-117">子要素</span><span class="sxs-lookup"><span data-stu-id="bb07a-117">Child elements</span></span>

<span data-ttu-id="bb07a-118">なし。</span><span class="sxs-lookup"><span data-stu-id="bb07a-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bb07a-119">親要素</span><span class="sxs-lookup"><span data-stu-id="bb07a-119">Parent elements</span></span>

|<span data-ttu-id="bb07a-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="bb07a-120">**Element**</span></span>|<span data-ttu-id="bb07a-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="bb07a-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb07a-122">提案</span><span class="sxs-lookup"><span data-stu-id="bb07a-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="bb07a-123">1つの会議時間の提案を表します。</span><span class="sxs-lookup"><span data-stu-id="bb07a-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="bb07a-124">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bb07a-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bb07a-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bb07a-125">Text value</span></span>

<span data-ttu-id="bb07a-126">**SuggestionQuality**値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb07a-126">A text value that represents a **SuggestionQuality** value is required.</span></span> <span data-ttu-id="bb07a-127">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="bb07a-127">The following are the possible values:</span></span> 
  
- <span data-ttu-id="bb07a-128">推奨される会議時間について、ユーザーとリソース**の 100%** が利用可能です。</span><span class="sxs-lookup"><span data-stu-id="bb07a-128">**Excellent** 100 percent of users and resources are available for the suggested meeting time.</span></span> 
    
- <span data-ttu-id="bb07a-129">**適切な**使用可能なユーザーとリソースの最小パーセンテージは、 [GoodThreshold](goodthreshold.md)要素の値に50を加えた値と等しいか、それよりも大きくなっています。</span><span class="sxs-lookup"><span data-stu-id="bb07a-129">**Good** The minimum percentage of users and resources available is equal to or greater than the [GoodThreshold](goodthreshold.md) element value plus 50.</span></span> 
    
- <span data-ttu-id="bb07a-130">**公正**提案された会議の時間に対して使用できるユーザーとリソースの最大パーセンテージは、 [GoodThreshold](goodthreshold.md)要素の値と50に等しくなります。</span><span class="sxs-lookup"><span data-stu-id="bb07a-130">**Fair** The maximum percentage of users and resources available for a suggested meeting time is equal to the [GoodThreshold](goodthreshold.md) element value plus 50.</span></span> <span data-ttu-id="bb07a-131">**フェア**クオリティ会議の時間の最小値は50% です。</span><span class="sxs-lookup"><span data-stu-id="bb07a-131">The minimum value for a **Fair** quality meeting time is 50 percent.</span></span> 
    
- <span data-ttu-id="bb07a-132">**低**提案された会議の時間について、ユーザーとリソースの50% 未満が利用可能です。</span><span class="sxs-lookup"><span data-stu-id="bb07a-132">**Poor** Less than 50 percent of the users and resources are available for the suggested meeting time.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="bb07a-133">注釈</span><span class="sxs-lookup"><span data-stu-id="bb07a-133">Remarks</span></span>

<span data-ttu-id="bb07a-134">**SuggestionQuality**型は、 [Dayquality](dayquality.md)および[MinimumSuggestionQuality](minimumsuggestionquality.md)要素の型でもあります。</span><span class="sxs-lookup"><span data-stu-id="bb07a-134">The **SuggestionQuality** type is also the type for the [DayQuality](dayquality.md) and the [MinimumSuggestionQuality](minimumsuggestionquality.md) elements.</span></span> 
  
<span data-ttu-id="bb07a-135">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="bb07a-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb07a-136">要素の情報</span><span class="sxs-lookup"><span data-stu-id="bb07a-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb07a-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="bb07a-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bb07a-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bb07a-138">Schema Name</span></span>  <br/> |<span data-ttu-id="bb07a-139">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="bb07a-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="bb07a-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bb07a-140">Validation File</span></span>  <br/> |<span data-ttu-id="bb07a-141">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="bb07a-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bb07a-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bb07a-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="bb07a-143">正しくない</span><span class="sxs-lookup"><span data-stu-id="bb07a-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bb07a-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="bb07a-144">See also</span></span>



[<span data-ttu-id="bb07a-145">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="bb07a-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="bb07a-146">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="bb07a-146">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="bb07a-147">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="bb07a-147">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


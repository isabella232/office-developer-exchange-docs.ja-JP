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
ms.openlocfilehash: e67e0149226b36c22cdd00acd78f6582f826dd3e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839624"
---
# <a name="suggestionquality"></a><span data-ttu-id="08a4f-103">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="08a4f-103">SuggestionQuality</span></span>

<span data-ttu-id="08a4f-104">**SuggestionQuality**要素は、提案された会議の時間の品質を表します。</span><span class="sxs-lookup"><span data-stu-id="08a4f-104">The **SuggestionQuality** element represents the quality of the suggested meeting time.</span></span> 
  
[<span data-ttu-id="08a4f-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="08a4f-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="08a4f-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="08a4f-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="08a4f-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="08a4f-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="08a4f-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="08a4f-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="08a4f-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="08a4f-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="08a4f-110">提案</span><span class="sxs-lookup"><span data-stu-id="08a4f-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="08a4f-111">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="08a4f-111">SuggestionQuality</span></span>](suggestionquality.md)
  
```xml
<SuggestionQuality>Excellent or Good or Fair or Poor</SuggestionQuality>
```

 <span data-ttu-id="08a4f-112">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="08a4f-112">**SuggestionQuality**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08a4f-113">属性および要素</span><span class="sxs-lookup"><span data-stu-id="08a4f-113">Attributes and elements</span></span>

<span data-ttu-id="08a4f-114">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="08a4f-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08a4f-115">属性</span><span class="sxs-lookup"><span data-stu-id="08a4f-115">Attributes</span></span>

<span data-ttu-id="08a4f-116">なし。</span><span class="sxs-lookup"><span data-stu-id="08a4f-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08a4f-117">子要素</span><span class="sxs-lookup"><span data-stu-id="08a4f-117">Child elements</span></span>

<span data-ttu-id="08a4f-118">なし。</span><span class="sxs-lookup"><span data-stu-id="08a4f-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="08a4f-119">親要素</span><span class="sxs-lookup"><span data-stu-id="08a4f-119">Parent elements</span></span>

|<span data-ttu-id="08a4f-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="08a4f-120">**Element**</span></span>|<span data-ttu-id="08a4f-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="08a4f-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08a4f-122">提案</span><span class="sxs-lookup"><span data-stu-id="08a4f-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="08a4f-123">単一会議の時間を提案します。</span><span class="sxs-lookup"><span data-stu-id="08a4f-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="08a4f-124">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="08a4f-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="08a4f-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="08a4f-125">Text value</span></span>

<span data-ttu-id="08a4f-126">**SuggestionQuality**の値を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="08a4f-126">A text value that represents a **SuggestionQuality** value is required.</span></span> <span data-ttu-id="08a4f-127">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="08a4f-127">The following are the possible values:</span></span> 
  
- <span data-ttu-id="08a4f-128">**優れた**ユーザーおよびリソースの 100% は、推奨される会議の時刻を使用できます。</span><span class="sxs-lookup"><span data-stu-id="08a4f-128">**Excellent** 100 percent of users and resources are available for the suggested meeting time.</span></span> 
    
- <span data-ttu-id="08a4f-129">**良い**ユーザーおよびリソースの利用可能な最小の割合は、 [GoodThreshold](goodthreshold.md)要素の値に 50 を加えたよりも同等以上です。</span><span class="sxs-lookup"><span data-stu-id="08a4f-129">**Good** The minimum percentage of users and resources available is equal to or greater than the [GoodThreshold](goodthreshold.md) element value plus 50.</span></span> 
    
- <span data-ttu-id="08a4f-130">**フェア**ユーザーおよび提案された会議の時間に利用できるリソースの最大の割合は、 [GoodThreshold](goodthreshold.md)要素の値に 50 を加算した値です。</span><span class="sxs-lookup"><span data-stu-id="08a4f-130">**Fair** The maximum percentage of users and resources available for a suggested meeting time is equal to the [GoodThreshold](goodthreshold.md) element value plus 50.</span></span> <span data-ttu-id="08a4f-131">**公正な**品質会議の時間の最小値は、50% です。</span><span class="sxs-lookup"><span data-stu-id="08a4f-131">The minimum value for a **Fair** quality meeting time is 50 percent.</span></span> 
    
- <span data-ttu-id="08a4f-132">**低下**ユーザーおよびリソースの 50% 未満の場合は、提案された会議の時間を利用できます。</span><span class="sxs-lookup"><span data-stu-id="08a4f-132">**Poor** Less than 50 percent of the users and resources are available for the suggested meeting time.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="08a4f-133">備考</span><span class="sxs-lookup"><span data-stu-id="08a4f-133">Remarks</span></span>

<span data-ttu-id="08a4f-134">**SuggestionQuality**型は、また、 [DayQuality](dayquality.md)と[MinimumSuggestionQuality](minimumsuggestionquality.md)の要素の型です。</span><span class="sxs-lookup"><span data-stu-id="08a4f-134">The **SuggestionQuality** type is also the type for the [DayQuality](dayquality.md) and the [MinimumSuggestionQuality](minimumsuggestionquality.md) elements.</span></span> 
  
<span data-ttu-id="08a4f-135">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="08a4f-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08a4f-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="08a4f-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08a4f-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="08a4f-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="08a4f-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="08a4f-138">Schema Name</span></span>  <br/> |<span data-ttu-id="08a4f-139">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="08a4f-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="08a4f-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="08a4f-140">Validation File</span></span>  <br/> |<span data-ttu-id="08a4f-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="08a4f-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="08a4f-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="08a4f-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="08a4f-143">False</span><span class="sxs-lookup"><span data-stu-id="08a4f-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08a4f-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="08a4f-144">See also</span></span>



[<span data-ttu-id="08a4f-145">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="08a4f-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="08a4f-146">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="08a4f-146">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="08a4f-147">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="08a4f-147">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


---
title: SuggestionArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionArray
api_type:
- schema
ms.assetid: c1c26008-7b14-4563-8db5-bceb0f475b1b
description: SuggestionArray 要素には、会議の提案の配列が含まれています。
ms.openlocfilehash: d595ae77de293a1975e15102f3f2c3395e6da633
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839622"
---
# <a name="suggestionarray"></a><span data-ttu-id="afe7a-103">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="afe7a-103">SuggestionArray</span></span>

<span data-ttu-id="afe7a-104">**SuggestionArray**要素には、会議の提案の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="afe7a-104">The **SuggestionArray** element contains an array of meeting suggestions.</span></span> 
  
[<span data-ttu-id="afe7a-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="afe7a-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="afe7a-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="afe7a-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="afe7a-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="afe7a-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="afe7a-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="afe7a-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="afe7a-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="afe7a-109">SuggestionArray</span></span>](suggestionarray.md)
  
```xml
<SuggestionArray>
   <Suggestion>...</Suggestion>
</SuggestionArray>
```

 <span data-ttu-id="afe7a-110">**ArrayOfSuggestion**</span><span class="sxs-lookup"><span data-stu-id="afe7a-110">**ArrayOfSuggestion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="afe7a-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="afe7a-111">Attributes and elements</span></span>

<span data-ttu-id="afe7a-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="afe7a-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="afe7a-113">属性</span><span class="sxs-lookup"><span data-stu-id="afe7a-113">Attributes</span></span>

<span data-ttu-id="afe7a-114">なし。</span><span class="sxs-lookup"><span data-stu-id="afe7a-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="afe7a-115">子要素</span><span class="sxs-lookup"><span data-stu-id="afe7a-115">Child elements</span></span>

|<span data-ttu-id="afe7a-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="afe7a-116">**Element**</span></span>|<span data-ttu-id="afe7a-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="afe7a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afe7a-118">提案</span><span class="sxs-lookup"><span data-stu-id="afe7a-118">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="afe7a-119">提案された 1 つの会議を表します。</span><span class="sxs-lookup"><span data-stu-id="afe7a-119">Represents a single meeting suggestion.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="afe7a-120">親要素</span><span class="sxs-lookup"><span data-stu-id="afe7a-120">Parent elements</span></span>

|<span data-ttu-id="afe7a-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="afe7a-121">**Element**</span></span>|<span data-ttu-id="afe7a-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="afe7a-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afe7a-123">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="afe7a-123">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="afe7a-124">推奨される会議の時刻を含む 1 つの日付を表します。</span><span class="sxs-lookup"><span data-stu-id="afe7a-124">Represents a single day that contains suggested meeting times.</span></span>  <br/> <span data-ttu-id="afe7a-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="afe7a-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="afe7a-126">備考</span><span class="sxs-lookup"><span data-stu-id="afe7a-126">Remarks</span></span>

<span data-ttu-id="afe7a-127">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="afe7a-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="afe7a-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="afe7a-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="afe7a-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="afe7a-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="afe7a-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="afe7a-130">Schema Name</span></span>  <br/> |<span data-ttu-id="afe7a-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="afe7a-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="afe7a-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="afe7a-132">Validation File</span></span>  <br/> |<span data-ttu-id="afe7a-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="afe7a-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="afe7a-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="afe7a-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="afe7a-135">False</span><span class="sxs-lookup"><span data-stu-id="afe7a-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="afe7a-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="afe7a-136">See also</span></span>



[<span data-ttu-id="afe7a-137">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="afe7a-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="afe7a-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="afe7a-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="afe7a-139">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="afe7a-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


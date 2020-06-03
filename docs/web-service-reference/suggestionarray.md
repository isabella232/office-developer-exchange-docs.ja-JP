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
description: SuggestionArray 要素には、会議提案の配列が含まれています。
ms.openlocfilehash: ec982417c39569820beef82ae837eacbe316740c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466676"
---
# <a name="suggestionarray"></a><span data-ttu-id="7ced3-103">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="7ced3-103">SuggestionArray</span></span>

<span data-ttu-id="7ced3-104">**SuggestionArray**要素には、会議提案の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7ced3-104">The **SuggestionArray** element contains an array of meeting suggestions.</span></span> 
  
[<span data-ttu-id="7ced3-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7ced3-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="7ced3-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="7ced3-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="7ced3-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="7ced3-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="7ced3-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="7ced3-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="7ced3-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="7ced3-109">SuggestionArray</span></span>](suggestionarray.md)
  
```xml
<SuggestionArray>
   <Suggestion>...</Suggestion>
</SuggestionArray>
```

 <span data-ttu-id="7ced3-110">**ArrayOfSuggestion**</span><span class="sxs-lookup"><span data-stu-id="7ced3-110">**ArrayOfSuggestion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7ced3-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7ced3-111">Attributes and elements</span></span>

<span data-ttu-id="7ced3-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7ced3-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ced3-113">属性</span><span class="sxs-lookup"><span data-stu-id="7ced3-113">Attributes</span></span>

<span data-ttu-id="7ced3-114">なし。</span><span class="sxs-lookup"><span data-stu-id="7ced3-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7ced3-115">子要素</span><span class="sxs-lookup"><span data-stu-id="7ced3-115">Child elements</span></span>

|<span data-ttu-id="7ced3-116">**Element**</span><span class="sxs-lookup"><span data-stu-id="7ced3-116">**Element**</span></span>|<span data-ttu-id="7ced3-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="7ced3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ced3-118">提案</span><span class="sxs-lookup"><span data-stu-id="7ced3-118">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="7ced3-119">1つの会議の提案を表します。</span><span class="sxs-lookup"><span data-stu-id="7ced3-119">Represents a single meeting suggestion.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7ced3-120">親要素</span><span class="sxs-lookup"><span data-stu-id="7ced3-120">Parent elements</span></span>

|<span data-ttu-id="7ced3-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="7ced3-121">**Element**</span></span>|<span data-ttu-id="7ced3-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="7ced3-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ced3-123">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="7ced3-123">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="7ced3-124">提案された会議時間を含む1つの日を表します。</span><span class="sxs-lookup"><span data-stu-id="7ced3-124">Represents a single day that contains suggested meeting times.</span></span>  <br/> <span data-ttu-id="7ced3-125">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ced3-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7ced3-126">注釈</span><span class="sxs-lookup"><span data-stu-id="7ced3-126">Remarks</span></span>

<span data-ttu-id="7ced3-127">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7ced3-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ced3-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7ced3-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ced3-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="7ced3-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7ced3-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7ced3-130">Schema Name</span></span>  <br/> |<span data-ttu-id="7ced3-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7ced3-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="7ced3-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7ced3-132">Validation File</span></span>  <br/> |<span data-ttu-id="7ced3-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7ced3-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7ced3-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7ced3-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="7ced3-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="7ced3-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ced3-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="7ced3-136">See also</span></span>



[<span data-ttu-id="7ced3-137">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="7ced3-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="7ced3-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7ced3-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="7ced3-139">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="7ced3-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


---
title: SuggestionDayResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionDayResult
api_type:
- schema
ms.assetid: 916b1cbb-f2e3-471d-84b0-e33467616652
description: SuggestionDayResult 要素は、提案された会議時間を含む1つの日を表します。
ms.openlocfilehash: af907b62acefb4913814907722b98d326bd0535b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457992"
---
# <a name="suggestiondayresult"></a><span data-ttu-id="2b1e1-103">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="2b1e1-103">SuggestionDayResult</span></span>

<span data-ttu-id="2b1e1-104">**SuggestionDayResult**要素は、提案された会議時間を含む1つの日を表します。</span><span class="sxs-lookup"><span data-stu-id="2b1e1-104">The **SuggestionDayResult** element represents a single day that contains suggested meeting times.</span></span> 
  
[<span data-ttu-id="2b1e1-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="2b1e1-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="2b1e1-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="2b1e1-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="2b1e1-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="2b1e1-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="2b1e1-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="2b1e1-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
```xml
<SuggestionDayResult>
   <Date>...</Date>
   <DayQuality>...</DayQuality>
   <SuggestionArray>...</SuggestionArray>
</SuggestionDayResult>
```

 <span data-ttu-id="2b1e1-109">**SuggestionDayResult**</span><span class="sxs-lookup"><span data-stu-id="2b1e1-109">**SuggestionDayResult**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b1e1-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2b1e1-110">Attributes and elements</span></span>

<span data-ttu-id="2b1e1-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2b1e1-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b1e1-112">属性</span><span class="sxs-lookup"><span data-stu-id="2b1e1-112">Attributes</span></span>

<span data-ttu-id="2b1e1-113">なし。</span><span class="sxs-lookup"><span data-stu-id="2b1e1-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b1e1-114">子要素</span><span class="sxs-lookup"><span data-stu-id="2b1e1-114">Child elements</span></span>

|<span data-ttu-id="2b1e1-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="2b1e1-115">**Element**</span></span>|<span data-ttu-id="2b1e1-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="2b1e1-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b1e1-117">Date</span><span class="sxs-lookup"><span data-stu-id="2b1e1-117">Date</span></span>](date.md) <br/> |<span data-ttu-id="2b1e1-118">提案された会議時間を含む日付を表します。</span><span class="sxs-lookup"><span data-stu-id="2b1e1-118">Represents the date that contains the suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="2b1e1-119">DayQuality</span><span class="sxs-lookup"><span data-stu-id="2b1e1-119">DayQuality</span></span>](dayquality.md) <br/> |<span data-ttu-id="2b1e1-120">品質に推奨される会議時間を含む日の品質を表します。</span><span class="sxs-lookup"><span data-stu-id="2b1e1-120">Represents the quality of the day for containing quality suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="2b1e1-121">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="2b1e1-121">SuggestionArray</span></span>](suggestionarray.md) <br/> |<span data-ttu-id="2b1e1-122">会議提案の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2b1e1-122">Contains an array of meeting suggestions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2b1e1-123">親要素</span><span class="sxs-lookup"><span data-stu-id="2b1e1-123">Parent elements</span></span>

|<span data-ttu-id="2b1e1-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="2b1e1-124">**Element**</span></span>|<span data-ttu-id="2b1e1-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="2b1e1-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b1e1-126">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="2b1e1-126">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md) <br/> |<span data-ttu-id="2b1e1-127">会議提案の配列が日付別に整理されています。</span><span class="sxs-lookup"><span data-stu-id="2b1e1-127">Contains an array of meeting suggestions organized by date.</span></span>  <br/> <span data-ttu-id="2b1e1-128">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b1e1-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2b1e1-129">注釈</span><span class="sxs-lookup"><span data-stu-id="2b1e1-129">Remarks</span></span>

<span data-ttu-id="2b1e1-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2b1e1-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b1e1-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2b1e1-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b1e1-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="2b1e1-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2b1e1-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2b1e1-133">Schema Name</span></span>  <br/> |<span data-ttu-id="2b1e1-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="2b1e1-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="2b1e1-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2b1e1-135">Validation File</span></span>  <br/> |<span data-ttu-id="2b1e1-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="2b1e1-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2b1e1-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2b1e1-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="2b1e1-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="2b1e1-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2b1e1-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="2b1e1-139">See also</span></span>



[<span data-ttu-id="2b1e1-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="2b1e1-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="2b1e1-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="2b1e1-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="2b1e1-142">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="2b1e1-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


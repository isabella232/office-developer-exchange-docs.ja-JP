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
description: SuggestionDayResult 要素は、推奨される会議の時刻を含む 1 つの日付を表します。
ms.openlocfilehash: 7b75258a9e70f1ec6feed6a0b18beb76f356c7f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839623"
---
# <a name="suggestiondayresult"></a><span data-ttu-id="906ef-103">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="906ef-103">SuggestionDayResult</span></span>

<span data-ttu-id="906ef-104">**SuggestionDayResult**要素は、推奨される会議の時刻を含む 1 つの日付を表します。</span><span class="sxs-lookup"><span data-stu-id="906ef-104">The **SuggestionDayResult** element represents a single day that contains suggested meeting times.</span></span> 
  
[<span data-ttu-id="906ef-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="906ef-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="906ef-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="906ef-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="906ef-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="906ef-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="906ef-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="906ef-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
```xml
<SuggestionDayResult>
   <Date>...</Date>
   <DayQuality>...</DayQuality>
   <SuggestionArray>...</SuggestionArray>
</SuggestionDayResult>
```

 <span data-ttu-id="906ef-109">**SuggestionDayResult**</span><span class="sxs-lookup"><span data-stu-id="906ef-109">**SuggestionDayResult**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="906ef-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="906ef-110">Attributes and elements</span></span>

<span data-ttu-id="906ef-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="906ef-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="906ef-112">属性</span><span class="sxs-lookup"><span data-stu-id="906ef-112">Attributes</span></span>

<span data-ttu-id="906ef-113">なし。</span><span class="sxs-lookup"><span data-stu-id="906ef-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="906ef-114">子要素</span><span class="sxs-lookup"><span data-stu-id="906ef-114">Child elements</span></span>

|<span data-ttu-id="906ef-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="906ef-115">**Element**</span></span>|<span data-ttu-id="906ef-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="906ef-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="906ef-117">Date</span><span class="sxs-lookup"><span data-stu-id="906ef-117">Date</span></span>](date.md) <br/> |<span data-ttu-id="906ef-118">提案された会議の時間を含む日付を表します。</span><span class="sxs-lookup"><span data-stu-id="906ef-118">Represents the date that contains the suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="906ef-119">DayQuality</span><span class="sxs-lookup"><span data-stu-id="906ef-119">DayQuality</span></span>](dayquality.md) <br/> |<span data-ttu-id="906ef-120">品質の提案された会議の時刻を格納する 1 日の品質を表します。</span><span class="sxs-lookup"><span data-stu-id="906ef-120">Represents the quality of the day for containing quality suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="906ef-121">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="906ef-121">SuggestionArray</span></span>](suggestionarray.md) <br/> |<span data-ttu-id="906ef-122">会議の提案の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="906ef-122">Contains an array of meeting suggestions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="906ef-123">親要素</span><span class="sxs-lookup"><span data-stu-id="906ef-123">Parent elements</span></span>

|<span data-ttu-id="906ef-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="906ef-124">**Element**</span></span>|<span data-ttu-id="906ef-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="906ef-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="906ef-126">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="906ef-126">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md) <br/> |<span data-ttu-id="906ef-127">会議の提案の日付順の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="906ef-127">Contains an array of meeting suggestions organized by date.</span></span>  <br/> <span data-ttu-id="906ef-128">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="906ef-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="906ef-129">備考</span><span class="sxs-lookup"><span data-stu-id="906ef-129">Remarks</span></span>

<span data-ttu-id="906ef-130">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="906ef-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="906ef-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="906ef-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="906ef-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="906ef-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="906ef-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="906ef-133">Schema Name</span></span>  <br/> |<span data-ttu-id="906ef-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="906ef-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="906ef-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="906ef-135">Validation File</span></span>  <br/> |<span data-ttu-id="906ef-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="906ef-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="906ef-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="906ef-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="906ef-138">False</span><span class="sxs-lookup"><span data-stu-id="906ef-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="906ef-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="906ef-139">See also</span></span>



[<span data-ttu-id="906ef-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="906ef-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="906ef-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="906ef-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="906ef-142">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="906ef-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


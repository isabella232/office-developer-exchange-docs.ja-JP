---
title: IsWorkTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsWorkTime
api_type:
- schema
ms.assetid: 5243dd19-3593-4a81-bb2d-90496e04cb98
description: IsWorkTime 要素は、スケジュールされた作業時間の中に提案された会議の時間が発生するかどうかを表します。
ms.openlocfilehash: c687b29df226ebb28cdf01d3a2da62590f790924
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832135"
---
# <a name="isworktime"></a><span data-ttu-id="61615-103">IsWorkTime</span><span class="sxs-lookup"><span data-stu-id="61615-103">IsWorkTime</span></span>

<span data-ttu-id="61615-104">**IsWorkTime**要素は、スケジュールされた作業時間の中に提案された会議の時間が発生するかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="61615-104">The **IsWorkTime** element represents whether the suggested meeting time occurs during scheduled work hours.</span></span> 
  
[<span data-ttu-id="61615-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="61615-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="61615-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="61615-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="61615-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="61615-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="61615-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="61615-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="61615-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="61615-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="61615-110">提案</span><span class="sxs-lookup"><span data-stu-id="61615-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="61615-111">IsWorkTime</span><span class="sxs-lookup"><span data-stu-id="61615-111">IsWorkTime</span></span>](isworktime.md)
  
```xml
<IsWorkTime>true or false</IsWorkTime>
```

 <span data-ttu-id="61615-112">**boolean**</span><span class="sxs-lookup"><span data-stu-id="61615-112">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="61615-113">属性および要素</span><span class="sxs-lookup"><span data-stu-id="61615-113">Attributes and elements</span></span>

<span data-ttu-id="61615-114">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="61615-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61615-115">属性</span><span class="sxs-lookup"><span data-stu-id="61615-115">Attributes</span></span>

<span data-ttu-id="61615-116">なし。</span><span class="sxs-lookup"><span data-stu-id="61615-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="61615-117">子要素</span><span class="sxs-lookup"><span data-stu-id="61615-117">Child elements</span></span>

<span data-ttu-id="61615-118">なし。</span><span class="sxs-lookup"><span data-stu-id="61615-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="61615-119">親要素</span><span class="sxs-lookup"><span data-stu-id="61615-119">Parent elements</span></span>

|<span data-ttu-id="61615-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="61615-120">**Element**</span></span>|<span data-ttu-id="61615-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="61615-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61615-122">提案</span><span class="sxs-lookup"><span data-stu-id="61615-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="61615-123">単一会議の時間を提案します。</span><span class="sxs-lookup"><span data-stu-id="61615-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="61615-124">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="61615-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="61615-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="61615-125">Text value</span></span>

<span data-ttu-id="61615-126">ブール値を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="61615-126">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="61615-127">備考</span><span class="sxs-lookup"><span data-stu-id="61615-127">Remarks</span></span>

<span data-ttu-id="61615-128">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="61615-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="61615-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="61615-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61615-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="61615-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="61615-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="61615-131">Schema Name</span></span>  <br/> |<span data-ttu-id="61615-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="61615-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="61615-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="61615-133">Validation File</span></span>  <br/> |<span data-ttu-id="61615-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="61615-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="61615-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="61615-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="61615-136">False</span><span class="sxs-lookup"><span data-stu-id="61615-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="61615-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="61615-137">See also</span></span>



[<span data-ttu-id="61615-138">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="61615-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="61615-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="61615-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="61615-140">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="61615-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


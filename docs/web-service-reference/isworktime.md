---
title: Iswork Time
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
description: Iswork Time 要素は、提案された会議時間が、スケジュールされた作業時間内に発生するかどうかを表します。
ms.openlocfilehash: a3f3c73d585bee6f73863e2be64eea245be674f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467579"
---
# <a name="isworktime"></a><span data-ttu-id="6941d-103">Iswork Time</span><span class="sxs-lookup"><span data-stu-id="6941d-103">IsWorkTime</span></span>

<span data-ttu-id="6941d-104">**Iswork time**要素は、提案された会議時間が、スケジュールされた作業時間内に発生するかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="6941d-104">The **IsWorkTime** element represents whether the suggested meeting time occurs during scheduled work hours.</span></span> 
  
[<span data-ttu-id="6941d-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="6941d-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="6941d-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="6941d-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="6941d-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="6941d-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="6941d-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="6941d-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="6941d-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="6941d-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="6941d-110">提案</span><span class="sxs-lookup"><span data-stu-id="6941d-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="6941d-111">Iswork Time</span><span class="sxs-lookup"><span data-stu-id="6941d-111">IsWorkTime</span></span>](isworktime.md)
  
```xml
<IsWorkTime>true or false</IsWorkTime>
```

 <span data-ttu-id="6941d-112">**boolean**</span><span class="sxs-lookup"><span data-stu-id="6941d-112">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6941d-113">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6941d-113">Attributes and elements</span></span>

<span data-ttu-id="6941d-114">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6941d-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6941d-115">属性</span><span class="sxs-lookup"><span data-stu-id="6941d-115">Attributes</span></span>

<span data-ttu-id="6941d-116">なし。</span><span class="sxs-lookup"><span data-stu-id="6941d-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6941d-117">子要素</span><span class="sxs-lookup"><span data-stu-id="6941d-117">Child elements</span></span>

<span data-ttu-id="6941d-118">なし。</span><span class="sxs-lookup"><span data-stu-id="6941d-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6941d-119">親要素</span><span class="sxs-lookup"><span data-stu-id="6941d-119">Parent elements</span></span>

|<span data-ttu-id="6941d-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="6941d-120">**Element**</span></span>|<span data-ttu-id="6941d-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="6941d-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6941d-122">提案</span><span class="sxs-lookup"><span data-stu-id="6941d-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="6941d-123">1つの会議時間の提案を表します。</span><span class="sxs-lookup"><span data-stu-id="6941d-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="6941d-124">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6941d-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6941d-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6941d-125">Text value</span></span>

<span data-ttu-id="6941d-126">ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="6941d-126">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6941d-127">注釈</span><span class="sxs-lookup"><span data-stu-id="6941d-127">Remarks</span></span>

<span data-ttu-id="6941d-128">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6941d-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6941d-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6941d-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6941d-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="6941d-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6941d-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6941d-131">Schema Name</span></span>  <br/> |<span data-ttu-id="6941d-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6941d-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="6941d-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6941d-133">Validation File</span></span>  <br/> |<span data-ttu-id="6941d-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6941d-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6941d-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6941d-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="6941d-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="6941d-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6941d-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="6941d-137">See also</span></span>



[<span data-ttu-id="6941d-138">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="6941d-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="6941d-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="6941d-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="6941d-140">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="6941d-140">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


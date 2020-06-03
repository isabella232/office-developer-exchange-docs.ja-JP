---
title: 会議時間
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingTime
api_type:
- schema
ms.assetid: 6e6d2d8b-e8a2-43e6-a715-0fc7d6dd44b9
description: 会議の時間要素は、提案された会議の時間を表します。
ms.openlocfilehash: 3a7031e70eb8b22adc8030c1cec09d33399332ee
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530451"
---
# <a name="meetingtime"></a><span data-ttu-id="40eb6-103">会議時間</span><span class="sxs-lookup"><span data-stu-id="40eb6-103">MeetingTime</span></span>

<span data-ttu-id="40eb6-104">会議の**時間**要素は、提案された会議の時間を表します。</span><span class="sxs-lookup"><span data-stu-id="40eb6-104">The **MeetingTime** element represents a suggested meeting time.</span></span> 
  
[<span data-ttu-id="40eb6-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="40eb6-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="40eb6-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="40eb6-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="40eb6-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="40eb6-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="40eb6-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="40eb6-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="40eb6-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="40eb6-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="40eb6-110">提案</span><span class="sxs-lookup"><span data-stu-id="40eb6-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="40eb6-111">会議時間</span><span class="sxs-lookup"><span data-stu-id="40eb6-111">MeetingTime</span></span>](meetingtime.md)
  
```xml
<MeetingTime>...</MeetingTime
```

 <span data-ttu-id="40eb6-112">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="40eb6-112">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="40eb6-113">属性と要素</span><span class="sxs-lookup"><span data-stu-id="40eb6-113">Attributes and elements</span></span>

<span data-ttu-id="40eb6-114">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="40eb6-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40eb6-115">属性</span><span class="sxs-lookup"><span data-stu-id="40eb6-115">Attributes</span></span>

<span data-ttu-id="40eb6-116">なし。</span><span class="sxs-lookup"><span data-stu-id="40eb6-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="40eb6-117">子要素</span><span class="sxs-lookup"><span data-stu-id="40eb6-117">Child elements</span></span>

<span data-ttu-id="40eb6-118">なし。</span><span class="sxs-lookup"><span data-stu-id="40eb6-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="40eb6-119">親要素</span><span class="sxs-lookup"><span data-stu-id="40eb6-119">Parent elements</span></span>

|<span data-ttu-id="40eb6-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="40eb6-120">**Element**</span></span>|<span data-ttu-id="40eb6-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="40eb6-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40eb6-122">提案</span><span class="sxs-lookup"><span data-stu-id="40eb6-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="40eb6-123">1つの会議時間の提案を表します。</span><span class="sxs-lookup"><span data-stu-id="40eb6-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="40eb6-124">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="40eb6-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="40eb6-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="40eb6-125">Text value</span></span>

<span data-ttu-id="40eb6-126">**DateTime**値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="40eb6-126">A text value that represents a **dateTime** value is required.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="40eb6-127">注釈</span><span class="sxs-lookup"><span data-stu-id="40eb6-127">Remarks</span></span>

<span data-ttu-id="40eb6-128">[会議の時間](meetingtime.md)要素は、[提案](suggestion.md)要素の必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="40eb6-128">The [MeetingTime](meetingtime.md) element is a required child element of the [Suggestion](suggestion.md) element.</span></span> 
  
<span data-ttu-id="40eb6-129">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="40eb6-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="40eb6-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="40eb6-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="40eb6-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="40eb6-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="40eb6-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="40eb6-132">Schema Name</span></span>  <br/> |<span data-ttu-id="40eb6-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="40eb6-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="40eb6-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="40eb6-134">Validation File</span></span>  <br/> |<span data-ttu-id="40eb6-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="40eb6-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="40eb6-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="40eb6-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="40eb6-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="40eb6-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="40eb6-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="40eb6-138">See also</span></span>



[<span data-ttu-id="40eb6-139">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="40eb6-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="40eb6-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="40eb6-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="40eb6-141">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="40eb6-141">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


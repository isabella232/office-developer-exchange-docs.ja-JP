---
title: MeetingTime
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
description: MeetingTime 要素は、提案された会議の時間を表します。
ms.openlocfilehash: 1ea79be394124431aa1279ee94d5e5c6331d377b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832435"
---
# <a name="meetingtime"></a><span data-ttu-id="2927c-103">MeetingTime</span><span class="sxs-lookup"><span data-stu-id="2927c-103">MeetingTime</span></span>

<span data-ttu-id="2927c-104">**MeetingTime**要素は、提案された会議の時間を表します。</span><span class="sxs-lookup"><span data-stu-id="2927c-104">The **MeetingTime** element represents a suggested meeting time.</span></span> 
  
[<span data-ttu-id="2927c-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="2927c-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="2927c-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="2927c-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="2927c-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="2927c-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="2927c-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="2927c-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="2927c-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="2927c-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="2927c-110">提案</span><span class="sxs-lookup"><span data-stu-id="2927c-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="2927c-111">MeetingTime</span><span class="sxs-lookup"><span data-stu-id="2927c-111">MeetingTime</span></span>](meetingtime.md)
  
```xml
<MeetingTime>...</MeetingTime
```

 <span data-ttu-id="2927c-112">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="2927c-112">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2927c-113">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2927c-113">Attributes and elements</span></span>

<span data-ttu-id="2927c-114">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2927c-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2927c-115">属性</span><span class="sxs-lookup"><span data-stu-id="2927c-115">Attributes</span></span>

<span data-ttu-id="2927c-116">なし。</span><span class="sxs-lookup"><span data-stu-id="2927c-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2927c-117">子要素</span><span class="sxs-lookup"><span data-stu-id="2927c-117">Child elements</span></span>

<span data-ttu-id="2927c-118">なし。</span><span class="sxs-lookup"><span data-stu-id="2927c-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2927c-119">親要素</span><span class="sxs-lookup"><span data-stu-id="2927c-119">Parent elements</span></span>

|<span data-ttu-id="2927c-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="2927c-120">**Element**</span></span>|<span data-ttu-id="2927c-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="2927c-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2927c-122">提案</span><span class="sxs-lookup"><span data-stu-id="2927c-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="2927c-123">単一会議の時間を提案します。</span><span class="sxs-lookup"><span data-stu-id="2927c-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="2927c-124">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="2927c-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2927c-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2927c-125">Text value</span></span>

<span data-ttu-id="2927c-126">**日時**の値を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="2927c-126">A text value that represents a **dateTime** value is required.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2927c-127">備考</span><span class="sxs-lookup"><span data-stu-id="2927c-127">Remarks</span></span>

<span data-ttu-id="2927c-128">[MeetingTime](meetingtime.md)要素は、[提案](suggestion.md)の要素の必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="2927c-128">The [MeetingTime](meetingtime.md) element is a required child element of the [Suggestion](suggestion.md) element.</span></span> 
  
<span data-ttu-id="2927c-129">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="2927c-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2927c-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="2927c-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2927c-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="2927c-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2927c-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2927c-132">Schema Name</span></span>  <br/> |<span data-ttu-id="2927c-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="2927c-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="2927c-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2927c-134">Validation File</span></span>  <br/> |<span data-ttu-id="2927c-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2927c-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2927c-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2927c-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="2927c-137">False</span><span class="sxs-lookup"><span data-stu-id="2927c-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2927c-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="2927c-138">See also</span></span>



[<span data-ttu-id="2927c-139">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="2927c-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="2927c-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="2927c-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="2927c-141">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="2927c-141">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


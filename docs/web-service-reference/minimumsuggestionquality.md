---
title: MinimumSuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MinimumSuggestionQuality
api_type:
- schema
ms.assetid: 3725cbd4-9bc1-4f7d-8929-b2c68cb46114
description: MinimumSuggestionQuality 要素は、応答で返される会議の提案の品質を定義します。
ms.openlocfilehash: c85cbf65a63ac0b09408c14e01889f97a05b27b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467481"
---
# <a name="minimumsuggestionquality"></a><span data-ttu-id="6c70f-103">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="6c70f-103">MinimumSuggestionQuality</span></span>

<span data-ttu-id="6c70f-104">**MinimumSuggestionQuality**要素は、応答で返される会議の提案の品質を定義します。</span><span class="sxs-lookup"><span data-stu-id="6c70f-104">The **MinimumSuggestionQuality** element defines the quality of meeting suggestions to be returned in the response.</span></span> 
  
[<span data-ttu-id="6c70f-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="6c70f-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="6c70f-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="6c70f-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="6c70f-107">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="6c70f-107">MinimumSuggestionQuality</span></span>](minimumsuggestionquality.md)
  
```xml
<MinimumSuggestionQuality>...</MinimumSuggestionQuality>
```

 <span data-ttu-id="6c70f-108">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="6c70f-108">**SuggestionQuality**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c70f-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6c70f-109">Attributes and elements</span></span>

<span data-ttu-id="6c70f-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6c70f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c70f-111">属性</span><span class="sxs-lookup"><span data-stu-id="6c70f-111">Attributes</span></span>

<span data-ttu-id="6c70f-112">なし。</span><span class="sxs-lookup"><span data-stu-id="6c70f-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c70f-113">子要素</span><span class="sxs-lookup"><span data-stu-id="6c70f-113">Child elements</span></span>

<span data-ttu-id="6c70f-114">なし。</span><span class="sxs-lookup"><span data-stu-id="6c70f-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6c70f-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6c70f-115">Parent elements</span></span>

|<span data-ttu-id="6c70f-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="6c70f-116">**Element**</span></span>|<span data-ttu-id="6c70f-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c70f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c70f-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="6c70f-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="6c70f-119">会議提案情報を取得するためのオプションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c70f-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="6c70f-120">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6c70f-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6c70f-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6c70f-121">Text value</span></span>

<span data-ttu-id="6c70f-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="6c70f-122">A text value is required.</span></span> <span data-ttu-id="6c70f-123">次の表に、この要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="6c70f-123">The following table lists the possible values for this element:</span></span>
  
|<span data-ttu-id="6c70f-124">**値**</span><span class="sxs-lookup"><span data-stu-id="6c70f-124">**Value**</span></span>|<span data-ttu-id="6c70f-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c70f-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6c70f-126">**優秀**</span><span class="sxs-lookup"><span data-stu-id="6c70f-126">**Excellent**</span></span> <br/> |<span data-ttu-id="6c70f-127">出席者の0% が、提案された会議の時間と競合しています。</span><span class="sxs-lookup"><span data-stu-id="6c70f-127">0% of the attendees have a conflict with the suggested meeting time.</span></span>  <br/> |
|<span data-ttu-id="6c70f-128">**標準**</span><span class="sxs-lookup"><span data-stu-id="6c70f-128">**Good**</span></span> <br/> |<span data-ttu-id="6c70f-129">Good と見なされるパーセンテージは、 [GoodThreshold](goodthreshold.md)要素を使用して設定されます。</span><span class="sxs-lookup"><span data-stu-id="6c70f-129">The percentage that is considered good is set by using the [GoodThreshold](goodthreshold.md) element.</span></span>  <br/> |
|<span data-ttu-id="6c70f-130">**かなり**</span><span class="sxs-lookup"><span data-stu-id="6c70f-130">**Fair**</span></span> <br/> |<span data-ttu-id="6c70f-131">公平と見なされる割合は、 [GoodThreshold](goodthreshold.md)要素を使用して設定されます。</span><span class="sxs-lookup"><span data-stu-id="6c70f-131">The percentage that is considered fair is set by using the [GoodThreshold](goodthreshold.md) element.</span></span>  <br/> |
|<span data-ttu-id="6c70f-132">**悪い**</span><span class="sxs-lookup"><span data-stu-id="6c70f-132">**Poor**</span></span> <br/> |<span data-ttu-id="6c70f-133">50% 以上の出席者が、提案された会議の時間と競合しています。</span><span class="sxs-lookup"><span data-stu-id="6c70f-133">50% or more of the attendees have a conflict with the suggested meeting time.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6c70f-134">注釈</span><span class="sxs-lookup"><span data-stu-id="6c70f-134">Remarks</span></span>

<span data-ttu-id="6c70f-135">この要素は、 [SuggestionsViewOptions](suggestionsviewoptions.md)要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="6c70f-135">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="6c70f-136">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6c70f-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="6c70f-137">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6c70f-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c70f-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="6c70f-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6c70f-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6c70f-139">Schema Name</span></span>  <br/> |<span data-ttu-id="6c70f-140">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6c70f-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="6c70f-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6c70f-141">Validation File</span></span>  <br/> |<span data-ttu-id="6c70f-142">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6c70f-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6c70f-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6c70f-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="6c70f-144">正しくない</span><span class="sxs-lookup"><span data-stu-id="6c70f-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c70f-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="6c70f-145">See also</span></span>



[<span data-ttu-id="6c70f-146">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="6c70f-146">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="6c70f-147">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="6c70f-147">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


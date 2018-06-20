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
ms.openlocfilehash: ac79682bd761f678f23fc2d698a50fd7704f6fab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832468"
---
# <a name="minimumsuggestionquality"></a><span data-ttu-id="7bcbd-103">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="7bcbd-103">MinimumSuggestionQuality</span></span>

<span data-ttu-id="7bcbd-104">**MinimumSuggestionQuality**要素は、応答で返される会議の提案の品質を定義します。</span><span class="sxs-lookup"><span data-stu-id="7bcbd-104">The **MinimumSuggestionQuality** element defines the quality of meeting suggestions to be returned in the response.</span></span> 
  
[<span data-ttu-id="7bcbd-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="7bcbd-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="7bcbd-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="7bcbd-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="7bcbd-107">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="7bcbd-107">MinimumSuggestionQuality</span></span>](minimumsuggestionquality.md)
  
```xml
<MinimumSuggestionQuality>...</MinimumSuggestionQuality>
```

 <span data-ttu-id="7bcbd-108">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="7bcbd-108">**SuggestionQuality**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7bcbd-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7bcbd-109">Attributes and elements</span></span>

<span data-ttu-id="7bcbd-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7bcbd-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7bcbd-111">属性</span><span class="sxs-lookup"><span data-stu-id="7bcbd-111">Attributes</span></span>

<span data-ttu-id="7bcbd-112">なし。</span><span class="sxs-lookup"><span data-stu-id="7bcbd-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7bcbd-113">子要素</span><span class="sxs-lookup"><span data-stu-id="7bcbd-113">Child elements</span></span>

<span data-ttu-id="7bcbd-114">なし。</span><span class="sxs-lookup"><span data-stu-id="7bcbd-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7bcbd-115">親要素</span><span class="sxs-lookup"><span data-stu-id="7bcbd-115">Parent elements</span></span>

|<span data-ttu-id="7bcbd-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="7bcbd-116">**Element**</span></span>|<span data-ttu-id="7bcbd-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="7bcbd-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7bcbd-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="7bcbd-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="7bcbd-119">取得するためのオプションが含まれています会議の情報を提案します。</span><span class="sxs-lookup"><span data-stu-id="7bcbd-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="7bcbd-120">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="7bcbd-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7bcbd-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7bcbd-121">Text value</span></span>

<span data-ttu-id="7bcbd-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="7bcbd-122">A text value is required.</span></span> <span data-ttu-id="7bcbd-123">この要素の値を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="7bcbd-123">The following table lists the possible values for this element:</span></span>
  
|<span data-ttu-id="7bcbd-124">**値**</span><span class="sxs-lookup"><span data-stu-id="7bcbd-124">**Value**</span></span>|<span data-ttu-id="7bcbd-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="7bcbd-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7bcbd-126">**たいへん良い**</span><span class="sxs-lookup"><span data-stu-id="7bcbd-126">**Excellent**</span></span> <br/> |<span data-ttu-id="7bcbd-127">出席者の 0% では、提案された会議の時間と競合が存在します。</span><span class="sxs-lookup"><span data-stu-id="7bcbd-127">0% of the attendees have a conflict with the suggested meeting time.</span></span>  <br/> |
|<span data-ttu-id="7bcbd-128">**よし**</span><span class="sxs-lookup"><span data-stu-id="7bcbd-128">**Good**</span></span> <br/> |<span data-ttu-id="7bcbd-129">良いと考えられている割合は、 [GoodThreshold](goodthreshold.md)要素を使用して設定されています。</span><span class="sxs-lookup"><span data-stu-id="7bcbd-129">The percentage that is considered good is set by using the [GoodThreshold](goodthreshold.md) element.</span></span>  <br/> |
|<span data-ttu-id="7bcbd-130">**フェア**</span><span class="sxs-lookup"><span data-stu-id="7bcbd-130">**Fair**</span></span> <br/> |<span data-ttu-id="7bcbd-131">公平と考えられている割合は、 [GoodThreshold](goodthreshold.md)要素を使用して設定されています。</span><span class="sxs-lookup"><span data-stu-id="7bcbd-131">The percentage that is considered fair is set by using the [GoodThreshold](goodthreshold.md) element.</span></span>  <br/> |
|<span data-ttu-id="7bcbd-132">**低下**</span><span class="sxs-lookup"><span data-stu-id="7bcbd-132">**Poor**</span></span> <br/> |<span data-ttu-id="7bcbd-133">50% 以上の参加者の提案された会議の時間との競合があります。</span><span class="sxs-lookup"><span data-stu-id="7bcbd-133">50% or more of the attendees have a conflict with the suggested meeting time.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7bcbd-134">備考</span><span class="sxs-lookup"><span data-stu-id="7bcbd-134">Remarks</span></span>

<span data-ttu-id="7bcbd-135">[SuggestionsViewOptions](suggestionsviewoptions.md)要素を使用する場合、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="7bcbd-135">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="7bcbd-136">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="7bcbd-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="7bcbd-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="7bcbd-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7bcbd-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="7bcbd-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7bcbd-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7bcbd-139">Schema Name</span></span>  <br/> |<span data-ttu-id="7bcbd-140">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7bcbd-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="7bcbd-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7bcbd-141">Validation File</span></span>  <br/> |<span data-ttu-id="7bcbd-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7bcbd-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7bcbd-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7bcbd-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="7bcbd-144">False</span><span class="sxs-lookup"><span data-stu-id="7bcbd-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7bcbd-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="7bcbd-145">See also</span></span>



[<span data-ttu-id="7bcbd-146">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="7bcbd-146">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="7bcbd-147">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="7bcbd-147">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


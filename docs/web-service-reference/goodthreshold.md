---
title: GoodThreshold
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GoodThreshold
api_type:
- schema
ms.assetid: 68f607f5-7271-46a6-8ffc-91878185a683
description: GoodThreshold 要素には、適切な会議時間として期間を修飾するために期間を開いておく必要がある出席者の割合を指定します。
ms.openlocfilehash: 34ea433ad7315d61df8cf8e22bae1166d3210af3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457313"
---
# <a name="goodthreshold"></a><span data-ttu-id="e8072-103">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="e8072-103">GoodThreshold</span></span>

<span data-ttu-id="e8072-104">**GoodThreshold**要素には、適切な会議時間として期間を修飾するために期間を開いておく必要がある出席者の割合を指定します。</span><span class="sxs-lookup"><span data-stu-id="e8072-104">The **GoodThreshold** element specifies the percentage of attendees that must have the time period open in order for the time period to qualify as a Good suggested meeting time.</span></span> 
  
[<span data-ttu-id="e8072-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="e8072-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="e8072-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="e8072-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="e8072-107">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="e8072-107">GoodThreshold</span></span>](goodthreshold.md)
  
```xml
<GoodThreshold>...</GoodThreshold>
```

 <span data-ttu-id="e8072-108">**int**</span><span class="sxs-lookup"><span data-stu-id="e8072-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8072-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e8072-109">Attributes and elements</span></span>

<span data-ttu-id="e8072-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e8072-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8072-111">属性</span><span class="sxs-lookup"><span data-stu-id="e8072-111">Attributes</span></span>

<span data-ttu-id="e8072-112">なし。</span><span class="sxs-lookup"><span data-stu-id="e8072-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8072-113">子要素</span><span class="sxs-lookup"><span data-stu-id="e8072-113">Child elements</span></span>

<span data-ttu-id="e8072-114">なし。</span><span class="sxs-lookup"><span data-stu-id="e8072-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e8072-115">親要素</span><span class="sxs-lookup"><span data-stu-id="e8072-115">Parent elements</span></span>

|<span data-ttu-id="e8072-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="e8072-116">**Element**</span></span>|<span data-ttu-id="e8072-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="e8072-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8072-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="e8072-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="e8072-119">会議提案情報を取得するためのオプションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e8072-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="e8072-120">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e8072-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e8072-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e8072-121">Text value</span></span>

<span data-ttu-id="e8072-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="e8072-122">A text value is required.</span></span> <span data-ttu-id="e8072-123">必要な整数値は、0 ~ 50 です。</span><span class="sxs-lookup"><span data-stu-id="e8072-123">The expected integer values are between 0 and 50.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e8072-124">注釈</span><span class="sxs-lookup"><span data-stu-id="e8072-124">Remarks</span></span>

<span data-ttu-id="e8072-125">この要素は、 [SuggestionsViewOptions](suggestionsviewoptions.md)要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="e8072-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> <span data-ttu-id="e8072-126">**GoodThreshold**要素は、どの会議が公正であると見なされるかも決定します。</span><span class="sxs-lookup"><span data-stu-id="e8072-126">The **GoodThreshold** element also determines what meetings are considered Fair.</span></span> <span data-ttu-id="e8072-127">競合のある出席者の割合が、適切なしきい値を超え、かつ50パーセントよりも大きい場合、会議の提案時間は公正になります。</span><span class="sxs-lookup"><span data-stu-id="e8072-127">It the percentage of attendees with conflicts is less than the Good Threshold and higher than 50 percent, the suggested meeting time qualifies as Fair.</span></span> <span data-ttu-id="e8072-128">良好しきい値 + 50 は、適正/公正しきい値を定義するパーセンテージと等しくなります。</span><span class="sxs-lookup"><span data-stu-id="e8072-128">The Good Threshold plus 50 equals the percentage that defines the Good/Fair threshold.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e8072-129">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e8072-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="e8072-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e8072-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8072-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="e8072-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e8072-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e8072-132">Schema Name</span></span>  <br/> |<span data-ttu-id="e8072-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e8072-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="e8072-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e8072-134">Validation File</span></span>  <br/> |<span data-ttu-id="e8072-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e8072-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e8072-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e8072-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="e8072-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="e8072-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8072-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="e8072-138">See also</span></span>



[<span data-ttu-id="e8072-139">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="e8072-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="e8072-140">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="e8072-140">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


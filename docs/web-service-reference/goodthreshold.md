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
description: GoodThreshold 要素は、適切な提案された会議の時間として修飾するまでの時間のために開くまでの時間が必要な出席者の割合を指定します。
ms.openlocfilehash: 8044cb2b52cb572fad8731253dffa34de9d097fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831746"
---
# <a name="goodthreshold"></a><span data-ttu-id="73e12-103">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="73e12-103">GoodThreshold</span></span>

<span data-ttu-id="73e12-104">**GoodThreshold**要素は、適切な提案された会議の時間として修飾するまでの時間のために開くまでの時間が必要な出席者の割合を指定します。</span><span class="sxs-lookup"><span data-stu-id="73e12-104">The **GoodThreshold** element specifies the percentage of attendees that must have the time period open in order for the time period to qualify as a Good suggested meeting time.</span></span> 
  
[<span data-ttu-id="73e12-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="73e12-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="73e12-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="73e12-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="73e12-107">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="73e12-107">GoodThreshold</span></span>](goodthreshold.md)
  
```xml
<GoodThreshold>...</GoodThreshold>
```

 <span data-ttu-id="73e12-108">**int**</span><span class="sxs-lookup"><span data-stu-id="73e12-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73e12-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="73e12-109">Attributes and elements</span></span>

<span data-ttu-id="73e12-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="73e12-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73e12-111">属性</span><span class="sxs-lookup"><span data-stu-id="73e12-111">Attributes</span></span>

<span data-ttu-id="73e12-112">なし。</span><span class="sxs-lookup"><span data-stu-id="73e12-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73e12-113">子要素</span><span class="sxs-lookup"><span data-stu-id="73e12-113">Child elements</span></span>

<span data-ttu-id="73e12-114">なし。</span><span class="sxs-lookup"><span data-stu-id="73e12-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="73e12-115">親要素</span><span class="sxs-lookup"><span data-stu-id="73e12-115">Parent elements</span></span>

|<span data-ttu-id="73e12-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="73e12-116">**Element**</span></span>|<span data-ttu-id="73e12-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="73e12-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73e12-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="73e12-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="73e12-119">取得するためのオプションが含まれています会議の情報を提案します。</span><span class="sxs-lookup"><span data-stu-id="73e12-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="73e12-120">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="73e12-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="73e12-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="73e12-121">Text value</span></span>

<span data-ttu-id="73e12-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="73e12-122">A text value is required.</span></span> <span data-ttu-id="73e12-123">整数型の値は 0 から 50 です。</span><span class="sxs-lookup"><span data-stu-id="73e12-123">The expected integer values are between 0 and 50.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="73e12-124">備考</span><span class="sxs-lookup"><span data-stu-id="73e12-124">Remarks</span></span>

<span data-ttu-id="73e12-125">[SuggestionsViewOptions](suggestionsviewoptions.md)要素を使用する場合、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="73e12-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> <span data-ttu-id="73e12-126">**GoodThreshold**要素は、どのような会議は公正と見なされますも決定します。</span><span class="sxs-lookup"><span data-stu-id="73e12-126">The **GoodThreshold** element also determines what meetings are considered Fair.</span></span> <span data-ttu-id="73e12-127">競合している参加者の割合は、以下より適切なしきい値と、50% よりも高い提案された会議の時間として修飾公平にします。</span><span class="sxs-lookup"><span data-stu-id="73e12-127">It the percentage of attendees with conflicts is less than the Good Threshold and higher than 50 percent, the suggested meeting time qualifies as Fair.</span></span> <span data-ttu-id="73e12-128">適切なしきい値を加えた 50 な公平としきい値を定義している割合に相当します。</span><span class="sxs-lookup"><span data-stu-id="73e12-128">The Good Threshold plus 50 equals the percentage that defines the Good/Fair threshold.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="73e12-129">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="73e12-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="73e12-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="73e12-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73e12-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="73e12-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="73e12-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="73e12-132">Schema Name</span></span>  <br/> |<span data-ttu-id="73e12-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="73e12-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="73e12-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="73e12-134">Validation File</span></span>  <br/> |<span data-ttu-id="73e12-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="73e12-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="73e12-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="73e12-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="73e12-137">False</span><span class="sxs-lookup"><span data-stu-id="73e12-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="73e12-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="73e12-138">See also</span></span>



[<span data-ttu-id="73e12-139">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="73e12-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="73e12-140">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="73e12-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


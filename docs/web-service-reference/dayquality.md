---
title: DayQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayQuality
api_type:
- schema
ms.assetid: cd0eb239-6e7f-4a5a-b245-659f170550b7
description: DayQuality 要素は、品質の提案された会議の時刻を格納する 1 日の品質を表します。
ms.openlocfilehash: 156d5bc58d481c9c812793da4722272ac76adaad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759943"
---
# <a name="dayquality"></a><span data-ttu-id="765a6-103">DayQuality</span><span class="sxs-lookup"><span data-stu-id="765a6-103">DayQuality</span></span>

<span data-ttu-id="765a6-104">**DayQuality**要素は、会議の提案の品質を含む、1 日の品質を表します。</span><span class="sxs-lookup"><span data-stu-id="765a6-104">The **DayQuality** element represents the quality of the day for containing quality suggested meeting times.</span></span> 
  
- [<span data-ttu-id="765a6-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="765a6-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)  
- [<span data-ttu-id="765a6-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="765a6-106">SuggestionsResponse</span></span>](suggestionsresponse.md) 
- [<span data-ttu-id="765a6-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="765a6-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)  
- [<span data-ttu-id="765a6-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="765a6-108">SuggestionDayResult</span></span>](suggestiondayresult.md) 
- [<span data-ttu-id="765a6-109">DayQuality</span><span class="sxs-lookup"><span data-stu-id="765a6-109">DayQuality</span></span>](dayquality.md)
  
```xml
<DayQuality>Excellent or Good or Fair or Poor</DayQuality>
```

<span data-ttu-id="765a6-110">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="765a6-110">**SuggestionQuality**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="765a6-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="765a6-111">Attributes and elements</span></span>

<span data-ttu-id="765a6-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="765a6-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="765a6-113">属性</span><span class="sxs-lookup"><span data-stu-id="765a6-113">Attributes</span></span>

<span data-ttu-id="765a6-114">なし。</span><span class="sxs-lookup"><span data-stu-id="765a6-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="765a6-115">子要素</span><span class="sxs-lookup"><span data-stu-id="765a6-115">Child elements</span></span>

<span data-ttu-id="765a6-116">なし。</span><span class="sxs-lookup"><span data-stu-id="765a6-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="765a6-117">親要素</span><span class="sxs-lookup"><span data-stu-id="765a6-117">Parent elements</span></span>

|<span data-ttu-id="765a6-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="765a6-118">**Element**</span></span>|<span data-ttu-id="765a6-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="765a6-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="765a6-120">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="765a6-120">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="765a6-121">推奨される会議の時刻を含む 1 つの日付を表します。</span><span class="sxs-lookup"><span data-stu-id="765a6-121">Represents a single day that contains suggested meeting times.</span></span>  <br/><br/><span data-ttu-id="765a6-122">この要素への XPath 2.0 の式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="765a6-122">The following is the XPath 2.0 expression to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="765a6-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="765a6-123">Text value</span></span>

<span data-ttu-id="765a6-124">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="765a6-124">A text value is required.</span></span> <span data-ttu-id="765a6-125">以下は、この要素の有効な値です。</span><span class="sxs-lookup"><span data-stu-id="765a6-125">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="765a6-126">**たいへん良い**</span><span class="sxs-lookup"><span data-stu-id="765a6-126">**Excellent**</span></span>   
- <span data-ttu-id="765a6-127">**よし**</span><span class="sxs-lookup"><span data-stu-id="765a6-127">**Good**</span></span>    
- <span data-ttu-id="765a6-128">**フェア**</span><span class="sxs-lookup"><span data-stu-id="765a6-128">**Fair**</span></span>    
- <span data-ttu-id="765a6-129">**低下**</span><span class="sxs-lookup"><span data-stu-id="765a6-129">**Poor**</span></span>
    
## <a name="remarks"></a><span data-ttu-id="765a6-130">備考</span><span class="sxs-lookup"><span data-stu-id="765a6-130">Remarks</span></span>

<span data-ttu-id="765a6-131">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="765a6-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="765a6-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="765a6-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="765a6-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="765a6-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="765a6-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="765a6-134">Schema Name</span></span>  <br/> |<span data-ttu-id="765a6-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="765a6-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="765a6-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="765a6-136">Validation File</span></span>  <br/> |<span data-ttu-id="765a6-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="765a6-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="765a6-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="765a6-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="765a6-139">False</span><span class="sxs-lookup"><span data-stu-id="765a6-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="765a6-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="765a6-140">See also</span></span>

- [<span data-ttu-id="765a6-141">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="765a6-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="765a6-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="765a6-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="765a6-143">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="765a6-143">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


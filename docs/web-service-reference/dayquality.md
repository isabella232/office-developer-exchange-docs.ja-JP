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
description: DayQuality 要素は、品質が推奨される会議時間を含む日の品質を表します。
ms.openlocfilehash: 41cc8313dccb1a5172fefc167e6ed90a21109ec5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455115"
---
# <a name="dayquality"></a><span data-ttu-id="f3e5b-103">DayQuality</span><span class="sxs-lookup"><span data-stu-id="f3e5b-103">DayQuality</span></span>

<span data-ttu-id="f3e5b-104">**Dayquality**要素は、品質が推奨される会議時間を含む日の品質を表します。</span><span class="sxs-lookup"><span data-stu-id="f3e5b-104">The **DayQuality** element represents the quality of the day for containing quality suggested meeting times.</span></span> 
  
- [<span data-ttu-id="f3e5b-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f3e5b-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)  
- [<span data-ttu-id="f3e5b-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="f3e5b-106">SuggestionsResponse</span></span>](suggestionsresponse.md) 
- [<span data-ttu-id="f3e5b-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="f3e5b-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)  
- [<span data-ttu-id="f3e5b-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="f3e5b-108">SuggestionDayResult</span></span>](suggestiondayresult.md) 
- [<span data-ttu-id="f3e5b-109">DayQuality</span><span class="sxs-lookup"><span data-stu-id="f3e5b-109">DayQuality</span></span>](dayquality.md)
  
```xml
<DayQuality>Excellent or Good or Fair or Poor</DayQuality>
```

<span data-ttu-id="f3e5b-110">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="f3e5b-110">**SuggestionQuality**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f3e5b-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f3e5b-111">Attributes and elements</span></span>

<span data-ttu-id="f3e5b-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f3e5b-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3e5b-113">属性</span><span class="sxs-lookup"><span data-stu-id="f3e5b-113">Attributes</span></span>

<span data-ttu-id="f3e5b-114">なし。</span><span class="sxs-lookup"><span data-stu-id="f3e5b-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3e5b-115">子要素</span><span class="sxs-lookup"><span data-stu-id="f3e5b-115">Child elements</span></span>

<span data-ttu-id="f3e5b-116">なし。</span><span class="sxs-lookup"><span data-stu-id="f3e5b-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f3e5b-117">親要素</span><span class="sxs-lookup"><span data-stu-id="f3e5b-117">Parent elements</span></span>

|<span data-ttu-id="f3e5b-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="f3e5b-118">**Element**</span></span>|<span data-ttu-id="f3e5b-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="f3e5b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3e5b-120">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="f3e5b-120">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="f3e5b-121">提案された会議時間を含む1つの日を表します。</span><span class="sxs-lookup"><span data-stu-id="f3e5b-121">Represents a single day that contains suggested meeting times.</span></span>  <br/><br/><span data-ttu-id="f3e5b-122">この要素の XPath 2.0 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f3e5b-122">The following is the XPath 2.0 expression to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f3e5b-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f3e5b-123">Text value</span></span>

<span data-ttu-id="f3e5b-124">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="f3e5b-124">A text value is required.</span></span> <span data-ttu-id="f3e5b-125">この要素に使用できる値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="f3e5b-125">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="f3e5b-126">**優秀**</span><span class="sxs-lookup"><span data-stu-id="f3e5b-126">**Excellent**</span></span>   
- <span data-ttu-id="f3e5b-127">**標準**</span><span class="sxs-lookup"><span data-stu-id="f3e5b-127">**Good**</span></span>    
- <span data-ttu-id="f3e5b-128">**かなり**</span><span class="sxs-lookup"><span data-stu-id="f3e5b-128">**Fair**</span></span>    
- <span data-ttu-id="f3e5b-129">**悪い**</span><span class="sxs-lookup"><span data-stu-id="f3e5b-129">**Poor**</span></span>
    
## <a name="remarks"></a><span data-ttu-id="f3e5b-130">注釈</span><span class="sxs-lookup"><span data-stu-id="f3e5b-130">Remarks</span></span>

<span data-ttu-id="f3e5b-131">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f3e5b-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3e5b-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f3e5b-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3e5b-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="f3e5b-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f3e5b-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f3e5b-134">Schema Name</span></span>  <br/> |<span data-ttu-id="f3e5b-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f3e5b-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="f3e5b-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f3e5b-136">Validation File</span></span>  <br/> |<span data-ttu-id="f3e5b-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f3e5b-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f3e5b-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f3e5b-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="f3e5b-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="f3e5b-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f3e5b-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="f3e5b-140">See also</span></span>

- [<span data-ttu-id="f3e5b-141">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="f3e5b-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="f3e5b-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f3e5b-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="f3e5b-143">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="f3e5b-143">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


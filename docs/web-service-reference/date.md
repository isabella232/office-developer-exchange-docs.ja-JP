---
title: 日付
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Date
api_type:
- schema
ms.assetid: 2f6bc090-fff4-45b1-8d7e-8fd6e060cce2
description: Date 要素は、提案された会議時間を含む日付を表します。
ms.openlocfilehash: bcc152ed6aba94907189b5579b998815be45db16
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44443789"
---
# <a name="date"></a><span data-ttu-id="f0b4d-103">日付</span><span class="sxs-lookup"><span data-stu-id="f0b4d-103">Date</span></span>

<span data-ttu-id="f0b4d-104">**Date**要素は、提案された会議時間を含む日付を表します。</span><span class="sxs-lookup"><span data-stu-id="f0b4d-104">The **Date** element represents the date that contains the suggested meeting times.</span></span> 
  
- [<span data-ttu-id="f0b4d-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f0b4d-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) 
- [<span data-ttu-id="f0b4d-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="f0b4d-106">SuggestionsResponse</span></span>](suggestionsresponse.md) 
- [<span data-ttu-id="f0b4d-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="f0b4d-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)  
- [<span data-ttu-id="f0b4d-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="f0b4d-108">SuggestionDayResult</span></span>](suggestiondayresult.md)  
- [<span data-ttu-id="f0b4d-109">Date</span><span class="sxs-lookup"><span data-stu-id="f0b4d-109">Date</span></span>](date.md)
  
```xml
<Date>...</Date>
```

<span data-ttu-id="f0b4d-110">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="f0b4d-110">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f0b4d-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f0b4d-111">Attributes and elements</span></span>

<span data-ttu-id="f0b4d-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f0b4d-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0b4d-113">属性</span><span class="sxs-lookup"><span data-stu-id="f0b4d-113">Attributes</span></span>

<span data-ttu-id="f0b4d-114">なし。</span><span class="sxs-lookup"><span data-stu-id="f0b4d-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f0b4d-115">子要素</span><span class="sxs-lookup"><span data-stu-id="f0b4d-115">Child elements</span></span>

<span data-ttu-id="f0b4d-116">なし。</span><span class="sxs-lookup"><span data-stu-id="f0b4d-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f0b4d-117">親要素</span><span class="sxs-lookup"><span data-stu-id="f0b4d-117">Parent elements</span></span>

|<span data-ttu-id="f0b4d-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="f0b4d-118">**Element**</span></span>|<span data-ttu-id="f0b4d-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="f0b4d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0b4d-120">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="f0b4d-120">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="f0b4d-121">提案された会議時間を含む1つの日を表します。</span><span class="sxs-lookup"><span data-stu-id="f0b4d-121">Represents a single day that contains suggested meeting times.</span></span>  <br/><br/><span data-ttu-id="f0b4d-122">この要素の XPath 2.0 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f0b4d-122">The following is the XPath 2.0 expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f0b4d-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f0b4d-123">Text value</span></span>

<span data-ttu-id="f0b4d-124">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="f0b4d-124">A text value is required.</span></span> <span data-ttu-id="f0b4d-125">DateTime プリミティブ型の形式については、「World Wide Web コンソーシアム (W3C) スキーマデータ型に関する推奨事項」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0b4d-125">Review the World Wide Web Consortium (W3C) schema datatype recommendations for the format of the dateTime primitive datatype.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f0b4d-126">注釈</span><span class="sxs-lookup"><span data-stu-id="f0b4d-126">Remarks</span></span>

<span data-ttu-id="f0b4d-127">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f0b4d-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0b4d-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f0b4d-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0b4d-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="f0b4d-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f0b4d-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f0b4d-130">Schema Name</span></span>  <br/> |<span data-ttu-id="f0b4d-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f0b4d-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="f0b4d-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f0b4d-132">Validation File</span></span>  <br/> |<span data-ttu-id="f0b4d-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f0b4d-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f0b4d-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f0b4d-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="f0b4d-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="f0b4d-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0b4d-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="f0b4d-136">See also</span></span>

- [<span data-ttu-id="f0b4d-137">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="f0b4d-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md) 
- [<span data-ttu-id="f0b4d-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f0b4d-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="f0b4d-139">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="f0b4d-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


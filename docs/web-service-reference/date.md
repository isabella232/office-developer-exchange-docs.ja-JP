---
title: Date
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
description: Date 要素では、提案された会議の時間を含む日付を表します。
ms.openlocfilehash: 98dc9d6c599222c819b2c9ed1bacd05758ae1655
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759911"
---
# <a name="date"></a><span data-ttu-id="1691b-103">Date</span><span class="sxs-lookup"><span data-stu-id="1691b-103">Date</span></span>

<span data-ttu-id="1691b-104">**Date**要素では、提案された会議の時間を含む日付を表します。</span><span class="sxs-lookup"><span data-stu-id="1691b-104">The **Date** element represents the date that contains the suggested meeting times.</span></span> 
  
- [<span data-ttu-id="1691b-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1691b-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) 
- [<span data-ttu-id="1691b-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="1691b-106">SuggestionsResponse</span></span>](suggestionsresponse.md) 
- [<span data-ttu-id="1691b-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="1691b-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)  
- [<span data-ttu-id="1691b-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="1691b-108">SuggestionDayResult</span></span>](suggestiondayresult.md)  
- [<span data-ttu-id="1691b-109">日付</span><span class="sxs-lookup"><span data-stu-id="1691b-109">Date</span></span>](date.md)
  
```xml
<Date>...</Date>
```

<span data-ttu-id="1691b-110">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="1691b-110">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1691b-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1691b-111">Attributes and elements</span></span>

<span data-ttu-id="1691b-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1691b-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1691b-113">属性</span><span class="sxs-lookup"><span data-stu-id="1691b-113">Attributes</span></span>

<span data-ttu-id="1691b-114">なし。</span><span class="sxs-lookup"><span data-stu-id="1691b-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1691b-115">子要素</span><span class="sxs-lookup"><span data-stu-id="1691b-115">Child elements</span></span>

<span data-ttu-id="1691b-116">なし。</span><span class="sxs-lookup"><span data-stu-id="1691b-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1691b-117">親要素</span><span class="sxs-lookup"><span data-stu-id="1691b-117">Parent elements</span></span>

|<span data-ttu-id="1691b-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="1691b-118">**Element**</span></span>|<span data-ttu-id="1691b-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="1691b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1691b-120">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="1691b-120">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="1691b-121">推奨される会議の時刻を含む 1 つの日付を表します。</span><span class="sxs-lookup"><span data-stu-id="1691b-121">Represents a single day that contains suggested meeting times.</span></span>  <br/><br/><span data-ttu-id="1691b-122">この要素への XPath 2.0 の式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="1691b-122">The following is the XPath 2.0 expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1691b-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1691b-123">Text value</span></span>

<span data-ttu-id="1691b-124">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="1691b-124">A text value is required.</span></span> <span data-ttu-id="1691b-125">World Wide Web コンソーシアム (W3C) スキーマのデータ型に関する推奨事項形式の dateTime のプリミティブ データ型を確認します。</span><span class="sxs-lookup"><span data-stu-id="1691b-125">Review the World Wide Web Consortium (W3C) schema datatype recommendations for the format of the dateTime primitive datatype.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1691b-126">備考</span><span class="sxs-lookup"><span data-stu-id="1691b-126">Remarks</span></span>

<span data-ttu-id="1691b-127">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="1691b-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1691b-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="1691b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1691b-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="1691b-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1691b-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1691b-130">Schema Name</span></span>  <br/> |<span data-ttu-id="1691b-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1691b-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="1691b-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1691b-132">Validation File</span></span>  <br/> |<span data-ttu-id="1691b-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1691b-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1691b-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1691b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="1691b-135">False</span><span class="sxs-lookup"><span data-stu-id="1691b-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1691b-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="1691b-136">See also</span></span>

- [<span data-ttu-id="1691b-137">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="1691b-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md) 
- [<span data-ttu-id="1691b-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1691b-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="1691b-139">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="1691b-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


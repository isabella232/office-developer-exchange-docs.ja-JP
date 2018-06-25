---
title: SuggestionDayResultArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionDayResultArray
api_type:
- schema
ms.assetid: eeba9eff-5eca-4002-b5a5-8fb794feaba1
description: SuggestionDayResultArray 要素には、会議の提案の日付順の配列が含まれています。
ms.openlocfilehash: c208104356606a5d9961461ad8743a772d2410d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839625"
---
# <a name="suggestiondayresultarray"></a><span data-ttu-id="e5db3-103">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="e5db3-103">SuggestionDayResultArray</span></span>

<span data-ttu-id="e5db3-104">**SuggestionDayResultArray**要素には、会議の提案の日付順の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e5db3-104">The **SuggestionDayResultArray** element contains an array of meeting suggestions organized by date.</span></span> 
  
[<span data-ttu-id="e5db3-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e5db3-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="e5db3-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="e5db3-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="e5db3-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="e5db3-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
```xml
<SuggestionDayResultArray>
   <SuggestionDayResult>...</SuggestionDayResult>
</SuggestionDayResultArray>
```

 <span data-ttu-id="e5db3-108">**ArrayOfSuggestionDayResult**</span><span class="sxs-lookup"><span data-stu-id="e5db3-108">**ArrayOfSuggestionDayResult**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e5db3-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e5db3-109">Attributes and elements</span></span>

<span data-ttu-id="e5db3-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e5db3-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e5db3-111">属性</span><span class="sxs-lookup"><span data-stu-id="e5db3-111">Attributes</span></span>

<span data-ttu-id="e5db3-112">なし。</span><span class="sxs-lookup"><span data-stu-id="e5db3-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e5db3-113">子要素</span><span class="sxs-lookup"><span data-stu-id="e5db3-113">Child elements</span></span>

|<span data-ttu-id="e5db3-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="e5db3-114">**Element**</span></span>|<span data-ttu-id="e5db3-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="e5db3-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5db3-116">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="e5db3-116">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="e5db3-117">推奨される会議の時刻を含む 1 つの日付を表します。</span><span class="sxs-lookup"><span data-stu-id="e5db3-117">Represents a single day that contains suggested meeting times.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e5db3-118">親要素</span><span class="sxs-lookup"><span data-stu-id="e5db3-118">Parent elements</span></span>

|<span data-ttu-id="e5db3-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="e5db3-119">**Element**</span></span>|<span data-ttu-id="e5db3-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="e5db3-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5db3-121">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="e5db3-121">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="e5db3-122">会議の提案の要求の応答の情報と提案のデータが含まれています</span><span class="sxs-lookup"><span data-stu-id="e5db3-122">Contains response information and suggestion data for requested meeting suggestions</span></span>  <br/> <span data-ttu-id="e5db3-123">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="e5db3-123">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e5db3-124">備考</span><span class="sxs-lookup"><span data-stu-id="e5db3-124">Remarks</span></span>

<span data-ttu-id="e5db3-125">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="e5db3-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e5db3-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="e5db3-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e5db3-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="e5db3-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e5db3-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e5db3-128">Schema Name</span></span>  <br/> |<span data-ttu-id="e5db3-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e5db3-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e5db3-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e5db3-130">Validation File</span></span>  <br/> |<span data-ttu-id="e5db3-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e5db3-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e5db3-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e5db3-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="e5db3-133">False</span><span class="sxs-lookup"><span data-stu-id="e5db3-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e5db3-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="e5db3-134">See also</span></span>



[<span data-ttu-id="e5db3-135">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="e5db3-135">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="e5db3-136">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e5db3-136">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="e5db3-137">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="e5db3-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


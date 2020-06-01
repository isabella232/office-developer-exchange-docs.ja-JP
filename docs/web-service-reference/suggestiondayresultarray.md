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
description: SuggestionDayResultArray 要素には、日付で整理された会議提案の配列が含まれています。
ms.openlocfilehash: 277d4cf71c31aba26cbff6f598eaa62769cae552
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457985"
---
# <a name="suggestiondayresultarray"></a><span data-ttu-id="cc6d4-103">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="cc6d4-103">SuggestionDayResultArray</span></span>

<span data-ttu-id="cc6d4-104">**SuggestionDayResultArray**要素には、日付で整理された会議提案の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cc6d4-104">The **SuggestionDayResultArray** element contains an array of meeting suggestions organized by date.</span></span> 
  
[<span data-ttu-id="cc6d4-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="cc6d4-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="cc6d4-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="cc6d4-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="cc6d4-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="cc6d4-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
```xml
<SuggestionDayResultArray>
   <SuggestionDayResult>...</SuggestionDayResult>
</SuggestionDayResultArray>
```

 <span data-ttu-id="cc6d4-108">**ArrayOfSuggestionDayResult**</span><span class="sxs-lookup"><span data-stu-id="cc6d4-108">**ArrayOfSuggestionDayResult**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cc6d4-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cc6d4-109">Attributes and elements</span></span>

<span data-ttu-id="cc6d4-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cc6d4-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc6d4-111">属性</span><span class="sxs-lookup"><span data-stu-id="cc6d4-111">Attributes</span></span>

<span data-ttu-id="cc6d4-112">なし。</span><span class="sxs-lookup"><span data-stu-id="cc6d4-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc6d4-113">子要素</span><span class="sxs-lookup"><span data-stu-id="cc6d4-113">Child elements</span></span>

|<span data-ttu-id="cc6d4-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="cc6d4-114">**Element**</span></span>|<span data-ttu-id="cc6d4-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="cc6d4-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc6d4-116">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="cc6d4-116">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="cc6d4-117">提案された会議時間を含む1つの日を表します。</span><span class="sxs-lookup"><span data-stu-id="cc6d4-117">Represents a single day that contains suggested meeting times.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cc6d4-118">親要素</span><span class="sxs-lookup"><span data-stu-id="cc6d4-118">Parent elements</span></span>

|<span data-ttu-id="cc6d4-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="cc6d4-119">**Element**</span></span>|<span data-ttu-id="cc6d4-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="cc6d4-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc6d4-121">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="cc6d4-121">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="cc6d4-122">要求された会議提案の応答情報と提案データが含まれています</span><span class="sxs-lookup"><span data-stu-id="cc6d4-122">Contains response information and suggestion data for requested meeting suggestions</span></span>  <br/> <span data-ttu-id="cc6d4-123">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cc6d4-123">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cc6d4-124">注釈</span><span class="sxs-lookup"><span data-stu-id="cc6d4-124">Remarks</span></span>

<span data-ttu-id="cc6d4-125">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="cc6d4-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cc6d4-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cc6d4-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc6d4-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="cc6d4-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cc6d4-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cc6d4-128">Schema Name</span></span>  <br/> |<span data-ttu-id="cc6d4-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="cc6d4-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cc6d4-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cc6d4-130">Validation File</span></span>  <br/> |<span data-ttu-id="cc6d4-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="cc6d4-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cc6d4-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cc6d4-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="cc6d4-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="cc6d4-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cc6d4-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="cc6d4-134">See also</span></span>



[<span data-ttu-id="cc6d4-135">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="cc6d4-135">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="cc6d4-136">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="cc6d4-136">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="cc6d4-137">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="cc6d4-137">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


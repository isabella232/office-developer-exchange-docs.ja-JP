---
title: SuggestionsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionsResponse
api_type:
- schema
ms.assetid: d25ca143-f80c-4458-b669-346fda29a5a7
description: SuggestionsResponse 要素には、要求された会議に関する推奨事項についての応答のステータス情報と提案のデータが含まれています。
ms.openlocfilehash: 614b58a1df8e340c6be468ccddd3b37537d32591
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839626"
---
# <a name="suggestionsresponse"></a><span data-ttu-id="4828a-103">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="4828a-103">SuggestionsResponse</span></span>

<span data-ttu-id="4828a-104">**SuggestionsResponse**要素には、要求された会議に関する推奨事項についての応答のステータス情報と提案のデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4828a-104">The **SuggestionsResponse** element contains response status information and suggestion data for requested meeting suggestions.</span></span> 
  
[<span data-ttu-id="4828a-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="4828a-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="4828a-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="4828a-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
```xml
<SuggestionsResponse>
   <ResponseMessage>...</ResponseMessage>
   <SuggestionDayResultArray>...</SuggestionDayResultArray>
</SuggestionsResponse>
```

 <span data-ttu-id="4828a-107">**SuggestionsResponseType**</span><span class="sxs-lookup"><span data-stu-id="4828a-107">**SuggestionsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4828a-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4828a-108">Attributes and elements</span></span>

<span data-ttu-id="4828a-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4828a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4828a-110">属性</span><span class="sxs-lookup"><span data-stu-id="4828a-110">Attributes</span></span>

<span data-ttu-id="4828a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4828a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4828a-112">子要素</span><span class="sxs-lookup"><span data-stu-id="4828a-112">Child elements</span></span>

|<span data-ttu-id="4828a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4828a-113">**Element**</span></span>|<span data-ttu-id="4828a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4828a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4828a-115">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4828a-115">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="4828a-116">応答ステータスに関する説明情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="4828a-116">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="4828a-117">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="4828a-117">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md) <br/> |<span data-ttu-id="4828a-118">会議の提案の日付順の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4828a-118">Contains an array of meeting suggestions organized by date.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4828a-119">親要素</span><span class="sxs-lookup"><span data-stu-id="4828a-119">Parent elements</span></span>

|<span data-ttu-id="4828a-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="4828a-120">**Element**</span></span>|<span data-ttu-id="4828a-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="4828a-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4828a-122">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="4828a-122">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) <br/> |<span data-ttu-id="4828a-123">要求されたユーザーの利用可能時間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4828a-123">Contains the requested users' availability information.</span></span>  <br/> <span data-ttu-id="4828a-124">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="4828a-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4828a-125">備考</span><span class="sxs-lookup"><span data-stu-id="4828a-125">Remarks</span></span>

<span data-ttu-id="4828a-126">[SuggestionsViewOptions](suggestionsviewoptions.md)は、GetUserAvailability 要求メッセージに設定されていない場合、この要素は GetUserAvailability の応答に含まれません。</span><span class="sxs-lookup"><span data-stu-id="4828a-126">This element is not included in a GetUserAvailability response if [SuggestionsViewOptions](suggestionsviewoptions.md) is not set in the GetUserAvailability request message.</span></span> 
  
<span data-ttu-id="4828a-127">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="4828a-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4828a-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="4828a-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4828a-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="4828a-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4828a-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4828a-130">Schema Name</span></span>  <br/> |<span data-ttu-id="4828a-131">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="4828a-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4828a-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4828a-132">Validation File</span></span>  <br/> |<span data-ttu-id="4828a-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4828a-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4828a-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4828a-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="4828a-135">False</span><span class="sxs-lookup"><span data-stu-id="4828a-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4828a-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="4828a-136">See also</span></span>



[<span data-ttu-id="4828a-137">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="4828a-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="4828a-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="4828a-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="4828a-139">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="4828a-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


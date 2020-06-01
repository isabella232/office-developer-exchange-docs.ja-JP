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
description: SuggestionsResponse 要素には、要求された会議の提案の応答状態情報と提案データが含まれています。
ms.openlocfilehash: cba344f3f97777580c2cc6d296f110f20b550063
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466655"
---
# <a name="suggestionsresponse"></a><span data-ttu-id="f2738-103">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="f2738-103">SuggestionsResponse</span></span>

<span data-ttu-id="f2738-104">**SuggestionsResponse**要素には、要求された会議の提案の応答状態情報と提案データが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f2738-104">The **SuggestionsResponse** element contains response status information and suggestion data for requested meeting suggestions.</span></span> 
  
[<span data-ttu-id="f2738-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f2738-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="f2738-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="f2738-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
```xml
<SuggestionsResponse>
   <ResponseMessage>...</ResponseMessage>
   <SuggestionDayResultArray>...</SuggestionDayResultArray>
</SuggestionsResponse>
```

 <span data-ttu-id="f2738-107">**SuggestionsResponseType**</span><span class="sxs-lookup"><span data-stu-id="f2738-107">**SuggestionsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2738-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f2738-108">Attributes and elements</span></span>

<span data-ttu-id="f2738-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f2738-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2738-110">属性</span><span class="sxs-lookup"><span data-stu-id="f2738-110">Attributes</span></span>

<span data-ttu-id="f2738-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f2738-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2738-112">子要素</span><span class="sxs-lookup"><span data-stu-id="f2738-112">Child elements</span></span>

|<span data-ttu-id="f2738-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="f2738-113">**Element**</span></span>|<span data-ttu-id="f2738-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f2738-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2738-115">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f2738-115">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="f2738-116">応答状態に関する説明情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="f2738-116">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="f2738-117">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="f2738-117">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md) <br/> |<span data-ttu-id="f2738-118">会議提案の配列が日付別に整理されています。</span><span class="sxs-lookup"><span data-stu-id="f2738-118">Contains an array of meeting suggestions organized by date.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f2738-119">親要素</span><span class="sxs-lookup"><span data-stu-id="f2738-119">Parent elements</span></span>

|<span data-ttu-id="f2738-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="f2738-120">**Element**</span></span>|<span data-ttu-id="f2738-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="f2738-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2738-122">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f2738-122">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) <br/> |<span data-ttu-id="f2738-123">要求されたユーザーの空き時間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f2738-123">Contains the requested users' availability information.</span></span>  <br/> <span data-ttu-id="f2738-124">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f2738-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f2738-125">注釈</span><span class="sxs-lookup"><span data-stu-id="f2738-125">Remarks</span></span>

<span data-ttu-id="f2738-126">この要素は、 [SuggestionsViewOptions](suggestionsviewoptions.md)が getuseravailability 要求メッセージに設定されていない場合は、getuseravailability 応答に含まれません。</span><span class="sxs-lookup"><span data-stu-id="f2738-126">This element is not included in a GetUserAvailability response if [SuggestionsViewOptions](suggestionsviewoptions.md) is not set in the GetUserAvailability request message.</span></span> 
  
<span data-ttu-id="f2738-127">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f2738-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2738-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f2738-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2738-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="f2738-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f2738-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f2738-130">Schema Name</span></span>  <br/> |<span data-ttu-id="f2738-131">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="f2738-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f2738-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f2738-132">Validation File</span></span>  <br/> |<span data-ttu-id="f2738-133">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="f2738-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f2738-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f2738-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="f2738-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="f2738-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2738-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="f2738-136">See also</span></span>



[<span data-ttu-id="f2738-137">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="f2738-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="f2738-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f2738-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="f2738-139">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="f2738-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


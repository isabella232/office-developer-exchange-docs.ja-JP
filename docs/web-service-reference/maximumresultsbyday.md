---
title: MaximumResultsByDay
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaximumResultsByDay
api_type:
- schema
ms.assetid: d581a12a-2b8e-4960-ae14-c8c4aa0b1849
description: MaximumResultsByDay 要素は、応答で返される1日あたりの推奨会議時間数を指定します。
ms.openlocfilehash: 46d5c35a83034b8b968901fbc4ee57d046b6c164
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468419"
---
# <a name="maximumresultsbyday"></a><span data-ttu-id="709bc-103">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="709bc-103">MaximumResultsByDay</span></span>

<span data-ttu-id="709bc-104">**Maximumresultsbyday**要素は、応答で返される1日あたりの推奨会議時間数を指定します。</span><span class="sxs-lookup"><span data-stu-id="709bc-104">The **MaximumResultsByDay** element specifies the number of suggested meeting times per a day returned in the response.</span></span> 
  
[<span data-ttu-id="709bc-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="709bc-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="709bc-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="709bc-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="709bc-107">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="709bc-107">MaximumResultsByDay</span></span>](maximumresultsbyday.md)
  
```xml
<MaximumResultsByDay>...</MaximumResultsByDay>
```

<span data-ttu-id="709bc-108">**int**</span><span class="sxs-lookup"><span data-stu-id="709bc-108">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="709bc-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="709bc-109">Attributes and elements</span></span>

<span data-ttu-id="709bc-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="709bc-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="709bc-111">属性</span><span class="sxs-lookup"><span data-stu-id="709bc-111">Attributes</span></span>

<span data-ttu-id="709bc-112">なし。</span><span class="sxs-lookup"><span data-stu-id="709bc-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="709bc-113">子要素</span><span class="sxs-lookup"><span data-stu-id="709bc-113">Child elements</span></span>

<span data-ttu-id="709bc-114">なし。</span><span class="sxs-lookup"><span data-stu-id="709bc-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="709bc-115">親要素</span><span class="sxs-lookup"><span data-stu-id="709bc-115">Parent elements</span></span>

|<span data-ttu-id="709bc-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="709bc-116">**Element**</span></span>|<span data-ttu-id="709bc-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="709bc-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="709bc-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="709bc-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="709bc-119">会議提案情報を取得するためのオプションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="709bc-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="709bc-120">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="709bc-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="709bc-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="709bc-121">Text value</span></span>

<span data-ttu-id="709bc-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="709bc-122">A text value is required.</span></span> <span data-ttu-id="709bc-123">テキスト値は、整数を表します。</span><span class="sxs-lookup"><span data-stu-id="709bc-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="709bc-124">注釈</span><span class="sxs-lookup"><span data-stu-id="709bc-124">Remarks</span></span>

<span data-ttu-id="709bc-125">この要素は、 [SuggestionsViewOptions](suggestionsviewoptions.md)要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="709bc-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="709bc-126">この要素を記述するスキーマは、Microsoft® Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="709bc-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="709bc-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="709bc-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="709bc-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="709bc-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="709bc-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="709bc-129">Schema Name</span></span>  <br/> |<span data-ttu-id="709bc-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="709bc-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="709bc-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="709bc-131">Validation File</span></span>  <br/> |<span data-ttu-id="709bc-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="709bc-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="709bc-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="709bc-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="709bc-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="709bc-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="709bc-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="709bc-135">See also</span></span>

- [<span data-ttu-id="709bc-136">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="709bc-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="709bc-137">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="709bc-137">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


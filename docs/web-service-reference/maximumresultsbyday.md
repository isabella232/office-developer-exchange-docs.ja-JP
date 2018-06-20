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
description: MaximumResultsByDay 要素は、応答で返される 1 日あたりの推奨される会議の時刻の数を指定します。
ms.openlocfilehash: 69ab4e0b23f85e5b8786ba2dd934850cadc88f0e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832381"
---
# <a name="maximumresultsbyday"></a><span data-ttu-id="4dc54-103">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="4dc54-103">MaximumResultsByDay</span></span>

<span data-ttu-id="4dc54-104">**MaximumResultsByDay**要素は、応答で返される 1 日あたりの推奨される会議の時刻の数を指定します。</span><span class="sxs-lookup"><span data-stu-id="4dc54-104">The **MaximumResultsByDay** element specifies the number of suggested meeting times per a day returned in the response.</span></span> 
  
[<span data-ttu-id="4dc54-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="4dc54-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="4dc54-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="4dc54-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="4dc54-107">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="4dc54-107">MaximumResultsByDay</span></span>](maximumresultsbyday.md)
  
```xml
<MaximumResultsByDay>...</MaximumResultsByDay>
```

<span data-ttu-id="4dc54-108">**int**</span><span class="sxs-lookup"><span data-stu-id="4dc54-108">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4dc54-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4dc54-109">Attributes and elements</span></span>

<span data-ttu-id="4dc54-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4dc54-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4dc54-111">属性</span><span class="sxs-lookup"><span data-stu-id="4dc54-111">Attributes</span></span>

<span data-ttu-id="4dc54-112">なし。</span><span class="sxs-lookup"><span data-stu-id="4dc54-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4dc54-113">子要素</span><span class="sxs-lookup"><span data-stu-id="4dc54-113">Child elements</span></span>

<span data-ttu-id="4dc54-114">なし。</span><span class="sxs-lookup"><span data-stu-id="4dc54-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4dc54-115">親要素</span><span class="sxs-lookup"><span data-stu-id="4dc54-115">Parent elements</span></span>

|<span data-ttu-id="4dc54-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="4dc54-116">**Element**</span></span>|<span data-ttu-id="4dc54-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="4dc54-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4dc54-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="4dc54-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="4dc54-119">取得するためのオプションが含まれています会議の情報を提案します。</span><span class="sxs-lookup"><span data-stu-id="4dc54-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="4dc54-120">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="4dc54-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4dc54-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4dc54-121">Text value</span></span>

<span data-ttu-id="4dc54-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="4dc54-122">A text value is required.</span></span> <span data-ttu-id="4dc54-123">テキスト値は、整数を表します。</span><span class="sxs-lookup"><span data-stu-id="4dc54-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4dc54-124">備考</span><span class="sxs-lookup"><span data-stu-id="4dc54-124">Remarks</span></span>

<span data-ttu-id="4dc54-125">[SuggestionsViewOptions](suggestionsviewoptions.md)要素を使用する場合、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="4dc54-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="4dc54-126">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft® Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="4dc54-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="4dc54-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="4dc54-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4dc54-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="4dc54-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4dc54-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4dc54-129">Schema Name</span></span>  <br/> |<span data-ttu-id="4dc54-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4dc54-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="4dc54-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4dc54-131">Validation File</span></span>  <br/> |<span data-ttu-id="4dc54-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4dc54-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4dc54-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4dc54-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="4dc54-134">False</span><span class="sxs-lookup"><span data-stu-id="4dc54-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4dc54-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="4dc54-135">See also</span></span>

- [<span data-ttu-id="4dc54-136">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="4dc54-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="4dc54-137">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="4dc54-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


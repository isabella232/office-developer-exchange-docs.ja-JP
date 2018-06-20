---
title: MeetingDurationInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingDurationInMinutes
api_type:
- schema
ms.assetid: bb86b275-9c29-4daf-8196-8d505b87a4f4
description: MeetingDurationInMinutes 要素は、提案された会議の期間を指定します。
ms.openlocfilehash: 2ff60b69fb352c2ac7316f1ca231bb04da67ead2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832433"
---
# <a name="meetingdurationinminutes"></a><span data-ttu-id="b8163-103">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="b8163-103">MeetingDurationInMinutes</span></span>

<span data-ttu-id="b8163-104">**MeetingDurationInMinutes**要素は、提案された会議の期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="b8163-104">The **MeetingDurationInMinutes** element specifies the duration of the meeting to be suggested.</span></span> 
  
[<span data-ttu-id="b8163-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="b8163-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="b8163-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="b8163-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="b8163-107">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="b8163-107">MeetingDurationInMinutes</span></span>](meetingdurationinminutes.md)
  
```xml
<MeetingDurationInMinutes>...</MeetingDurationInMinutes>
```

 <span data-ttu-id="b8163-108">**int**</span><span class="sxs-lookup"><span data-stu-id="b8163-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b8163-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b8163-109">Attributes and elements</span></span>

<span data-ttu-id="b8163-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b8163-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8163-111">属性</span><span class="sxs-lookup"><span data-stu-id="b8163-111">Attributes</span></span>

<span data-ttu-id="b8163-112">なし。</span><span class="sxs-lookup"><span data-stu-id="b8163-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8163-113">子要素</span><span class="sxs-lookup"><span data-stu-id="b8163-113">Child elements</span></span>

<span data-ttu-id="b8163-114">なし。</span><span class="sxs-lookup"><span data-stu-id="b8163-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b8163-115">親要素</span><span class="sxs-lookup"><span data-stu-id="b8163-115">Parent elements</span></span>

|<span data-ttu-id="b8163-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="b8163-116">**Element**</span></span>|<span data-ttu-id="b8163-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="b8163-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8163-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="b8163-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="b8163-119">取得するためのオプションが含まれています会議の情報を提案します。</span><span class="sxs-lookup"><span data-stu-id="b8163-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="b8163-120">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="b8163-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b8163-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b8163-121">Text value</span></span>

<span data-ttu-id="b8163-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="b8163-122">A text value is required.</span></span> <span data-ttu-id="b8163-123">テキスト値は、整数を表します。</span><span class="sxs-lookup"><span data-stu-id="b8163-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b8163-124">備考</span><span class="sxs-lookup"><span data-stu-id="b8163-124">Remarks</span></span>

<span data-ttu-id="b8163-125">[SuggestionsViewOptions](suggestionsviewoptions.md)要素を使用する場合、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="b8163-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b8163-126">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="b8163-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="b8163-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="b8163-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8163-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="b8163-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b8163-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b8163-129">Schema Name</span></span>  <br/> |<span data-ttu-id="b8163-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b8163-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="b8163-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b8163-131">Validation File</span></span>  <br/> |<span data-ttu-id="b8163-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b8163-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b8163-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b8163-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="b8163-134">False</span><span class="sxs-lookup"><span data-stu-id="b8163-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b8163-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="b8163-135">See also</span></span>



[<span data-ttu-id="b8163-136">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="b8163-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="b8163-137">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="b8163-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


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
description: MeetingDurationInMinutes 要素は、提案される会議の期間を指定します。
ms.openlocfilehash: b41e234be40c2ad8b28047ae2e812edfd66af644
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467488"
---
# <a name="meetingdurationinminutes"></a><span data-ttu-id="3cec7-103">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="3cec7-103">MeetingDurationInMinutes</span></span>

<span data-ttu-id="3cec7-104">**MeetingDurationInMinutes**要素は、提案される会議の期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="3cec7-104">The **MeetingDurationInMinutes** element specifies the duration of the meeting to be suggested.</span></span> 
  
[<span data-ttu-id="3cec7-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="3cec7-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="3cec7-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="3cec7-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="3cec7-107">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="3cec7-107">MeetingDurationInMinutes</span></span>](meetingdurationinminutes.md)
  
```xml
<MeetingDurationInMinutes>...</MeetingDurationInMinutes>
```

 <span data-ttu-id="3cec7-108">**int**</span><span class="sxs-lookup"><span data-stu-id="3cec7-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3cec7-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3cec7-109">Attributes and elements</span></span>

<span data-ttu-id="3cec7-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3cec7-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3cec7-111">属性</span><span class="sxs-lookup"><span data-stu-id="3cec7-111">Attributes</span></span>

<span data-ttu-id="3cec7-112">なし。</span><span class="sxs-lookup"><span data-stu-id="3cec7-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3cec7-113">子要素</span><span class="sxs-lookup"><span data-stu-id="3cec7-113">Child elements</span></span>

<span data-ttu-id="3cec7-114">なし。</span><span class="sxs-lookup"><span data-stu-id="3cec7-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3cec7-115">親要素</span><span class="sxs-lookup"><span data-stu-id="3cec7-115">Parent elements</span></span>

|<span data-ttu-id="3cec7-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="3cec7-116">**Element**</span></span>|<span data-ttu-id="3cec7-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="3cec7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3cec7-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="3cec7-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="3cec7-119">会議提案情報を取得するためのオプションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3cec7-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="3cec7-120">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3cec7-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3cec7-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3cec7-121">Text value</span></span>

<span data-ttu-id="3cec7-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="3cec7-122">A text value is required.</span></span> <span data-ttu-id="3cec7-123">テキスト値は、整数を表します。</span><span class="sxs-lookup"><span data-stu-id="3cec7-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3cec7-124">注釈</span><span class="sxs-lookup"><span data-stu-id="3cec7-124">Remarks</span></span>

<span data-ttu-id="3cec7-125">この要素は、 [SuggestionsViewOptions](suggestionsviewoptions.md)要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="3cec7-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="3cec7-126">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="3cec7-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="3cec7-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3cec7-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3cec7-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="3cec7-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3cec7-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3cec7-129">Schema Name</span></span>  <br/> |<span data-ttu-id="3cec7-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="3cec7-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="3cec7-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3cec7-131">Validation File</span></span>  <br/> |<span data-ttu-id="3cec7-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="3cec7-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3cec7-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3cec7-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="3cec7-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="3cec7-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3cec7-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="3cec7-135">See also</span></span>



[<span data-ttu-id="3cec7-136">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="3cec7-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="3cec7-137">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="3cec7-137">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


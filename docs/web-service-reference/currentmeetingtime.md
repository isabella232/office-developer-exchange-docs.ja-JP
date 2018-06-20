---
title: CurrentMeetingTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CurrentMeetingTime
api_type:
- schema
ms.assetid: 1ff68154-24b5-465a-a31c-3d3bab0d491e
description: CurrentMeetingTime 要素は、会議の出席者によって提案された会議の時刻を更新する会議の開始時刻を表します。
ms.openlocfilehash: 88adbe566270d759986e9b55afd4827c0513ca43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759882"
---
# <a name="currentmeetingtime"></a><span data-ttu-id="01cf7-103">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="01cf7-103">CurrentMeetingTime</span></span>

<span data-ttu-id="01cf7-104">**CurrentMeetingTime**要素は、会議の出席者によって提案された会議の時刻を更新する会議の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="01cf7-104">The **CurrentMeetingTime** element represents the start time of a meeting that you want to update with a meeting time proposed by a meeting attendee.</span></span> 
  
[<span data-ttu-id="01cf7-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="01cf7-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="01cf7-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="01cf7-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="01cf7-107">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="01cf7-107">CurrentMeetingTime</span></span>](currentmeetingtime.md)
  
```xml
<CurrentMeetingTime>...</CurrentMeetingTime>
```

 <span data-ttu-id="01cf7-108">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="01cf7-108">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01cf7-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="01cf7-109">Attributes and elements</span></span>

<span data-ttu-id="01cf7-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="01cf7-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01cf7-111">属性</span><span class="sxs-lookup"><span data-stu-id="01cf7-111">Attributes</span></span>

<span data-ttu-id="01cf7-112">なし。</span><span class="sxs-lookup"><span data-stu-id="01cf7-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01cf7-113">子要素</span><span class="sxs-lookup"><span data-stu-id="01cf7-113">Child elements</span></span>

<span data-ttu-id="01cf7-114">なし。</span><span class="sxs-lookup"><span data-stu-id="01cf7-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="01cf7-115">親要素</span><span class="sxs-lookup"><span data-stu-id="01cf7-115">Parent elements</span></span>

|<span data-ttu-id="01cf7-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="01cf7-116">**Element**</span></span>|<span data-ttu-id="01cf7-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="01cf7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01cf7-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="01cf7-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="01cf7-119">取得するためのオプションが含まれています会議の情報を提案します。</span><span class="sxs-lookup"><span data-stu-id="01cf7-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="01cf7-120">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="01cf7-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="01cf7-121">備考</span><span class="sxs-lookup"><span data-stu-id="01cf7-121">Remarks</span></span>

<span data-ttu-id="01cf7-122">この要素は必須ではありません。</span><span class="sxs-lookup"><span data-stu-id="01cf7-122">This element is not required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="01cf7-123">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割を持つ MicrosoftExchange Server 2007 を実行しているコンピューターの/EWS/ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="01cf7-123">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="01cf7-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="01cf7-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01cf7-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="01cf7-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="01cf7-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="01cf7-126">Schema Name</span></span>  <br/> |<span data-ttu-id="01cf7-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="01cf7-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="01cf7-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="01cf7-128">Validation File</span></span>  <br/> |<span data-ttu-id="01cf7-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="01cf7-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="01cf7-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="01cf7-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="01cf7-131">False</span><span class="sxs-lookup"><span data-stu-id="01cf7-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01cf7-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="01cf7-132">See also</span></span>



[<span data-ttu-id="01cf7-133">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="01cf7-133">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="01cf7-134">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="01cf7-134">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


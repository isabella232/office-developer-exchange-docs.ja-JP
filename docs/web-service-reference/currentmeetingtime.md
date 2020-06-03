---
title: Current会議時間
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
description: Currentmeeting Time 要素は、会議の出席者から提案された会議時間で更新する会議の開始時刻を表します。
ms.openlocfilehash: e79616fd735cbf6410e85450bd75c1276923f171
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458776"
---
# <a name="currentmeetingtime"></a><span data-ttu-id="e736b-103">Current会議時間</span><span class="sxs-lookup"><span data-stu-id="e736b-103">CurrentMeetingTime</span></span>

<span data-ttu-id="e736b-104">**Currentmeeting time**要素は、会議の出席者から提案された会議時間で更新する会議の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="e736b-104">The **CurrentMeetingTime** element represents the start time of a meeting that you want to update with a meeting time proposed by a meeting attendee.</span></span> 
  
[<span data-ttu-id="e736b-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="e736b-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="e736b-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="e736b-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="e736b-107">Current会議時間</span><span class="sxs-lookup"><span data-stu-id="e736b-107">CurrentMeetingTime</span></span>](currentmeetingtime.md)
  
```xml
<CurrentMeetingTime>...</CurrentMeetingTime>
```

 <span data-ttu-id="e736b-108">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="e736b-108">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e736b-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e736b-109">Attributes and elements</span></span>

<span data-ttu-id="e736b-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e736b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e736b-111">属性</span><span class="sxs-lookup"><span data-stu-id="e736b-111">Attributes</span></span>

<span data-ttu-id="e736b-112">なし。</span><span class="sxs-lookup"><span data-stu-id="e736b-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e736b-113">子要素</span><span class="sxs-lookup"><span data-stu-id="e736b-113">Child elements</span></span>

<span data-ttu-id="e736b-114">なし。</span><span class="sxs-lookup"><span data-stu-id="e736b-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e736b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="e736b-115">Parent elements</span></span>

|<span data-ttu-id="e736b-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="e736b-116">**Element**</span></span>|<span data-ttu-id="e736b-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="e736b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e736b-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="e736b-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="e736b-119">会議提案情報を取得するためのオプションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e736b-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="e736b-120">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e736b-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e736b-121">注釈</span><span class="sxs-lookup"><span data-stu-id="e736b-121">Remarks</span></span>

<span data-ttu-id="e736b-122">この要素は必須ではありません。</span><span class="sxs-lookup"><span data-stu-id="e736b-122">This element is not required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="e736b-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの/EWS/ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e736b-123">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="e736b-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e736b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e736b-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="e736b-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e736b-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e736b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="e736b-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e736b-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="e736b-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e736b-128">Validation File</span></span>  <br/> |<span data-ttu-id="e736b-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e736b-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e736b-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e736b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="e736b-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="e736b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e736b-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="e736b-132">See also</span></span>



[<span data-ttu-id="e736b-133">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="e736b-133">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="e736b-134">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="e736b-134">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


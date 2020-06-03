---
title: TooBigGroupAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TooBigGroupAttendeeConflictData
api_type:
- schema
ms.assetid: 1512428d-ce22-4da9-b1c1-446b4bcd0a21
description: TooBigGroupAttendeeConflictData 要素は、配布リストとして解決されたが、配布リストが大きすぎて展開できなかった出席者を表します。
ms.openlocfilehash: 407a4a49e5f32c81439063f47df2e131dd663a4f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468601"
---
# <a name="toobiggroupattendeeconflictdata"></a><span data-ttu-id="6a73e-103">TooBigGroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="6a73e-103">TooBigGroupAttendeeConflictData</span></span>

<span data-ttu-id="6a73e-104">**TooBigGroupAttendeeConflictData**要素は、配布リストとして解決されたが、配布リストが大きすぎて展開できなかった出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="6a73e-104">The **TooBigGroupAttendeeConflictData** element represents an attendee that was resolved as a distribution list but the distribution list was too large to expand.</span></span> 
  
[<span data-ttu-id="6a73e-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="6a73e-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="6a73e-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="6a73e-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="6a73e-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="6a73e-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="6a73e-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="6a73e-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="6a73e-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="6a73e-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="6a73e-110">提案</span><span class="sxs-lookup"><span data-stu-id="6a73e-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="6a73e-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="6a73e-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="6a73e-112">TooBigGroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="6a73e-112">TooBigGroupAttendeeConflictData</span></span>](toobiggroupattendeeconflictdata.md)
  
```xml
<TooBigGroupAttendeeConflictData/>
```

 <span data-ttu-id="6a73e-113">**TooBigGroupAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="6a73e-113">**TooBigGroupAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a73e-114">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6a73e-114">Attributes and elements</span></span>

<span data-ttu-id="6a73e-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6a73e-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a73e-116">属性</span><span class="sxs-lookup"><span data-stu-id="6a73e-116">Attributes</span></span>

<span data-ttu-id="6a73e-117">なし。</span><span class="sxs-lookup"><span data-stu-id="6a73e-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a73e-118">子要素</span><span class="sxs-lookup"><span data-stu-id="6a73e-118">Child elements</span></span>

<span data-ttu-id="6a73e-119">なし。</span><span class="sxs-lookup"><span data-stu-id="6a73e-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6a73e-120">親要素</span><span class="sxs-lookup"><span data-stu-id="6a73e-120">Parent elements</span></span>

|<span data-ttu-id="6a73e-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="6a73e-121">**Element**</span></span>|<span data-ttu-id="6a73e-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="6a73e-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a73e-123">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="6a73e-123">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="6a73e-124">[GetUserAvailabilityRequest](getuseravailabilityrequest.md)で特定された参加者の競合データの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6a73e-124">Contains an array of conflict data for attendees identified in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span></span>  <br/> <span data-ttu-id="6a73e-125">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6a73e-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6a73e-126">注釈</span><span class="sxs-lookup"><span data-stu-id="6a73e-126">Remarks</span></span>

<span data-ttu-id="6a73e-127">100を超えるメンバーを含む配布リストを展開することはできません。</span><span class="sxs-lookup"><span data-stu-id="6a73e-127">Distribution lists that contain more than 100 members cannot be expanded.</span></span>
  
<span data-ttu-id="6a73e-128">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6a73e-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a73e-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6a73e-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a73e-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="6a73e-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6a73e-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6a73e-131">Schema Name</span></span>  <br/> |<span data-ttu-id="6a73e-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6a73e-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="6a73e-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6a73e-133">Validation File</span></span>  <br/> |<span data-ttu-id="6a73e-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6a73e-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6a73e-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6a73e-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="6a73e-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="6a73e-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6a73e-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="6a73e-137">See also</span></span>



[<span data-ttu-id="6a73e-138">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="6a73e-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="6a73e-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="6a73e-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="6a73e-140">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="6a73e-140">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


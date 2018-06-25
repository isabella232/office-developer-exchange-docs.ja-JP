---
title: SuggestionsViewOptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionsViewOptions
api_type:
- schema
ms.assetid: bb04ae38-e62d-4a69-a479-8ff326ca726e
description: SuggestionsViewOptions 要素を取得するためのオプションには、会議の情報を提案します。
ms.openlocfilehash: 09ff317ae0b2ebf1eadc89dc3bb1cf5b3ae19dcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839627"
---
# <a name="suggestionsviewoptions"></a><span data-ttu-id="593c8-103">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="593c8-103">SuggestionsViewOptions</span></span>

<span data-ttu-id="593c8-104">**SuggestionsViewOptions**要素を取得するためのオプションには、会議の情報を提案します。</span><span class="sxs-lookup"><span data-stu-id="593c8-104">The **SuggestionsViewOptions** element contains the options for obtaining meeting suggestion information.</span></span> 
  
[<span data-ttu-id="593c8-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="593c8-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="593c8-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="593c8-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
```xml
<SuggestionsViewOptions>
   <GoodThreshold>...</GoodThreshold>
   <MaximumResultsByDay>...</MaximumResultsByDay>
   <MaximumNonWorkingHourResultsByDay>...</MaximumNonWorkingHourResultsByDay>
   <MeetingDurationInMinutes>...</MeetingDurationInMinutes>
   <MinimumSuggestionQuality>...</MinimumSuggestionQuality>
   <SuggestionIntervalInMinutes>...</SuggestionIntervalInMinutes>
   <DetailedSuggestionsWindow>...</DetailedSuggestionsWindow>
   <CurrentMeetingTime>...</CurrentMeetingTime>
   <GlobalObjectId>...</GlobalObjectId>
</SuggestionsViewOptions>
```

 <span data-ttu-id="593c8-107">**SuggestionsViewOptionsType**</span><span class="sxs-lookup"><span data-stu-id="593c8-107">**SuggestionsViewOptionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="593c8-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="593c8-108">Attributes and elements</span></span>

<span data-ttu-id="593c8-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="593c8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="593c8-110">属性</span><span class="sxs-lookup"><span data-stu-id="593c8-110">Attributes</span></span>

<span data-ttu-id="593c8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="593c8-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="593c8-112">子要素</span><span class="sxs-lookup"><span data-stu-id="593c8-112">Child elements</span></span>

|<span data-ttu-id="593c8-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="593c8-113">**Element**</span></span>|<span data-ttu-id="593c8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="593c8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="593c8-115">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="593c8-115">GoodThreshold</span></span>](goodthreshold.md) <br/> |<span data-ttu-id="593c8-116">良い提案された会議の時間と判断するまでの時間を開くまでの時間が必要な出席者の割合を指定します。</span><span class="sxs-lookup"><span data-stu-id="593c8-116">Specifies the percentage of attendees that must have the time period open for the time period to qualify as a good suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="593c8-117">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="593c8-117">MaximumResultsByDay</span></span>](maximumresultsbyday.md) <br/> |<span data-ttu-id="593c8-118">応答で返される 1 日あたりの推奨される会議の時刻の数を指定します。</span><span class="sxs-lookup"><span data-stu-id="593c8-118">Specifies the number of suggested meeting times per day returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="593c8-119">MaximumNonWorkHourResultsByDay</span><span class="sxs-lookup"><span data-stu-id="593c8-119">MaximumNonWorkHourResultsByDay</span></span>](maximumnonworkhourresultsbyday.md) <br/> |<span data-ttu-id="593c8-120">1 日あたりの通常の勤務時間外の時間を満たすために提示された結果の数を指定します。</span><span class="sxs-lookup"><span data-stu-id="593c8-120">Specifies the number of suggested results for meeting times outside regular working hours per day.</span></span>  <br/> |
|[<span data-ttu-id="593c8-121">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="593c8-121">MeetingDurationInMinutes</span></span>](meetingdurationinminutes.md) <br/> |<span data-ttu-id="593c8-122">提案された会議の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="593c8-122">Specifies the length of the meeting to be suggested.</span></span>  <br/> |
|[<span data-ttu-id="593c8-123">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="593c8-123">MinimumSuggestionQuality</span></span>](minimumsuggestionquality.md) <br/> |<span data-ttu-id="593c8-124">応答で返される会議の提案の品質を指定します。</span><span class="sxs-lookup"><span data-stu-id="593c8-124">Specifies the quality of meeting suggestions to be returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="593c8-125">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="593c8-125">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="593c8-126">提案された会議の時間についての詳細情報を照会する期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="593c8-126">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="593c8-127">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="593c8-127">CurrentMeetingTime</span></span>](currentmeetingtime.md) <br/> |<span data-ttu-id="593c8-128">時間の結果を提案された会議を更新する会議の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="593c8-128">Represents the start time of a meeting that you want to update with the suggested meeting time results.</span></span>  <br/> |
|[<span data-ttu-id="593c8-129">GlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="593c8-129">GlobalObjectId</span></span>](globalobjectid.md) <br/> |<span data-ttu-id="593c8-130">この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="593c8-130">This element is not used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="593c8-131">親要素</span><span class="sxs-lookup"><span data-stu-id="593c8-131">Parent elements</span></span>

|<span data-ttu-id="593c8-132">**要素**</span><span class="sxs-lookup"><span data-stu-id="593c8-132">**Element**</span></span>|<span data-ttu-id="593c8-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="593c8-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="593c8-134">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="593c8-134">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="593c8-135">ユーザーの利用可能時間情報を取得するための引数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="593c8-135">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="593c8-136">これは、ルート要素です。</span><span class="sxs-lookup"><span data-stu-id="593c8-136">This is a root element.</span></span>  <br/> <span data-ttu-id="593c8-137">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="593c8-137">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="593c8-138">備考</span><span class="sxs-lookup"><span data-stu-id="593c8-138">Remarks</span></span>

<span data-ttu-id="593c8-139">この要素は必須ではなく、発生は一度のみを使用する場合。</span><span class="sxs-lookup"><span data-stu-id="593c8-139">This element is not required and can only occur once if used.</span></span> <span data-ttu-id="593c8-140">[FreeBusyViewOptions](freebusyviewoptions.md)要素の値が null でない場合、この値を null にすることができます。</span><span class="sxs-lookup"><span data-stu-id="593c8-140">This value can be null if the value of the [FreeBusyViewOptions](freebusyviewoptions.md) element is not null.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="593c8-141">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="593c8-141">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="593c8-142">要素情報</span><span class="sxs-lookup"><span data-stu-id="593c8-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="593c8-143">名前空間</span><span class="sxs-lookup"><span data-stu-id="593c8-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="593c8-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="593c8-144">Schema Name</span></span>  <br/> |<span data-ttu-id="593c8-145">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="593c8-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="593c8-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="593c8-146">Validation File</span></span>  <br/> |<span data-ttu-id="593c8-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="593c8-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="593c8-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="593c8-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="593c8-149">False</span><span class="sxs-lookup"><span data-stu-id="593c8-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="593c8-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="593c8-150">See also</span></span>



[<span data-ttu-id="593c8-151">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="593c8-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="593c8-152">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="593c8-152">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


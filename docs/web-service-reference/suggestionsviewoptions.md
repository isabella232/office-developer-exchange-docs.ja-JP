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
description: SuggestionsViewOptions 要素には、会議提案情報を取得するためのオプションが含まれています。
ms.openlocfilehash: f584b19997f98760bd4e438dcd48a5c18cc63e4b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44433995"
---
# <a name="suggestionsviewoptions"></a><span data-ttu-id="fb670-103">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="fb670-103">SuggestionsViewOptions</span></span>

<span data-ttu-id="fb670-104">**SuggestionsViewOptions**要素には、会議提案情報を取得するためのオプションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fb670-104">The **SuggestionsViewOptions** element contains the options for obtaining meeting suggestion information.</span></span> 
  
[<span data-ttu-id="fb670-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="fb670-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="fb670-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="fb670-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
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

 <span data-ttu-id="fb670-107">**SuggestionsViewOptionsType**</span><span class="sxs-lookup"><span data-stu-id="fb670-107">**SuggestionsViewOptionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb670-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fb670-108">Attributes and elements</span></span>

<span data-ttu-id="fb670-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fb670-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb670-110">属性</span><span class="sxs-lookup"><span data-stu-id="fb670-110">Attributes</span></span>

<span data-ttu-id="fb670-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fb670-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb670-112">子要素</span><span class="sxs-lookup"><span data-stu-id="fb670-112">Child elements</span></span>

|<span data-ttu-id="fb670-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="fb670-113">**Element**</span></span>|<span data-ttu-id="fb670-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb670-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb670-115">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="fb670-115">GoodThreshold</span></span>](goodthreshold.md) <br/> |<span data-ttu-id="fb670-116">適切な会議の時間として評価される期間に、期間を開いておく必要がある出席者の割合を指定します。</span><span class="sxs-lookup"><span data-stu-id="fb670-116">Specifies the percentage of attendees that must have the time period open for the time period to qualify as a good suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="fb670-117">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="fb670-117">MaximumResultsByDay</span></span>](maximumresultsbyday.md) <br/> |<span data-ttu-id="fb670-118">応答で返される1日あたりの提案された会議時間数を指定します。</span><span class="sxs-lookup"><span data-stu-id="fb670-118">Specifies the number of suggested meeting times per day returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="fb670-119">Maximumnonwork 時間の日付</span><span class="sxs-lookup"><span data-stu-id="fb670-119">MaximumNonWorkHourResultsByDay</span></span>](maximumnonworkhourresultsbyday.md) <br/> |<span data-ttu-id="fb670-120">通常の稼働時間外の1日の会議時間について提案される結果の数を指定します。</span><span class="sxs-lookup"><span data-stu-id="fb670-120">Specifies the number of suggested results for meeting times outside regular working hours per day.</span></span>  <br/> |
|[<span data-ttu-id="fb670-121">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="fb670-121">MeetingDurationInMinutes</span></span>](meetingdurationinminutes.md) <br/> |<span data-ttu-id="fb670-122">提案される会議の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="fb670-122">Specifies the length of the meeting to be suggested.</span></span>  <br/> |
|[<span data-ttu-id="fb670-123">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="fb670-123">MinimumSuggestionQuality</span></span>](minimumsuggestionquality.md) <br/> |<span data-ttu-id="fb670-124">応答で返される会議の提案の品質を指定します。</span><span class="sxs-lookup"><span data-stu-id="fb670-124">Specifies the quality of meeting suggestions to be returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="fb670-125">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="fb670-125">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="fb670-126">提案された会議時間に関する詳細情報について、クエリされる期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="fb670-126">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="fb670-127">Current会議時間</span><span class="sxs-lookup"><span data-stu-id="fb670-127">CurrentMeetingTime</span></span>](currentmeetingtime.md) <br/> |<span data-ttu-id="fb670-128">提案された会議時間の結果で更新する会議の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="fb670-128">Represents the start time of a meeting that you want to update with the suggested meeting time results.</span></span>  <br/> |
|[<span data-ttu-id="fb670-129">GlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="fb670-129">GlobalObjectId</span></span>](globalobjectid.md) <br/> |<span data-ttu-id="fb670-130">この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="fb670-130">This element is not used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fb670-131">親要素</span><span class="sxs-lookup"><span data-stu-id="fb670-131">Parent elements</span></span>

|<span data-ttu-id="fb670-132">**要素**</span><span class="sxs-lookup"><span data-stu-id="fb670-132">**Element**</span></span>|<span data-ttu-id="fb670-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb670-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb670-134">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="fb670-134">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="fb670-135">ユーザーの空き時間情報を取得するために使用する引数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fb670-135">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="fb670-136">これはルート要素です。</span><span class="sxs-lookup"><span data-stu-id="fb670-136">This is a root element.</span></span>  <br/> <span data-ttu-id="fb670-137">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fb670-137">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fb670-138">注釈</span><span class="sxs-lookup"><span data-stu-id="fb670-138">Remarks</span></span>

<span data-ttu-id="fb670-139">この要素は必須ではなく、使用されている場合に1回だけ発生します。</span><span class="sxs-lookup"><span data-stu-id="fb670-139">This element is not required and can only occur once if used.</span></span> <span data-ttu-id="fb670-140">[FreeBusyViewOptions](freebusyviewoptions.md)要素の値が null でない場合は、この値を null にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fb670-140">This value can be null if the value of the [FreeBusyViewOptions](freebusyviewoptions.md) element is not null.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="fb670-141">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="fb670-141">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="fb670-142">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fb670-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb670-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="fb670-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fb670-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fb670-144">Schema Name</span></span>  <br/> |<span data-ttu-id="fb670-145">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="fb670-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="fb670-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fb670-146">Validation File</span></span>  <br/> |<span data-ttu-id="fb670-147">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="fb670-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fb670-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fb670-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="fb670-149">正しくない</span><span class="sxs-lookup"><span data-stu-id="fb670-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb670-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="fb670-150">See also</span></span>



[<span data-ttu-id="fb670-151">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="fb670-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="fb670-152">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="fb670-152">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


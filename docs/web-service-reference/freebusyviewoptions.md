---
title: FreeBusyViewOptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyViewOptions
api_type:
- schema
ms.assetid: c07f3ddb-874b-4d30-a60e-7e5c7793bb6f
description: FreeBusyViewOptions 要素は、応答で返される空き時間情報の種類を指定します。
ms.openlocfilehash: b67d3f461e0edaa82f074f75b0c1c54efc8af4d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459575"
---
# <a name="freebusyviewoptions"></a><span data-ttu-id="85330-103">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="85330-103">FreeBusyViewOptions</span></span>

<span data-ttu-id="85330-104">**FreeBusyViewOptions**要素は、応答で返される空き時間情報の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="85330-104">The **FreeBusyViewOptions** element specifies the type of free/busy information returned in the response.</span></span> 
  
[<span data-ttu-id="85330-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="85330-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="85330-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="85330-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
```xml
<FreeBusyViewOptions>
   <TimeWindow>...</TimeWindow>
   <MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
<RequestedView>...</RequestedView>
</FreeBusyViewOptions>

```

 <span data-ttu-id="85330-107">**FreeBusyViewOptionsType**</span><span class="sxs-lookup"><span data-stu-id="85330-107">**FreeBusyViewOptionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85330-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="85330-108">Attributes and elements</span></span>

<span data-ttu-id="85330-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="85330-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85330-110">属性</span><span class="sxs-lookup"><span data-stu-id="85330-110">Attributes</span></span>

<span data-ttu-id="85330-111">なし。</span><span class="sxs-lookup"><span data-stu-id="85330-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85330-112">子要素</span><span class="sxs-lookup"><span data-stu-id="85330-112">Child elements</span></span>

|<span data-ttu-id="85330-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="85330-113">**Element**</span></span>|<span data-ttu-id="85330-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="85330-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85330-115">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="85330-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="85330-116">ユーザーの空き時間情報を照会した期間を識別します。</span><span class="sxs-lookup"><span data-stu-id="85330-116">Identifies the time span queried for the user availability information.</span></span>  <br/> |
|[<span data-ttu-id="85330-117">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="85330-117">MergedFreeBusyIntervalInMinutes</span></span>](mergedfreebusyintervalinminutes.md) <br/> |<span data-ttu-id="85330-118">**FreeBusyMerged**ビューの2つの連続するスロット間の時間差を表します。</span><span class="sxs-lookup"><span data-stu-id="85330-118">Represents the time difference between two successive slots in the **FreeBusyMerged** view.</span></span>  <br/> |
|[<span data-ttu-id="85330-119">RequestedView</span><span class="sxs-lookup"><span data-stu-id="85330-119">RequestedView</span></span>](requestedview.md) <br/> |<span data-ttu-id="85330-120">クライアントが要求する予定表情報の種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="85330-120">Defines the type of calendar information that a client requests.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="85330-121">親要素</span><span class="sxs-lookup"><span data-stu-id="85330-121">Parent elements</span></span>

|<span data-ttu-id="85330-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="85330-122">**Element**</span></span>|<span data-ttu-id="85330-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="85330-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85330-124">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="85330-124">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="85330-125">ユーザーの空き時間情報を取得するために使用する引数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="85330-125">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="85330-126">これはルート要素です。</span><span class="sxs-lookup"><span data-stu-id="85330-126">This is a root element.</span></span>  <br/> <span data-ttu-id="85330-127">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="85330-127">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="85330-128">注釈</span><span class="sxs-lookup"><span data-stu-id="85330-128">Remarks</span></span>

<span data-ttu-id="85330-129">この要素は必須ではなく、使用されている場合に1回だけ発生します。</span><span class="sxs-lookup"><span data-stu-id="85330-129">This element is not required and can only occur once if used.</span></span> <span data-ttu-id="85330-130">[SuggestionsViewOptions](suggestionsviewoptions.md)要素の値が null でない場合は、この値を null にすることができます。</span><span class="sxs-lookup"><span data-stu-id="85330-130">This value can be null if the value of the [SuggestionsViewOptions](suggestionsviewoptions.md) element is not null.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="85330-131">この要素を記述するスキーマは、Microsoft® Exchange Server 2007 を実行しているコンピューターの/epi/ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="85330-131">The schema that describes this element is located in the /epi/ directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="example"></a><span data-ttu-id="85330-132">例</span><span class="sxs-lookup"><span data-stu-id="85330-132">Example</span></span>

<span data-ttu-id="85330-133">次の例では、会議の一覧と空き時間ストリームを60分間隔で取得します。</span><span class="sxs-lookup"><span data-stu-id="85330-133">The following example obtains a list of meetings and a free/busy stream in 60-minute intervals.</span></span>
  
```
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserAvailabilityRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Bias>480</Bias>
        <StandardTime>
          <Bias>0</Bias>
          <Time>02:00:00</Time>
          <DayOrder>5</DayOrder>
          <Month>10</Month>
          <DayOfWeek>Sunday</DayOfWeek>
        </StandardTime>
        <DaylightTime>
          <Bias>-60</Bias>
          <Time>02:00:00</Time>
          <DayOrder>1</DayOrder>
          <Month>4</Month>
          <DayOfWeek>Sunday</DayOfWeek>
        </DaylightTime>
      </TimeZone>
      <MailboxDataArray>
        <MailboxData xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Email>
            <Name></Name>
            <Address>someone@ExServer.example.com</Address>
            <RoutingType>SMTP</RoutingType>
          </Email>
          <AttendeeType>Organizer</AttendeeType>
          <ExcludeConflicts>false</ExcludeConflicts>
          <ExcludeNonWorkingHours>false</ExcludeNonWorkingHours>
        </MailboxData>
      </MailboxDataArray>
      <FreeBusyViewOptions xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <TimeWindow>
          <StartTime>2006-02-06T00:00:00</StartTime>
          <EndTime>2006-02-25T23:59:59</EndTime>
        </TimeWindow>
        <MergedFreeBusyIntervalInMinutes>60</MergedFreeBusyIntervalInMinutes>
        <RequestedView>FreeBusyMerged</RequestedView>
      </FreeBusyViewOptions>
    </GetUserAvailabilityRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="85330-134">要素の情報</span><span class="sxs-lookup"><span data-stu-id="85330-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85330-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="85330-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="85330-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="85330-136">Schema Name</span></span>  <br/> |<span data-ttu-id="85330-137">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="85330-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="85330-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="85330-138">Validation File</span></span>  <br/> |<span data-ttu-id="85330-139">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="85330-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="85330-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="85330-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="85330-141">正しくない</span><span class="sxs-lookup"><span data-stu-id="85330-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="85330-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="85330-142">See also</span></span>



[<span data-ttu-id="85330-143">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="85330-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="85330-144">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="85330-144">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


---
title: GetUserAvailabilityRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserAvailabilityRequest
api_type:
- schema
ms.assetid: 7906711b-80a1-42ae-8b33-26eeac036a5a
description: GetUserAvailabilityRequest 要素には、ユーザーの空き時間情報を取得するために使用される引数が含まれています。 これはルート要素です。
ms.openlocfilehash: 6c2e2c5452b6379171e49cf6aea2d437152ecb9b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459119"
---
# <a name="getuseravailabilityrequest"></a><span data-ttu-id="b5c1e-104">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="b5c1e-104">GetUserAvailabilityRequest</span></span>

<span data-ttu-id="b5c1e-105">**GetUserAvailabilityRequest**要素には、ユーザーの空き時間情報を取得するために使用される引数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b5c1e-105">The **GetUserAvailabilityRequest** element contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="b5c1e-106">これはルート要素です。</span><span class="sxs-lookup"><span data-stu-id="b5c1e-106">This is a root element.</span></span> 
  
```xml
<GetUserAvailabilityRequest>
   <TimeZone>...</TimeZone>
   <MailboxDataArray>...</MailboxDataArray>
   <FreeBusyViewOptions>...</FreeBusyViewOptions>
   <SuggestionsViewOptions>...</SuggestionsViewOptions>
</GetUserAvailabilityRequest>
```

 <span data-ttu-id="b5c1e-107">**GetUserAvailabilityRequestType**</span><span class="sxs-lookup"><span data-stu-id="b5c1e-107">**GetUserAvailabilityRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b5c1e-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b5c1e-108">Attributes and elements</span></span>

<span data-ttu-id="b5c1e-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b5c1e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b5c1e-110">属性</span><span class="sxs-lookup"><span data-stu-id="b5c1e-110">Attributes</span></span>

<span data-ttu-id="b5c1e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b5c1e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b5c1e-112">子要素</span><span class="sxs-lookup"><span data-stu-id="b5c1e-112">Child elements</span></span>

|<span data-ttu-id="b5c1e-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="b5c1e-113">**Element**</span></span>|<span data-ttu-id="b5c1e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b5c1e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b5c1e-115">TimeZone (Availability)</span><span class="sxs-lookup"><span data-stu-id="b5c1e-115">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> |<span data-ttu-id="b5c1e-116">タイムゾーン情報を識別する要素を格納します。</span><span class="sxs-lookup"><span data-stu-id="b5c1e-116">Contains elements that identify time zone information.</span></span> <span data-ttu-id="b5c1e-117">この要素には、標準時から夏時間への切り替えに関する情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="b5c1e-117">This element also contains information about the transition between standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="b5c1e-118">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="b5c1e-118">MailboxDataArray</span></span>](mailboxdataarray.md) <br/> |<span data-ttu-id="b5c1e-119">可用性情報を照会するメールボックスの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b5c1e-119">Contains a list of mailboxes to query for availability information.</span></span>  <br/> |
|[<span data-ttu-id="b5c1e-120">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="b5c1e-120">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="b5c1e-121">応答で返される空き時間情報の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="b5c1e-121">Specifies the type of free/busy information returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="b5c1e-122">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="b5c1e-122">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="b5c1e-123">会議提案情報を取得するためのオプションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b5c1e-123">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b5c1e-124">親要素</span><span class="sxs-lookup"><span data-stu-id="b5c1e-124">Parent elements</span></span>

<span data-ttu-id="b5c1e-125">なし。</span><span class="sxs-lookup"><span data-stu-id="b5c1e-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b5c1e-126">注釈</span><span class="sxs-lookup"><span data-stu-id="b5c1e-126">Remarks</span></span>

<span data-ttu-id="b5c1e-127">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの/EWS/ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="b5c1e-127">The schema that describes this element is located in the /EWS/ directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="b5c1e-128">例</span><span class="sxs-lookup"><span data-stu-id="b5c1e-128">Example</span></span>

<span data-ttu-id="b5c1e-129">次の例は、空き時間情報の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="b5c1e-129">The following example shows a request for free/busy information.</span></span>
  
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
            <Address>someone@exchangeserver.example.com</Address>
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
          <EndTime>2006-02-30T23:59:59</EndTime>
        </TimeWindow>
        <MergedFreeBusyIntervalInMinutes>60</MergedFreeBusyIntervalInMinutes>
        <RequestedView>FreeBusyMerged</RequestedView>
      </FreeBusyViewOptions>
    </GetUserAvailabilityRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="b5c1e-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b5c1e-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b5c1e-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="b5c1e-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b5c1e-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b5c1e-132">Schema Name</span></span>  <br/> |<span data-ttu-id="b5c1e-133">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b5c1e-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b5c1e-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b5c1e-134">Validation File</span></span>  <br/> |<span data-ttu-id="b5c1e-135">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b5c1e-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b5c1e-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b5c1e-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="b5c1e-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="b5c1e-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b5c1e-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="b5c1e-138">See also</span></span>



[<span data-ttu-id="b5c1e-139">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="b5c1e-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="b5c1e-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b5c1e-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="b5c1e-141">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="b5c1e-141">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


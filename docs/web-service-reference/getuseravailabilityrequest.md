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
description: GetUserAvailabilityRequest 要素には、ユーザーの利用可能時間情報を取得するための引数が含まれています。 これは、ルート要素です。
ms.openlocfilehash: 5440f739b09bfbe27ad97cba99c08756686594f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831683"
---
# <a name="getuseravailabilityrequest"></a><span data-ttu-id="af05a-104">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="af05a-104">GetUserAvailabilityRequest</span></span>

<span data-ttu-id="af05a-105">**GetUserAvailabilityRequest**要素には、ユーザーの利用可能時間情報を取得するための引数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="af05a-105">The **GetUserAvailabilityRequest** element contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="af05a-106">これは、ルート要素です。</span><span class="sxs-lookup"><span data-stu-id="af05a-106">This is a root element.</span></span> 
  
```xml
<GetUserAvailabilityRequest>
   <TimeZone>...</TimeZone>
   <MailboxDataArray>...</MailboxDataArray>
   <FreeBusyViewOptions>...</FreeBusyViewOptions>
   <SuggestionsViewOptions>...</SuggestionsViewOptions>
</GetUserAvailabilityRequest>
```

 <span data-ttu-id="af05a-107">**GetUserAvailabilityRequestType**</span><span class="sxs-lookup"><span data-stu-id="af05a-107">**GetUserAvailabilityRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af05a-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="af05a-108">Attributes and elements</span></span>

<span data-ttu-id="af05a-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="af05a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af05a-110">属性</span><span class="sxs-lookup"><span data-stu-id="af05a-110">Attributes</span></span>

<span data-ttu-id="af05a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="af05a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af05a-112">子要素</span><span class="sxs-lookup"><span data-stu-id="af05a-112">Child elements</span></span>

|<span data-ttu-id="af05a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="af05a-113">**Element**</span></span>|<span data-ttu-id="af05a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="af05a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af05a-115">タイムゾーン (可用性)</span><span class="sxs-lookup"><span data-stu-id="af05a-115">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> |<span data-ttu-id="af05a-116">タイム ゾーン情報を識別する要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="af05a-116">Contains elements that identify time zone information.</span></span> <span data-ttu-id="af05a-117">この要素には、標準時と夏時間の切り替えに関する情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="af05a-117">This element also contains information about the transition between standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="af05a-118">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="af05a-118">MailboxDataArray</span></span>](mailboxdataarray.md) <br/> |<span data-ttu-id="af05a-119">利用可能時間情報のクエリを実行するメールボックスの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="af05a-119">Contains a list of mailboxes to query for availability information.</span></span>  <br/> |
|[<span data-ttu-id="af05a-120">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="af05a-120">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="af05a-121">応答で返される空き時間情報の情報の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="af05a-121">Specifies the type of free/busy information returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="af05a-122">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="af05a-122">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="af05a-123">取得するためのオプションが含まれています会議の情報を提案します。</span><span class="sxs-lookup"><span data-stu-id="af05a-123">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="af05a-124">親要素</span><span class="sxs-lookup"><span data-stu-id="af05a-124">Parent elements</span></span>

<span data-ttu-id="af05a-125">なし。</span><span class="sxs-lookup"><span data-stu-id="af05a-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="af05a-126">備考</span><span class="sxs-lookup"><span data-stu-id="af05a-126">Remarks</span></span>

<span data-ttu-id="af05a-127">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの/EWS/ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="af05a-127">The schema that describes this element is located in the /EWS/ directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="af05a-128">例</span><span class="sxs-lookup"><span data-stu-id="af05a-128">Example</span></span>

<span data-ttu-id="af05a-129">次の例では、空き時間情報の要求を示します。</span><span class="sxs-lookup"><span data-stu-id="af05a-129">The following example shows a request for free/busy information.</span></span>
  
```
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserAvailabilityRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
        <MailboxData xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
      <FreeBusyViewOptions xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="af05a-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="af05a-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af05a-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="af05a-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="af05a-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="af05a-132">Schema Name</span></span>  <br/> |<span data-ttu-id="af05a-133">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="af05a-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="af05a-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="af05a-134">Validation File</span></span>  <br/> |<span data-ttu-id="af05a-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="af05a-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="af05a-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="af05a-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="af05a-137">False</span><span class="sxs-lookup"><span data-stu-id="af05a-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af05a-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="af05a-138">See also</span></span>



[<span data-ttu-id="af05a-139">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="af05a-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="af05a-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="af05a-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="af05a-141">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="af05a-141">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


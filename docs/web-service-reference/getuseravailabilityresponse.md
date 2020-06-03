---
title: GetUserAvailabilityResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserAvailabilityResponse
api_type:
- schema
ms.assetid: 6999510a-d60e-43da-8964-57b5fb3e9d11
description: GetUserAvailabilityResponse 要素は、ユーザーの空き時間情報または推奨される会議時刻情報を定義するプロパティを含むルート要素です。
ms.openlocfilehash: ceb24bc8b31a7d7313add213c26bef5efd3c89ae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458216"
---
# <a name="getuseravailabilityresponse"></a><span data-ttu-id="0871c-103">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="0871c-103">GetUserAvailabilityResponse</span></span>

<span data-ttu-id="0871c-104">**GetUserAvailabilityResponse**要素は、ユーザーの空き時間情報または推奨される会議時刻情報を定義するプロパティを含むルート要素です。</span><span class="sxs-lookup"><span data-stu-id="0871c-104">The **GetUserAvailabilityResponse** element is the root element that contains the properties that define user availability information or suggested meeting time information.</span></span> 
  
```xml
<GetUserAvailabilityResponse>
   <FreeBusyResponseArray>...</FreeBusyResponseArray>
   <SuggestionsResponse>...</SuggestionsResponse>
</GetUserAvailabilityResponse>
```

 <span data-ttu-id="0871c-105">**GetUserAvailabilityResponseType**</span><span class="sxs-lookup"><span data-stu-id="0871c-105">**GetUserAvailabilityResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0871c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0871c-106">Attributes and elements</span></span>

<span data-ttu-id="0871c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0871c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0871c-108">属性</span><span class="sxs-lookup"><span data-stu-id="0871c-108">Attributes</span></span>

<span data-ttu-id="0871c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0871c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0871c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0871c-110">Child elements</span></span>

|<span data-ttu-id="0871c-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="0871c-111">**Element**</span></span>|<span data-ttu-id="0871c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0871c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0871c-113">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="0871c-113">FreeBusyResponseArray</span></span>](freebusyresponsearray.md) <br/> |<span data-ttu-id="0871c-114">要求されたユーザーの空き時間情報と応答の状態を含みます。</span><span class="sxs-lookup"><span data-stu-id="0871c-114">Contains the requested users' availability information and the response status.</span></span>  <br/> |
|[<span data-ttu-id="0871c-115">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="0871c-115">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="0871c-116">要求された会議の提案の応答状態情報と提案データを格納します。</span><span class="sxs-lookup"><span data-stu-id="0871c-116">Contains response status information and suggestion data for requested meeting suggestions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0871c-117">親要素</span><span class="sxs-lookup"><span data-stu-id="0871c-117">Parent elements</span></span>

<span data-ttu-id="0871c-118">なし。</span><span class="sxs-lookup"><span data-stu-id="0871c-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0871c-119">注釈</span><span class="sxs-lookup"><span data-stu-id="0871c-119">Remarks</span></span>

<span data-ttu-id="0871c-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0871c-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="0871c-121">例</span><span class="sxs-lookup"><span data-stu-id="0871c-121">Example</span></span>

<span data-ttu-id="0871c-122">GetUserAvailability 応答の次の例は、GetUserAvailability 要求に対する応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="0871c-122">The following example of a GetUserAvailability response shows a response to a GetUserAvailability request.</span></span>
  
```
<?xml version="1.0" encoding="utf-8" ?>
<GetUserAvailabilityResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <FreeBusyResponseArray xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <FreeBusyResponse>
      <ResponseMessage ResponseClass="Success">
        <Path select="/m:GetUserAvailabilityRequest/MailboxDataArray[0]" />
      </ResponseMessage>
      <FreeBusyView>
        <FreeBusyViewType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Detailed</FreeBusyViewType>
        <CalendarEventArray xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <CalendarEvent>
            <StartTime>2006-02-28T19:00:00-08:00</StartTime>
            <EndTime>2006-02-28T23:30:00-08:00</EndTime>
            <BusyType>OOF</BusyType>
            <IsPrivate>false</IsPrivate>
            <CalendarEventDetails>
              <ID>00000</ID>
              <Subject>Exercise</Subject>
              <Location>the gym</Location>
              <IsMeeting>false</IsMeeting>
              <IsRecurring>false</IsRecurring>
              <IsException>false</IsException>
              <IsReminderSet>true</IsReminderSet>
            </CalendarEventDetails>
          </CalendarEvent>
        </CalendarEventArray>
        <WorkingHours xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <TimeZone>
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
          <WorkingPeriodArray>
            <WorkingPeriod>
              <DayOfWeek>Monday Tuesday Wednesday Thursday Friday</DayOfWeek>
              <StartTimeInMinutes>480</StartTimeInMinutes>
              <EndTimeInMinutes>1020</EndTimeInMinutes>
            </WorkingPeriod>
          </WorkingPeriodArray>
        </WorkingHours>
      </FreeBusyView>
    </FreeBusyResponse>
  </FreeBusyResponseArray>
</GetUserAvailabilityResponse>
```

<span data-ttu-id="0871c-123">[ID](id.md)要素の内容は、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="0871c-123">The [ID](id.md) element contents were shortened to preserve readability.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="0871c-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0871c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0871c-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="0871c-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0871c-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0871c-126">Schema Name</span></span>  <br/> |<span data-ttu-id="0871c-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="0871c-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0871c-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0871c-128">Validation File</span></span>  <br/> |<span data-ttu-id="0871c-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0871c-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0871c-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0871c-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="0871c-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="0871c-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0871c-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="0871c-132">See also</span></span>



[<span data-ttu-id="0871c-133">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="0871c-133">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)


[<span data-ttu-id="0871c-134">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="0871c-134">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


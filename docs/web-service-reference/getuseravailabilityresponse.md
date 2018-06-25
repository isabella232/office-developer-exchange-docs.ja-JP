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
description: GetUserAvailabilityResponse 要素は、ユーザーの利用可能時間情報を定義するか、会議の時刻の情報を提示するプロパティを格納するルート要素です。
ms.openlocfilehash: 0a30dc8ebc11b1f818b2c27b0ea68fc135ec0925
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831684"
---
# <a name="getuseravailabilityresponse"></a><span data-ttu-id="7be6d-103">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7be6d-103">GetUserAvailabilityResponse</span></span>

<span data-ttu-id="7be6d-104">**GetUserAvailabilityResponse**要素は、ユーザーの利用可能時間情報を定義するか、会議の時刻の情報を提示するプロパティを格納するルート要素です。</span><span class="sxs-lookup"><span data-stu-id="7be6d-104">The **GetUserAvailabilityResponse** element is the root element that contains the properties that define user availability information or suggested meeting time information.</span></span> 
  
```xml
<GetUserAvailabilityResponse>
   <FreeBusyResponseArray>...</FreeBusyResponseArray>
   <SuggestionsResponse>...</SuggestionsResponse>
</GetUserAvailabilityResponse>
```

 <span data-ttu-id="7be6d-105">**GetUserAvailabilityResponseType**</span><span class="sxs-lookup"><span data-stu-id="7be6d-105">**GetUserAvailabilityResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7be6d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7be6d-106">Attributes and elements</span></span>

<span data-ttu-id="7be6d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7be6d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7be6d-108">属性</span><span class="sxs-lookup"><span data-stu-id="7be6d-108">Attributes</span></span>

<span data-ttu-id="7be6d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7be6d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7be6d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7be6d-110">Child elements</span></span>

|<span data-ttu-id="7be6d-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="7be6d-111">**Element**</span></span>|<span data-ttu-id="7be6d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7be6d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7be6d-113">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="7be6d-113">FreeBusyResponseArray</span></span>](freebusyresponsearray.md) <br/> |<span data-ttu-id="7be6d-114">要求されたユーザーの利用可能時間情報と応答のステータスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7be6d-114">Contains the requested users' availability information and the response status.</span></span>  <br/> |
|[<span data-ttu-id="7be6d-115">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="7be6d-115">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="7be6d-116">会議の提案の要求の応答ステータスの情報と提案のデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7be6d-116">Contains response status information and suggestion data for requested meeting suggestions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7be6d-117">親要素</span><span class="sxs-lookup"><span data-stu-id="7be6d-117">Parent elements</span></span>

<span data-ttu-id="7be6d-118">なし。</span><span class="sxs-lookup"><span data-stu-id="7be6d-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7be6d-119">備考</span><span class="sxs-lookup"><span data-stu-id="7be6d-119">Remarks</span></span>

<span data-ttu-id="7be6d-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="7be6d-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="7be6d-121">例</span><span class="sxs-lookup"><span data-stu-id="7be6d-121">Example</span></span>

<span data-ttu-id="7be6d-122">GetUserAvailability 要求への応答を GetUserAvailability の応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7be6d-122">The following example of a GetUserAvailability response shows a response to a GetUserAvailability request.</span></span>
  
```
<?xml version="1.0" encoding="utf-8" ?>
<GetUserAvailabilityResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <FreeBusyResponseArray xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <FreeBusyResponse>
      <ResponseMessage ResponseClass="Success">
        <Path select="/m:GetUserAvailabilityRequest/MailboxDataArray[0]" />
      </ResponseMessage>
      <FreeBusyView>
        <FreeBusyViewType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Detailed</FreeBusyViewType>
        <CalendarEventArray xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
        <WorkingHours xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="7be6d-123">[ID](id.md)要素の内容は、読みやすさを保持するために短縮されました。</span><span class="sxs-lookup"><span data-stu-id="7be6d-123">The [ID](id.md) element contents were shortened to preserve readability.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="7be6d-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="7be6d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7be6d-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="7be6d-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7be6d-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7be6d-126">Schema Name</span></span>  <br/> |<span data-ttu-id="7be6d-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="7be6d-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7be6d-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7be6d-128">Validation File</span></span>  <br/> |<span data-ttu-id="7be6d-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7be6d-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7be6d-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7be6d-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="7be6d-131">False</span><span class="sxs-lookup"><span data-stu-id="7be6d-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7be6d-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="7be6d-132">See also</span></span>



[<span data-ttu-id="7be6d-133">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="7be6d-133">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)


[<span data-ttu-id="7be6d-134">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="7be6d-134">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)


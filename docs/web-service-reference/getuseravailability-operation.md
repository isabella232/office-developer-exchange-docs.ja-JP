---
title: GetUserAvailability 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserAvailability
api_type:
- schema
ms.assetid: 8da17226-5d3a-4525-9ffa-d83730f47bb1
description: 操作 GetUserAvailability EWS についての情報を検索します。
ms.openlocfilehash: 41246fe22bfb7444cd4aa7b1d4651d475dd9231c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831686"
---
# <a name="getuseravailability-operation"></a><span data-ttu-id="78e47-103">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="78e47-103">GetUserAvailability operation</span></span>

<span data-ttu-id="78e47-104">**GetUserAvailability** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="78e47-104">Find information about the **GetUserAvailability** EWS operation.</span></span> 
  
<span data-ttu-id="78e47-105">**GetUserAvailability**操作は、指定された期間内で一連のユーザー、会議室、およびリソースの可用性についての詳細な情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="78e47-105">The **GetUserAvailability** operation provides detailed information about the availability of a set of users, rooms, and resources within a specified time period.</span></span> 
  
## <a name="using-the-getuseravailability-operation"></a><span data-ttu-id="78e47-106">GetUserAvailability 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="78e47-106">Using the GetUserAvailability operation</span></span>

<span data-ttu-id="78e47-107">**GetUserAvailability**操作では、詳細情報の指定したレベルでの現在のユーザーの可用性の情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="78e47-107">The **GetUserAvailability** operation provides current user availability information at a specified level of detail.</span></span> <span data-ttu-id="78e47-108">Outlook、Outlook Web Access、Outlook Mobile Access、およびその他のユーザーなどのクライアント アプリケーションは、要求されたユーザー情報を識別するのに SMTP アドレスを使用します。</span><span class="sxs-lookup"><span data-stu-id="78e47-108">Client applications such as Outlook, Outlook Web Access, Outlook Mobile Access, and others use SMTP addresses to identify the requested user information.</span></span> 
  
<span data-ttu-id="78e47-109">配布リスト内のメールボックスの数が 100 未満の id の最大数である限り、リストの各メンバーの空き時間情報のステータスを取得するために配布リストの展開を可用性サービスを**GetUserAvailability**操作を要求できます。</span><span class="sxs-lookup"><span data-stu-id="78e47-109">The Availability service expands distribution lists to retrieve the free/busy status for each member of the list, as long as the number of mailboxes in the distribution list is less than 100, which is the maximum number of identities that the **GetUserAvailability** operation can request.</span></span> <span data-ttu-id="78e47-110">配布リストのメンバーの空き時間情報のステータスは、全体の配布リストの 1 つの空き時間情報のステータスにマージされます。</span><span class="sxs-lookup"><span data-stu-id="78e47-110">The free/busy statuses of the members of the distribution list are merged into a single free/busy status for the whole distribution list.</span></span> 
  
<span data-ttu-id="78e47-111">クライアント アプリケーションの要求は、可用性のクエリの期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="78e47-111">Client application requests specify the time period of the availability query.</span></span> <span data-ttu-id="78e47-112">要求された情報の有効期間は 42 日です。</span><span class="sxs-lookup"><span data-stu-id="78e47-112">The default time period for the requested information is 42 days.</span></span> <span data-ttu-id="78e47-113">ユーザーの予定表は、予定または会議内と外部の両方のクエリの定義された期間には含まれている、予定が返されます。</span><span class="sxs-lookup"><span data-stu-id="78e47-113">If the user's calendar contains appointments or meetings that are both within and outside the defined time period for the query, the appointment is returned.</span></span> 
  
<span data-ttu-id="78e47-114">返される予定と会議の時間は、会議を要求しているクライアント アプリケーションと同じタイム ゾーンです。</span><span class="sxs-lookup"><span data-stu-id="78e47-114">The appointment and meeting times that are returned are in the same time zone as the client application that is requesting the meeting.</span></span>
  
<span data-ttu-id="78e47-115">可用性サービスは、各クライアントの要求を処理します。</span><span class="sxs-lookup"><span data-stu-id="78e47-115">The Availability service processes the request for each client.</span></span> <span data-ttu-id="78e47-116">サービスは、すべての定期的な予定を展開し、要求元のクライアント アクセス許可を持つが表示される予定表の詳細の最大数を返します。</span><span class="sxs-lookup"><span data-stu-id="78e47-116">The service expands all the recurring appointments and returns the maximum number of calendar details that the requesting client has permission to receive.</span></span>
  
> [!NOTE]
> <span data-ttu-id="78e47-117">移動先のメールボックスが使用できないか、見つからない、 **MailRecipientNotFoundException**例外がスローされます。</span><span class="sxs-lookup"><span data-stu-id="78e47-117">If the target mailbox is unavailable or cannot be found, a **MailRecipientNotFoundException** exception is thrown.</span></span> <span data-ttu-id="78e47-118">クライアントは、Active Directory ドメイン サービス (AD DS) または Active Directory ディレクトリ サービスでメールの宛先が見つからないことを示すエラー メッセージを受信します。</span><span class="sxs-lookup"><span data-stu-id="78e47-118">The client receives an error message that states that the mail recipient is not found in the Active Directory directory service or Active Directory Domain Services (AD DS).</span></span> 
  
### <a name="getuseravailability-operation-soap-headers"></a><span data-ttu-id="78e47-119">GetUserAvailability 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78e47-119">GetUserAvailability operation SOAP headers</span></span>

<span data-ttu-id="78e47-120">**GetUserAvailability**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="78e47-120">The **GetUserAvailability** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="78e47-121">**Header**</span><span class="sxs-lookup"><span data-stu-id="78e47-121">**Header**</span></span>|<span data-ttu-id="78e47-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="78e47-122">**Element**</span></span>|<span data-ttu-id="78e47-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="78e47-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="78e47-124">**偽装**</span><span class="sxs-lookup"><span data-stu-id="78e47-124">**Impersonation**</span></span> <br/> |[<span data-ttu-id="78e47-125">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="78e47-125">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="78e47-126">クライアントを偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="78e47-126">Identifies the user whom the client is impersonating.</span></span> <span data-ttu-id="78e47-127">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="78e47-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="78e47-128">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="78e47-128">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="78e47-129">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="78e47-129">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="78e47-130">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="78e47-130">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="78e47-131">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="78e47-131">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="78e47-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="78e47-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="78e47-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="78e47-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="78e47-134">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="78e47-134">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="78e47-135">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="78e47-135">This header is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="78e47-136">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="78e47-136">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="78e47-137">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="78e47-137">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="78e47-138">サーバーからのすべての応答に使用するタイム ゾーンを識別する SOAP ヘッダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="78e47-138">Specifies a SOAP header that identifies the time zone to be used for all responses from the server.</span></span> <span data-ttu-id="78e47-139">サーバーから返されるすべての時間は、指定されたタイム ゾーンに変換されます。</span><span class="sxs-lookup"><span data-stu-id="78e47-139">All times that are returned from the server will be converted to the specified time zone.</span></span> <span data-ttu-id="78e47-140">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="78e47-140">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getuseravailability-request-example-get-availability-information"></a><span data-ttu-id="78e47-141">GetUserAvailability 要求の例: 利用可能時間情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="78e47-141">GetUserAvailability request example: Get availability information</span></span>

<span data-ttu-id="78e47-142">**GetUserAvailability**操作要求の次の例では、太平洋標準時タイム ゾーンで 2 人のユーザーの詳細な情報を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="78e47-142">The following example of a **GetUserAvailability** operation request shows how to get detailed availability information for two users in the Pacific Time time zone.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetUserAvailabilityRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <t:TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
      </t:TimeZone>
      <MailboxDataArray>
        <t:MailboxData>
          <t:Email>
            <t:Address>user1@example.com</t:Address>
          </t:Email>
          <t:AttendeeType>Required</t:AttendeeType>
          <t:ExcludeConflicts>false</t:ExcludeConflicts>
        </t:MailboxData>
        <t:MailboxData>
          <t:Email>
            <t:Address>user2@example.com</t:Address>
          </t:Email>
          <t:AttendeeType>Required</t:AttendeeType>
          <t:ExcludeConflicts>false</t:ExcludeConflicts>
        </t:MailboxData>
      </MailboxDataArray>
      <t:FreeBusyViewOptions>
        <t:TimeWindow>
          <t:StartTime>2006-10-16T00:00:00</t:StartTime>
          <t:EndTime>2006-10-16T23:59:59</t:EndTime>
        </t:TimeWindow>
        <t:MergedFreeBusyIntervalInMinutes>60</t:MergedFreeBusyIntervalInMinutes>
        <t:RequestedView>DetailedMerged</t:RequestedView>
      </t:FreeBusyViewOptions>
    </GetUserAvailabilityRequest>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="78e47-143">[SuggestionsViewOptions](suggestionsviewoptions.md)要素を使用して提案された会議を取得する方法の詳細については、EWS 仮想ディレクトリ内のスキーマを参照してください。</span><span class="sxs-lookup"><span data-stu-id="78e47-143">For more information about retrieving suggested meetings by using the [SuggestionsViewOptions](suggestionsviewoptions.md) element, see the schema in the EWS virtual directory.</span></span> 
  
<span data-ttu-id="78e47-144">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="78e47-144">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="78e47-145">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="78e47-145">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
    
- [<span data-ttu-id="78e47-146">タイムゾーン (可用性)</span><span class="sxs-lookup"><span data-stu-id="78e47-146">TimeZone (Availability)</span></span>](timezone-availability.md)
    
- [<span data-ttu-id="78e47-147">バイアス (UTC)</span><span class="sxs-lookup"><span data-stu-id="78e47-147">Bias (UTC)</span></span>](bias-utc.md)
    
- [<span data-ttu-id="78e47-148">StandardTime</span><span class="sxs-lookup"><span data-stu-id="78e47-148">StandardTime</span></span>](standardtime.md)
    
- [<span data-ttu-id="78e47-149">Bias</span><span class="sxs-lookup"><span data-stu-id="78e47-149">Bias</span></span>](bias.md)
    
- [<span data-ttu-id="78e47-150">時間</span><span class="sxs-lookup"><span data-stu-id="78e47-150">Time</span></span>](time.md)
    
- [<span data-ttu-id="78e47-151">DayOrder</span><span class="sxs-lookup"><span data-stu-id="78e47-151">DayOrder</span></span>](dayorder.md)
    
- [<span data-ttu-id="78e47-152">Month</span><span class="sxs-lookup"><span data-stu-id="78e47-152">Month</span></span>](month.md)
    
- [<span data-ttu-id="78e47-153">DayOfWeek (タイムゾーン)</span><span class="sxs-lookup"><span data-stu-id="78e47-153">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md)
    
- [<span data-ttu-id="78e47-154">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="78e47-154">DaylightTime</span></span>](daylighttime.md)
    
- [<span data-ttu-id="78e47-155">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="78e47-155">MailboxDataArray</span></span>](mailboxdataarray.md)
    
- [<span data-ttu-id="78e47-156">MailboxData</span><span class="sxs-lookup"><span data-stu-id="78e47-156">MailboxData</span></span>](mailboxdata.md)
    
- [<span data-ttu-id="78e47-157">電子メール (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="78e47-157">Email (EmailAddressType)</span></span>](email-emailaddresstype.md)
    
- [<span data-ttu-id="78e47-158">アドレス (文字列)</span><span class="sxs-lookup"><span data-stu-id="78e47-158">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="78e47-159">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="78e47-159">AttendeeType</span></span>](attendeetype.md)
    
- [<span data-ttu-id="78e47-160">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="78e47-160">ExcludeConflicts</span></span>](excludeconflicts.md)
    
- [<span data-ttu-id="78e47-161">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="78e47-161">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
    
- [<span data-ttu-id="78e47-162">時間</span><span class="sxs-lookup"><span data-stu-id="78e47-162">TimeWindow</span></span>](timewindow.md)
    
- [<span data-ttu-id="78e47-163">開始時刻</span><span class="sxs-lookup"><span data-stu-id="78e47-163">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="78e47-164">終了時刻</span><span class="sxs-lookup"><span data-stu-id="78e47-164">EndTime</span></span>](endtime.md)
    
## <a name="successful-getuseravailability-operation-response"></a><span data-ttu-id="78e47-165">GetUserAvailability 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="78e47-165">Successful GetUserAvailability operation response</span></span>

<span data-ttu-id="78e47-166">成功した要求への応答、 **GetUserAvailability**操作の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="78e47-166">The following example shows a successful response to the **GetUserAvailability** operation request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="78e47-167">予定表イベントの識別子は、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="78e47-167">The calendar event identifiers have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="665" MinorBuildNumber="7" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetUserAvailabilityResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FreeBusyResponseArray>
        <FreeBusyResponse>
          <ResponseMessage ResponseClass="Success">
            <ResponseCode>NoError</ResponseCode>
          </ResponseMessage>
          <FreeBusyView>
            <FreeBusyViewType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">DetailedMerged</FreeBusyViewType>
            <MergedFreeBusy xmlns="http://schemas.microsoft.com/exchange/services/2006/types">000002220220000000000000</MergedFreeBusy>
            <CalendarEventArray xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
              <CalendarEvent>
                <StartTime>2006-10-16T06:00:00-07:00</StartTime>
                <EndTime>2006-10-16T06:30:00-07:00</EndTime>
                <BusyType>Busy</BusyType>
                <CalendarEventDetails>
                  <ID>14B6414B0</ID>
                  <Subject>Meet with Contoso Account Executives</Subject>
                  <Location />
                  <IsMeeting>false</IsMeeting>
                  <IsRecurring>false</IsRecurring>
                  <IsException>false</IsException>
                  <IsReminderSet>false</IsReminderSet>
                  <IsPrivate>false</IsPrivate>
                </CalendarEventDetails>
              </CalendarEvent>
              <CalendarEvent>
                <StartTime>2006-10-16T07:00:00-07:00</StartTime>
                <EndTime>2006-10-16T08:00:00-07:00</EndTime>
                <BusyType>Busy</BusyType>
                <CalendarEventDetails>
                  <ID>E14B6414B0B</ID>
                  <Subject>Pick up my groceries</Subject>
                  <Location />
                  <IsMeeting>false</IsMeeting>
                  <IsRecurring>false</IsRecurring>
                  <IsException>false</IsException>
                  <IsReminderSet>false</IsReminderSet>
                  <IsPrivate>false</IsPrivate>
                </CalendarEventDetails>
              </CalendarEvent>
              <CalendarEvent>
                <StartTime>2006-10-16T09:40:00-07:00</StartTime>
                <EndTime>2006-10-16T10:10:00-07:00</EndTime>
                <BusyType>Busy</BusyType>
                <CalendarEventDetails>
                  <ID>14B6414B0B1</ID>
                  <Subject>Meet with doctor</Subject>
                  <Location>Kirkland</Location>
                  <IsMeeting>false</IsMeeting>
                  <IsRecurring>false</IsRecurring>
                  <IsException>false</IsException>
                  <IsReminderSet>false</IsReminderSet>
                  <IsPrivate>false</IsPrivate>
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
        <FreeBusyResponse>
          <ResponseMessage ResponseClass="Success">
            <ResponseCode>NoError</ResponseCode>
          </ResponseMessage>
          <FreeBusyView>
            <FreeBusyViewType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">FreeBusyMerged</FreeBusyViewType>
            <MergedFreeBusy xmlns="http://schemas.microsoft.com/exchange/services/2006/types">000000001100000000000000</MergedFreeBusy>
            <CalendarEventArray xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
              <CalendarEvent>
                <StartTime>2006-10-16T09:00:00-07:00</StartTime>
                <EndTime>2006-10-16T10:00:00-07:00</EndTime>
                <BusyType>Tentative</BusyType>
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
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="78e47-168">[FreeBusyResponse](freebusyresponse.md)の一意の要素に、ユーザーごとに利用可能時間情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="78e47-168">The availability information for each user appears in a unique [FreeBusyResponse](freebusyresponse.md) element.</span></span> <span data-ttu-id="78e47-169">**GetUserAvailability**操作の要求でのユーザーの順序は、応答内の各ユーザーの利用状況データの順序を決定します。</span><span class="sxs-lookup"><span data-stu-id="78e47-169">The order of users in the **GetUserAvailability** operation request determines the order of availability data for each user in the response.</span></span> 
  
<span data-ttu-id="78e47-170">エラーに戻りますクライアント管理者が指定した最大数よりも大きい場合は、クエリで定義されている時間内に予定の数です。</span><span class="sxs-lookup"><span data-stu-id="78e47-170">An error will be returned to the client if the number of appointments in the time period that is defined in the query is greater than the administrator-specified maximum number.</span></span> <span data-ttu-id="78e47-171">予定の既定の最大数は 10,000 の 1 つのインスタンスは、し、定期的なアイテムを展開します。</span><span class="sxs-lookup"><span data-stu-id="78e47-171">The default maximum number of appointments is 10,000 single instances and expanded recurrence items.</span></span> <span data-ttu-id="78e47-172">管理者のみがこのプロパティを構成することができます。</span><span class="sxs-lookup"><span data-stu-id="78e47-172">This property can be configured only by an administrator.</span></span>
  
<span data-ttu-id="78e47-173">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="78e47-173">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="78e47-174">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="78e47-174">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="78e47-175">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="78e47-175">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
    
- [<span data-ttu-id="78e47-176">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="78e47-176">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
    
- [<span data-ttu-id="78e47-177">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="78e47-177">FreeBusyResponse</span></span>](freebusyresponse.md)
    
- [<span data-ttu-id="78e47-178">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="78e47-178">ResponseMessage</span></span>](responsemessage.md)
    
- [<span data-ttu-id="78e47-179">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="78e47-179">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="78e47-180">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="78e47-180">FreeBusyView</span></span>](freebusyview.md)
    
- [<span data-ttu-id="78e47-181">FreeBusyViewType</span><span class="sxs-lookup"><span data-stu-id="78e47-181">FreeBusyViewType</span></span>](freebusyviewtype.md)
    
- [<span data-ttu-id="78e47-182">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="78e47-182">MergedFreeBusy</span></span>](mergedfreebusy.md)
    
- [<span data-ttu-id="78e47-183">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="78e47-183">CalendarEventArray</span></span>](calendareventarray.md)
    
- [<span data-ttu-id="78e47-184">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="78e47-184">CalendarEvent</span></span>](calendarevent.md)
    
- [<span data-ttu-id="78e47-185">開始時刻</span><span class="sxs-lookup"><span data-stu-id="78e47-185">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="78e47-186">終了時刻</span><span class="sxs-lookup"><span data-stu-id="78e47-186">EndTime</span></span>](endtime.md)
    
- [<span data-ttu-id="78e47-187">BusyType</span><span class="sxs-lookup"><span data-stu-id="78e47-187">BusyType</span></span>](busytype.md)
    
- [<span data-ttu-id="78e47-188">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="78e47-188">CalendarEventDetails</span></span>](calendareventdetails.md)
    
- [<span data-ttu-id="78e47-189">ID</span><span class="sxs-lookup"><span data-stu-id="78e47-189">ID</span></span>](id.md)
    
- [<span data-ttu-id="78e47-190">件名 (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="78e47-190">Subject (CalendarEventDetails)</span></span>](subject-calendareventdetails.md)
    
- [<span data-ttu-id="78e47-191">場所 (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="78e47-191">Location (CalendarEventDetails)</span></span>](location-calendareventdetails.md)
    
- [<span data-ttu-id="78e47-192">IsMeeting (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="78e47-192">IsMeeting (CalendarEventDetails)</span></span>](ismeeting-calendareventdetails.md)
    
- [<span data-ttu-id="78e47-193">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="78e47-193">IsRecurring (CalendarEventDetails)</span></span>](isrecurring-calendareventdetails.md)
    
- [<span data-ttu-id="78e47-194">IsException</span><span class="sxs-lookup"><span data-stu-id="78e47-194">IsException</span></span>](isexception.md)
    
- [<span data-ttu-id="78e47-195">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="78e47-195">IsReminderSet</span></span>](isreminderset.md)
    
- [<span data-ttu-id="78e47-196">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="78e47-196">IsPrivate</span></span>](isprivate.md)
    
- [<span data-ttu-id="78e47-197">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="78e47-197">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
    
- [<span data-ttu-id="78e47-198">タイムゾーン (可用性)</span><span class="sxs-lookup"><span data-stu-id="78e47-198">TimeZone (Availability)</span></span>](timezone-availability.md)
    
- [<span data-ttu-id="78e47-199">バイアス (UTC)</span><span class="sxs-lookup"><span data-stu-id="78e47-199">Bias (UTC)</span></span>](bias-utc.md)
    
- [<span data-ttu-id="78e47-200">StandardTime</span><span class="sxs-lookup"><span data-stu-id="78e47-200">StandardTime</span></span>](standardtime.md)
    
- [<span data-ttu-id="78e47-201">Bias</span><span class="sxs-lookup"><span data-stu-id="78e47-201">Bias</span></span>](bias.md)
    
- [<span data-ttu-id="78e47-202">時間</span><span class="sxs-lookup"><span data-stu-id="78e47-202">Time</span></span>](time.md)
    
- [<span data-ttu-id="78e47-203">DayOrder</span><span class="sxs-lookup"><span data-stu-id="78e47-203">DayOrder</span></span>](dayorder.md)
    
- [<span data-ttu-id="78e47-204">Month</span><span class="sxs-lookup"><span data-stu-id="78e47-204">Month</span></span>](month.md)
    
- [<span data-ttu-id="78e47-205">DayOfWeek (タイムゾーン)</span><span class="sxs-lookup"><span data-stu-id="78e47-205">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md)
    
- [<span data-ttu-id="78e47-206">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="78e47-206">DaylightTime</span></span>](daylighttime.md)
    
- [<span data-ttu-id="78e47-207">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="78e47-207">WorkingPeriodArray</span></span>](workingperiodarray.md)
    
- [<span data-ttu-id="78e47-208">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="78e47-208">WorkingPeriod</span></span>](workingperiod.md)
    
- [<span data-ttu-id="78e47-209">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="78e47-209">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md)
    
- [<span data-ttu-id="78e47-210">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="78e47-210">StartTimeInMinutes</span></span>](starttimeinminutes.md)
    
- [<span data-ttu-id="78e47-211">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="78e47-211">EndTimeInMinutes</span></span>](endtimeinminutes.md)
    
## <a name="see-also"></a><span data-ttu-id="78e47-212">関連項目</span><span class="sxs-lookup"><span data-stu-id="78e47-212">See also</span></span>

- [<span data-ttu-id="78e47-213">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="78e47-213">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="78e47-214">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="78e47-214">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
    


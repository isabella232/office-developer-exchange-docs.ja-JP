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
# <a name="getuseravailability-operation"></a>GetUserAvailability 操作

**GetUserAvailability** EWS の操作に関する情報を検索します。 
  
**GetUserAvailability**操作は、指定された期間内で一連のユーザー、会議室、およびリソースの可用性についての詳細な情報を提供します。 
  
## <a name="using-the-getuseravailability-operation"></a>GetUserAvailability 操作を使用します。

**GetUserAvailability**操作では、詳細情報の指定したレベルでの現在のユーザーの可用性の情報を提供します。 Outlook、Outlook Web Access、Outlook Mobile Access、およびその他のユーザーなどのクライアント アプリケーションは、要求されたユーザー情報を識別するのに SMTP アドレスを使用します。 
  
配布リスト内のメールボックスの数が 100 未満の id の最大数である限り、リストの各メンバーの空き時間情報のステータスを取得するために配布リストの展開を可用性サービスを**GetUserAvailability**操作を要求できます。 配布リストのメンバーの空き時間情報のステータスは、全体の配布リストの 1 つの空き時間情報のステータスにマージされます。 
  
クライアント アプリケーションの要求は、可用性のクエリの期間を指定します。 要求された情報の有効期間は 42 日です。 ユーザーの予定表は、予定または会議内と外部の両方のクエリの定義された期間には含まれている、予定が返されます。 
  
返される予定と会議の時間は、会議を要求しているクライアント アプリケーションと同じタイム ゾーンです。
  
可用性サービスは、各クライアントの要求を処理します。 サービスは、すべての定期的な予定を展開し、要求元のクライアント アクセス許可を持つが表示される予定表の詳細の最大数を返します。
  
> [!NOTE]
> 移動先のメールボックスが使用できないか、見つからない、 **MailRecipientNotFoundException**例外がスローされます。 クライアントは、Active Directory ドメイン サービス (AD DS) または Active Directory ディレクトリ サービスでメールの宛先が見つからないことを示すエラー メッセージを受信します。 
  
### <a name="getuseravailability-operation-soap-headers"></a>GetUserAvailability 操作の SOAP ヘッダー

**GetUserAvailability**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**Header**|**要素**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアントを偽装するユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |サーバーからのすべての応答に使用するタイム ゾーンを識別する SOAP ヘッダーを指定します。 サーバーから返されるすべての時間は、指定されたタイム ゾーンに変換されます。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="getuseravailability-request-example-get-availability-information"></a>GetUserAvailability 要求の例: 利用可能時間情報を取得します。

**GetUserAvailability**操作要求の次の例では、太平洋標準時タイム ゾーンで 2 人のユーザーの詳細な情報を取得する方法を示します。 
  
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

[SuggestionsViewOptions](suggestionsviewoptions.md)要素を使用して提案された会議を取得する方法の詳細については、EWS 仮想ディレクトリ内のスキーマを参照してください。 
  
要求 SOAP 本体にはには、次の要素が含まれています。
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
    
- [タイムゾーン (可用性)](timezone-availability.md)
    
- [バイアス (UTC)](bias-utc.md)
    
- [StandardTime](standardtime.md)
    
- [Bias](bias.md)
    
- [時間](time.md)
    
- [DayOrder](dayorder.md)
    
- [Month](month.md)
    
- [DayOfWeek (タイムゾーン)](dayofweek-timezone.md)
    
- [DaylightTime](daylighttime.md)
    
- [MailboxDataArray](mailboxdataarray.md)
    
- [MailboxData](mailboxdata.md)
    
- [電子メール (EmailAddressType)](email-emailaddresstype.md)
    
- [アドレス (文字列)](address-string.md)
    
- [AttendeeType](attendeetype.md)
    
- [ExcludeConflicts](excludeconflicts.md)
    
- [FreeBusyViewOptions](freebusyviewoptions.md)
    
- [時間](timewindow.md)
    
- [開始時刻](starttime.md)
    
- [終了時刻](endtime.md)
    
## <a name="successful-getuseravailability-operation-response"></a>GetUserAvailability 操作の成功の応答

成功した要求への応答、 **GetUserAvailability**操作の例を次に示します。 
  
> [!NOTE]
> 予定表イベントの識別子は、読みやすさを保持するために短縮されています。 
  
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

[FreeBusyResponse](freebusyresponse.md)の一意の要素に、ユーザーごとに利用可能時間情報が表示されます。 **GetUserAvailability**操作の要求でのユーザーの順序は、応答内の各ユーザーの利用状況データの順序を決定します。 
  
エラーに戻りますクライアント管理者が指定した最大数よりも大きい場合は、クエリで定義されている時間内に予定の数です。 予定の既定の最大数は 10,000 の 1 つのインスタンスは、し、定期的なアイテムを展開します。 管理者のみがこのプロパティを構成することができます。
  
次の要素は、応答で使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
    
- [FreeBusyResponseArray](freebusyresponsearray.md)
    
- [FreeBusyResponse](freebusyresponse.md)
    
- [ResponseMessage](responsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [FreeBusyView](freebusyview.md)
    
- [FreeBusyViewType](freebusyviewtype.md)
    
- [MergedFreeBusy](mergedfreebusy.md)
    
- [CalendarEventArray](calendareventarray.md)
    
- [CalendarEvent](calendarevent.md)
    
- [開始時刻](starttime.md)
    
- [終了時刻](endtime.md)
    
- [BusyType](busytype.md)
    
- [CalendarEventDetails](calendareventdetails.md)
    
- [ID](id.md)
    
- [件名 (CalendarEventDetails)](subject-calendareventdetails.md)
    
- [場所 (CalendarEventDetails)](location-calendareventdetails.md)
    
- [IsMeeting (CalendarEventDetails)](ismeeting-calendareventdetails.md)
    
- [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md)
    
- [IsException](isexception.md)
    
- [IsReminderSet](isreminderset.md)
    
- [IsPrivate](isprivate.md)
    
- [WorkingHours](workinghours-ex15websvcsotherref.md)
    
- [タイムゾーン (可用性)](timezone-availability.md)
    
- [バイアス (UTC)](bias-utc.md)
    
- [StandardTime](standardtime.md)
    
- [Bias](bias.md)
    
- [時間](time.md)
    
- [DayOrder](dayorder.md)
    
- [Month](month.md)
    
- [DayOfWeek (タイムゾーン)](dayofweek-timezone.md)
    
- [DaylightTime](daylighttime.md)
    
- [WorkingPeriodArray](workingperiodarray.md)
    
- [WorkingPeriod](workingperiod.md)
    
- [DayOfWeek (WorkingPeriod)](dayofweek-workingperiod.md)
    
- [StartTimeInMinutes](starttimeinminutes.md)
    
- [EndTimeInMinutes](endtimeinminutes.md)
    
## <a name="see-also"></a>関連項目

- [Exchange での EWS の操作](ews-operations-in-exchange.md)
    
- [ユーザーの状態を取得します。](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
    


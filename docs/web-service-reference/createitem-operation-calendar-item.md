---
title: CreateItem 操作 (予定表アイテム)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: aa4a7c94-f668-4bd2-8079-c855f6ab17e1
description: CreateItem 操作は、Exchange ストア内の予定表アイテムを作成します。
ms.openlocfilehash: c2174dd806b922e640ef7afcab32b98c67c65b41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759833"
---
# <a name="createitem-operation-calendar-item"></a>CreateItem 操作 (予定表アイテム)

CreateItem 操作は、Exchange ストア内の予定表アイテムを作成します。
  
## <a name="remarks"></a>備考

CreateItem 操作は、予定、会議、および会議出席依頼を作成します。 出席者なしの予定表アイテムが作成されると、予定とみなされます。 出席者が指定されている場合、予定表アイテムは会議です。 CreateItem 操作を使用して会議を作成するとき、会議出席依頼は、会議出席依頼を送信するのには、SendMeetingInvitations 属性が設定されている場合に特定の出席者に自動的に送信します。
  
## <a name="createitem-calendar-item-request-example"></a>Createitem メソッド (予定表アイテム) の要求の例

### <a name="description"></a>説明

CreateItem 要求の次の例では、2 つの必須出席者に会議を作成する方法を示します。 この要求では、2 つの出席者に会議出席依頼を送信します。
  
### <a name="code"></a>コード

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                SendMeetingInvitations="SendToAllAndSaveCopy" >
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar"/>
      </SavedItemFolderId>
      <Items>
        <t:CalendarItem xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Subject>Planning Meeting</Subject>
          <Body BodyType="Text">Plan the agenda for next week's meeting.</Body>
          <ReminderIsSet>true</ReminderIsSet>
          <ReminderMinutesBeforeStart>60</ReminderMinutesBeforeStart>
          <Start>2006-11-02T14:00:00</Start>
          <End>2006-11-02T15:00:00</End>
          <IsAllDayEvent>false</IsAllDayEvent>
          <LegacyFreeBusyStatus>Busy</LegacyFreeBusyStatus>
          <Location>Conference Room 721</Location>
          <RequiredAttendees>
            <Attendee>
              <Mailbox>
                <EmailAddress>User1@example.com</EmailAddress>
              </Mailbox>
            </Attendee>
            <Attendee>
              <Mailbox>
                <EmailAddress>User2@example.com</EmailAddress>
              </Mailbox>
            </Attendee>
          </RequiredAttendees>
        </t:CalendarItem>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

会議出席依頼に応答する方法の例は、 [CreateItem 操作 (会議出席依頼)](createitem-operation-meeting-request.md)のトピックを参照してください。 
  
### <a name="request-elements"></a>要素を要求します。

次の要素は、要求で使用されます。
  
- [CreateItem](createitem.md)
    
- [SavedItemFolderId](saveditemfolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [アイテム (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [カレンダー項目](calendaritem.md)
    
- [Subject](subject.md)
    
- [Body/本文](body.md)
    
- [ReminderIsSet](reminderisset.md)
    
- [ReminderMinutesBeforeStart](reminderminutesbeforestart.md)
    
- [Start](start.md)
    
- [終わり](end-ex15websvcsotherref.md)
    
- [IsAllDayEvent](isalldayevent.md)
    
- [LegacyFreeBusyStatus](legacyfreebusystatus.md)
    
- [場所](location.md)
    
- [RequiredAttendees](requiredattendees.md)
    
- [Attendee](attendee.md)
    
- [メールボックス](mailbox.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
## <a name="successful-createitem-calendar-item-response"></a>Createitem メソッドが成功した (予定表アイテム) の応答

### <a name="description"></a>説明

次の使用例は、CreateItem 要求に正常な応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAAlAFV" ChangeKey="DwAAABYA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

[ItemId](itemid.md)要素の**Id**と**変更キー**属性は、読みやすさを保持するために短縮されています。 
  
### <a name="successful-response-elements"></a>正常な応答の要素

次の要素は、応答で使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items](items.md)
    
- [カレンダー項目](calendaritem.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>関連項目




  [CreateItem 操作](createitem-operation.md)


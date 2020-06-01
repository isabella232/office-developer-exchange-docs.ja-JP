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
description: CreateItem 操作は、Exchange ストアに予定表アイテムを作成します。
ms.openlocfilehash: 535edf9fe567bc3063a5b853f01d604ea4c7eb95
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457502"
---
# <a name="createitem-operation-calendar-item"></a>CreateItem 操作 (予定表アイテム)

CreateItem 操作は、Exchange ストアに予定表アイテムを作成します。
  
## <a name="remarks"></a>注釈

CreateItem 操作は、予定、会議、および会議出席依頼を作成します。 予定表アイテムが出席者なしで作成された場合は、予定と見なされます。 出席者が指定されている場合、予定表アイテムは会議です。 CreateItem 操作を使用して会議を作成する場合、会議出席依頼を送信するように Sendmeeting の招待属性が設定されている場合、会議出席依頼は特定の出席者に自動的に送信されます。
  
## <a name="createitem-calendar-item-request-example"></a>CreateItem (予定表アイテム) の要求の例

### <a name="description"></a>説明

次の CreateItem 要求の例は、2つの必須出席者を含む会議を作成する方法を示しています。 この要求は、2人の出席者に会議出席依頼を送信します。
  
### <a name="code"></a>コード

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                SendMeetingInvitations="SendToAllAndSaveCopy" >
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar"/>
      </SavedItemFolderId>
      <Items>
        <t:CalendarItem xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

会議出席依頼に返信する方法の例については、「 [CreateItem 操作 (会議出席依頼)](createitem-operation-meeting-request.md) 」を参照してください。 
  
### <a name="request-elements"></a>Request 要素

要求では、次の要素が使用されます。
  
- [CreateItem](createitem.md)
    
- [SavedItemFolderId](saveditemfolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [アイテム (非 Emptyarrayofallitemstype)](items-nonemptyarrayofallitemstype.md)
    
- [CalendarItem](calendaritem.md)
    
- [[件名]](subject.md)
    
- [Body](body.md)
    
- [ReminderIsSet](reminderisset.md)
    
- [ReminderMinutesBeforeStart](reminderminutesbeforestart.md)
    
- [開始](start.md)
    
- [終わり](end-ex15websvcsotherref.md)
    
- [IsAllDayEvent](isalldayevent.md)
    
- [LegacyFreeBusyStatus](legacyfreebusystatus.md)
    
- [場所](location.md)
    
- [RequiredAttendees](requiredattendees.md)
    
- [出席者](attendee.md)
    
- [メールボックス](mailbox.md)
    
- [EmailAddress (非 Emptystringtype)](emailaddress-nonemptystringtype.md)
    
## <a name="successful-createitem-calendar-item-response"></a>成功した CreateItem (予定表アイテム) の応答

### <a name="description"></a>説明

次の例は、CreateItem 要求に対する正常な応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

[ItemId](itemid.md)要素**Id**および**changekey**属性は読みやすいように短縮されています。 
  
### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items](items.md)
    
- [CalendarItem](calendaritem.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>関連項目




  [CreateItem 操作](createitem-operation.md)


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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457502"
---
# <a name="createitem-operation-calendar-item"></a><span data-ttu-id="27635-103">CreateItem 操作 (予定表アイテム)</span><span class="sxs-lookup"><span data-stu-id="27635-103">CreateItem operation (calendar item)</span></span>

<span data-ttu-id="27635-104">CreateItem 操作は、Exchange ストアに予定表アイテムを作成します。</span><span class="sxs-lookup"><span data-stu-id="27635-104">The CreateItem operation creates calendar items in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="27635-105">注釈</span><span class="sxs-lookup"><span data-stu-id="27635-105">Remarks</span></span>

<span data-ttu-id="27635-106">CreateItem 操作は、予定、会議、および会議出席依頼を作成します。</span><span class="sxs-lookup"><span data-stu-id="27635-106">The CreateItem operation creates appointments, meetings, and meeting requests.</span></span> <span data-ttu-id="27635-107">予定表アイテムが出席者なしで作成された場合は、予定と見なされます。</span><span class="sxs-lookup"><span data-stu-id="27635-107">If a calendar item is created without attendees, it is considered an appointment.</span></span> <span data-ttu-id="27635-108">出席者が指定されている場合、予定表アイテムは会議です。</span><span class="sxs-lookup"><span data-stu-id="27635-108">If attendees are specified, the calendar item is a meeting.</span></span> <span data-ttu-id="27635-109">CreateItem 操作を使用して会議を作成する場合、会議出席依頼を送信するように Sendmeeting の招待属性が設定されている場合、会議出席依頼は特定の出席者に自動的に送信されます。</span><span class="sxs-lookup"><span data-stu-id="27635-109">When a meeting is created by using the CreateItem operation, meeting requests are automatically sent to the identified attendees if the SendMeetingInvitations attribute is set to send the meeting requests.</span></span>
  
## <a name="createitem-calendar-item-request-example"></a><span data-ttu-id="27635-110">CreateItem (予定表アイテム) の要求の例</span><span class="sxs-lookup"><span data-stu-id="27635-110">CreateItem (Calendar Item) request example</span></span>

### <a name="description"></a><span data-ttu-id="27635-111">Description</span><span class="sxs-lookup"><span data-stu-id="27635-111">Description</span></span>

<span data-ttu-id="27635-112">次の CreateItem 要求の例は、2つの必須出席者を含む会議を作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="27635-112">The following example of a CreateItem request shows how to create a meeting with two required attendees.</span></span> <span data-ttu-id="27635-113">この要求は、2人の出席者に会議出席依頼を送信します。</span><span class="sxs-lookup"><span data-stu-id="27635-113">This request will send the meeting requests to the two attendees.</span></span>
  
### <a name="code"></a><span data-ttu-id="27635-114">コード</span><span class="sxs-lookup"><span data-stu-id="27635-114">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="27635-115">コメント</span><span class="sxs-lookup"><span data-stu-id="27635-115">Comments</span></span>

<span data-ttu-id="27635-116">会議出席依頼に返信する方法の例については、「 [CreateItem 操作 (会議出席依頼)](createitem-operation-meeting-request.md) 」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27635-116">For an example of how to respond to a meeting request, see the [CreateItem operation (meeting request)](createitem-operation-meeting-request.md) topic.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="27635-117">Request 要素</span><span class="sxs-lookup"><span data-stu-id="27635-117">Request elements</span></span>

<span data-ttu-id="27635-118">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="27635-118">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="27635-119">CreateItem</span><span class="sxs-lookup"><span data-stu-id="27635-119">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="27635-120">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="27635-120">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="27635-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="27635-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="27635-122">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="27635-122">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="27635-123">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="27635-123">CalendarItem</span></span>](calendaritem.md)
    
- [<span data-ttu-id="27635-124">件名</span><span class="sxs-lookup"><span data-stu-id="27635-124">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="27635-125">Body</span><span class="sxs-lookup"><span data-stu-id="27635-125">Body</span></span>](body.md)
    
- [<span data-ttu-id="27635-126">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="27635-126">ReminderIsSet</span></span>](reminderisset.md)
    
- [<span data-ttu-id="27635-127">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="27635-127">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md)
    
- [<span data-ttu-id="27635-128">開始</span><span class="sxs-lookup"><span data-stu-id="27635-128">Start</span></span>](start.md)
    
- [<span data-ttu-id="27635-129">終わり</span><span class="sxs-lookup"><span data-stu-id="27635-129">End </span></span>](end-ex15websvcsotherref.md)
    
- [<span data-ttu-id="27635-130">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="27635-130">IsAllDayEvent</span></span>](isalldayevent.md)
    
- [<span data-ttu-id="27635-131">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="27635-131">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md)
    
- [<span data-ttu-id="27635-132">場所</span><span class="sxs-lookup"><span data-stu-id="27635-132">Location</span></span>](location.md)
    
- [<span data-ttu-id="27635-133">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="27635-133">RequiredAttendees</span></span>](requiredattendees.md)
    
- [<span data-ttu-id="27635-134">出席者</span><span class="sxs-lookup"><span data-stu-id="27635-134">Attendee</span></span>](attendee.md)
    
- [<span data-ttu-id="27635-135">メールボックス</span><span class="sxs-lookup"><span data-stu-id="27635-135">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="27635-136">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="27635-136">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
## <a name="successful-createitem-calendar-item-response"></a><span data-ttu-id="27635-137">成功した CreateItem (予定表アイテム) の応答</span><span class="sxs-lookup"><span data-stu-id="27635-137">Successful CreateItem (Calendar Item) Response</span></span>

### <a name="description"></a><span data-ttu-id="27635-138">Description</span><span class="sxs-lookup"><span data-stu-id="27635-138">Description</span></span>

<span data-ttu-id="27635-139">次の例は、CreateItem 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="27635-139">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="27635-140">コード</span><span class="sxs-lookup"><span data-stu-id="27635-140">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="27635-141">コメント</span><span class="sxs-lookup"><span data-stu-id="27635-141">Comments</span></span>

<span data-ttu-id="27635-142">[ItemId](itemid.md)要素**Id**および**changekey**属性は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="27635-142">The [ItemId](itemid.md) element **Id** and **ChangeKey** attributes have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="27635-143">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="27635-143">Successful response elements</span></span>

<span data-ttu-id="27635-144">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="27635-144">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="27635-145">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="27635-145">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="27635-146">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="27635-146">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="27635-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="27635-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="27635-148">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="27635-148">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="27635-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="27635-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="27635-150">Items</span><span class="sxs-lookup"><span data-stu-id="27635-150">Items</span></span>](items.md)
    
- [<span data-ttu-id="27635-151">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="27635-151">CalendarItem</span></span>](calendaritem.md)
    
- [<span data-ttu-id="27635-152">ItemId</span><span class="sxs-lookup"><span data-stu-id="27635-152">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="27635-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="27635-153">See also</span></span>



[<span data-ttu-id="27635-154">CreateItem 操作</span><span class="sxs-lookup"><span data-stu-id="27635-154">CreateItem operation</span></span>](createitem-operation.md)


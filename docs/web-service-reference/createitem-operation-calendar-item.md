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
# <a name="createitem-operation-calendar-item"></a><span data-ttu-id="399ba-103">CreateItem 操作 (予定表アイテム)</span><span class="sxs-lookup"><span data-stu-id="399ba-103">CreateItem operation (calendar item)</span></span>

<span data-ttu-id="399ba-104">CreateItem 操作は、Exchange ストア内の予定表アイテムを作成します。</span><span class="sxs-lookup"><span data-stu-id="399ba-104">The CreateItem operation creates calendar items in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="399ba-105">備考</span><span class="sxs-lookup"><span data-stu-id="399ba-105">Remarks</span></span>

<span data-ttu-id="399ba-106">CreateItem 操作は、予定、会議、および会議出席依頼を作成します。</span><span class="sxs-lookup"><span data-stu-id="399ba-106">The CreateItem operation creates appointments, meetings, and meeting requests.</span></span> <span data-ttu-id="399ba-107">出席者なしの予定表アイテムが作成されると、予定とみなされます。</span><span class="sxs-lookup"><span data-stu-id="399ba-107">If a calendar item is created without attendees, it is considered an appointment.</span></span> <span data-ttu-id="399ba-108">出席者が指定されている場合、予定表アイテムは会議です。</span><span class="sxs-lookup"><span data-stu-id="399ba-108">If attendees are specified, the calendar item is a meeting.</span></span> <span data-ttu-id="399ba-109">CreateItem 操作を使用して会議を作成するとき、会議出席依頼は、会議出席依頼を送信するのには、SendMeetingInvitations 属性が設定されている場合に特定の出席者に自動的に送信します。</span><span class="sxs-lookup"><span data-stu-id="399ba-109">When a meeting is created by using the CreateItem operation, meeting requests are automatically sent to the identified attendees if the SendMeetingInvitations attribute is set to send the meeting requests.</span></span>
  
## <a name="createitem-calendar-item-request-example"></a><span data-ttu-id="399ba-110">Createitem メソッド (予定表アイテム) の要求の例</span><span class="sxs-lookup"><span data-stu-id="399ba-110">CreateItem (Calendar Item) request example</span></span>

### <a name="description"></a><span data-ttu-id="399ba-111">説明</span><span class="sxs-lookup"><span data-stu-id="399ba-111">Description</span></span>

<span data-ttu-id="399ba-112">CreateItem 要求の次の例では、2 つの必須出席者に会議を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="399ba-112">The following example of a CreateItem request shows how to create a meeting with two required attendees.</span></span> <span data-ttu-id="399ba-113">この要求では、2 つの出席者に会議出席依頼を送信します。</span><span class="sxs-lookup"><span data-stu-id="399ba-113">This request will send the meeting requests to the two attendees.</span></span>
  
### <a name="code"></a><span data-ttu-id="399ba-114">コード</span><span class="sxs-lookup"><span data-stu-id="399ba-114">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="399ba-115">コメント</span><span class="sxs-lookup"><span data-stu-id="399ba-115">Comments</span></span>

<span data-ttu-id="399ba-116">会議出席依頼に応答する方法の例は、 [CreateItem 操作 (会議出席依頼)](createitem-operation-meeting-request.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="399ba-116">For an example of how to respond to a meeting request, see the [CreateItem operation (meeting request)](createitem-operation-meeting-request.md) topic.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="399ba-117">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="399ba-117">Request elements</span></span>

<span data-ttu-id="399ba-118">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="399ba-118">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="399ba-119">CreateItem</span><span class="sxs-lookup"><span data-stu-id="399ba-119">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="399ba-120">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="399ba-120">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="399ba-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="399ba-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="399ba-122">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="399ba-122">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="399ba-123">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="399ba-123">CalendarItem</span></span>](calendaritem.md)
    
- [<span data-ttu-id="399ba-124">Subject</span><span class="sxs-lookup"><span data-stu-id="399ba-124">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="399ba-125">Body/本文</span><span class="sxs-lookup"><span data-stu-id="399ba-125">Body</span></span>](body.md)
    
- [<span data-ttu-id="399ba-126">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="399ba-126">ReminderIsSet</span></span>](reminderisset.md)
    
- [<span data-ttu-id="399ba-127">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="399ba-127">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md)
    
- [<span data-ttu-id="399ba-128">Start</span><span class="sxs-lookup"><span data-stu-id="399ba-128">Start</span></span>](start.md)
    
- [<span data-ttu-id="399ba-129">終わり</span><span class="sxs-lookup"><span data-stu-id="399ba-129">End </span></span>](end-ex15websvcsotherref.md)
    
- [<span data-ttu-id="399ba-130">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="399ba-130">IsAllDayEvent</span></span>](isalldayevent.md)
    
- [<span data-ttu-id="399ba-131">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="399ba-131">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md)
    
- [<span data-ttu-id="399ba-132">場所</span><span class="sxs-lookup"><span data-stu-id="399ba-132">Location</span></span>](location.md)
    
- [<span data-ttu-id="399ba-133">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="399ba-133">RequiredAttendees</span></span>](requiredattendees.md)
    
- [<span data-ttu-id="399ba-134">Attendee</span><span class="sxs-lookup"><span data-stu-id="399ba-134">Attendee</span></span>](attendee.md)
    
- [<span data-ttu-id="399ba-135">メールボックス</span><span class="sxs-lookup"><span data-stu-id="399ba-135">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="399ba-136">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="399ba-136">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
## <a name="successful-createitem-calendar-item-response"></a><span data-ttu-id="399ba-137">Createitem メソッドが成功した (予定表アイテム) の応答</span><span class="sxs-lookup"><span data-stu-id="399ba-137">Successful CreateItem (Calendar Item) Response</span></span>

### <a name="description"></a><span data-ttu-id="399ba-138">説明</span><span class="sxs-lookup"><span data-stu-id="399ba-138">Description</span></span>

<span data-ttu-id="399ba-139">次の使用例は、CreateItem 要求に正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="399ba-139">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="399ba-140">コード</span><span class="sxs-lookup"><span data-stu-id="399ba-140">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="399ba-141">コメント</span><span class="sxs-lookup"><span data-stu-id="399ba-141">Comments</span></span>

<span data-ttu-id="399ba-142">[ItemId](itemid.md)要素の**Id**と**変更キー**属性は、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="399ba-142">The [ItemId](itemid.md) element **Id** and **ChangeKey** attributes have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="399ba-143">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="399ba-143">Successful response elements</span></span>

<span data-ttu-id="399ba-144">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="399ba-144">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="399ba-145">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="399ba-145">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="399ba-146">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="399ba-146">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="399ba-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="399ba-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="399ba-148">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="399ba-148">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="399ba-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="399ba-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="399ba-150">Items</span><span class="sxs-lookup"><span data-stu-id="399ba-150">Items</span></span>](items.md)
    
- [<span data-ttu-id="399ba-151">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="399ba-151">CalendarItem</span></span>](calendaritem.md)
    
- [<span data-ttu-id="399ba-152">ItemId</span><span class="sxs-lookup"><span data-stu-id="399ba-152">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="399ba-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="399ba-153">See also</span></span>



<span data-ttu-id="399ba-154">
  [CreateItem 操作](createitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="399ba-154">[CreateItem operation](createitem-operation.md)</span></span>


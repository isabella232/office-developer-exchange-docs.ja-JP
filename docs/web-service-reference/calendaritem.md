---
title: CalendarItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarItem
api_type:
- schema
ms.assetid: b0c1fd27-b6da-46e5-88b8-88f00c71ba80
description: CalendarItem 要素は、Exchange 予定表アイテムを表します。
ms.openlocfilehash: b29141470d157ef5bd67be06a1e1fa1c9536b042
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529484"
---
# <a name="calendaritem"></a><span data-ttu-id="909c2-103">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="909c2-103">CalendarItem</span></span>

<span data-ttu-id="909c2-104">**Calendaritem**要素は、Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-104">The **CalendarItem** element represents an Exchange calendar item.</span></span> 
  
```XML
<CalendarItem>
   <MimeContent/>
   <ItemId/>
   <ParentFolderId/>
   <ItemClass/>
   <Subject/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <DateTimeReceived/>
   <Size/>
   <Categories/>
   <InReplyTo/>
   <IsSubmitted/>
   <IsDraft/>
   <IsFromMe/>
   <IsResend/>
   <IsUnmodified/>
   <InternetMessageHeaders/>
   <DateTimeSent/>
   <DateTimeCreated/>
   <ResponseObjects/>
   <ReminderDueBy/>
   <ReminderIsSet/>
   <ReminderMinutesBeforeStart/>
   <DisplayCc/>
   <DisplayTo/>
   <HasAttachments/>
   <ExtendedProperty/>
   <Culture/>
   <Start/>
   <End/>
   <OriginalStart/>
   <IsAllDayEvent/>
   <LegacyFreeBusyStatus/>
   <Location/>
   <When/>
   <IsMeeting/>
   <IsCancelled/>
   <IsRecurring/>
   <MeetingRequestWasSent/>
   <IsResponseRequested/>
   <CalendarItemType/>
   <MyResponseType/>
   <Organizer/>
   <RequiredAttendees/>
   <OptionalAttendees/>
   <Resources/>
   <ConflictingMeetingCount/>
   <AdjacentMeetingCount/>
   <ConflictingMeetings/>
   <AdjacentMeetings/>
   <Duration/>
   <TimeZone/>
   <AppointmentReplyTime/>
   <AppointmentSequenceNumber/>
   <AppointmentState/>
   <Recurrence/>
   <FirstOccurrence/>
   <LastOccurrence/>
   <ModifiedOccurrences/>
   <DeletedOccurrences/>
   <MeetingTimeZone/>
   <StartTimeZone/>
   <EndTimeZone/>
   <ConferenceType/>
   <AllowNewTimeProposal/>
   <IsOnlineMeeting/>
   <MeetingWorkspaceUrl/>
   <NetShowUrl/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</CalendarItem>
```

 <span data-ttu-id="909c2-105">**CalendarItemType**</span><span class="sxs-lookup"><span data-stu-id="909c2-105">**CalendarItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="909c2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="909c2-106">Attributes and elements</span></span>

<span data-ttu-id="909c2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="909c2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="909c2-108">属性</span><span class="sxs-lookup"><span data-stu-id="909c2-108">Attributes</span></span>

<span data-ttu-id="909c2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="909c2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="909c2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="909c2-110">Child elements</span></span>

|<span data-ttu-id="909c2-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="909c2-111">**Element**</span></span>|<span data-ttu-id="909c2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="909c2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="909c2-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="909c2-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="909c2-114">Base64Binary 形式で表されるオブジェクトのネイティブな汎用インターネットメール内線 (MIME) ストリームが保存されています。</span><span class="sxs-lookup"><span data-stu-id="909c2-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="909c2-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="909c2-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="909c2-116">Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="909c2-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="909c2-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="909c2-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="909c2-118">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-118">Represents the identifier of the parent folder that contains the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="909c2-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="909c2-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="909c2-120">アイテムのメッセージクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-120">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-121">件名</span><span class="sxs-lookup"><span data-stu-id="909c2-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="909c2-122">Exchange ストアアイテムおよび応答オブジェクトの件名を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="909c2-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="909c2-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="909c2-124">アイテムの秘密度レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-124">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-125">Body</span><span class="sxs-lookup"><span data-stu-id="909c2-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="909c2-126">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-126">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="909c2-127">Attachments</span><span class="sxs-lookup"><span data-stu-id="909c2-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="909c2-128">Exchange ストア内のアイテムに添付されているアイテムまたはファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="909c2-128">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="909c2-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="909c2-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="909c2-130">メールボックス内のアイテムが受信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-130">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="909c2-131">Size</span><span class="sxs-lookup"><span data-stu-id="909c2-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="909c2-132">アイテムのサイズ (バイト単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-132">Represents the size in bytes of an item.</span></span> <span data-ttu-id="909c2-133">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="909c2-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="909c2-134">Categories</span><span class="sxs-lookup"><span data-stu-id="909c2-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="909c2-135">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-135">Represents a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="909c2-136">Importance</span><span class="sxs-lookup"><span data-stu-id="909c2-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="909c2-137">アイテムの重要度について説明します。</span><span class="sxs-lookup"><span data-stu-id="909c2-137">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="909c2-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="909c2-139">このアイテムが返信であるアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-139">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="909c2-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="909c2-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="909c2-141">アイテムが送信トレイの既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="909c2-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="909c2-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="909c2-143">アイテムがまだ送信されていないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-143">Indicates whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="909c2-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="909c2-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="909c2-145">ユーザーが自分にアイテムを送信したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-145">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="909c2-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="909c2-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="909c2-147">アイテムが以前に送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="909c2-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="909c2-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="909c2-149">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="909c2-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="909c2-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="909c2-151">メールボックス内のアイテムに含まれるすべてのインターネットメッセージヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-151">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="909c2-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="909c2-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="909c2-153">メールボックス内のアイテムが送信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="909c2-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="909c2-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="909c2-155">メールボックス内の特定のアイテムが作成された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="909c2-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="909c2-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="909c2-157">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="909c2-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="909c2-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="909c2-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="909c2-159">イベントが発生した日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="909c2-160">これは、アラームがいつ表示されるかを決定するために[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="909c2-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="909c2-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="909c2-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="909c2-162">Exchange ストア内のアイテムにアラームが設定されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="909c2-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="909c2-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="909c2-164">アラームが表示されるイベントの前の時間 (分単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="909c2-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="909c2-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="909c2-166">[Cc] 行の内容として使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-166">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="909c2-167">これは、すべての Cc 受信者表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="909c2-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="909c2-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="909c2-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="909c2-169">To 行の内容として使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-169">Represents the display string that is used for the contents of the To line.</span></span> <span data-ttu-id="909c2-170">これは、すべての受信者の表示名の連結文字列です。</span><span class="sxs-lookup"><span data-stu-id="909c2-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="909c2-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="909c2-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="909c2-172">アイテムに少なくとも1つの添付ファイルがある場合に**true**に設定されるプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="909c2-173">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="909c2-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="909c2-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="909c2-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="909c2-175">フォルダーとアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="909c2-175">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="909c2-176">Culture</span><span class="sxs-lookup"><span data-stu-id="909c2-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="909c2-177">メールボックス内の特定のアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-177">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="909c2-178">UID</span><span class="sxs-lookup"><span data-stu-id="909c2-178">UID</span></span>](uid.md) <br/> |<span data-ttu-id="909c2-179">予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="909c2-179">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-180">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="909c2-180">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="909c2-181">定期的な予定表アイテムの特定のインスタンスを識別するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="909c2-181">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-182">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="909c2-182">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="909c2-183">ICalendar オブジェクトのインスタンスが作成された日付と時刻を示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-183">Indicates the date and time that an instance of a iCalendar object was created.</span></span>  <br/> |
|[<span data-ttu-id="909c2-184">開始</span><span class="sxs-lookup"><span data-stu-id="909c2-184">Start</span></span>](start.md) <br/> |<span data-ttu-id="909c2-185">予定表アイテムの開始を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-185">Represents the start of a calendar item.</span></span> <span data-ttu-id="909c2-186">この要素は、予定表アイテムの1回だけに適用されます。</span><span class="sxs-lookup"><span data-stu-id="909c2-186">This element only applies to a single occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-187">終わり</span><span class="sxs-lookup"><span data-stu-id="909c2-187">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="909c2-188">期間の最後の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-188">Represents the end of a duration.</span></span> <span data-ttu-id="909c2-189">この要素は、予定表アイテムの1回だけに適用されます。</span><span class="sxs-lookup"><span data-stu-id="909c2-189">This element only applies to a single occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-190">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="909c2-190">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="909c2-191">予定表アイテムの元の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-191">Represents the original start time of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-192">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="909c2-192">IsAllDayEvent</span></span>](isalldayevent.md) <br/> |<span data-ttu-id="909c2-193">予定表アイテムまたは会議出席依頼が終日イベントを表しているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-193">Indicates whether a calendar item or meeting request represents an all-day event.</span></span>  <br/> |
|[<span data-ttu-id="909c2-194">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="909c2-194">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md) <br/> |<span data-ttu-id="909c2-195">予定表アイテムの空き時間状態を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-195">Represents the free/busy status of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-196">場所</span><span class="sxs-lookup"><span data-stu-id="909c2-196">Location</span></span>](location.md) <br/> |<span data-ttu-id="909c2-197">会議または予定の場所を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-197">Represents the location of a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="909c2-198">When</span><span class="sxs-lookup"><span data-stu-id="909c2-198">When</span></span>](when.md) <br/> |<span data-ttu-id="909c2-199">予定表アイテムがいつ発生するかについての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="909c2-199">Provides information about when a calendar item occurs.</span></span>  <br/> |
|[<span data-ttu-id="909c2-200">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="909c2-200">IsMeeting</span></span>](ismeeting.md) <br/> |<span data-ttu-id="909c2-201">予定表アイテムが会議または予定であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-201">Indicates whether the calendar item is a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="909c2-202">IsCancelled</span><span class="sxs-lookup"><span data-stu-id="909c2-202">IsCancelled</span></span>](iscancelled.md) <br/> |<span data-ttu-id="909c2-203">予定または会議がキャンセルされたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-203">Indicates whether an appointment or meeting has been canceled.</span></span>  <br/> |
|[<span data-ttu-id="909c2-204">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="909c2-204">IsRecurring</span></span>](isrecurring.md) <br/> |<span data-ttu-id="909c2-205">予定表アイテムが定期的なアイテムの一部であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-205">Indicates whether a calendar item is part of a recurring item.</span></span> <span data-ttu-id="909c2-206">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="909c2-206">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="909c2-207">MeetingRequestWasSent</span><span class="sxs-lookup"><span data-stu-id="909c2-207">MeetingRequestWasSent</span></span>](meetingrequestwassent.md) <br/> |<span data-ttu-id="909c2-208">出席依頼が出席者に送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-208">Indicates whether a meeting request has been sent to requested attendees.</span></span>  <br/> |
|[<span data-ttu-id="909c2-209">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="909c2-209">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="909c2-210">アイテムへの応答が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-210">Indicates whether a response to an item is required.</span></span>  <br/> |
|[<span data-ttu-id="909c2-211">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="909c2-211">CalendarItemType</span></span>](calendaritemtype.md) <br/> |<span data-ttu-id="909c2-212">予定表アイテムの発生の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-212">Represents the occurrence type of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-213">MyResponseType</span><span class="sxs-lookup"><span data-stu-id="909c2-213">MyResponseType</span></span>](myresponsetype.md) <br/> |<span data-ttu-id="909c2-214">予定表アイテムの状態または応答を含みます。</span><span class="sxs-lookup"><span data-stu-id="909c2-214">Contains the status of or response to a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-215">Organizer</span><span class="sxs-lookup"><span data-stu-id="909c2-215">Organizer</span></span>](organizer.md) <br/> |<span data-ttu-id="909c2-216">会議の開催者を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-216">Represents the organizer of a meeting.</span></span>  <br/> |
|[<span data-ttu-id="909c2-217">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="909c2-217">RequiredAttendees</span></span>](requiredattendees.md) <br/> |<span data-ttu-id="909c2-218">会議に出席するために必要な出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-218">Represents attendees that are required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="909c2-219">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="909c2-219">OptionalAttendees</span></span>](optionalattendees.md) <br/> |<span data-ttu-id="909c2-220">会議に出席する必要がない出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-220">Represents attendees that are not required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="909c2-221">リソース</span><span class="sxs-lookup"><span data-stu-id="909c2-221">Resources</span></span>](resources.md) <br/> |<span data-ttu-id="909c2-222">会議のスケジュールされたリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-222">Represents a scheduled resource for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="909c2-223">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="909c2-223">ConflictingMeetingCount</span></span>](conflictingmeetingcount.md) <br/> |<span data-ttu-id="909c2-224">予定表アイテムと競合する会議の数を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-224">Represents the number of meetings that conflict with the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-225">AdjacentMeetingCount</span><span class="sxs-lookup"><span data-stu-id="909c2-225">AdjacentMeetingCount</span></span>](adjacentmeetingcount.md) <br/> |<span data-ttu-id="909c2-226">会議の時間に隣接する予定表アイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-226">Represents the total number of calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="909c2-227">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="909c2-227">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="909c2-228">会議の時間と競合するすべてのアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="909c2-228">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="909c2-229">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="909c2-229">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="909c2-230">会議の時刻に隣接しているすべての予定表アイテムを説明します。</span><span class="sxs-lookup"><span data-stu-id="909c2-230">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="909c2-231">期間 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="909c2-231">Duration (Items)</span></span>](duration-items.md) <br/> |<span data-ttu-id="909c2-232">予定表アイテムの期間を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-232">Represents the duration of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-233">TimeZone (Item)</span><span class="sxs-lookup"><span data-stu-id="909c2-233">TimeZone (Item)</span></span>](timezone-item.md) <br/> |<span data-ttu-id="909c2-234">タイムゾーンのテキストの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="909c2-234">Provides a text description of a time zone.</span></span>  <br/> |
|[<span data-ttu-id="909c2-235">AppointmentReplyTime</span><span class="sxs-lookup"><span data-stu-id="909c2-235">AppointmentReplyTime</span></span>](appointmentreplytime.md) <br/> |<span data-ttu-id="909c2-236">出席者が会議出席依頼に返信した日時を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-236">Represents the date and time when an attendee replied to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="909c2-237">AppointmentSequenceNumber</span><span class="sxs-lookup"><span data-stu-id="909c2-237">AppointmentSequenceNumber</span></span>](appointmentsequencenumber.md) <br/> |<span data-ttu-id="909c2-238">予定のバージョンのシーケンス番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="909c2-238">Specifies the sequence number of a version of an appointment.</span></span>  <br/> |
|[<span data-ttu-id="909c2-239">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="909c2-239">AppointmentState</span></span>](appointmentstate.md) <br/> |<span data-ttu-id="909c2-240">予定の状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="909c2-240">Specifies the status of the appointment.</span></span>  <br/> |
|[<span data-ttu-id="909c2-241">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="909c2-241">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="909c2-242">予定表アイテムと会議出席依頼の定期的なパターンを含みます。</span><span class="sxs-lookup"><span data-stu-id="909c2-242">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> <span data-ttu-id="909c2-243">[Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。</span><span class="sxs-lookup"><span data-stu-id="909c2-243">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="909c2-244">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="909c2-244">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="909c2-245">定期的な予定表アイテムの最初の出現を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-245">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="909c2-246">[Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。</span><span class="sxs-lookup"><span data-stu-id="909c2-246">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="909c2-247">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="909c2-247">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="909c2-248">定期的な予定表アイテムの最後の発生を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-248">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="909c2-249">[Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。</span><span class="sxs-lookup"><span data-stu-id="909c2-249">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="909c2-250">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="909c2-250">ModifiedOccurrences</span></span>](modifiedoccurrences.md) <br/> |<span data-ttu-id="909c2-251">定期的な予定表アイテムの定期的なアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="909c2-251">Contains an array of recurring calendar item occurrences that have been modified so that they differ from the recurrence master item.</span></span>  <br/> <span data-ttu-id="909c2-252">[Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。</span><span class="sxs-lookup"><span data-stu-id="909c2-252">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="909c2-253">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="909c2-253">DeletedOccurrences</span></span>](deletedoccurrences.md) <br/> |<span data-ttu-id="909c2-254">定期的な予定表アイテムの削除された出現の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="909c2-254">Contains an array of deleted occurrences of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="909c2-255">[Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。</span><span class="sxs-lookup"><span data-stu-id="909c2-255">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="909c2-256">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="909c2-256">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="909c2-257">会議がホストされている場所のタイムゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-257">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
|[<span data-ttu-id="909c2-258">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="909c2-258">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="909c2-259">予定表アイテムの開始タイムゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-259">Represents the start time zone of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-260">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="909c2-260">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="909c2-261">予定表アイテムの終了タイムゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-261">Represents the end time zone of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-262">ConferenceType</span><span class="sxs-lookup"><span data-stu-id="909c2-262">ConferenceType</span></span>](conferencetype.md) <br/> |<span data-ttu-id="909c2-263">予定表アイテムで実行される会議の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-263">Describes the type of conferencing that is performed with a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-264">AllowNewTimeProposal</span><span class="sxs-lookup"><span data-stu-id="909c2-264">AllowNewTimeProposal</span></span>](allownewtimeproposal.md) <br/> |<span data-ttu-id="909c2-265">出席者が会議に対して会議の新しい日時を提案できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-265">Indicates whether a new meeting time can be proposed for a meeting by an attendee.</span></span>  <br/> |
|[<span data-ttu-id="909c2-266">IsOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="909c2-266">IsOnlineMeeting</span></span>](isonlinemeeting.md) <br/> |<span data-ttu-id="909c2-267">会議がオンラインかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-267">Indicates whether the meeting is online.</span></span>  <br/> |
|[<span data-ttu-id="909c2-268">MeetingWorkspaceUrl</span><span class="sxs-lookup"><span data-stu-id="909c2-268">MeetingWorkspaceUrl</span></span>](meetingworkspaceurl.md) <br/> |<span data-ttu-id="909c2-269">予定表アイテムにリンクされている会議ワークスペースの URL が含まれます。</span><span class="sxs-lookup"><span data-stu-id="909c2-269">Contains the URL for the meeting workspace that is linked to by the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-270">NetShowUrl</span><span class="sxs-lookup"><span data-stu-id="909c2-270">NetShowUrl</span></span>](netshowurl.md) <br/> |<span data-ttu-id="909c2-271">Microsoft NetShow online 会議の URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="909c2-271">Specifies the URL for a Microsoft NetShow online meeting.</span></span>  <br/> |
|[<span data-ttu-id="909c2-272">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="909c2-272">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="909c2-273">アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="909c2-273">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="909c2-274">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="909c2-274">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="909c2-275">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="909c2-275">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="909c2-276">アイテムを最後に変更したユーザーの表示名を含みます。</span><span class="sxs-lookup"><span data-stu-id="909c2-276">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-277">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="909c2-277">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="909c2-278">アイテムが最後に変更された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-278">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="909c2-279">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="909c2-279">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="909c2-280">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="909c2-280">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="909c2-281">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="909c2-281">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="909c2-282">Outlook Web app のアイテムを読み取るために Microsoft Office Outlook Web App エンドポイントに連結する URL を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-282">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="909c2-283">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="909c2-283">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="909c2-284">Outlook Web App のアイテムを編集するために Microsoft Office Outlook Web App エンドポイントに連結する URL を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-284">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="909c2-285">ConversationId</span><span class="sxs-lookup"><span data-stu-id="909c2-285">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="909c2-286">アイテムまたは会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="909c2-286">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="909c2-287">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="909c2-287">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="909c2-288">この会話の一意の本文を表す HTML フラグメントまたはプレーンテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-288">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="909c2-289">親要素</span><span class="sxs-lookup"><span data-stu-id="909c2-289">Parent elements</span></span>

|<span data-ttu-id="909c2-290">**要素**</span><span class="sxs-lookup"><span data-stu-id="909c2-290">**Element**</span></span>|<span data-ttu-id="909c2-291">**説明**</span><span class="sxs-lookup"><span data-stu-id="909c2-291">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="909c2-292">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="909c2-292">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="909c2-293">会議の時刻に隣接しているすべての予定表アイテムを説明します。</span><span class="sxs-lookup"><span data-stu-id="909c2-293">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="909c2-294">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="909c2-294">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="909c2-295">[Updateitem 操作](updateitem-operation.md)中に、アイテムまたはフォルダーの1つのプロパティに追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="909c2-295">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="909c2-296">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="909c2-296">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="909c2-297">会議の時間と競合するすべてのアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="909c2-297">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="909c2-298">Create (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="909c2-298">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="909c2-299">ローカルクライアントストアに作成する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="909c2-299">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="909c2-300">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="909c2-300">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="909c2-301">別の Exchange アイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-301">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="909c2-302">Items</span><span class="sxs-lookup"><span data-stu-id="909c2-302">Items</span></span>](items.md) <br/> |<span data-ttu-id="909c2-303">項目の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="909c2-303">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="909c2-304">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="909c2-304">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="909c2-305">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="909c2-305">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="909c2-306">SetItemField</span><span class="sxs-lookup"><span data-stu-id="909c2-306">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="909c2-307">[Updateitem 操作](updateitem-operation.md)のアイテムの1つのプロパティに対する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="909c2-307">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="909c2-308">Update (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="909c2-308">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="909c2-309">ローカルクライアントストアで更新する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="909c2-309">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="909c2-310">テキスト値</span><span class="sxs-lookup"><span data-stu-id="909c2-310">Text value</span></span>

<span data-ttu-id="909c2-311">なし。</span><span class="sxs-lookup"><span data-stu-id="909c2-311">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="909c2-312">注釈</span><span class="sxs-lookup"><span data-stu-id="909c2-312">Remarks</span></span>

<span data-ttu-id="909c2-313">1つの予定表アイテムを定期的な予定のマスター予定アイテムに更新する場合は、予定表アイテムの元のタイムゾーンを保持するために、[会議 timezone](meetingtimezone.md)要素を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="909c2-313">When a single calendar item is updated to become a recurring master calendar item, the [MeetingTimeZone](meetingtimezone.md) element must be specified in order to preserve the calendar item's original time zone.</span></span> 
  
<span data-ttu-id="909c2-314">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="909c2-314">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="909c2-315">要素の情報</span><span class="sxs-lookup"><span data-stu-id="909c2-315">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="909c2-316">Namespace</span><span class="sxs-lookup"><span data-stu-id="909c2-316">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="909c2-317">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="909c2-317">Schema name</span></span>  <br/> |<span data-ttu-id="909c2-318">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="909c2-318">Types schema</span></span>  <br/> |
|<span data-ttu-id="909c2-319">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="909c2-319">Validation file</span></span>  <br/> |<span data-ttu-id="909c2-320">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="909c2-320">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="909c2-321">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="909c2-321">Can be empty</span></span>  <br/> |<span data-ttu-id="909c2-322">正しくない</span><span class="sxs-lookup"><span data-stu-id="909c2-322">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="909c2-323">関連項目</span><span class="sxs-lookup"><span data-stu-id="909c2-323">See also</span></span>



- [<span data-ttu-id="909c2-324">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="909c2-324">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="909c2-325">Exchange 用 EWS リファレンス</span><span class="sxs-lookup"><span data-stu-id="909c2-325">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)


---
title: カレンダー項目
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
description: カレンダー項目要素は、Exchange 予定表アイテムを表します。
ms.openlocfilehash: c7b6d4930bc42fbe26d35264e2eae0c986cc8db7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759590"
---
# <a name="calendaritem"></a><span data-ttu-id="ea61c-103">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="ea61c-103">CalendarItem</span></span>

<span data-ttu-id="ea61c-104">**カレンダー項目**要素は、Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-104">The **CalendarItem** element represents an Exchange calendar item.</span></span> 
  
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

 <span data-ttu-id="ea61c-105">**CalendarItemType**</span><span class="sxs-lookup"><span data-stu-id="ea61c-105">**CalendarItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea61c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ea61c-106">Attributes and elements</span></span>

<span data-ttu-id="ea61c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea61c-108">属性</span><span class="sxs-lookup"><span data-stu-id="ea61c-108">Attributes</span></span>

<span data-ttu-id="ea61c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ea61c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea61c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ea61c-110">Child elements</span></span>

|<span data-ttu-id="ea61c-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="ea61c-111">**Element**</span></span>|<span data-ttu-id="ea61c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ea61c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea61c-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="ea61c-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="ea61c-114">Base64Binary の形式で表されるオブジェクトのネイティブの多目的インターネット メール拡張 (MIME) ストリームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea61c-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="ea61c-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ea61c-116">Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea61c-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="ea61c-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="ea61c-118">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-118">Represents the identifier of the parent folder that contains the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="ea61c-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="ea61c-120">アイテムのメッセージ クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-120">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-121">Subject</span><span class="sxs-lookup"><span data-stu-id="ea61c-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="ea61c-122">Exchange ストアのアイテムおよび応答オブジェクトのサブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="ea61c-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="ea61c-124">アイテムの秘密度レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-124">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-125">Body/本文</span><span class="sxs-lookup"><span data-stu-id="ea61c-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="ea61c-126">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-126">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-127">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="ea61c-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ea61c-128">アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea61c-128">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="ea61c-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="ea61c-130">メールボックス内のアイテムを受信したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-130">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-131">Size</span><span class="sxs-lookup"><span data-stu-id="ea61c-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="ea61c-132">アイテムのバイト単位のサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-132">Represents the size in bytes of an item.</span></span> <span data-ttu-id="ea61c-133">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="ea61c-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-134">Categories</span><span class="sxs-lookup"><span data-stu-id="ea61c-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ea61c-135">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-135">Represents a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-136">Importance</span><span class="sxs-lookup"><span data-stu-id="ea61c-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="ea61c-137">アイテムの重要性をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-137">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="ea61c-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="ea61c-139">このアイテムの返信するアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-139">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="ea61c-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="ea61c-141">アイテムが [送信トレイ] 既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="ea61c-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="ea61c-143">かどうかの項目がまだ送信されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-143">Indicates whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="ea61c-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="ea61c-145">ユーザーが彼または彼女自身にアイテムを送信するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-145">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="ea61c-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="ea61c-147">アイテムが以前送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="ea61c-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="ea61c-149">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="ea61c-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="ea61c-151">メールボックス内のアイテムに含まれるすべてのインターネット メッセージ ヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-151">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="ea61c-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="ea61c-153">メールボックス内のアイテムが送信された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="ea61c-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="ea61c-155">メールボックス内の特定のアイテムが作成された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="ea61c-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="ea61c-157">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea61c-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="ea61c-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="ea61c-159">イベントが発生したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="ea61c-160">[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によってアラームが表示されたときを決定する使用されます。</span><span class="sxs-lookup"><span data-stu-id="ea61c-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="ea61c-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="ea61c-162">Exchange ストアのアイテムのアラームが設定されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="ea61c-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="ea61c-164">分前にアラームが表示されるときに、イベントの数を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="ea61c-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="ea61c-166">[Cc] 行の内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-166">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="ea61c-167">これは、すべての Cc 受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="ea61c-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="ea61c-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="ea61c-169">行の内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-169">Represents the display string that is used for the contents of the To line.</span></span> <span data-ttu-id="ea61c-170">これは、すべての受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="ea61c-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-171">添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="ea61c-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="ea61c-172">アイテムに表示されている 1 つ以上の添付ファイルがある場合に**true**に設定されているプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="ea61c-173">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="ea61c-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="ea61c-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="ea61c-175">フォルダーおよびアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-175">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-176">カルチャ</span><span class="sxs-lookup"><span data-stu-id="ea61c-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="ea61c-177">メールボックス内の指定したアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-177">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-178">UID</span><span class="sxs-lookup"><span data-stu-id="ea61c-178">UID</span></span>](uid.md) <br/> |<span data-ttu-id="ea61c-179">予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-179">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-180">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="ea61c-180">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="ea61c-181">定期的な予定表アイテムの特定のインスタンスを識別するために使用します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-181">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-182">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="ea61c-182">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="ea61c-183">ICalendar オブジェクトのインスタンスが作成された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-183">Indicates the date and time that an instance of a iCalendar object was created.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-184">Start</span><span class="sxs-lookup"><span data-stu-id="ea61c-184">Start</span></span>](start.md) <br/> |<span data-ttu-id="ea61c-185">予定表アイテムの開始を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-185">Represents the start of a calendar item.</span></span> <span data-ttu-id="ea61c-186">この要素は、予定表アイテムの 1 回のみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="ea61c-186">This element only applies to a single occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-187">終わり</span><span class="sxs-lookup"><span data-stu-id="ea61c-187">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ea61c-188">期間の終了を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-188">Represents the end of a duration.</span></span> <span data-ttu-id="ea61c-189">この要素は、予定表アイテムの 1 回のみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="ea61c-189">This element only applies to a single occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-190">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="ea61c-190">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="ea61c-191">予定表アイテムの元の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-191">Represents the original start time of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-192">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="ea61c-192">IsAllDayEvent</span></span>](isalldayevent.md) <br/> |<span data-ttu-id="ea61c-193">予定表アイテムまたは会議出席依頼が終日のイベントを表すかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-193">Indicates whether a calendar item or meeting request represents an all-day event.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-194">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="ea61c-194">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md) <br/> |<span data-ttu-id="ea61c-195">予定表アイテムの空き/予約済み状態を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-195">Represents the free/busy status of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-196">場所</span><span class="sxs-lookup"><span data-stu-id="ea61c-196">Location</span></span>](location.md) <br/> |<span data-ttu-id="ea61c-197">会議または予定の場所を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-197">Represents the location of a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-198">When</span><span class="sxs-lookup"><span data-stu-id="ea61c-198">When</span></span>](when.md) <br/> |<span data-ttu-id="ea61c-199">予定表アイテムが発生した場合についてを説明します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-199">Provides information about when a calendar item occurs.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-200">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="ea61c-200">IsMeeting</span></span>](ismeeting.md) <br/> |<span data-ttu-id="ea61c-201">予定表アイテムが会議または予定があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-201">Indicates whether the calendar item is a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-202">IsCancelled</span><span class="sxs-lookup"><span data-stu-id="ea61c-202">IsCancelled</span></span>](iscancelled.md) <br/> |<span data-ttu-id="ea61c-203">予定または会議がキャンセルされたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-203">Indicates whether an appointment or meeting has been canceled.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-204">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="ea61c-204">IsRecurring</span></span>](isrecurring.md) <br/> |<span data-ttu-id="ea61c-205">予定表アイテムが定期的なアイテムの一部であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-205">Indicates whether a calendar item is part of a recurring item.</span></span> <span data-ttu-id="ea61c-206">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ea61c-206">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-207">MeetingRequestWasSent</span><span class="sxs-lookup"><span data-stu-id="ea61c-207">MeetingRequestWasSent</span></span>](meetingrequestwassent.md) <br/> |<span data-ttu-id="ea61c-208">要求された出席者に会議出席依頼が送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-208">Indicates whether a meeting request has been sent to requested attendees.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-209">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="ea61c-209">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="ea61c-210">項目への応答が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-210">Indicates whether a response to an item is required.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-211">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="ea61c-211">CalendarItemType</span></span>](calendaritemtype.md) <br/> |<span data-ttu-id="ea61c-212">予定表アイテムのアイテムの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-212">Represents the occurrence type of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-213">MyResponseType</span><span class="sxs-lookup"><span data-stu-id="ea61c-213">MyResponseType</span></span>](myresponsetype.md) <br/> |<span data-ttu-id="ea61c-214">ステータス、または予定表アイテムへの応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea61c-214">Contains the status of or response to a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-215">Organizer</span><span class="sxs-lookup"><span data-stu-id="ea61c-215">Organizer</span></span>](organizer.md) <br/> |<span data-ttu-id="ea61c-216">会議の開催者を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-216">Represents the organizer of a meeting.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-217">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="ea61c-217">RequiredAttendees</span></span>](requiredattendees.md) <br/> |<span data-ttu-id="ea61c-218">会議に出席するために必要な出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-218">Represents attendees that are required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-219">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="ea61c-219">OptionalAttendees</span></span>](optionalattendees.md) <br/> |<span data-ttu-id="ea61c-220">出席者が会議に出席する必要がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-220">Represents attendees that are not required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-221">リソース</span><span class="sxs-lookup"><span data-stu-id="ea61c-221">Resources</span></span>](resources.md) <br/> |<span data-ttu-id="ea61c-222">会議のスケジュール設定されたリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-222">Represents a scheduled resource for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-223">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="ea61c-223">ConflictingMeetingCount</span></span>](conflictingmeetingcount.md) <br/> |<span data-ttu-id="ea61c-224">予定表のアイテムと競合する会議の数を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-224">Represents the number of meetings that conflict with the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-225">AdjacentMeetingCount</span><span class="sxs-lookup"><span data-stu-id="ea61c-225">AdjacentMeetingCount</span></span>](adjacentmeetingcount.md) <br/> |<span data-ttu-id="ea61c-226">会議の時刻に隣接している予定表アイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-226">Represents the total number of calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-227">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="ea61c-227">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="ea61c-228">会議の時間と競合するすべての項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-228">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-229">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="ea61c-229">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="ea61c-230">会議の時刻に隣接しているすべての予定表のアイテムについて説明します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-230">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-231">期間 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="ea61c-231">Duration (Items)</span></span>](duration-items.md) <br/> |<span data-ttu-id="ea61c-232">予定表アイテムの期間を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-232">Represents the duration of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-233">タイムゾーン (アイテム)</span><span class="sxs-lookup"><span data-stu-id="ea61c-233">TimeZone (Item)</span></span>](timezone-item.md) <br/> |<span data-ttu-id="ea61c-234">タイム ゾーンの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-234">Provides a text description of a time zone.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-235">AppointmentReplyTime</span><span class="sxs-lookup"><span data-stu-id="ea61c-235">AppointmentReplyTime</span></span>](appointmentreplytime.md) <br/> |<span data-ttu-id="ea61c-236">会議出席依頼に出席者が返信したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-236">Represents the date and time when an attendee replied to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-237">AppointmentSequenceNumber</span><span class="sxs-lookup"><span data-stu-id="ea61c-237">AppointmentSequenceNumber</span></span>](appointmentsequencenumber.md) <br/> |<span data-ttu-id="ea61c-238">予定のバージョンのシーケンス番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-238">Specifies the sequence number of a version of an appointment.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-239">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="ea61c-239">AppointmentState</span></span>](appointmentstate.md) <br/> |<span data-ttu-id="ea61c-240">予定の状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-240">Specifies the status of the appointment.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-241">定期的なアイテム (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="ea61c-241">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="ea61c-242">予定表アイテムおよび会議出席依頼に定期的なパターンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea61c-242">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> <span data-ttu-id="ea61c-243">この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。</span><span class="sxs-lookup"><span data-stu-id="ea61c-243">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-244">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="ea61c-244">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="ea61c-245">定期的な予定表アイテムが最初に見つかった位置を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-245">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="ea61c-246">この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。</span><span class="sxs-lookup"><span data-stu-id="ea61c-246">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-247">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="ea61c-247">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="ea61c-248">定期的な予定表アイテムが最後に見つかった位置を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-248">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="ea61c-249">この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。</span><span class="sxs-lookup"><span data-stu-id="ea61c-249">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-250">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="ea61c-250">ModifiedOccurrences</span></span>](modifiedoccurrences.md) <br/> |<span data-ttu-id="ea61c-251">定期的な予定のマスター アイテムが異なるように変更された定期的な予定表アイテム アイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea61c-251">Contains an array of recurring calendar item occurrences that have been modified so that they differ from the recurrence master item.</span></span>  <br/> <span data-ttu-id="ea61c-252">この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。</span><span class="sxs-lookup"><span data-stu-id="ea61c-252">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-253">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="ea61c-253">DeletedOccurrences</span></span>](deletedoccurrences.md) <br/> |<span data-ttu-id="ea61c-254">定期的な予定表アイテムの削除済みアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea61c-254">Contains an array of deleted occurrences of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="ea61c-255">この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。</span><span class="sxs-lookup"><span data-stu-id="ea61c-255">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-256">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="ea61c-256">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="ea61c-257">会議がホストされている場所のタイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-257">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-258">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="ea61c-258">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="ea61c-259">予定表アイテムの開始タイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-259">Represents the start time zone of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-260">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="ea61c-260">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="ea61c-261">予定表アイテムの終了タイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-261">Represents the end time zone of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-262">ConferenceType</span><span class="sxs-lookup"><span data-stu-id="ea61c-262">ConferenceType</span></span>](conferencetype.md) <br/> |<span data-ttu-id="ea61c-263">予定表アイテムで実行される会議の種類について説明します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-263">Describes the type of conferencing that is performed with a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-264">AllowNewTimeProposal</span><span class="sxs-lookup"><span data-stu-id="ea61c-264">AllowNewTimeProposal</span></span>](allownewtimeproposal.md) <br/> |<span data-ttu-id="ea61c-265">出席者によって会議の会議の新しい日時を提案ことができるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-265">Indicates whether a new meeting time can be proposed for a meeting by an attendee.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-266">IsOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ea61c-266">IsOnlineMeeting</span></span>](isonlinemeeting.md) <br/> |<span data-ttu-id="ea61c-267">会議がオンラインかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-267">Indicates whether the meeting is online.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-268">MeetingWorkspaceUrl</span><span class="sxs-lookup"><span data-stu-id="ea61c-268">MeetingWorkspaceUrl</span></span>](meetingworkspaceurl.md) <br/> |<span data-ttu-id="ea61c-269">予定表アイテムにリンクされている会議ワークスペースの URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea61c-269">Contains the URL for the meeting workspace that is linked to by the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-270">NetShowUrl</span><span class="sxs-lookup"><span data-stu-id="ea61c-270">NetShowUrl</span></span>](netshowurl.md) <br/> |<span data-ttu-id="ea61c-271">Microsoft NetShow オンライン会議の URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-271">Specifies the URL for a Microsoft NetShow online meeting.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-272">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="ea61c-272">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="ea61c-273">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea61c-273">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="ea61c-274">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ea61c-274">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-275">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="ea61c-275">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="ea61c-276">最後の項目を変更するのにはユーザーの表示名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea61c-276">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-277">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="ea61c-277">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="ea61c-278">アイテムが最後に修正された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-278">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-279">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="ea61c-279">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="ea61c-280">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-280">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-281">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="ea61c-281">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="ea61c-282">Outlook Web App 内の項目を参照するのには Microsoft Office Outlook の Web アプリケーションのエンドポイントを結合するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-282">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-283">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="ea61c-283">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="ea61c-284">Outlook Web App 内の項目を編集するのには Microsoft Office Outlook の Web アプリケーションのエンドポイントを結合するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-284">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-285">ConversationId</span><span class="sxs-lookup"><span data-stu-id="ea61c-285">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="ea61c-286">アイテムや会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea61c-286">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-287">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="ea61c-287">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="ea61c-288">このスレッドの一意の本文を表すテキストまたは HTML フラグメントを表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-288">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ea61c-289">親要素</span><span class="sxs-lookup"><span data-stu-id="ea61c-289">Parent elements</span></span>

|<span data-ttu-id="ea61c-290">**要素**</span><span class="sxs-lookup"><span data-stu-id="ea61c-290">**Element**</span></span>|<span data-ttu-id="ea61c-291">**説明**</span><span class="sxs-lookup"><span data-stu-id="ea61c-291">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea61c-292">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="ea61c-292">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="ea61c-293">会議の時刻に隣接しているすべての予定表のアイテムについて説明します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-293">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-294">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="ea61c-294">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="ea61c-295">[UpdateItem 操作](updateitem-operation.md)中に 1 つのアイテムまたはフォルダーのプロパティを追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-295">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ea61c-296">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="ea61c-296">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="ea61c-297">会議の時間と競合するすべての項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-297">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-298">(ItemSync) を作成します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-298">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="ea61c-299">ローカル クライアント ストアに作成する 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-299">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-300">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="ea61c-300">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="ea61c-301">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-301">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-302">Items</span><span class="sxs-lookup"><span data-stu-id="ea61c-302">Items</span></span>](items.md) <br/> |<span data-ttu-id="ea61c-303">項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea61c-303">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-304">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="ea61c-304">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="ea61c-305">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で識別されるフォルダーを作成する項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea61c-305">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="ea61c-306">SetItemField</span><span class="sxs-lookup"><span data-stu-id="ea61c-306">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="ea61c-307">[UpdateItem 操作](updateitem-operation.md)内の項目の 1 つのプロパティには、更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-307">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ea61c-308">更新プログラム (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="ea61c-308">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="ea61c-309">ローカル クライアント ストアで更新する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="ea61c-309">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ea61c-310">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ea61c-310">Text value</span></span>

<span data-ttu-id="ea61c-311">なし。</span><span class="sxs-lookup"><span data-stu-id="ea61c-311">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ea61c-312">備考</span><span class="sxs-lookup"><span data-stu-id="ea61c-312">Remarks</span></span>

<span data-ttu-id="ea61c-313">マスターの予定表の定期的なアイテムを 1 つの予定表アイテムが更新されると、予定表アイテムの元のタイム ゾーンを保持するために[MeetingTimeZone](meetingtimezone.md)要素を指定してください。</span><span class="sxs-lookup"><span data-stu-id="ea61c-313">When a single calendar item is updated to become a recurring master calendar item, the [MeetingTimeZone](meetingtimezone.md) element must be specified in order to preserve the calendar item's original time zone.</span></span> 
  
<span data-ttu-id="ea61c-314">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ea61c-314">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea61c-315">要素情報</span><span class="sxs-lookup"><span data-stu-id="ea61c-315">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea61c-316">名前空間</span><span class="sxs-lookup"><span data-stu-id="ea61c-316">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ea61c-317">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ea61c-317">Schema name</span></span>  <br/> |<span data-ttu-id="ea61c-318">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ea61c-318">Types schema</span></span>  <br/> |
|<span data-ttu-id="ea61c-319">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ea61c-319">Validation file</span></span>  <br/> |<span data-ttu-id="ea61c-320">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ea61c-320">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ea61c-321">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ea61c-321">Can be empty</span></span>  <br/> |<span data-ttu-id="ea61c-322">False</span><span class="sxs-lookup"><span data-stu-id="ea61c-322">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea61c-323">関連項目</span><span class="sxs-lookup"><span data-stu-id="ea61c-323">See also</span></span>



- [<span data-ttu-id="ea61c-324">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ea61c-324">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
<span data-ttu-id="ea61c-325">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="ea61c-325">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>


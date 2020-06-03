---
title: MeetingRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingRequest
api_type:
- schema
ms.assetid: c44f8804-a355-473d-a837-48cc91617251
description: 会議出席依頼要素は、Exchange ストア内の会議出席依頼を表します。
ms.openlocfilehash: 7b39ec52d2b4fe8b3cdd2b6fd5e7ba97cfa69c7e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465829"
---
# <a name="meetingrequest"></a><span data-ttu-id="27666-103">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="27666-103">MeetingRequest</span></span>

<span data-ttu-id="27666-104">会議出席**依頼**要素は、Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-104">The **MeetingRequest** element represents a meeting request in the Exchange store.</span></span> 
  
```xml
<MeetingRequest>
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
   <Importance/>
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
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ConversationIndex/>
   <ConversationTopic/>
   <From/>
   <InternetMessageId/>
   <IsRead/>
   <IsResponseRequested/>
   <References/>
   <ReplyTo/>
   <AssociatedCalendarItemId/>
   <IsDelegated/>
   <IsOutOfDate/>
   <HasBeenProcessed/>
   <ResponseType/>
   <MeetingRequestType/>
   <IntendedFreeBusyStatus/>
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
</MeetingRequest>
```

 <span data-ttu-id="27666-105">**MeetingRequestMessageType**</span><span class="sxs-lookup"><span data-stu-id="27666-105">**MeetingRequestMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27666-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="27666-106">Attributes and elements</span></span>

<span data-ttu-id="27666-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="27666-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27666-108">属性</span><span class="sxs-lookup"><span data-stu-id="27666-108">Attributes</span></span>

<span data-ttu-id="27666-109">なし。</span><span class="sxs-lookup"><span data-stu-id="27666-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27666-110">子要素</span><span class="sxs-lookup"><span data-stu-id="27666-110">Child elements</span></span>

|<span data-ttu-id="27666-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="27666-111">**Element**</span></span>|<span data-ttu-id="27666-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="27666-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27666-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="27666-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="27666-114">Base64Binary 形式で表されるオブジェクトの、ネイティブな汎用インターネットメール内線 (MIME) ストリームが保存されています。</span><span class="sxs-lookup"><span data-stu-id="27666-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="27666-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="27666-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="27666-116">Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="27666-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="27666-117">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="27666-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="27666-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="27666-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="27666-119">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="27666-120">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="27666-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="27666-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="27666-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="27666-122">アイテムのメッセージクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="27666-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="27666-123">件名</span><span class="sxs-lookup"><span data-stu-id="27666-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="27666-124">Exchange ストアアイテムおよび応答オブジェクトの件名を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="27666-125">件名は255文字に制限されます。</span><span class="sxs-lookup"><span data-stu-id="27666-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="27666-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="27666-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="27666-127">アイテムの秘密度レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="27666-128">Body</span><span class="sxs-lookup"><span data-stu-id="27666-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="27666-129">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="27666-130">Attachments</span><span class="sxs-lookup"><span data-stu-id="27666-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="27666-131">Exchange ストア内のアイテムに添付されているアイテムまたはファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="27666-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="27666-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="27666-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="27666-133">メールボックス内のアイテムが受信されたデータと時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-133">Represents the data and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="27666-134">Size</span><span class="sxs-lookup"><span data-stu-id="27666-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="27666-135">アイテムのサイズ (バイト単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="27666-136">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="27666-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="27666-137">Categories</span><span class="sxs-lookup"><span data-stu-id="27666-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="27666-138">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="27666-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="27666-139">Importance</span><span class="sxs-lookup"><span data-stu-id="27666-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="27666-140">アイテムの重要度について説明します。</span><span class="sxs-lookup"><span data-stu-id="27666-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="27666-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="27666-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="27666-142">このアイテムが返信であるアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="27666-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="27666-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="27666-144">アイテムが送信トレイの既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="27666-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="27666-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="27666-146">アイテムがまだ送信されていないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-146">Indicates whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="27666-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="27666-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="27666-148">ユーザーがアイテムを自分自身に送信したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-148">Indicates whether a user sent an item to itself.</span></span>  <br/> |
|[<span data-ttu-id="27666-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="27666-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="27666-150">アイテムが以前に送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="27666-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="27666-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="27666-152">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="27666-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="27666-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="27666-154">メールボックス内のアイテム内に含まれるすべてのインターネットメッセージヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="27666-154">Represents the collection of all Internet message headers contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="27666-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="27666-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="27666-156">メールボックス内のアイテムが送信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="27666-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="27666-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="27666-158">メールボックス内の特定のアイテムが作成された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="27666-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="27666-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="27666-160">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="27666-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="27666-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="27666-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="27666-162">イベントが発生した日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="27666-163">これは、アラームがいつ表示されるかを決定するために[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="27666-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="27666-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="27666-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="27666-165">Exchange ストア内のアイテムにアラームが設定されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="27666-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="27666-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="27666-167">アラームが表示されるイベントの前の時間 (分単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="27666-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="27666-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="27666-169">[CC] 行の内容として使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-169">Represents the display string that is used for the contents of the CC line.</span></span> <span data-ttu-id="27666-170">これは、すべての CC 受信者表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="27666-170">This is the concatenated string of all CC recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="27666-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="27666-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="27666-172">To 行の内容として使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-172">Represents the display string that is used for the contents of the To line.</span></span> <span data-ttu-id="27666-173">これは、すべての受信者の表示名の連結文字列です。</span><span class="sxs-lookup"><span data-stu-id="27666-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="27666-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="27666-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="27666-175">アイテムに少なくとも1つの添付ファイルがある場合に**true**に設定されるプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="27666-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="27666-176">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="27666-176">This property is read only.</span></span>  <br/> |
|[<span data-ttu-id="27666-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="27666-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="27666-178">フォルダーとアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="27666-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="27666-179">Culture</span><span class="sxs-lookup"><span data-stu-id="27666-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="27666-180">メールボックス内の特定のアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="27666-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="27666-181">Sender</span><span class="sxs-lookup"><span data-stu-id="27666-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="27666-182">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="27666-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="27666-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="27666-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="27666-184">メッセージの受信者のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="27666-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="27666-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="27666-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="27666-186">メッセージのコピーを受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="27666-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="27666-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="27666-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="27666-188">電子メールのブラインドカーボンコピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="27666-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="27666-189">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="27666-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="27666-190">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="27666-191">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="27666-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="27666-192">アイテムの送信者が配信確認を要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="27666-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="27666-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="27666-194">このメッセージが属しているスレッドを表すバイナリ ID を含みます。</span><span class="sxs-lookup"><span data-stu-id="27666-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="27666-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="27666-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="27666-196">会話識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="27666-197">From</span><span class="sxs-lookup"><span data-stu-id="27666-197">From</span></span>](from.md) <br/> |<span data-ttu-id="27666-198">メッセージが送信された相手のアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="27666-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="27666-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="27666-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="27666-200">アイテムのインターネットメッセージ識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="27666-201">IsRead</span><span class="sxs-lookup"><span data-stu-id="27666-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="27666-202">メッセージが開封されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="27666-203">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="27666-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="27666-204">電子メールメッセージに対する応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="27666-205">References</span><span class="sxs-lookup"><span data-stu-id="27666-205">References</span></span>](references.md) <br/> |<span data-ttu-id="27666-206">返信と元のメッセージを相互に関連付けるために使用される Usenet ヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="27666-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="27666-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="27666-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="27666-208">返信を送信する宛先のアドレスのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="27666-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="27666-209">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="27666-209">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="27666-210">[会議メッセージ](meetingmessage.md)に関連付けられている予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="27666-210">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="27666-211">IsDelegated</span><span class="sxs-lookup"><span data-stu-id="27666-211">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="27666-212">代理人アクセス権を持つアカウントによって会議が処理されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-212">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="27666-213">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="27666-213">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="27666-214">会議メッセージが古くなっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-214">Indicates whether a meeting message is out of date.</span></span>  <br/> |
|[<span data-ttu-id="27666-215">Hasが処理されました</span><span class="sxs-lookup"><span data-stu-id="27666-215">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="27666-216">会議メッセージアイテムが処理されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-216">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="27666-217">ResponseType</span><span class="sxs-lookup"><span data-stu-id="27666-217">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="27666-218">会議の受信者の応答の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-218">Represents the kind of recipient response that is received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="27666-219">会議の Requesttype</span><span class="sxs-lookup"><span data-stu-id="27666-219">MeetingRequestType</span></span>](meetingrequesttype.md) <br/> |<span data-ttu-id="27666-220">会議出席依頼の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-220">Describes the type of the meeting request.</span></span>  <br/> |
|[<span data-ttu-id="27666-221">IntendedFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="27666-221">IntendedFreeBusyStatus</span></span>](intendedfreebusystatus.md) <br/> |<span data-ttu-id="27666-222">会議出席依頼に関連付けられている予定表アイテムの目的の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-222">Represents the intended status for the calendar item that is associated with the meeting request.</span></span>  <br/> |
|[<span data-ttu-id="27666-223">開始</span><span class="sxs-lookup"><span data-stu-id="27666-223">Start</span></span>](start.md) <br/> |<span data-ttu-id="27666-224">予定表アイテムの開始を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-224">Represents the start of a calendar item.</span></span> <span data-ttu-id="27666-225">この要素は、予定表アイテムの1回だけに適用されます。</span><span class="sxs-lookup"><span data-stu-id="27666-225">This element only applies to a single occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="27666-226">終わり</span><span class="sxs-lookup"><span data-stu-id="27666-226">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="27666-227">期間の最後の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-227">Represents the end of a duration.</span></span> <span data-ttu-id="27666-228">この要素は、予定表アイテムの1回だけに適用されます。</span><span class="sxs-lookup"><span data-stu-id="27666-228">This element only applies to a single occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="27666-229">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="27666-229">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="27666-230">予定表アイテムの元の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-230">Represents the original start time of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="27666-231">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="27666-231">IsAllDayEvent</span></span>](isalldayevent.md) <br/> |<span data-ttu-id="27666-232">予定表アイテムまたは会議出席依頼が終日イベントを表しているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-232">Indicates whether a calendar item or meeting request represents an all-day event.</span></span>  <br/> |
|[<span data-ttu-id="27666-233">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="27666-233">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md) <br/> |<span data-ttu-id="27666-234">予定表アイテムの空き時間状態を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-234">Represents the free/busy status of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="27666-235">場所</span><span class="sxs-lookup"><span data-stu-id="27666-235">Location</span></span>](location.md) <br/> |<span data-ttu-id="27666-236">会議または予定の場所を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-236">Represents the location of a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="27666-237">When</span><span class="sxs-lookup"><span data-stu-id="27666-237">When</span></span>](when.md) <br/> |<span data-ttu-id="27666-238">会議がいつ発生したかについての説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="27666-238">Provides a description of when a meeting occurs.</span></span>  <br/> |
|[<span data-ttu-id="27666-239">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="27666-239">IsMeeting</span></span>](ismeeting.md) <br/> |<span data-ttu-id="27666-240">予定表アイテムが会議または予定のどちらかであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-240">Indicates whether the calendar item is either a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="27666-241">IsCancelled</span><span class="sxs-lookup"><span data-stu-id="27666-241">IsCancelled</span></span>](iscancelled.md) <br/> |<span data-ttu-id="27666-242">予定または会議がキャンセルされたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-242">Indicates whether an appointment or meeting has been cancelled.</span></span>  <br/> |
|[<span data-ttu-id="27666-243">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="27666-243">IsRecurring</span></span>](isrecurring.md) <br/> |<span data-ttu-id="27666-244">予定表アイテムが定期的なアイテムの一部であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-244">Indicates whether a calendar item is part of a recurring item.</span></span> <span data-ttu-id="27666-245">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="27666-245">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="27666-246">MeetingRequestWasSent</span><span class="sxs-lookup"><span data-stu-id="27666-246">MeetingRequestWasSent</span></span>](meetingrequestwassent.md) <br/> |<span data-ttu-id="27666-247">出席依頼が出席者に送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-247">Indicates whether a meeting request has been sent to requested attendees.</span></span>  <br/> |
|[<span data-ttu-id="27666-248">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="27666-248">CalendarItemType</span></span>](calendaritemtype.md) <br/> |<span data-ttu-id="27666-249">予定表アイテムの発生の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-249">Represents the occurrence type of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="27666-250">MyResponseType</span><span class="sxs-lookup"><span data-stu-id="27666-250">MyResponseType</span></span>](myresponsetype.md) <br/> |<span data-ttu-id="27666-251">予定表アイテムの状態または応答を含みます。</span><span class="sxs-lookup"><span data-stu-id="27666-251">Contains the status of or response to a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="27666-252">Organizer</span><span class="sxs-lookup"><span data-stu-id="27666-252">Organizer</span></span>](organizer.md) <br/> |<span data-ttu-id="27666-253">会議の開催者を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-253">Represents the organizer of a meeting.</span></span>  <br/> |
|[<span data-ttu-id="27666-254">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="27666-254">RequiredAttendees</span></span>](requiredattendees.md) <br/> |<span data-ttu-id="27666-255">会議に出席するために必要な出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-255">Represents attendees that are required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="27666-256">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="27666-256">OptionalAttendees</span></span>](optionalattendees.md) <br/> |<span data-ttu-id="27666-257">会議に出席する必要がない出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-257">Represents attendees that are not required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="27666-258">リソース</span><span class="sxs-lookup"><span data-stu-id="27666-258">Resources</span></span>](resources.md) <br/> |<span data-ttu-id="27666-259">会議のスケジュールされたリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="27666-259">Represents a scheduled resource for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="27666-260">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="27666-260">ConflictingMeetingCount</span></span>](conflictingmeetingcount.md) <br/> |<span data-ttu-id="27666-261">会議出席依頼と競合する会議の数を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-261">Represents the number of meetings that conflict with the meeting request.</span></span>  <br/> |
|[<span data-ttu-id="27666-262">AdjacentMeetingCount</span><span class="sxs-lookup"><span data-stu-id="27666-262">AdjacentMeetingCount</span></span>](adjacentmeetingcount.md) <br/> |<span data-ttu-id="27666-263">会議の時間に隣接する予定表アイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-263">Represents the total number of calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="27666-264">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="27666-264">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="27666-265">会議の時間と競合するすべてのアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="27666-265">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="27666-266">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="27666-266">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="27666-267">会議の時刻に隣接しているすべての予定表アイテムを説明します。</span><span class="sxs-lookup"><span data-stu-id="27666-267">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="27666-268">期間 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="27666-268">Duration (Items)</span></span>](duration-items.md) <br/> |<span data-ttu-id="27666-269">予定表アイテムの期間を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-269">Represents the duration of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="27666-270">TimeZone (Item)</span><span class="sxs-lookup"><span data-stu-id="27666-270">TimeZone (Item)</span></span>](timezone-item.md) <br/> |<span data-ttu-id="27666-271">タイムゾーンのテキストの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="27666-271">Provides a text description of a time zone.</span></span>  <br/> |
|[<span data-ttu-id="27666-272">AppointmentReplyTime</span><span class="sxs-lookup"><span data-stu-id="27666-272">AppointmentReplyTime</span></span>](appointmentreplytime.md) <br/> |<span data-ttu-id="27666-273">出席者が会議出席依頼に返信した日時を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-273">Represents the date and time when an attendee replied to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="27666-274">AppointmentSequenceNumber</span><span class="sxs-lookup"><span data-stu-id="27666-274">AppointmentSequenceNumber</span></span>](appointmentsequencenumber.md) <br/> |<span data-ttu-id="27666-275">予定のバージョンのシーケンス番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="27666-275">Specifies the sequence number of a version of an appointment.</span></span>  <br/> |
|[<span data-ttu-id="27666-276">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="27666-276">AppointmentState</span></span>](appointmentstate.md) <br/> |<span data-ttu-id="27666-277">予定の状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="27666-277">Specifies the status of the appointment.</span></span>  <br/> |
|[<span data-ttu-id="27666-278">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="27666-278">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="27666-279">予定表アイテムと会議出席依頼の定期的なパターンを含みます。</span><span class="sxs-lookup"><span data-stu-id="27666-279">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="27666-280">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="27666-280">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="27666-281">定期的な予定表アイテムの最初の出現を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-281">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="27666-282">[Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。</span><span class="sxs-lookup"><span data-stu-id="27666-282">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="27666-283">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="27666-283">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="27666-284">定期的な予定表アイテムの最後の発生を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-284">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="27666-285">[Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。</span><span class="sxs-lookup"><span data-stu-id="27666-285">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="27666-286">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="27666-286">ModifiedOccurrences</span></span>](modifiedoccurrences.md) <br/> |<span data-ttu-id="27666-287">定期的な予定表アイテムの定期的なアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="27666-287">Contains an array of recurring calendar item occurrences that have been modified so that they are different than the recurrence master item.</span></span>  <br/> <span data-ttu-id="27666-288">[Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。</span><span class="sxs-lookup"><span data-stu-id="27666-288">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="27666-289">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="27666-289">DeletedOccurrences</span></span>](deletedoccurrences.md) <br/> |<span data-ttu-id="27666-290">定期的な予定表アイテムの削除された出現の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="27666-290">Contains an array of deleted occurrences of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="27666-291">[Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。</span><span class="sxs-lookup"><span data-stu-id="27666-291">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="27666-292">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="27666-292">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="27666-293">会議がホストされている場所のタイムゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="27666-293">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
|[<span data-ttu-id="27666-294">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="27666-294">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="27666-295">予定表アイテムの開始タイムゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="27666-295">Represents the start time zone of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="27666-296">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="27666-296">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="27666-297">予定表アイテムの終了タイムゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="27666-297">Represents the end time zone of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="27666-298">ConferenceType</span><span class="sxs-lookup"><span data-stu-id="27666-298">ConferenceType</span></span>](conferencetype.md) <br/> |<span data-ttu-id="27666-299">予定表アイテムで実行される会議の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="27666-299">Describes the type of conferencing that is performed with a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="27666-300">AllowNewTimeProposal</span><span class="sxs-lookup"><span data-stu-id="27666-300">AllowNewTimeProposal</span></span>](allownewtimeproposal.md) <br/> |<span data-ttu-id="27666-301">会議の新しい会議日時を提案できるかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="27666-301">Represents whether a new meeting time can be proposed for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="27666-302">IsOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="27666-302">IsOnlineMeeting</span></span>](isonlinemeeting.md) <br/> |<span data-ttu-id="27666-303">会議がオンラインかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-303">Indicates whether the meeting is online.</span></span>  <br/> |
|[<span data-ttu-id="27666-304">MeetingWorkspaceUrl</span><span class="sxs-lookup"><span data-stu-id="27666-304">MeetingWorkspaceUrl</span></span>](meetingworkspaceurl.md) <br/> |<span data-ttu-id="27666-305">予定表アイテムにリンクされている会議ワークスペースの URL が含まれます。</span><span class="sxs-lookup"><span data-stu-id="27666-305">Contains the URL for the meeting workspace that is linked to by the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="27666-306">NetShowUrl</span><span class="sxs-lookup"><span data-stu-id="27666-306">NetShowUrl</span></span>](netshowurl.md) <br/> |<span data-ttu-id="27666-307">Microsoft Netshow online 会議の URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="27666-307">Specifies the URL for a Microsoft Netshow online meeting.</span></span>  <br/> |
|[<span data-ttu-id="27666-308">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="27666-308">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="27666-309">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="27666-309">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="27666-310">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="27666-310">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="27666-311">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="27666-311">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="27666-312">アイテムを最後に変更したユーザーの表示名を含みます。</span><span class="sxs-lookup"><span data-stu-id="27666-312">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="27666-313">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="27666-313">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="27666-314">アイテムが最後に変更された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="27666-314">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="27666-315">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="27666-315">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="27666-316">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="27666-316">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="27666-317">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="27666-317">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="27666-318">Outlook Web app のアイテムを読み取るために Microsoft Office Outlook Web App エンドポイントに連結する URL を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-318">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="27666-319">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="27666-319">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="27666-320">Outlook web app エンドポイントに連結して Outlook Web App のアイテムを編集するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-320">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="27666-321">ConversationId</span><span class="sxs-lookup"><span data-stu-id="27666-321">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="27666-322">アイテムまたは会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="27666-322">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="27666-323">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="27666-323">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="27666-324">この会話の一意の本文を表す HTML フラグメントまたはプレーンテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="27666-324">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="27666-325">UID</span><span class="sxs-lookup"><span data-stu-id="27666-325">UID</span></span>](uid.md) <br/> |<span data-ttu-id="27666-326">予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="27666-326">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="27666-327">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="27666-327">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="27666-328">定期的な予定表アイテムの特定のインスタンスを識別するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="27666-328">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="27666-329">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="27666-329">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="27666-330">ICalendar オブジェクトのインスタンスが作成された日付と時刻を示します。</span><span class="sxs-lookup"><span data-stu-id="27666-330">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="27666-331">親要素</span><span class="sxs-lookup"><span data-stu-id="27666-331">Parent elements</span></span>

|<span data-ttu-id="27666-332">**要素**</span><span class="sxs-lookup"><span data-stu-id="27666-332">**Element**</span></span>|<span data-ttu-id="27666-333">**説明**</span><span class="sxs-lookup"><span data-stu-id="27666-333">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27666-334">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="27666-334">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="27666-335">会議の時刻に隣接しているすべての予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="27666-335">Identifies all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="27666-336">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="27666-336">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="27666-337">[Updateitem 操作](updateitem-operation.md)中に、アイテムの1つのプロパティに追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="27666-337">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="27666-338">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="27666-338">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="27666-339">会議の時間と競合するすべてのアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="27666-339">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="27666-340">Create (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="27666-340">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="27666-341">ローカルクライアントストアに作成する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="27666-341">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="27666-342">Items</span><span class="sxs-lookup"><span data-stu-id="27666-342">Items</span></span>](items.md) <br/> |<span data-ttu-id="27666-343">項目の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="27666-343">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="27666-344">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="27666-344">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="27666-345">作成するアイテムの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="27666-345">Contains an array of items to create.</span></span>  <br/> |
|[<span data-ttu-id="27666-346">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="27666-346">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="27666-347">別の Exchange アイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="27666-347">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="27666-348">SetItemField</span><span class="sxs-lookup"><span data-stu-id="27666-348">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="27666-349">[Updateitem 操作](updateitem-operation.md)のアイテムの1つのプロパティに対する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="27666-349">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="27666-350">Update (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="27666-350">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="27666-351">ローカルクライアントストアで更新する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="27666-351">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="27666-352">テキスト値</span><span class="sxs-lookup"><span data-stu-id="27666-352">Text value</span></span>

<span data-ttu-id="27666-353">なし。</span><span class="sxs-lookup"><span data-stu-id="27666-353">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="27666-354">注釈</span><span class="sxs-lookup"><span data-stu-id="27666-354">Remarks</span></span>

<span data-ttu-id="27666-355">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="27666-355">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27666-356">要素の情報</span><span class="sxs-lookup"><span data-stu-id="27666-356">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27666-357">Namespace</span><span class="sxs-lookup"><span data-stu-id="27666-357">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="27666-358">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="27666-358">Schema Name</span></span>  <br/> |<span data-ttu-id="27666-359">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="27666-359">Types schema</span></span>  <br/> |
|<span data-ttu-id="27666-360">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="27666-360">Validation File</span></span>  <br/> |<span data-ttu-id="27666-361">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="27666-361">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="27666-362">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="27666-362">Can be Empty</span></span>  <br/> |<span data-ttu-id="27666-363">正しくない</span><span class="sxs-lookup"><span data-stu-id="27666-363">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27666-364">関連項目</span><span class="sxs-lookup"><span data-stu-id="27666-364">See also</span></span>



- [<span data-ttu-id="27666-365">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="27666-365">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


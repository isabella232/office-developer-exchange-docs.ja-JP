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
description: MeetingRequest 要素は、Exchange ストア内の会議出席依頼を表します。
ms.openlocfilehash: 3e290613293cb6ad1563912e5015742ffc503d08
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832450"
---
# <a name="meetingrequest"></a><span data-ttu-id="5c151-103">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="5c151-103">MeetingRequest</span></span>

<span data-ttu-id="5c151-104">**MeetingRequest**要素は、Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-104">The **MeetingRequest** element represents a meeting request in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="5c151-105">**MeetingRequestMessageType**</span><span class="sxs-lookup"><span data-stu-id="5c151-105">**MeetingRequestMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c151-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5c151-106">Attributes and elements</span></span>

<span data-ttu-id="5c151-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5c151-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c151-108">属性</span><span class="sxs-lookup"><span data-stu-id="5c151-108">Attributes</span></span>

<span data-ttu-id="5c151-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5c151-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c151-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5c151-110">Child elements</span></span>

|<span data-ttu-id="5c151-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="5c151-111">**Element**</span></span>|<span data-ttu-id="5c151-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5c151-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c151-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="5c151-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="5c151-114">Base64Binary の形式で表されるオブジェクトのネイティブの多目的インターネット メール拡張 (MIME) ストリームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c151-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="5c151-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="5c151-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="5c151-116">Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c151-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="5c151-117">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="5c151-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5c151-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="5c151-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="5c151-119">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="5c151-120">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="5c151-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5c151-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="5c151-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="5c151-122">アイテムのメッセージ クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-123">Subject</span><span class="sxs-lookup"><span data-stu-id="5c151-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="5c151-124">Exchange ストアのアイテムおよび応答オブジェクトのサブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="5c151-125">件名は、255 文字までに制限されています。</span><span class="sxs-lookup"><span data-stu-id="5c151-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="5c151-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="5c151-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="5c151-127">アイテムの秘密度レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-128">Body/本文</span><span class="sxs-lookup"><span data-stu-id="5c151-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="5c151-129">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="5c151-130">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="5c151-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5c151-131">アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c151-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c151-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="5c151-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="5c151-133">データと、メールボックス内のアイテムを受信した時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-133">Represents the data and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="5c151-134">Size</span><span class="sxs-lookup"><span data-stu-id="5c151-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="5c151-135">アイテムのバイト単位のサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="5c151-136">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="5c151-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5c151-137">Categories</span><span class="sxs-lookup"><span data-stu-id="5c151-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5c151-138">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="5c151-139">Importance</span><span class="sxs-lookup"><span data-stu-id="5c151-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="5c151-140">アイテムの重要性をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="5c151-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="5c151-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="5c151-142">このアイテムの返信するアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="5c151-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="5c151-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="5c151-144">アイテムが [送信トレイ] 既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="5c151-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="5c151-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="5c151-146">かどうかの項目がまだ送信されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-146">Indicates whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="5c151-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="5c151-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="5c151-148">ユーザーが自身にアイテムを送信するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-148">Indicates whether a user sent an item to itself.</span></span>  <br/> |
|[<span data-ttu-id="5c151-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="5c151-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="5c151-150">アイテムが以前送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="5c151-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="5c151-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="5c151-152">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="5c151-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="5c151-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="5c151-154">メールボックス内のアイテムに含まれているすべてのインターネット メッセージ ヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-154">Represents the collection of all Internet message headers contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5c151-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="5c151-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="5c151-156">メールボックス内のアイテムが送信された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="5c151-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="5c151-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="5c151-158">メールボックス内の特定のアイテムが作成された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="5c151-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="5c151-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="5c151-160">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c151-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c151-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="5c151-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="5c151-162">イベントが発生したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="5c151-163">[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によってアラームが表示されたときを決定する使用されます。</span><span class="sxs-lookup"><span data-stu-id="5c151-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="5c151-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="5c151-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="5c151-165">Exchange ストアのアイテムのアラームが設定されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5c151-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="5c151-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="5c151-167">分前にアラームが表示されるときに、イベントの数を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="5c151-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="5c151-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="5c151-169">[Cc] 行の内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-169">Represents the display string that is used for the contents of the CC line.</span></span> <span data-ttu-id="5c151-170">これは、すべての CC 受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="5c151-170">This is the concatenated string of all CC recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="5c151-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="5c151-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="5c151-172">行の内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-172">Represents the display string that is used for the contents of the To line.</span></span> <span data-ttu-id="5c151-173">これは、すべての受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="5c151-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="5c151-174">添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="5c151-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="5c151-175">アイテムに表示されている 1 つ以上の添付ファイルがある場合に**true**に設定されているプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="5c151-176">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5c151-176">This property is read only.</span></span>  <br/> |
|[<span data-ttu-id="5c151-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="5c151-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="5c151-178">フォルダーおよびアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="5c151-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="5c151-179">カルチャ</span><span class="sxs-lookup"><span data-stu-id="5c151-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="5c151-180">メールボックス内の指定したアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5c151-181">送信者</span><span class="sxs-lookup"><span data-stu-id="5c151-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="5c151-182">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="5c151-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="5c151-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="5c151-184">一連メッセージの受信者にはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c151-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="5c151-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="5c151-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="5c151-186">メッセージのコピーを受け取る受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="5c151-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="5c151-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="5c151-188">電子メールのブラインド カーボン コピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="5c151-189">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="5c151-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="5c151-190">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="5c151-191">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="5c151-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="5c151-192">アイテムの送信者が配信済みメッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="5c151-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="5c151-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="5c151-194">このメッセージが属するスレッドを表すバイナリの ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c151-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="5c151-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="5c151-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="5c151-196">会話 id を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="5c151-197">From</span><span class="sxs-lookup"><span data-stu-id="5c151-197">From</span></span>](from.md) <br/> |<span data-ttu-id="5c151-198">メッセージの送信元アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="5c151-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="5c151-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="5c151-200">アイテムのインターネット メッセージ id を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-201">IsRead</span><span class="sxs-lookup"><span data-stu-id="5c151-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="5c151-202">メッセージが読み取られたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="5c151-203">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="5c151-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="5c151-204">電子メール メッセージへの応答が要求されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="5c151-205">参照資料</span><span class="sxs-lookup"><span data-stu-id="5c151-205">References</span></span>](references.md) <br/> |<span data-ttu-id="5c151-206">元のメッセージに応答を関連付けるために使用する Usenet ヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="5c151-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="5c151-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="5c151-208">応答を送信するアドレスのセットを識別します。</span><span class="sxs-lookup"><span data-stu-id="5c151-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="5c151-209">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="5c151-209">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="5c151-210">の[MeetingMessage](meetingmessage.md)に関連付けられている予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-210">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="5c151-211">IsDelegated</span><span class="sxs-lookup"><span data-stu-id="5c151-211">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="5c151-212">会議は、代理人アクセスを持つアカウントによって処理されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-212">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="5c151-213">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="5c151-213">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="5c151-214">会議メッセージが期限切れかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-214">Indicates whether a meeting message is out of date.</span></span>  <br/> |
|[<span data-ttu-id="5c151-215">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="5c151-215">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="5c151-216">かどうか、会議出席依頼アイテムが処理されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-216">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="5c151-217">ResponseType</span><span class="sxs-lookup"><span data-stu-id="5c151-217">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="5c151-218">会議を受信する受信者の応答の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-218">Represents the kind of recipient response that is received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="5c151-219">MeetingRequestType</span><span class="sxs-lookup"><span data-stu-id="5c151-219">MeetingRequestType</span></span>](meetingrequesttype.md) <br/> |<span data-ttu-id="5c151-220">会議出席依頼の種類について説明します。</span><span class="sxs-lookup"><span data-stu-id="5c151-220">Describes the type of the meeting request.</span></span>  <br/> |
|[<span data-ttu-id="5c151-221">IntendedFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="5c151-221">IntendedFreeBusyStatus</span></span>](intendedfreebusystatus.md) <br/> |<span data-ttu-id="5c151-222">会議出席依頼に関連付けられている予定表アイテムの目的の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-222">Represents the intended status for the calendar item that is associated with the meeting request.</span></span>  <br/> |
|[<span data-ttu-id="5c151-223">Start</span><span class="sxs-lookup"><span data-stu-id="5c151-223">Start</span></span>](start.md) <br/> |<span data-ttu-id="5c151-224">予定表アイテムの開始を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-224">Represents the start of a calendar item.</span></span> <span data-ttu-id="5c151-225">この要素は、予定表アイテムの 1 回のみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="5c151-225">This element only applies to a single occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-226">終わり</span><span class="sxs-lookup"><span data-stu-id="5c151-226">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5c151-227">期間の終了を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-227">Represents the end of a duration.</span></span> <span data-ttu-id="5c151-228">この要素は、予定表アイテムの 1 回のみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="5c151-228">This element only applies to a single occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-229">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="5c151-229">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="5c151-230">予定表アイテムの元の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-230">Represents the original start time of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-231">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="5c151-231">IsAllDayEvent</span></span>](isalldayevent.md) <br/> |<span data-ttu-id="5c151-232">予定表アイテムまたは会議出席依頼が終日のイベントを表すかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-232">Indicates whether a calendar item or meeting request represents an all-day event.</span></span>  <br/> |
|[<span data-ttu-id="5c151-233">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="5c151-233">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md) <br/> |<span data-ttu-id="5c151-234">予定表アイテムの空き/予約済み状態を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-234">Represents the free/busy status of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-235">場所</span><span class="sxs-lookup"><span data-stu-id="5c151-235">Location</span></span>](location.md) <br/> |<span data-ttu-id="5c151-236">会議または予定の場所を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-236">Represents the location of a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="5c151-237">When</span><span class="sxs-lookup"><span data-stu-id="5c151-237">When</span></span>](when.md) <br/> |<span data-ttu-id="5c151-238">会議が発生した場合の説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="5c151-238">Provides a description of when a meeting occurs.</span></span>  <br/> |
|[<span data-ttu-id="5c151-239">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="5c151-239">IsMeeting</span></span>](ismeeting.md) <br/> |<span data-ttu-id="5c151-240">予定表アイテムを会議または予定のいずれかにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-240">Indicates whether the calendar item is either a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="5c151-241">IsCancelled</span><span class="sxs-lookup"><span data-stu-id="5c151-241">IsCancelled</span></span>](iscancelled.md) <br/> |<span data-ttu-id="5c151-242">予定または会議が取り消されましたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-242">Indicates whether an appointment or meeting has been cancelled.</span></span>  <br/> |
|[<span data-ttu-id="5c151-243">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="5c151-243">IsRecurring</span></span>](isrecurring.md) <br/> |<span data-ttu-id="5c151-244">予定表アイテムが定期的なアイテムの一部であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-244">Indicates whether a calendar item is part of a recurring item.</span></span> <span data-ttu-id="5c151-245">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5c151-245">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5c151-246">MeetingRequestWasSent</span><span class="sxs-lookup"><span data-stu-id="5c151-246">MeetingRequestWasSent</span></span>](meetingrequestwassent.md) <br/> |<span data-ttu-id="5c151-247">要求された出席者に会議出席依頼が送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-247">Indicates whether a meeting request has been sent to requested attendees.</span></span>  <br/> |
|[<span data-ttu-id="5c151-248">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="5c151-248">CalendarItemType</span></span>](calendaritemtype.md) <br/> |<span data-ttu-id="5c151-249">予定表アイテムのアイテムの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-249">Represents the occurrence type of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-250">MyResponseType</span><span class="sxs-lookup"><span data-stu-id="5c151-250">MyResponseType</span></span>](myresponsetype.md) <br/> |<span data-ttu-id="5c151-251">ステータス、または予定表アイテムへの応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c151-251">Contains the status of or response to a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-252">Organizer</span><span class="sxs-lookup"><span data-stu-id="5c151-252">Organizer</span></span>](organizer.md) <br/> |<span data-ttu-id="5c151-253">会議の開催者を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-253">Represents the organizer of a meeting.</span></span>  <br/> |
|[<span data-ttu-id="5c151-254">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="5c151-254">RequiredAttendees</span></span>](requiredattendees.md) <br/> |<span data-ttu-id="5c151-255">会議に出席するために必要な出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-255">Represents attendees that are required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="5c151-256">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="5c151-256">OptionalAttendees</span></span>](optionalattendees.md) <br/> |<span data-ttu-id="5c151-257">出席者が会議に出席する必要がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-257">Represents attendees that are not required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="5c151-258">リソース</span><span class="sxs-lookup"><span data-stu-id="5c151-258">Resources</span></span>](resources.md) <br/> |<span data-ttu-id="5c151-259">会議のスケジュール設定されたリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-259">Represents a scheduled resource for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="5c151-260">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="5c151-260">ConflictingMeetingCount</span></span>](conflictingmeetingcount.md) <br/> |<span data-ttu-id="5c151-261">競合する会議出席依頼と会議の数を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-261">Represents the number of meetings that conflict with the meeting request.</span></span>  <br/> |
|[<span data-ttu-id="5c151-262">AdjacentMeetingCount</span><span class="sxs-lookup"><span data-stu-id="5c151-262">AdjacentMeetingCount</span></span>](adjacentmeetingcount.md) <br/> |<span data-ttu-id="5c151-263">会議の時刻に隣接している予定表アイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-263">Represents the total number of calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="5c151-264">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="5c151-264">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="5c151-265">会議の時間と競合するすべての項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="5c151-265">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="5c151-266">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="5c151-266">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="5c151-267">会議の時刻に隣接しているすべての予定表のアイテムについて説明します。</span><span class="sxs-lookup"><span data-stu-id="5c151-267">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="5c151-268">期間 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="5c151-268">Duration (Items)</span></span>](duration-items.md) <br/> |<span data-ttu-id="5c151-269">予定表アイテムの期間を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-269">Represents the duration of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-270">タイムゾーン (アイテム)</span><span class="sxs-lookup"><span data-stu-id="5c151-270">TimeZone (Item)</span></span>](timezone-item.md) <br/> |<span data-ttu-id="5c151-271">タイム ゾーンの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="5c151-271">Provides a text description of a time zone.</span></span>  <br/> |
|[<span data-ttu-id="5c151-272">AppointmentReplyTime</span><span class="sxs-lookup"><span data-stu-id="5c151-272">AppointmentReplyTime</span></span>](appointmentreplytime.md) <br/> |<span data-ttu-id="5c151-273">会議出席依頼に出席者が返信したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-273">Represents the date and time when an attendee replied to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="5c151-274">AppointmentSequenceNumber</span><span class="sxs-lookup"><span data-stu-id="5c151-274">AppointmentSequenceNumber</span></span>](appointmentsequencenumber.md) <br/> |<span data-ttu-id="5c151-275">予定のバージョンのシーケンス番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="5c151-275">Specifies the sequence number of a version of an appointment.</span></span>  <br/> |
|[<span data-ttu-id="5c151-276">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="5c151-276">AppointmentState</span></span>](appointmentstate.md) <br/> |<span data-ttu-id="5c151-277">予定の状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="5c151-277">Specifies the status of the appointment.</span></span>  <br/> |
|[<span data-ttu-id="5c151-278">定期的なアイテム (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="5c151-278">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="5c151-279">予定表アイテムおよび会議出席依頼に定期的なパターンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c151-279">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="5c151-280">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="5c151-280">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="5c151-281">定期的な予定表アイテムが最初に見つかった位置を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-281">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="5c151-282">この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。</span><span class="sxs-lookup"><span data-stu-id="5c151-282">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="5c151-283">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="5c151-283">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="5c151-284">定期的な予定表アイテムが最後に見つかった位置を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-284">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="5c151-285">この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。</span><span class="sxs-lookup"><span data-stu-id="5c151-285">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="5c151-286">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="5c151-286">ModifiedOccurrences</span></span>](modifiedoccurrences.md) <br/> |<span data-ttu-id="5c151-287">定期的な予定のマスター アイテムとは異なるものに変更された定期的な予定表アイテム アイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c151-287">Contains an array of recurring calendar item occurrences that have been modified so that they are different than the recurrence master item.</span></span>  <br/> <span data-ttu-id="5c151-288">この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。</span><span class="sxs-lookup"><span data-stu-id="5c151-288">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="5c151-289">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="5c151-289">DeletedOccurrences</span></span>](deletedoccurrences.md) <br/> |<span data-ttu-id="5c151-290">定期的な予定表アイテムの削除済みアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c151-290">Contains an array of deleted occurrences of a recurring calendar item.</span></span>  <br/> <span data-ttu-id="5c151-291">この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。</span><span class="sxs-lookup"><span data-stu-id="5c151-291">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span>  <br/> |
|[<span data-ttu-id="5c151-292">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="5c151-292">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="5c151-293">会議がホストされている場所のタイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-293">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
|[<span data-ttu-id="5c151-294">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="5c151-294">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="5c151-295">予定表アイテムの開始タイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-295">Represents the start time zone of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-296">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="5c151-296">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="5c151-297">予定表アイテムの終了タイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-297">Represents the end time zone of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-298">ConferenceType</span><span class="sxs-lookup"><span data-stu-id="5c151-298">ConferenceType</span></span>](conferencetype.md) <br/> |<span data-ttu-id="5c151-299">予定表アイテムで実行される会議の種類について説明します。</span><span class="sxs-lookup"><span data-stu-id="5c151-299">Describes the type of conferencing that is performed with a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-300">AllowNewTimeProposal</span><span class="sxs-lookup"><span data-stu-id="5c151-300">AllowNewTimeProposal</span></span>](allownewtimeproposal.md) <br/> |<span data-ttu-id="5c151-301">会議の新しい日時を提案できるは会議のためかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-301">Represents whether a new meeting time can be proposed for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="5c151-302">IsOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="5c151-302">IsOnlineMeeting</span></span>](isonlinemeeting.md) <br/> |<span data-ttu-id="5c151-303">会議がオンラインかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-303">Indicates whether the meeting is online.</span></span>  <br/> |
|[<span data-ttu-id="5c151-304">MeetingWorkspaceUrl</span><span class="sxs-lookup"><span data-stu-id="5c151-304">MeetingWorkspaceUrl</span></span>](meetingworkspaceurl.md) <br/> |<span data-ttu-id="5c151-305">予定表アイテムにリンクされている会議ワークスペースの URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c151-305">Contains the URL for the meeting workspace that is linked to by the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-306">NetShowUrl</span><span class="sxs-lookup"><span data-stu-id="5c151-306">NetShowUrl</span></span>](netshowurl.md) <br/> |<span data-ttu-id="5c151-307">Microsoft Netshow オンライン会議の URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5c151-307">Specifies the URL for a Microsoft Netshow online meeting.</span></span>  <br/> |
|[<span data-ttu-id="5c151-308">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="5c151-308">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="5c151-309">アイテムまたはフォルダーのアクセス許可の設定に基づいてクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c151-309">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="5c151-310">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5c151-310">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5c151-311">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="5c151-311">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="5c151-312">最後の項目を変更するのにはユーザーの表示名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c151-312">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-313">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="5c151-313">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="5c151-314">アイテムが最後に修正された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-314">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="5c151-315">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="5c151-315">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="5c151-316">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-316">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="5c151-317">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="5c151-317">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="5c151-318">Outlook Web App 内の項目を参照するのには Microsoft Office Outlook の Web アプリケーションのエンドポイントを結合するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-318">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="5c151-319">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="5c151-319">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="5c151-320">Outlook Web App 内の項目を編集するのには Outlook Web App エンドポイントへの連結に URL を表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-320">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="5c151-321">ConversationId</span><span class="sxs-lookup"><span data-stu-id="5c151-321">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="5c151-322">アイテムや会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c151-322">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="5c151-323">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="5c151-323">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="5c151-324">このスレッドの一意の本文を表すテキストまたは HTML フラグメントを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-324">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="5c151-325">UID</span><span class="sxs-lookup"><span data-stu-id="5c151-325">UID</span></span>](uid.md) <br/> |<span data-ttu-id="5c151-326">予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="5c151-326">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-327">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="5c151-327">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="5c151-328">定期的な予定表アイテムの特定のインスタンスを識別するために使用します。</span><span class="sxs-lookup"><span data-stu-id="5c151-328">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-329">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="5c151-329">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="5c151-330">ICalendar オブジェクトのインスタンスが作成された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="5c151-330">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5c151-331">親要素</span><span class="sxs-lookup"><span data-stu-id="5c151-331">Parent elements</span></span>

|<span data-ttu-id="5c151-332">**要素**</span><span class="sxs-lookup"><span data-stu-id="5c151-332">**Element**</span></span>|<span data-ttu-id="5c151-333">**説明**</span><span class="sxs-lookup"><span data-stu-id="5c151-333">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c151-334">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="5c151-334">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="5c151-335">会議の時刻に隣接しているすべての予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="5c151-335">Identifies all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="5c151-336">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="5c151-336">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="5c151-337">[UpdateItem 操作](updateitem-operation.md)中に 1 つのアイテムのプロパティを追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="5c151-337">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="5c151-338">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="5c151-338">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="5c151-339">会議の時間と競合するすべての項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="5c151-339">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="5c151-340">(ItemSync) を作成します。</span><span class="sxs-lookup"><span data-stu-id="5c151-340">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="5c151-341">ローカル クライアント ストアに作成する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="5c151-341">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="5c151-342">Items</span><span class="sxs-lookup"><span data-stu-id="5c151-342">Items</span></span>](items.md) <br/> |<span data-ttu-id="5c151-343">項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c151-343">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="5c151-344">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="5c151-344">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="5c151-345">作成する項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c151-345">Contains an array of items to create.</span></span>  <br/> |
|[<span data-ttu-id="5c151-346">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="5c151-346">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="5c151-347">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-347">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="5c151-348">SetItemField</span><span class="sxs-lookup"><span data-stu-id="5c151-348">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="5c151-349">[UpdateItem 操作](updateitem-operation.md)内の項目の 1 つのプロパティには、更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="5c151-349">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="5c151-350">更新プログラム (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="5c151-350">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="5c151-351">ローカル クライアント ストアで更新する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="5c151-351">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5c151-352">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5c151-352">Text value</span></span>

<span data-ttu-id="5c151-353">なし。</span><span class="sxs-lookup"><span data-stu-id="5c151-353">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5c151-354">備考</span><span class="sxs-lookup"><span data-stu-id="5c151-354">Remarks</span></span>

<span data-ttu-id="5c151-355">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5c151-355">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c151-356">要素情報</span><span class="sxs-lookup"><span data-stu-id="5c151-356">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c151-357">名前空間</span><span class="sxs-lookup"><span data-stu-id="5c151-357">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5c151-358">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5c151-358">Schema Name</span></span>  <br/> |<span data-ttu-id="5c151-359">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5c151-359">Types schema</span></span>  <br/> |
|<span data-ttu-id="5c151-360">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5c151-360">Validation File</span></span>  <br/> |<span data-ttu-id="5c151-361">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5c151-361">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5c151-362">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5c151-362">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c151-363">False</span><span class="sxs-lookup"><span data-stu-id="5c151-363">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c151-364">関連項目</span><span class="sxs-lookup"><span data-stu-id="5c151-364">See also</span></span>



- [<span data-ttu-id="5c151-365">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5c151-365">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


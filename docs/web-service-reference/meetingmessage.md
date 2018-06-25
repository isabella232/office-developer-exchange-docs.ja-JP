---
title: MeetingMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingMessage
api_type:
- schema
ms.assetid: c95956a8-7505-44b4-bea4-11d1f5182796
description: MeetingMessage 要素は、Exchange ストア内の会議を表します。
ms.openlocfilehash: a2e87bc9800ee1dc66c1a3110df76745ac7c05b6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832443"
---
# <a name="meetingmessage"></a><span data-ttu-id="78a58-103">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="78a58-103">MeetingMessage</span></span>

<span data-ttu-id="78a58-104">**MeetingMessage**要素は、Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-104">The **MeetingMessage** element represents a meeting in the Exchange store.</span></span> 
  
```xml
<MeetingMessage>
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
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</MeetingMessage>
```

 <span data-ttu-id="78a58-105">**MeetingMessageType**</span><span class="sxs-lookup"><span data-stu-id="78a58-105">**MeetingMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="78a58-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="78a58-106">Attributes and elements</span></span>

<span data-ttu-id="78a58-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="78a58-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78a58-108">属性</span><span class="sxs-lookup"><span data-stu-id="78a58-108">Attributes</span></span>

<span data-ttu-id="78a58-109">なし。</span><span class="sxs-lookup"><span data-stu-id="78a58-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78a58-110">子要素</span><span class="sxs-lookup"><span data-stu-id="78a58-110">Child elements</span></span>

|<span data-ttu-id="78a58-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="78a58-111">**Element**</span></span>|<span data-ttu-id="78a58-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="78a58-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78a58-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="78a58-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="78a58-114">Base64Binary の形式で表されるオブジェクトのネイティブの MIME ストリームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="78a58-114">Contains the native MIME stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="78a58-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="78a58-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="78a58-116">Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="78a58-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="78a58-117">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="78a58-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="78a58-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="78a58-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="78a58-119">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="78a58-120">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="78a58-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="78a58-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="78a58-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="78a58-122">アイテムのメッセージ クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="78a58-123">Subject</span><span class="sxs-lookup"><span data-stu-id="78a58-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="78a58-124">Exchange ストアのアイテムおよび応答オブジェクトのサブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="78a58-125">件名は、255 文字までに制限されています。</span><span class="sxs-lookup"><span data-stu-id="78a58-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="78a58-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="78a58-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="78a58-127">アイテムの秘密度の状態が含まれています。</span><span class="sxs-lookup"><span data-stu-id="78a58-127">Contains the status for an item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="78a58-128">Body/本文</span><span class="sxs-lookup"><span data-stu-id="78a58-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="78a58-129">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="78a58-130">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="78a58-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="78a58-131">アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="78a58-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="78a58-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="78a58-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="78a58-133">メールボックス内のアイテムを受信したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="78a58-134">Size</span><span class="sxs-lookup"><span data-stu-id="78a58-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="78a58-135">アイテムのバイト単位のサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="78a58-136">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="78a58-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="78a58-137">Categories</span><span class="sxs-lookup"><span data-stu-id="78a58-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="78a58-138">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="78a58-139">Importance</span><span class="sxs-lookup"><span data-stu-id="78a58-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="78a58-140">アイテムの重要性をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="78a58-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="78a58-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="78a58-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="78a58-142">このアイテムの返信するアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="78a58-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="78a58-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="78a58-144">アイテムが [送信トレイ] 既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="78a58-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="78a58-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="78a58-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="78a58-146">アイテムはまだ送信されていないかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="78a58-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="78a58-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="78a58-148">ユーザーが彼または彼女自身にアイテムを送信するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="78a58-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="78a58-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="78a58-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="78a58-150">アイテムが以前送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="78a58-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="78a58-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="78a58-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="78a58-152">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="78a58-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="78a58-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="78a58-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="78a58-154">メールボックス内のアイテムに含まれているすべてのインターネット メッセージ ヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="78a58-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="78a58-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="78a58-156">メールボックス内のアイテムが送信された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="78a58-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="78a58-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="78a58-158">メールボックス内の特定のアイテムが作成された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="78a58-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="78a58-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="78a58-160">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="78a58-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="78a58-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="78a58-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="78a58-162">イベントが発生したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="78a58-163">[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によってアラームが表示されたときを決定する使用されます。</span><span class="sxs-lookup"><span data-stu-id="78a58-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="78a58-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="78a58-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="78a58-165">Exchange ストアのアイテムのアラームが設定されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="78a58-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="78a58-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="78a58-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="78a58-167">分前にアラームが表示されるときに、イベントの数を表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="78a58-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="78a58-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="78a58-169">[Cc] ボックスの内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="78a58-170">これは、すべての Cc 受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="78a58-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="78a58-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="78a58-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="78a58-172">ボックスの内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="78a58-173">これは、すべての受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="78a58-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="78a58-174">添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="78a58-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="78a58-175">アイテムに表示されている 1 つ以上の添付ファイルがある場合に**true**に設定されているプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="78a58-176">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="78a58-176">This property is read only.</span></span>  <br/> |
|[<span data-ttu-id="78a58-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="78a58-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="78a58-178">フォルダーおよびアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="78a58-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="78a58-179">カルチャ</span><span class="sxs-lookup"><span data-stu-id="78a58-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="78a58-180">メールボックス内の指定したアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="78a58-181">送信者</span><span class="sxs-lookup"><span data-stu-id="78a58-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="78a58-182">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="78a58-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="78a58-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="78a58-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="78a58-184">一連メッセージの受信者にはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="78a58-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="78a58-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="78a58-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="78a58-186">メッセージのコピーを受け取る受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="78a58-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="78a58-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="78a58-188">電子メールのブラインド カーボン コピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="78a58-189">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="78a58-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="78a58-190">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="78a58-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="78a58-191">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="78a58-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="78a58-192">アイテムの送信者が配信済みメッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="78a58-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="78a58-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="78a58-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="78a58-194">このメッセージが属するスレッドを表すバイナリの ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="78a58-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="78a58-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="78a58-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="78a58-196">会話 id を表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="78a58-197">From</span><span class="sxs-lookup"><span data-stu-id="78a58-197">From</span></span>](from.md) <br/> |<span data-ttu-id="78a58-198">メッセージの送信元アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="78a58-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="78a58-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="78a58-200">アイテムのインターネット メッセージ id を表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="78a58-201">IsRead</span><span class="sxs-lookup"><span data-stu-id="78a58-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="78a58-202">メッセージが読み取られたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="78a58-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="78a58-203">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="78a58-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="78a58-204">電子メール メッセージへの応答が要求されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="78a58-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="78a58-205">参照資料</span><span class="sxs-lookup"><span data-stu-id="78a58-205">References</span></span>](references.md) <br/> |<span data-ttu-id="78a58-206">元のメッセージに応答を関連付けるために使用する Usenet ヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="78a58-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="78a58-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="78a58-208">応答を送信するアドレスのセットを識別します。</span><span class="sxs-lookup"><span data-stu-id="78a58-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="78a58-209">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="78a58-209">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="78a58-210">の[MeetingMessage](meetingmessage.md)に関連付けられている予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-210">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="78a58-211">IsDelegated</span><span class="sxs-lookup"><span data-stu-id="78a58-211">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="78a58-212">会議は、代理人アクセスを持つアカウントによって処理されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="78a58-212">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="78a58-213">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="78a58-213">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="78a58-214">会議メッセージが期限切れかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="78a58-214">Indicates whether a meeting message is out-of-date.</span></span>  <br/> |
|[<span data-ttu-id="78a58-215">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="78a58-215">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="78a58-216">かどうか、会議出席依頼アイテムが処理されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="78a58-216">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="78a58-217">ResponseType</span><span class="sxs-lookup"><span data-stu-id="78a58-217">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="78a58-218">会議の受信者の応答の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-218">Represents the type of recipient response received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="78a58-219">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="78a58-219">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="78a58-220">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="78a58-220">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="78a58-221">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="78a58-221">This element is read-only.</span></span> <span data-ttu-id="78a58-222">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="78a58-222">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="78a58-223">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="78a58-223">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="78a58-224">最後の項目を変更するのにはユーザーの表示名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="78a58-224">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="78a58-225">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="78a58-225">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="78a58-226">アイテムが最後に修正された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="78a58-226">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="78a58-227">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="78a58-227">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="78a58-228">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="78a58-228">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="78a58-229">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="78a58-229">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="78a58-230">Outlook Web App 内の項目を参照するのには Microsoft Office Outlook の Web アプリケーションのエンドポイントを結合するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-230">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="78a58-231">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="78a58-231">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="78a58-232">Outlook Web App 内の項目を編集するのには Outlook Web App エンドポイントへの連結に URL を表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-232">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="78a58-233">ConversationId</span><span class="sxs-lookup"><span data-stu-id="78a58-233">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="78a58-234">アイテムや会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="78a58-234">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="78a58-235">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="78a58-235">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="78a58-236">このスレッドの一意の本文を表すテキストまたは HTML フラグメントを表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-236">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="78a58-237">UID</span><span class="sxs-lookup"><span data-stu-id="78a58-237">UID</span></span>](uid.md) <br/> |<span data-ttu-id="78a58-238">予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="78a58-238">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="78a58-239">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="78a58-239">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="78a58-240">定期的な予定表アイテムの特定のインスタンスを識別するために使用します。</span><span class="sxs-lookup"><span data-stu-id="78a58-240">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="78a58-241">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="78a58-241">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="78a58-242">ICalendar オブジェクトのインスタンスが作成された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="78a58-242">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="78a58-243">親要素</span><span class="sxs-lookup"><span data-stu-id="78a58-243">Parent elements</span></span>

|<span data-ttu-id="78a58-244">**要素**</span><span class="sxs-lookup"><span data-stu-id="78a58-244">**Element**</span></span>|<span data-ttu-id="78a58-245">**説明**</span><span class="sxs-lookup"><span data-stu-id="78a58-245">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78a58-246">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="78a58-246">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="78a58-247">会議の時刻に隣接しているすべての予定表のアイテムについて説明します。</span><span class="sxs-lookup"><span data-stu-id="78a58-247">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="78a58-248">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="78a58-248">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="78a58-249">[UpdateItem 操作](updateitem-operation.md)中に 1 つのアイテムのプロパティを追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="78a58-249">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="78a58-250">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="78a58-250">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="78a58-251">会議の時間と競合するすべての項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="78a58-251">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="78a58-252">(ItemSync) を作成します。</span><span class="sxs-lookup"><span data-stu-id="78a58-252">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="78a58-253">ローカル クライアント ストアに作成する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="78a58-253">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="78a58-254">更新プログラム (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="78a58-254">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="78a58-255">ローカル クライアント ストアで更新する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="78a58-255">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="78a58-256">Items</span><span class="sxs-lookup"><span data-stu-id="78a58-256">Items</span></span>](items.md) <br/> |<span data-ttu-id="78a58-257">項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="78a58-257">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="78a58-258">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="78a58-258">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="78a58-259">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で指定されたフォルダーに作成する項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="78a58-259">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="78a58-260">SetItemField</span><span class="sxs-lookup"><span data-stu-id="78a58-260">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="78a58-261">[UpdateItem 操作](updateitem-operation.md)内の項目の 1 つのプロパティには、更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-261">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="78a58-262">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="78a58-262">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="78a58-263">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="78a58-263">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="78a58-264">テキスト値</span><span class="sxs-lookup"><span data-stu-id="78a58-264">Text value</span></span>

<span data-ttu-id="78a58-265">なし。</span><span class="sxs-lookup"><span data-stu-id="78a58-265">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="78a58-266">備考</span><span class="sxs-lookup"><span data-stu-id="78a58-266">Remarks</span></span>

<span data-ttu-id="78a58-267">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="78a58-267">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="78a58-268">要素情報</span><span class="sxs-lookup"><span data-stu-id="78a58-268">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78a58-269">名前空間</span><span class="sxs-lookup"><span data-stu-id="78a58-269">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="78a58-270">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="78a58-270">Schema Name</span></span>  <br/> |<span data-ttu-id="78a58-271">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="78a58-271">Types schema</span></span>  <br/> |
|<span data-ttu-id="78a58-272">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="78a58-272">Validation File</span></span>  <br/> |<span data-ttu-id="78a58-273">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="78a58-273">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="78a58-274">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="78a58-274">Can be Empty</span></span>  <br/> |<span data-ttu-id="78a58-275">False</span><span class="sxs-lookup"><span data-stu-id="78a58-275">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="78a58-276">関連項目</span><span class="sxs-lookup"><span data-stu-id="78a58-276">See also</span></span>



- [<span data-ttu-id="78a58-277">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="78a58-277">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


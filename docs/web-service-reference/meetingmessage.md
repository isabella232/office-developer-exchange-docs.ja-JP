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
description: 会議メッセージ要素は、Exchange ストア内の会議を表します。
ms.openlocfilehash: fee615a1da117e5df03cd5ce8576bd66d7e89a4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468384"
---
# <a name="meetingmessage"></a><span data-ttu-id="ded9e-103">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="ded9e-103">MeetingMessage</span></span>

<span data-ttu-id="ded9e-104">会議**メッセージ**要素は、Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-104">The **MeetingMessage** element represents a meeting in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="ded9e-105">**MeetingMessageType**</span><span class="sxs-lookup"><span data-stu-id="ded9e-105">**MeetingMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ded9e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ded9e-106">Attributes and elements</span></span>

<span data-ttu-id="ded9e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ded9e-108">属性</span><span class="sxs-lookup"><span data-stu-id="ded9e-108">Attributes</span></span>

<span data-ttu-id="ded9e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ded9e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ded9e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ded9e-110">Child elements</span></span>

|<span data-ttu-id="ded9e-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="ded9e-111">**Element**</span></span>|<span data-ttu-id="ded9e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ded9e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ded9e-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="ded9e-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="ded9e-114">Base64Binary 形式で表されるオブジェクトのネイティブ MIME ストリームが格納されています。</span><span class="sxs-lookup"><span data-stu-id="ded9e-114">Contains the native MIME stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="ded9e-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ded9e-116">Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ded9e-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="ded9e-117">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="ded9e-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="ded9e-119">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="ded9e-120">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="ded9e-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="ded9e-122">アイテムのメッセージクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-122">Represents the message class of an item.</span></span>  <br/> |
|<span data-ttu-id="ded9e-123">[[件名]](subject.md)</span><span class="sxs-lookup"><span data-stu-id="ded9e-123">[Subject](subject.md)</span></span> <br/> |<span data-ttu-id="ded9e-124">Exchange ストアアイテムおよび応答オブジェクトの件名を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="ded9e-125">件名は255文字に制限されます。</span><span class="sxs-lookup"><span data-stu-id="ded9e-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="ded9e-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="ded9e-127">アイテムの秘密度の状態を格納します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-127">Contains the status for an item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-128">Body</span><span class="sxs-lookup"><span data-stu-id="ded9e-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="ded9e-129">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-130">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="ded9e-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ded9e-131">Exchange ストア内のアイテムに添付されているアイテムまたはファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="ded9e-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="ded9e-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="ded9e-133">メールボックス内のアイテムが受信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|<span data-ttu-id="ded9e-134">[[サイズ]](size.md)</span><span class="sxs-lookup"><span data-stu-id="ded9e-134">[Size](size.md)</span></span> <br/> |<span data-ttu-id="ded9e-135">アイテムのサイズ (バイト単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="ded9e-136">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-137">カテゴリ</span><span class="sxs-lookup"><span data-stu-id="ded9e-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ded9e-138">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-139">Importance</span><span class="sxs-lookup"><span data-stu-id="ded9e-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="ded9e-140">アイテムの重要度について説明します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="ded9e-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="ded9e-142">このアイテムが返信であるアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="ded9e-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="ded9e-144">アイテムが送信トレイの既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="ded9e-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="ded9e-146">アイテムがまだ送信されていないかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="ded9e-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="ded9e-148">ユーザーが自分にアイテムを送信したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="ded9e-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="ded9e-150">アイテムが以前に送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="ded9e-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="ded9e-152">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="ded9e-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="ded9e-154">メールボックス内のアイテム内に含まれるすべてのインターネットメッセージヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="ded9e-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="ded9e-156">メールボックス内のアイテムが送信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="ded9e-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="ded9e-158">メールボックス内の特定のアイテムが作成された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="ded9e-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="ded9e-160">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="ded9e-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="ded9e-162">イベントが発生した日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="ded9e-163">これは、アラームがいつ表示されるかを決定するために[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="ded9e-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="ded9e-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="ded9e-165">Exchange ストア内のアイテムにアラームが設定されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="ded9e-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="ded9e-167">アラームが表示されるイベントの前の時間 (分単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="ded9e-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="ded9e-169">[Cc] ボックスの内容に使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="ded9e-170">これは、すべての Cc 受信者表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="ded9e-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="ded9e-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="ded9e-172">[宛先] ボックスの内容に対して使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="ded9e-173">これは、すべての受信者の表示名の連結文字列です。</span><span class="sxs-lookup"><span data-stu-id="ded9e-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="ded9e-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="ded9e-175">アイテムに少なくとも1つの添付ファイルがある場合に**true**に設定されるプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="ded9e-176">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ded9e-176">This property is read only.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="ded9e-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="ded9e-178">フォルダーとアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-179">Culture</span><span class="sxs-lookup"><span data-stu-id="ded9e-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="ded9e-180">メールボックス内の特定のアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-181">Sender</span><span class="sxs-lookup"><span data-stu-id="ded9e-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="ded9e-182">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="ded9e-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="ded9e-184">メッセージの受信者のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ded9e-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="ded9e-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="ded9e-186">メッセージのコピーを受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="ded9e-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="ded9e-188">電子メールのブラインドカーボンコピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-189">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="ded9e-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="ded9e-190">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-191">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="ded9e-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="ded9e-192">アイテムの送信者が配信確認を要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="ded9e-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="ded9e-194">このメッセージが属しているスレッドを表すバイナリ ID を含みます。</span><span class="sxs-lookup"><span data-stu-id="ded9e-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="ded9e-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="ded9e-196">会話識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-197">From</span><span class="sxs-lookup"><span data-stu-id="ded9e-197">From</span></span>](from.md) <br/> |<span data-ttu-id="ded9e-198">メッセージが送信された相手のアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="ded9e-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="ded9e-200">アイテムのインターネットメッセージ識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-201">IsRead</span><span class="sxs-lookup"><span data-stu-id="ded9e-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="ded9e-202">メッセージが開封されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-203">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="ded9e-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="ded9e-204">電子メールメッセージに対する応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-205">References</span><span class="sxs-lookup"><span data-stu-id="ded9e-205">References</span></span>](references.md) <br/> |<span data-ttu-id="ded9e-206">返信と元のメッセージを相互に関連付けるために使用される Usenet ヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="ded9e-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="ded9e-208">返信を送信する宛先のアドレスのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-209">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="ded9e-209">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="ded9e-210">[会議メッセージ](meetingmessage.md)に関連付けられている予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-210">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="ded9e-211">IsDelegated</span><span class="sxs-lookup"><span data-stu-id="ded9e-211">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="ded9e-212">代理人アクセス権を持つアカウントによって会議が処理されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-212">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-213">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="ded9e-213">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="ded9e-214">会議メッセージが古くなっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-214">Indicates whether a meeting message is out-of-date.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-215">Hasが処理されました</span><span class="sxs-lookup"><span data-stu-id="ded9e-215">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="ded9e-216">会議メッセージアイテムが処理されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-216">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-217">ResponseType</span><span class="sxs-lookup"><span data-stu-id="ded9e-217">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="ded9e-218">会議で受信した受信者の応答の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-218">Represents the type of recipient response received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-219">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="ded9e-219">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="ded9e-220">アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ded9e-220">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="ded9e-221">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="ded9e-221">This element is read-only.</span></span> <span data-ttu-id="ded9e-222">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ded9e-222">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="ded9e-223">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="ded9e-223">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="ded9e-224">アイテムを最後に変更したユーザーの表示名を含みます。</span><span class="sxs-lookup"><span data-stu-id="ded9e-224">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-225">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="ded9e-225">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="ded9e-226">アイテムが最後に変更された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-226">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-227">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="ded9e-227">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="ded9e-228">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-228">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-229">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="ded9e-229">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="ded9e-230">Outlook Web app のアイテムを読み取るために Microsoft Office Outlook Web App エンドポイントに連結する URL を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-230">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-231">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="ded9e-231">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="ded9e-232">Outlook web app エンドポイントに連結して Outlook Web App のアイテムを編集するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-232">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-233">ConversationId</span><span class="sxs-lookup"><span data-stu-id="ded9e-233">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="ded9e-234">アイテムまたは会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ded9e-234">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-235">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="ded9e-235">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="ded9e-236">この会話の一意の本文を表す HTML フラグメントまたはプレーンテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-236">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-237">UID</span><span class="sxs-lookup"><span data-stu-id="ded9e-237">UID</span></span>](uid.md) <br/> |<span data-ttu-id="ded9e-238">予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-238">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-239">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="ded9e-239">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="ded9e-240">定期的な予定表アイテムの特定のインスタンスを識別するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="ded9e-240">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-241">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="ded9e-241">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="ded9e-242">ICalendar オブジェクトのインスタンスが作成された日付と時刻を示します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-242">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ded9e-243">親要素</span><span class="sxs-lookup"><span data-stu-id="ded9e-243">Parent elements</span></span>

|<span data-ttu-id="ded9e-244">**要素**</span><span class="sxs-lookup"><span data-stu-id="ded9e-244">**Element**</span></span>|<span data-ttu-id="ded9e-245">**説明**</span><span class="sxs-lookup"><span data-stu-id="ded9e-245">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ded9e-246">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="ded9e-246">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="ded9e-247">会議の時刻に隣接しているすべての予定表アイテムを説明します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-247">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-248">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="ded9e-248">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="ded9e-249">[Updateitem 操作](updateitem-operation.md)中に、アイテムの1つのプロパティに追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-249">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ded9e-250">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="ded9e-250">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="ded9e-251">会議の時間と競合するすべてのアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-251">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-252">Create (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="ded9e-252">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="ded9e-253">ローカルクライアントストアに作成する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-253">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-254">Update (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="ded9e-254">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="ded9e-255">ローカルクライアントストアで更新する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-255">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-256">Items</span><span class="sxs-lookup"><span data-stu-id="ded9e-256">Items</span></span>](items.md) <br/> |<span data-ttu-id="ded9e-257">項目の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-257">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-258">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="ded9e-258">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="ded9e-259">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-259">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="ded9e-260">SetItemField</span><span class="sxs-lookup"><span data-stu-id="ded9e-260">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="ded9e-261">[Updateitem 操作](updateitem-operation.md)のアイテムの1つのプロパティに対する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-261">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ded9e-262">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="ded9e-262">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="ded9e-263">別の Exchange アイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="ded9e-263">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ded9e-264">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ded9e-264">Text value</span></span>

<span data-ttu-id="ded9e-265">なし。</span><span class="sxs-lookup"><span data-stu-id="ded9e-265">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ded9e-266">注釈</span><span class="sxs-lookup"><span data-stu-id="ded9e-266">Remarks</span></span>

<span data-ttu-id="ded9e-267">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ded9e-267">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ded9e-268">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ded9e-268">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ded9e-269">Namespace</span><span class="sxs-lookup"><span data-stu-id="ded9e-269">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ded9e-270">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ded9e-270">Schema Name</span></span>  <br/> |<span data-ttu-id="ded9e-271">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ded9e-271">Types schema</span></span>  <br/> |
|<span data-ttu-id="ded9e-272">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ded9e-272">Validation File</span></span>  <br/> |<span data-ttu-id="ded9e-273">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ded9e-273">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ded9e-274">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ded9e-274">Can be Empty</span></span>  <br/> |<span data-ttu-id="ded9e-275">正しくない</span><span class="sxs-lookup"><span data-stu-id="ded9e-275">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ded9e-276">関連項目</span><span class="sxs-lookup"><span data-stu-id="ded9e-276">See also</span></span>



- [<span data-ttu-id="ded9e-277">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ded9e-277">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


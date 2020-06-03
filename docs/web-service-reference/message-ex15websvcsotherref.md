---
title: メッセージ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Message
api_type:
- schema
ms.assetid: 2400b33c-43b2-4fc2-b6fb-275a99e0e810
description: Message 要素は、Microsoft Exchange の電子メールメッセージを表します。
ms.openlocfilehash: 510e97572e54f0ea0cb65fc7c75910e69cc0651f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467782"
---
# <a name="message"></a><span data-ttu-id="376d7-103">メッセージ</span><span class="sxs-lookup"><span data-stu-id="376d7-103">Message</span></span>

<span data-ttu-id="376d7-104">**Message**要素は、Microsoft Exchange の電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-104">The **Message** element represents a Microsoft Exchange e-mail message.</span></span> 
  
```xml
<Message>
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
   <EffectiveRights/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
   <ReminderMessageData/>
</Message>
```

 <span data-ttu-id="376d7-105">**MessageType**</span><span class="sxs-lookup"><span data-stu-id="376d7-105">**MessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="376d7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="376d7-106">Attributes and elements</span></span>

<span data-ttu-id="376d7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="376d7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="376d7-108">属性</span><span class="sxs-lookup"><span data-stu-id="376d7-108">Attributes</span></span>

<span data-ttu-id="376d7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="376d7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="376d7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="376d7-110">Child elements</span></span>

|<span data-ttu-id="376d7-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="376d7-111">**Element**</span></span>|<span data-ttu-id="376d7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="376d7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="376d7-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="376d7-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="376d7-114">Base64Binary 形式で表されるオブジェクトのネイティブな汎用インターネットメール内線 (MIME) ストリームが保存されています。</span><span class="sxs-lookup"><span data-stu-id="376d7-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="376d7-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="376d7-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="376d7-116">Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="376d7-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="376d7-117">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="376d7-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="376d7-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="376d7-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="376d7-119">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="376d7-120">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="376d7-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="376d7-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="376d7-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="376d7-122">アイテムのメッセージクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="376d7-123">件名</span><span class="sxs-lookup"><span data-stu-id="376d7-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="376d7-124">Exchange ストアアイテムおよび応答オブジェクトの件名を表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="376d7-125">件名は255文字に制限されます。</span><span class="sxs-lookup"><span data-stu-id="376d7-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="376d7-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="376d7-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="376d7-127">アイテムの秘密度レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="376d7-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="376d7-128">Body</span><span class="sxs-lookup"><span data-stu-id="376d7-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="376d7-129">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="376d7-130">Attachments</span><span class="sxs-lookup"><span data-stu-id="376d7-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="376d7-131">Exchange ストア内のアイテムに添付されているアイテムまたはファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="376d7-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="376d7-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="376d7-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="376d7-133">メールボックス内のアイテムが受信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="376d7-134">Size</span><span class="sxs-lookup"><span data-stu-id="376d7-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="376d7-135">アイテムのサイズ (バイト単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="376d7-136">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="376d7-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="376d7-137">Categories</span><span class="sxs-lookup"><span data-stu-id="376d7-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="376d7-138">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="376d7-139">Importance</span><span class="sxs-lookup"><span data-stu-id="376d7-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="376d7-140">アイテムの重要度について説明します。</span><span class="sxs-lookup"><span data-stu-id="376d7-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="376d7-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="376d7-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="376d7-142">このアイテムが返信であるアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="376d7-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="376d7-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="376d7-144">アイテムが送信トレイの既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="376d7-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="376d7-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="376d7-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="376d7-146">アイテムがまだ送信されていないかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="376d7-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="376d7-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="376d7-148">ユーザーが自分にアイテムを送信したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="376d7-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="376d7-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="376d7-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="376d7-150">アイテムが以前に送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="376d7-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="376d7-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="376d7-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="376d7-152">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="376d7-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="376d7-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="376d7-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="376d7-154">メールボックス内のアイテム内に含まれるすべてのインターネットメッセージヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="376d7-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="376d7-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="376d7-156">メールボックス内のアイテムが送信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="376d7-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="376d7-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="376d7-158">メールボックス内の特定のアイテムが作成された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="376d7-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="376d7-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="376d7-160">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="376d7-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="376d7-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="376d7-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="376d7-162">イベントが発生した日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="376d7-163">これは、アラームがいつ表示されるかを決定するために[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="376d7-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="376d7-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="376d7-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="376d7-165">Exchange ストア内のアイテムにアラームが設定されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="376d7-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="376d7-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="376d7-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="376d7-167">アラームが表示されるイベントの前の時間 (分単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="376d7-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="376d7-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="376d7-169">[CC] 行の内容として使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-169">Represents the display string that is used for the contents of the CC line.</span></span> <span data-ttu-id="376d7-170">これは、すべての CC 受信者表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="376d7-170">This is the concatenated string of all CC recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="376d7-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="376d7-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="376d7-172">[宛先] ボックスの内容に対して使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="376d7-173">これは、すべての受信者の表示名の連結文字列です。</span><span class="sxs-lookup"><span data-stu-id="376d7-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="376d7-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="376d7-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="376d7-175">アイテムに少なくとも1つの添付ファイルがある場合に**true**に設定されるプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="376d7-176">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="376d7-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="376d7-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="376d7-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="376d7-178">フォルダーとアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="376d7-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="376d7-179">Culture</span><span class="sxs-lookup"><span data-stu-id="376d7-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="376d7-180">メールボックス内の特定のアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="376d7-181">Sender</span><span class="sxs-lookup"><span data-stu-id="376d7-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="376d7-182">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="376d7-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="376d7-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="376d7-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="376d7-184">メッセージの受信者のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="376d7-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="376d7-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="376d7-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="376d7-186">メッセージのコピーを受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="376d7-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="376d7-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="376d7-188">電子メールメッセージのブラインドカーボンコピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="376d7-189">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="376d7-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="376d7-190">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="376d7-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="376d7-191">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="376d7-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="376d7-192">アイテムの送信者が配信確認を要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="376d7-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="376d7-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="376d7-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="376d7-194">このメッセージが属しているスレッドを表すバイナリ ID を含みます。</span><span class="sxs-lookup"><span data-stu-id="376d7-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="376d7-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="376d7-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="376d7-196">会話識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="376d7-197">From</span><span class="sxs-lookup"><span data-stu-id="376d7-197">From</span></span>](from.md) <br/> |<span data-ttu-id="376d7-198">メッセージが送信された相手のアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="376d7-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="376d7-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="376d7-200">アイテムのインターネットメッセージ識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="376d7-201">IsRead</span><span class="sxs-lookup"><span data-stu-id="376d7-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="376d7-202">メッセージが開封されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="376d7-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="376d7-203">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="376d7-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="376d7-204">電子メールメッセージに対する応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="376d7-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="376d7-205">References</span><span class="sxs-lookup"><span data-stu-id="376d7-205">References</span></span>](references.md) <br/> |<span data-ttu-id="376d7-206">返信と元のメッセージを相互に関連付けるために使用される Usenet ヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="376d7-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="376d7-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="376d7-208">返信を送信する宛先のアドレスのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="376d7-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="376d7-209">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="376d7-209">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="376d7-210">アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="376d7-210">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="376d7-211">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="376d7-211">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="376d7-212">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="376d7-212">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="376d7-213">代理人アクセスシナリオの代理人を識別します。</span><span class="sxs-lookup"><span data-stu-id="376d7-213">Identifies the delegate in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="376d7-214">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="376d7-214">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="376d7-215">代理人アクセスシナリオのプリンシパルを識別します。</span><span class="sxs-lookup"><span data-stu-id="376d7-215">Identifies the principal in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="376d7-216">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="376d7-216">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="376d7-217">アイテムを最後に変更したユーザーの表示名を含みます。</span><span class="sxs-lookup"><span data-stu-id="376d7-217">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="376d7-218">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="376d7-218">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="376d7-219">アイテムが最後に変更された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="376d7-219">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="376d7-220">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="376d7-220">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="376d7-221">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="376d7-221">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="376d7-222">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="376d7-222">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="376d7-223">Outlook Web app のアイテムを読み取るために Microsoft Office Outlook Web App エンドポイントに連結する URL を表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-223">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="376d7-224">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="376d7-224">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="376d7-225">Outlook web app エンドポイントに連結して Outlook Web App のアイテムを編集するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-225">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="376d7-226">ConversationId</span><span class="sxs-lookup"><span data-stu-id="376d7-226">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="376d7-227">アイテムまたは会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="376d7-227">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="376d7-228">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="376d7-228">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="376d7-229">この会話の一意の本文を表す HTML フラグメントまたはプレーンテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-229">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="376d7-230">ReminderMessageData</span><span class="sxs-lookup"><span data-stu-id="376d7-230">ReminderMessageData</span></span>](remindermessagedata.md) <br/> |<span data-ttu-id="376d7-231">事前通知メッセージのデータが保存されています。</span><span class="sxs-lookup"><span data-stu-id="376d7-231">Contains the data for a reminder message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="376d7-232">親要素</span><span class="sxs-lookup"><span data-stu-id="376d7-232">Parent elements</span></span>

|<span data-ttu-id="376d7-233">**要素**</span><span class="sxs-lookup"><span data-stu-id="376d7-233">**Element**</span></span>|<span data-ttu-id="376d7-234">**説明**</span><span class="sxs-lookup"><span data-stu-id="376d7-234">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="376d7-235">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="376d7-235">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="376d7-236">会議の時刻に隣接しているすべての予定表アイテムを説明します。</span><span class="sxs-lookup"><span data-stu-id="376d7-236">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="376d7-237">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="376d7-237">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="376d7-238">[Updateitem 操作](updateitem-operation.md)中に、アイテムの1つのプロパティに追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="376d7-238">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="376d7-239">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="376d7-239">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="376d7-240">会議の時間と競合するすべてのアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="376d7-240">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="376d7-241">Create (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="376d7-241">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="376d7-242">ローカルクライアントストアに作成する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="376d7-242">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="376d7-243">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="376d7-243">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="376d7-244">別の Exchange アイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-244">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="376d7-245">Items</span><span class="sxs-lookup"><span data-stu-id="376d7-245">Items</span></span>](items.md) <br/> |<span data-ttu-id="376d7-246">項目の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="376d7-246">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="376d7-247">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="376d7-247">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="376d7-248">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="376d7-248">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="376d7-249">SetItemField</span><span class="sxs-lookup"><span data-stu-id="376d7-249">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="376d7-250">[Updateitem 操作](updateitem-operation.md)のアイテムの1つのプロパティに対する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-250">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="376d7-251">Update (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="376d7-251">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="376d7-252">ローカルクライアントストアで更新する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="376d7-252">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="376d7-253">テキスト値</span><span class="sxs-lookup"><span data-stu-id="376d7-253">Text value</span></span>

<span data-ttu-id="376d7-254">なし。</span><span class="sxs-lookup"><span data-stu-id="376d7-254">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="376d7-255">注釈</span><span class="sxs-lookup"><span data-stu-id="376d7-255">Remarks</span></span>

<span data-ttu-id="376d7-256">別の**message**要素[message (availability)](message-availability.md)は、空き時間情報の操作が OOF メッセージを返すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="376d7-256">Another **Message** element, [Message (Availability)](message-availability.md) is used by the Availability operations to return OOF messages.</span></span> 
  
<span data-ttu-id="376d7-257">[Message](message-ex15websvcsotherref.md)要素は、電子メールメッセージ、および Exchange Web サービス (EWS) スキーマで厳密に型指定されていないその他すべてのアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="376d7-257">[Message](message-ex15websvcsotherref.md) elements represent e-mail messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="376d7-258">IPM などのアイテム。共有と IPM. InfoPath は、**メッセージ**要素として返されます。</span><span class="sxs-lookup"><span data-stu-id="376d7-258">Items such as IPM.Sharing and IPM.InfoPath are returned as **Message** elements.</span></span> <span data-ttu-id="376d7-259">Exchange 2010 は、応答で基本**Item**要素を返しません。</span><span class="sxs-lookup"><span data-stu-id="376d7-259">Exchange 2010 does not return the base **Item** element in responses.</span></span> 
  
<span data-ttu-id="376d7-260">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="376d7-260">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="376d7-261">要素の情報</span><span class="sxs-lookup"><span data-stu-id="376d7-261">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="376d7-262">Namespace</span><span class="sxs-lookup"><span data-stu-id="376d7-262">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="376d7-263">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="376d7-263">Schema Name</span></span>  <br/> |<span data-ttu-id="376d7-264">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="376d7-264">Types schema</span></span>  <br/> |
|<span data-ttu-id="376d7-265">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="376d7-265">Validation File</span></span>  <br/> |<span data-ttu-id="376d7-266">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="376d7-266">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="376d7-267">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="376d7-267">Can be Empty</span></span>  <br/> |<span data-ttu-id="376d7-268">正しくない</span><span class="sxs-lookup"><span data-stu-id="376d7-268">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="376d7-269">関連項目</span><span class="sxs-lookup"><span data-stu-id="376d7-269">See also</span></span>



- [<span data-ttu-id="376d7-270">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="376d7-270">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


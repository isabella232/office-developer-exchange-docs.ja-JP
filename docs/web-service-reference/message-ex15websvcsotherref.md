---
title: Message
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
description: メッセージ要素は、Microsoft Exchange の電子メール メッセージを表します。
ms.openlocfilehash: 388b944cfa16899cb2376320882f5087396d7b82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832474"
---
# <a name="message"></a><span data-ttu-id="24792-103">Message</span><span class="sxs-lookup"><span data-stu-id="24792-103">Message</span></span>

<span data-ttu-id="24792-104">**メッセージ**要素は、Microsoft Exchange の電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="24792-104">The **Message** element represents a Microsoft Exchange e-mail message.</span></span> 
  
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

 <span data-ttu-id="24792-105">**メッセージの種類**</span><span class="sxs-lookup"><span data-stu-id="24792-105">**MessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="24792-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="24792-106">Attributes and elements</span></span>

<span data-ttu-id="24792-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="24792-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24792-108">属性</span><span class="sxs-lookup"><span data-stu-id="24792-108">Attributes</span></span>

<span data-ttu-id="24792-109">なし。</span><span class="sxs-lookup"><span data-stu-id="24792-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="24792-110">子要素</span><span class="sxs-lookup"><span data-stu-id="24792-110">Child elements</span></span>

|<span data-ttu-id="24792-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="24792-111">**Element**</span></span>|<span data-ttu-id="24792-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="24792-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24792-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="24792-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="24792-114">Base64Binary の形式で表されるオブジェクトのネイティブの多目的インターネット メール拡張 (MIME) ストリームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="24792-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="24792-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="24792-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="24792-116">Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="24792-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="24792-117">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="24792-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="24792-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="24792-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="24792-119">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="24792-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="24792-120">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="24792-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="24792-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="24792-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="24792-122">アイテムのメッセージ クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="24792-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="24792-123">Subject</span><span class="sxs-lookup"><span data-stu-id="24792-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="24792-124">Exchange ストアのアイテムおよび応答オブジェクトのサブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="24792-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="24792-125">件名は、255 文字までに制限されています。</span><span class="sxs-lookup"><span data-stu-id="24792-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="24792-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="24792-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="24792-127">アイテムの秘密度レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="24792-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="24792-128">Body/本文</span><span class="sxs-lookup"><span data-stu-id="24792-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="24792-129">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="24792-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="24792-130">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="24792-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="24792-131">アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="24792-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="24792-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="24792-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="24792-133">メールボックス内のアイテムを受信したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="24792-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="24792-134">Size</span><span class="sxs-lookup"><span data-stu-id="24792-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="24792-135">アイテムのバイト単位のサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="24792-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="24792-136">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="24792-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="24792-137">Categories</span><span class="sxs-lookup"><span data-stu-id="24792-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="24792-138">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="24792-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="24792-139">Importance</span><span class="sxs-lookup"><span data-stu-id="24792-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="24792-140">アイテムの重要性をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="24792-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="24792-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="24792-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="24792-142">このアイテムの返信するアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="24792-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="24792-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="24792-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="24792-144">アイテムが [送信トレイ] 既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24792-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="24792-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="24792-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="24792-146">アイテムはまだ送信されていないかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="24792-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="24792-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="24792-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="24792-148">ユーザーが彼または彼女自身にアイテムを送信するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24792-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="24792-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="24792-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="24792-150">アイテムが以前送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24792-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="24792-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="24792-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="24792-152">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24792-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="24792-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="24792-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="24792-154">メールボックス内のアイテムに含まれているすべてのインターネット メッセージ ヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="24792-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="24792-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="24792-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="24792-156">メールボックス内のアイテムが送信された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="24792-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="24792-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="24792-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="24792-158">メールボックス内の特定のアイテムが作成された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="24792-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="24792-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="24792-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="24792-160">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="24792-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="24792-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="24792-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="24792-162">イベントが発生したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="24792-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="24792-163">[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によってアラームが表示されたときを決定する使用されます。</span><span class="sxs-lookup"><span data-stu-id="24792-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="24792-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="24792-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="24792-165">Exchange ストアのアイテムのアラームが設定されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24792-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="24792-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="24792-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="24792-167">分前にアラームが表示されるときに、イベントの数を表します。</span><span class="sxs-lookup"><span data-stu-id="24792-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="24792-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="24792-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="24792-169">[Cc] 行の内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="24792-169">Represents the display string that is used for the contents of the CC line.</span></span> <span data-ttu-id="24792-170">これは、すべての CC 受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="24792-170">This is the concatenated string of all CC recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="24792-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="24792-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="24792-172">ボックスの内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="24792-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="24792-173">これは、すべての受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="24792-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="24792-174">添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="24792-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="24792-175">アイテムに表示されている 1 つ以上の添付ファイルがある場合に**true**に設定されているプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="24792-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="24792-176">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="24792-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="24792-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="24792-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="24792-178">フォルダーおよびアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="24792-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="24792-179">カルチャ</span><span class="sxs-lookup"><span data-stu-id="24792-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="24792-180">メールボックス内の指定したアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="24792-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="24792-181">送信者</span><span class="sxs-lookup"><span data-stu-id="24792-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="24792-182">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="24792-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="24792-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="24792-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="24792-184">一連メッセージの受信者にはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="24792-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="24792-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="24792-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="24792-186">メッセージのコピーを受け取る受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="24792-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="24792-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="24792-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="24792-188">電子メール メッセージのブラインド カーボン コピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="24792-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="24792-189">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="24792-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="24792-190">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24792-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="24792-191">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="24792-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="24792-192">アイテムの送信者が配信済みメッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24792-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="24792-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="24792-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="24792-194">このメッセージが属するスレッドを表すバイナリの ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="24792-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="24792-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="24792-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="24792-196">会話 id を表します。</span><span class="sxs-lookup"><span data-stu-id="24792-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="24792-197">From</span><span class="sxs-lookup"><span data-stu-id="24792-197">From</span></span>](from.md) <br/> |<span data-ttu-id="24792-198">メッセージの送信元アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="24792-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="24792-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="24792-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="24792-200">アイテムのインターネット メッセージ id を表します。</span><span class="sxs-lookup"><span data-stu-id="24792-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="24792-201">IsRead</span><span class="sxs-lookup"><span data-stu-id="24792-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="24792-202">メッセージが読み取られたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24792-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="24792-203">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="24792-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="24792-204">電子メール メッセージへの応答が要求されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24792-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="24792-205">参照資料</span><span class="sxs-lookup"><span data-stu-id="24792-205">References</span></span>](references.md) <br/> |<span data-ttu-id="24792-206">元のメッセージに応答を関連付けるために使用する Usenet ヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="24792-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="24792-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="24792-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="24792-208">応答を送信するアドレスのセットを識別します。</span><span class="sxs-lookup"><span data-stu-id="24792-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="24792-209">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="24792-209">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="24792-210">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="24792-210">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="24792-211">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="24792-211">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="24792-212">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="24792-212">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="24792-213">代理人アクセス シナリオでは、デリゲートを識別します。</span><span class="sxs-lookup"><span data-stu-id="24792-213">Identifies the delegate in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="24792-214">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="24792-214">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="24792-215">代理人アクセスのシナリオでプリンシパルを識別します。</span><span class="sxs-lookup"><span data-stu-id="24792-215">Identifies the principal in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="24792-216">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="24792-216">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="24792-217">最後の項目を変更するのにはユーザーの表示名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="24792-217">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="24792-218">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="24792-218">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="24792-219">アイテムが最後に修正された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="24792-219">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="24792-220">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="24792-220">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="24792-221">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24792-221">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="24792-222">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="24792-222">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="24792-223">Outlook Web App 内の項目を参照するのには Microsoft Office Outlook の Web アプリケーションのエンドポイントを結合するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="24792-223">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="24792-224">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="24792-224">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="24792-225">Outlook Web App 内の項目を編集するのには Outlook Web App エンドポイントへの連結に URL を表します。</span><span class="sxs-lookup"><span data-stu-id="24792-225">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="24792-226">ConversationId</span><span class="sxs-lookup"><span data-stu-id="24792-226">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="24792-227">アイテムや会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="24792-227">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="24792-228">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="24792-228">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="24792-229">このスレッドの一意の本文を表すテキストまたは HTML フラグメントを表します。</span><span class="sxs-lookup"><span data-stu-id="24792-229">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="24792-230">ReminderMessageData</span><span class="sxs-lookup"><span data-stu-id="24792-230">ReminderMessageData</span></span>](remindermessagedata.md) <br/> |<span data-ttu-id="24792-231">アラーム メッセージのデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="24792-231">Contains the data for a reminder message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="24792-232">親要素</span><span class="sxs-lookup"><span data-stu-id="24792-232">Parent elements</span></span>

|<span data-ttu-id="24792-233">**要素**</span><span class="sxs-lookup"><span data-stu-id="24792-233">**Element**</span></span>|<span data-ttu-id="24792-234">**説明**</span><span class="sxs-lookup"><span data-stu-id="24792-234">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24792-235">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="24792-235">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="24792-236">会議の時刻に隣接しているすべての予定表のアイテムについて説明します。</span><span class="sxs-lookup"><span data-stu-id="24792-236">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="24792-237">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="24792-237">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="24792-238">[UpdateItem 操作](updateitem-operation.md)中に 1 つのアイテムのプロパティを追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="24792-238">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="24792-239">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="24792-239">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="24792-240">会議の時間と競合するすべての項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="24792-240">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="24792-241">(ItemSync) を作成します。</span><span class="sxs-lookup"><span data-stu-id="24792-241">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="24792-242">ローカル クライアント ストアに作成する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="24792-242">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="24792-243">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="24792-243">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="24792-244">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="24792-244">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="24792-245">Items</span><span class="sxs-lookup"><span data-stu-id="24792-245">Items</span></span>](items.md) <br/> |<span data-ttu-id="24792-246">項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="24792-246">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="24792-247">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="24792-247">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="24792-248">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で識別されるフォルダーを作成する項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="24792-248">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="24792-249">SetItemField</span><span class="sxs-lookup"><span data-stu-id="24792-249">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="24792-250">[UpdateItem 操作](updateitem-operation.md)内の項目の 1 つのプロパティには、更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="24792-250">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="24792-251">更新プログラム (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="24792-251">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="24792-252">ローカル クライアント ストアで更新する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="24792-252">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="24792-253">テキスト値</span><span class="sxs-lookup"><span data-stu-id="24792-253">Text value</span></span>

<span data-ttu-id="24792-254">なし。</span><span class="sxs-lookup"><span data-stu-id="24792-254">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="24792-255">備考</span><span class="sxs-lookup"><span data-stu-id="24792-255">Remarks</span></span>

<span data-ttu-id="24792-256">[メッセージ (可用性)](message-availability.md) 、別の**メッセージ**要素は、不在時のメッセージを返すため、可用性の操作によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="24792-256">Another **Message** element, [Message (Availability)](message-availability.md) is used by the Availability operations to return OOF messages.</span></span> 
  
<span data-ttu-id="24792-257">[メッセージ](message-ex15websvcsotherref.md)要素は、電子メール メッセージ、Exchange Web サービス (EWS) スキーマが厳密に型指定されない他のすべての項目を表します。</span><span class="sxs-lookup"><span data-stu-id="24792-257">[Message](message-ex15websvcsotherref.md) elements represent e-mail messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="24792-258">IPM などの項目です。共有し、IPM.InfoPath は、**メッセージ**の要素として返されます。</span><span class="sxs-lookup"><span data-stu-id="24792-258">Items such as IPM.Sharing and IPM.InfoPath are returned as **Message** elements.</span></span> <span data-ttu-id="24792-259">Exchange 2010 では、応答の基本要素の**項目**が返されません。</span><span class="sxs-lookup"><span data-stu-id="24792-259">Exchange 2010 does not return the base **Item** element in responses.</span></span> 
  
<span data-ttu-id="24792-260">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="24792-260">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24792-261">要素情報</span><span class="sxs-lookup"><span data-stu-id="24792-261">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24792-262">名前空間</span><span class="sxs-lookup"><span data-stu-id="24792-262">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="24792-263">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="24792-263">Schema Name</span></span>  <br/> |<span data-ttu-id="24792-264">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="24792-264">Types schema</span></span>  <br/> |
|<span data-ttu-id="24792-265">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="24792-265">Validation File</span></span>  <br/> |<span data-ttu-id="24792-266">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="24792-266">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="24792-267">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="24792-267">Can be Empty</span></span>  <br/> |<span data-ttu-id="24792-268">False</span><span class="sxs-lookup"><span data-stu-id="24792-268">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="24792-269">関連項目</span><span class="sxs-lookup"><span data-stu-id="24792-269">See also</span></span>



- [<span data-ttu-id="24792-270">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="24792-270">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


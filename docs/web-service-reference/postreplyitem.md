---
title: PostReplyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PostReplyItem
api_type:
- schema
ms.assetid: e5d93d63-0a3b-470f-9a94-2d57284c6745
description: PostReplyItem 要素は、投稿アイテムへの返信を含みます。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 4104e79449acc6e358b729cf2de769d28dac52bd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461682"
---
# <a name="postreplyitem"></a><span data-ttu-id="6fabb-104">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="6fabb-104">PostReplyItem</span></span>

<span data-ttu-id="6fabb-105">**PostReplyItem**要素は、投稿アイテムへの返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="6fabb-105">The **PostReplyItem** element contains a reply to a post item.</span></span> <span data-ttu-id="6fabb-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6fabb-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PostReplyItem>
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
   <NewBodyContent/>
</PostReplyItem>
```

 <span data-ttu-id="6fabb-107">**PostReplyItemType**</span><span class="sxs-lookup"><span data-stu-id="6fabb-107">**PostReplyItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6fabb-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6fabb-108">Attributes and elements</span></span>

<span data-ttu-id="6fabb-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6fabb-110">属性</span><span class="sxs-lookup"><span data-stu-id="6fabb-110">Attributes</span></span>

<span data-ttu-id="6fabb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6fabb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6fabb-112">子要素</span><span class="sxs-lookup"><span data-stu-id="6fabb-112">Child elements</span></span>

|<span data-ttu-id="6fabb-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="6fabb-113">**Element**</span></span>|<span data-ttu-id="6fabb-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6fabb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6fabb-115">MimeContent</span><span class="sxs-lookup"><span data-stu-id="6fabb-115">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="6fabb-116">Base64Binary 形式で表されるオブジェクトのネイティブな汎用インターネットメール内線 (MIME) ストリームが保存されています。</span><span class="sxs-lookup"><span data-stu-id="6fabb-116">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="6fabb-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="6fabb-118">Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6fabb-118">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="6fabb-119">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-119">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-120">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="6fabb-120">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="6fabb-121">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-121">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="6fabb-122">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-122">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-123">ItemClass</span><span class="sxs-lookup"><span data-stu-id="6fabb-123">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="6fabb-124">アイテムのメッセージクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-124">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-125">件名</span><span class="sxs-lookup"><span data-stu-id="6fabb-125">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="6fabb-126">Exchange ストアアイテムおよび応答オブジェクトの件名を表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-126">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="6fabb-127">件名は255文字に制限されます。</span><span class="sxs-lookup"><span data-stu-id="6fabb-127">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-128">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="6fabb-128">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="6fabb-129">アイテムの秘密度レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-129">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-130">Body</span><span class="sxs-lookup"><span data-stu-id="6fabb-130">Body</span></span>](body.md) <br/> |<span data-ttu-id="6fabb-131">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-131">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-132">Attachments</span><span class="sxs-lookup"><span data-stu-id="6fabb-132">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6fabb-133">Exchange ストア内のアイテムに添付されているアイテムまたはファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="6fabb-133">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-134">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="6fabb-134">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="6fabb-135">メールボックス内のアイテムが受信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-135">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-136">Size</span><span class="sxs-lookup"><span data-stu-id="6fabb-136">Size</span></span>](size.md) <br/> |<span data-ttu-id="6fabb-137">アイテムのサイズ (バイト単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-137">Represents the size in bytes of an item.</span></span> <span data-ttu-id="6fabb-138">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-138">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-139">Categories</span><span class="sxs-lookup"><span data-stu-id="6fabb-139">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6fabb-140">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-140">Represents a collection of strings that identify categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-141">Importance</span><span class="sxs-lookup"><span data-stu-id="6fabb-141">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="6fabb-142">アイテムの重要度について説明します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-142">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-143">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="6fabb-143">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="6fabb-144">このアイテムが返信であるアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-144">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-145">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="6fabb-145">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="6fabb-146">アイテムが送信トレイの既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-146">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-147">IsDraft</span><span class="sxs-lookup"><span data-stu-id="6fabb-147">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="6fabb-148">アイテムがまだ送信されていないかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-148">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-149">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="6fabb-149">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="6fabb-150">ユーザーが自分にアイテムを送信したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-150">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-151">IsResend</span><span class="sxs-lookup"><span data-stu-id="6fabb-151">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="6fabb-152">アイテムが以前に送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-152">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-153">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="6fabb-153">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="6fabb-154">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-154">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-155">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="6fabb-155">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="6fabb-156">メールボックス内のアイテムに含まれるすべてのインターネットメッセージヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-156">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-157">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="6fabb-157">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="6fabb-158">メールボックス内のアイテムが送信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-158">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-159">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="6fabb-159">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="6fabb-160">メールボックス内の特定のアイテムが作成された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-160">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-161">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="6fabb-161">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="6fabb-162">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-162">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-163">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="6fabb-163">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="6fabb-164">イベントが発生した日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-164">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="6fabb-165">これは、アラームがいつ表示されるかを決定するために[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="6fabb-165">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-166">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="6fabb-166">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="6fabb-167">Exchange ストア内のアイテムにアラームが設定されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-167">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-168">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="6fabb-168">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="6fabb-169">アラームが表示されるイベントの前の時間 (分単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-169">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-170">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="6fabb-170">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="6fabb-171">[Cc] 行の内容として使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-171">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="6fabb-172">これは、すべての Cc 受信者表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="6fabb-172">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-173">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="6fabb-173">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="6fabb-174">[宛先] ボックスの内容に対して使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-174">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="6fabb-175">これは、すべての受信者の表示名の連結文字列です。</span><span class="sxs-lookup"><span data-stu-id="6fabb-175">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-176">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="6fabb-176">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="6fabb-177">アイテムに添付ファイルがある場合に**true**に設定されるプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-177">Represents a property that is set to **true** if an item has an attachment.</span></span> <span data-ttu-id="6fabb-178">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-178">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-179">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="6fabb-179">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="6fabb-180">フォルダーとアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-180">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-181">Culture</span><span class="sxs-lookup"><span data-stu-id="6fabb-181">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="6fabb-182">メールボックス内の特定のアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-182">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-183">Sender</span><span class="sxs-lookup"><span data-stu-id="6fabb-183">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="6fabb-184">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-184">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-185">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="6fabb-185">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="6fabb-186">メッセージの受信者のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6fabb-186">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-187">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="6fabb-187">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="6fabb-188">メッセージのコピーを受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-188">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-189">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="6fabb-189">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="6fabb-190">電子メールのブラインドカーボンコピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-190">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-191">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="6fabb-191">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="6fabb-192">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-192">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-193">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="6fabb-193">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="6fabb-194">アイテムの送信者が配信確認を要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-194">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-195">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="6fabb-195">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="6fabb-196">このメッセージが属しているスレッドを表すバイナリ ID を含みます。</span><span class="sxs-lookup"><span data-stu-id="6fabb-196">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-197">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="6fabb-197">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="6fabb-198">会話識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-198">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-199">From</span><span class="sxs-lookup"><span data-stu-id="6fabb-199">From</span></span>](from.md) <br/> |<span data-ttu-id="6fabb-200">メッセージの送信元のアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-200">Represents the address from which the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-201">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="6fabb-201">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="6fabb-202">アイテムのインターネットメッセージ識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-202">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-203">IsRead</span><span class="sxs-lookup"><span data-stu-id="6fabb-203">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="6fabb-204">メッセージが開封されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-204">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-205">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="6fabb-205">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="6fabb-206">電子メールメッセージに対する応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-206">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-207">References</span><span class="sxs-lookup"><span data-stu-id="6fabb-207">References</span></span>](references.md) <br/> |<span data-ttu-id="6fabb-208">返信を元のメッセージに関連付けるために使用される Usenet ヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-208">Represents the Usenet header that is used to associate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-209">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="6fabb-209">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="6fabb-210">返信を送信する宛先のアドレスのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-210">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-211">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="6fabb-211">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="6fabb-212">アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6fabb-212">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="6fabb-213">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="6fabb-213">This element is read-only.</span></span> <span data-ttu-id="6fabb-214">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6fabb-214">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-215">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="6fabb-215">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="6fabb-216">代理人アクセスシナリオの代理人を識別します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-216">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="6fabb-217">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6fabb-217">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-218">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="6fabb-218">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="6fabb-219">代理人アクセスシナリオのプリンシパルを識別します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-219">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="6fabb-220">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6fabb-220">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-221">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="6fabb-221">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="6fabb-222">投稿アイテムの新しい本文のコンテンツを表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-222">Represents the new body content of a post item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6fabb-223">親要素</span><span class="sxs-lookup"><span data-stu-id="6fabb-223">Parent elements</span></span>

|<span data-ttu-id="6fabb-224">**要素**</span><span class="sxs-lookup"><span data-stu-id="6fabb-224">**Element**</span></span>|<span data-ttu-id="6fabb-225">**説明**</span><span class="sxs-lookup"><span data-stu-id="6fabb-225">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6fabb-226">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="6fabb-226">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="6fabb-227">会議の時刻に隣接しているすべてのアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-227">Describes all items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-228">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="6fabb-228">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="6fabb-229">会議の時間と競合するすべてのアイテムについて説明します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-229">Describes all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-230">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="6fabb-230">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="6fabb-231">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="6fabb-231">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6fabb-232">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="6fabb-232">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="6fabb-233">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6fabb-233">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6fabb-234">注釈</span><span class="sxs-lookup"><span data-stu-id="6fabb-234">Remarks</span></span>

<span data-ttu-id="6fabb-235">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="6fabb-235">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6fabb-236">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6fabb-236">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6fabb-237">Namespace</span><span class="sxs-lookup"><span data-stu-id="6fabb-237">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6fabb-238">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6fabb-238">Schema Name</span></span>  <br/> |<span data-ttu-id="6fabb-239">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6fabb-239">Types schema</span></span>  <br/> |
|<span data-ttu-id="6fabb-240">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6fabb-240">Validation File</span></span>  <br/> |<span data-ttu-id="6fabb-241">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6fabb-241">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6fabb-242">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6fabb-242">Can be Empty</span></span>  <br/> |<span data-ttu-id="6fabb-243">正しくない</span><span class="sxs-lookup"><span data-stu-id="6fabb-243">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6fabb-244">関連項目</span><span class="sxs-lookup"><span data-stu-id="6fabb-244">See also</span></span>



- [<span data-ttu-id="6fabb-245">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6fabb-245">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


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
description: PostReplyItem 要素には、投稿するアイテムへの返信が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 70a0d6a7c670d0f16a55e66e7ef329331a04a5f8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832868"
---
# <a name="postreplyitem"></a><span data-ttu-id="e9775-104">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="e9775-104">PostReplyItem</span></span>

<span data-ttu-id="e9775-105">**PostReplyItem**要素には、投稿するアイテムへの返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9775-105">The **PostReplyItem** element contains a reply to a post item.</span></span> <span data-ttu-id="e9775-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e9775-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
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

 <span data-ttu-id="e9775-107">**PostReplyItemType**</span><span class="sxs-lookup"><span data-stu-id="e9775-107">**PostReplyItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9775-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e9775-108">Attributes and elements</span></span>

<span data-ttu-id="e9775-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e9775-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9775-110">属性</span><span class="sxs-lookup"><span data-stu-id="e9775-110">Attributes</span></span>

<span data-ttu-id="e9775-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e9775-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9775-112">子要素</span><span class="sxs-lookup"><span data-stu-id="e9775-112">Child elements</span></span>

|<span data-ttu-id="e9775-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e9775-113">**Element**</span></span>|<span data-ttu-id="e9775-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9775-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9775-115">MimeContent</span><span class="sxs-lookup"><span data-stu-id="e9775-115">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="e9775-116">Base64Binary の形式で表されるオブジェクトのネイティブの多目的インターネット メール拡張 (MIME) ストリームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9775-116">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="e9775-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="e9775-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="e9775-118">Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9775-118">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="e9775-119">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e9775-119">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="e9775-120">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="e9775-120">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="e9775-121">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-121">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="e9775-122">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e9775-122">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="e9775-123">ItemClass</span><span class="sxs-lookup"><span data-stu-id="e9775-123">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="e9775-124">アイテムのメッセージ クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-124">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="e9775-125">Subject</span><span class="sxs-lookup"><span data-stu-id="e9775-125">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="e9775-126">Exchange ストアのアイテムおよび応答オブジェクトのサブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-126">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="e9775-127">件名は、255 文字までに制限されています。</span><span class="sxs-lookup"><span data-stu-id="e9775-127">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="e9775-128">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="e9775-128">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="e9775-129">アイテムの秘密度レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="e9775-129">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="e9775-130">Body/本文</span><span class="sxs-lookup"><span data-stu-id="e9775-130">Body</span></span>](body.md) <br/> |<span data-ttu-id="e9775-131">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-131">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="e9775-132">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="e9775-132">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e9775-133">アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9775-133">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e9775-134">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="e9775-134">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="e9775-135">メールボックス内のアイテムを受信したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-135">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="e9775-136">Size</span><span class="sxs-lookup"><span data-stu-id="e9775-136">Size</span></span>](size.md) <br/> |<span data-ttu-id="e9775-137">アイテムのバイト単位のサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-137">Represents the size in bytes of an item.</span></span> <span data-ttu-id="e9775-138">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e9775-138">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="e9775-139">Categories</span><span class="sxs-lookup"><span data-stu-id="e9775-139">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e9775-140">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-140">Represents a collection of strings that identify categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="e9775-141">Importance</span><span class="sxs-lookup"><span data-stu-id="e9775-141">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="e9775-142">アイテムの重要性をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="e9775-142">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="e9775-143">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="e9775-143">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="e9775-144">このアイテムの返信するアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-144">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="e9775-145">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="e9775-145">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="e9775-146">アイテムが [送信トレイ] 既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e9775-146">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="e9775-147">IsDraft</span><span class="sxs-lookup"><span data-stu-id="e9775-147">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="e9775-148">アイテムはまだ送信されていないかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-148">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="e9775-149">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="e9775-149">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="e9775-150">ユーザーが彼または彼女自身にアイテムを送信するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e9775-150">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="e9775-151">IsResend</span><span class="sxs-lookup"><span data-stu-id="e9775-151">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="e9775-152">アイテムが以前送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e9775-152">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="e9775-153">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="e9775-153">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="e9775-154">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e9775-154">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="e9775-155">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="e9775-155">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="e9775-156">メールボックス内のアイテムに含まれるすべてのインターネット メッセージ ヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-156">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e9775-157">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="e9775-157">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="e9775-158">メールボックス内のアイテムが送信された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-158">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="e9775-159">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="e9775-159">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="e9775-160">メールボックス内の特定のアイテムが作成された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-160">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="e9775-161">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="e9775-161">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="e9775-162">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9775-162">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e9775-163">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="e9775-163">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="e9775-164">イベントが発生したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-164">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="e9775-165">[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によってアラームが表示されたときを決定する使用されます。</span><span class="sxs-lookup"><span data-stu-id="e9775-165">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="e9775-166">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="e9775-166">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="e9775-167">Exchange ストアのアイテムのアラームが設定されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e9775-167">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e9775-168">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="e9775-168">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="e9775-169">分前にアラームが表示されるときに、イベントの数を表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-169">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="e9775-170">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="e9775-170">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="e9775-171">[Cc] 行の内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-171">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="e9775-172">これは、すべての Cc 受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="e9775-172">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="e9775-173">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="e9775-173">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="e9775-174">ボックスの内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-174">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="e9775-175">これは、すべての受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="e9775-175">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="e9775-176">添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="e9775-176">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="e9775-177">アイテムに添付ファイルがある場合に**true**に設定されているプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-177">Represents a property that is set to **true** if an item has an attachment.</span></span> <span data-ttu-id="e9775-178">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e9775-178">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="e9775-179">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="e9775-179">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="e9775-180">フォルダーおよびアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="e9775-180">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="e9775-181">カルチャ</span><span class="sxs-lookup"><span data-stu-id="e9775-181">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="e9775-182">メールボックス内の指定したアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-182">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e9775-183">送信者</span><span class="sxs-lookup"><span data-stu-id="e9775-183">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="e9775-184">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="e9775-184">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="e9775-185">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="e9775-185">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="e9775-186">一連メッセージの受信者にはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9775-186">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="e9775-187">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="e9775-187">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="e9775-188">メッセージのコピーを受け取る受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-188">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="e9775-189">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="e9775-189">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="e9775-190">電子メールのブラインド カーボン コピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-190">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="e9775-191">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="e9775-191">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="e9775-192">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e9775-192">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="e9775-193">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="e9775-193">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="e9775-194">アイテムの送信者が配信済みメッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e9775-194">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="e9775-195">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="e9775-195">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="e9775-196">このメッセージが属するスレッドを表すバイナリの ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9775-196">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="e9775-197">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="e9775-197">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="e9775-198">会話 id を表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-198">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="e9775-199">From</span><span class="sxs-lookup"><span data-stu-id="e9775-199">From</span></span>](from.md) <br/> |<span data-ttu-id="e9775-200">メッセージの送信元アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-200">Represents the address from which the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="e9775-201">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="e9775-201">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="e9775-202">アイテムのインターネット メッセージ id を表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-202">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="e9775-203">IsRead</span><span class="sxs-lookup"><span data-stu-id="e9775-203">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="e9775-204">メッセージが読み取られたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e9775-204">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="e9775-205">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="e9775-205">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="e9775-206">電子メール メッセージへの応答が要求されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e9775-206">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="e9775-207">参照資料</span><span class="sxs-lookup"><span data-stu-id="e9775-207">References</span></span>](references.md) <br/> |<span data-ttu-id="e9775-208">元のメッセージに応答を関連付けるために使用する Usenet ヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-208">Represents the Usenet header that is used to associate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="e9775-209">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="e9775-209">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="e9775-210">応答を送信するアドレスのセットを識別します。</span><span class="sxs-lookup"><span data-stu-id="e9775-210">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="e9775-211">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="e9775-211">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="e9775-212">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9775-212">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="e9775-213">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e9775-213">This element is read-only.</span></span> <span data-ttu-id="e9775-214">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e9775-214">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="e9775-215">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="e9775-215">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="e9775-216">代理人アクセス シナリオでは、デリゲートを識別します。</span><span class="sxs-lookup"><span data-stu-id="e9775-216">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="e9775-217">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e9775-217">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="e9775-218">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="e9775-218">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="e9775-219">代理人アクセスのシナリオでプリンシパルを識別します。</span><span class="sxs-lookup"><span data-stu-id="e9775-219">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="e9775-220">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e9775-220">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="e9775-221">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="e9775-221">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="e9775-222">新しい投稿アイテムの本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="e9775-222">Represents the new body content of a post item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e9775-223">親要素</span><span class="sxs-lookup"><span data-stu-id="e9775-223">Parent elements</span></span>

|<span data-ttu-id="e9775-224">**要素**</span><span class="sxs-lookup"><span data-stu-id="e9775-224">**Element**</span></span>|<span data-ttu-id="e9775-225">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9775-225">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9775-226">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="e9775-226">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="e9775-227">会議の時刻に隣接しているすべての項目について説明します。</span><span class="sxs-lookup"><span data-stu-id="e9775-227">Describes all items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="e9775-228">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="e9775-228">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="e9775-229">会議の時間と競合するすべての項目について説明します。</span><span class="sxs-lookup"><span data-stu-id="e9775-229">Describes all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="e9775-230">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="e9775-230">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="e9775-231">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9775-231">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e9775-232">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="e9775-232">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="e9775-233">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で識別されるフォルダーを作成する項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9775-233">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e9775-234">備考</span><span class="sxs-lookup"><span data-stu-id="e9775-234">Remarks</span></span>

<span data-ttu-id="e9775-235">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e9775-235">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9775-236">要素情報</span><span class="sxs-lookup"><span data-stu-id="e9775-236">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9775-237">名前空間</span><span class="sxs-lookup"><span data-stu-id="e9775-237">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9775-238">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e9775-238">Schema Name</span></span>  <br/> |<span data-ttu-id="e9775-239">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e9775-239">Types schema</span></span>  <br/> |
|<span data-ttu-id="e9775-240">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e9775-240">Validation File</span></span>  <br/> |<span data-ttu-id="e9775-241">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e9775-241">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9775-242">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e9775-242">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9775-243">False</span><span class="sxs-lookup"><span data-stu-id="e9775-243">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9775-244">関連項目</span><span class="sxs-lookup"><span data-stu-id="e9775-244">See also</span></span>



- [<span data-ttu-id="e9775-245">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e9775-245">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


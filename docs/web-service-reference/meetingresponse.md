---
title: MeetingResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingResponse
api_type:
- schema
ms.assetid: 9f798e79-dafd-4d4d-9967-95fd8e5c0502
description: 会議の応答要素は、Exchange ストア内の会議の応答を表します。
ms.openlocfilehash: ff999a671c0321586fbc2adae6cbb5c1ad117ebf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467698"
---
# <a name="meetingresponse"></a><span data-ttu-id="5bb71-103">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="5bb71-103">MeetingResponse</span></span>

<span data-ttu-id="5bb71-104">会議の**応答**要素は、Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-104">The **MeetingResponse** element represents a meeting response in the Exchange store.</span></span> 
  
```xml
<MeetingResponse>
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
   <ReceivedBy/>
   <ReceivedRepresenting/>
</MeetingResponse>
```

 <span data-ttu-id="5bb71-105">**MeetingResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="5bb71-105">**MeetingResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5bb71-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5bb71-106">Attributes and elements</span></span>

<span data-ttu-id="5bb71-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5bb71-108">属性</span><span class="sxs-lookup"><span data-stu-id="5bb71-108">Attributes</span></span>

<span data-ttu-id="5bb71-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5bb71-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5bb71-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5bb71-110">Child elements</span></span>

|<span data-ttu-id="5bb71-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="5bb71-111">**Element**</span></span>|<span data-ttu-id="5bb71-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5bb71-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5bb71-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="5bb71-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="5bb71-114">Base64Binary 形式で表されるオブジェクトのネイティブ MIME ストリームが格納されています。</span><span class="sxs-lookup"><span data-stu-id="5bb71-114">Contains the native MIME stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="5bb71-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="5bb71-116">Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5bb71-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="5bb71-117">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="5bb71-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="5bb71-119">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="5bb71-120">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="5bb71-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="5bb71-122">アイテムのメッセージクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-122">Represents the message class of an item.</span></span>  <br/> |
|<span data-ttu-id="5bb71-123">[[件名]](subject.md)</span><span class="sxs-lookup"><span data-stu-id="5bb71-123">[Subject](subject.md)</span></span> <br/> |<span data-ttu-id="5bb71-124">Exchange ストアアイテムおよび応答オブジェクトの件名を表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="5bb71-125">件名は255文字に制限されます。</span><span class="sxs-lookup"><span data-stu-id="5bb71-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="5bb71-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="5bb71-127">アイテムの秘密度レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-128">Body</span><span class="sxs-lookup"><span data-stu-id="5bb71-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="5bb71-129">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-130">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="5bb71-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5bb71-131">Exchange ストア内のアイテムに添付されているアイテムまたはファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="5bb71-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="5bb71-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="5bb71-133">メールボックス内のアイテムが受信されたデータと時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-133">Represents the data and time that an item in a mailbox was received.</span></span>  <br/> |
|<span data-ttu-id="5bb71-134">[[サイズ]](size.md)</span><span class="sxs-lookup"><span data-stu-id="5bb71-134">[Size](size.md)</span></span> <br/> |<span data-ttu-id="5bb71-135">アイテムのサイズ (バイト単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="5bb71-136">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-137">カテゴリ</span><span class="sxs-lookup"><span data-stu-id="5bb71-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5bb71-138">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-139">Importance</span><span class="sxs-lookup"><span data-stu-id="5bb71-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="5bb71-140">アイテムの重要度について説明します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="5bb71-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="5bb71-142">このアイテムが返信であるアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="5bb71-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="5bb71-144">アイテムが送信トレイの既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="5bb71-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="5bb71-146">アイテムがまだ送信されていないかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="5bb71-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="5bb71-148">ユーザーが自分にアイテムを送信したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="5bb71-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="5bb71-150">アイテムが以前に送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="5bb71-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="5bb71-152">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="5bb71-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="5bb71-154">メールボックス内のアイテム内に含まれるすべてのインターネットメッセージヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="5bb71-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="5bb71-156">メールボックス内のアイテムが送信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="5bb71-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="5bb71-158">メールボックス内の特定のアイテムが作成された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="5bb71-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="5bb71-160">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="5bb71-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="5bb71-162">イベントが発生した日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="5bb71-163">これは、アラームがいつ表示されるかを決定するために[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="5bb71-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="5bb71-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="5bb71-165">Exchange ストア内のアイテムにアラームが設定されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="5bb71-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="5bb71-167">アラームが表示されるイベントの前の時間 (分単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="5bb71-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="5bb71-169">[Cc] ボックスの内容に使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="5bb71-170">これは、すべての Cc 受信者表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="5bb71-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="5bb71-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="5bb71-172">[宛先] ボックスの内容に対して使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="5bb71-173">これは、すべての受信者の表示名の連結文字列です。</span><span class="sxs-lookup"><span data-stu-id="5bb71-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="5bb71-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="5bb71-175">アイテムに少なくとも1つの添付ファイルがある場合に**true**に設定されるプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="5bb71-176">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="5bb71-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="5bb71-178">フォルダーとアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-179">Culture</span><span class="sxs-lookup"><span data-stu-id="5bb71-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="5bb71-180">メールボックス内の特定のアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-181">Sender</span><span class="sxs-lookup"><span data-stu-id="5bb71-181">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="5bb71-182">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-182">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-183">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="5bb71-183">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="5bb71-184">メッセージの受信者のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5bb71-184">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-185">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="5bb71-185">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="5bb71-186">メッセージのコピーを受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-186">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-187">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="5bb71-187">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="5bb71-188">電子メールのブラインドカーボンコピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-188">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-189">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="5bb71-189">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="5bb71-190">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-190">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-191">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="5bb71-191">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="5bb71-192">アイテムの送信者が配信確認を要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-192">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-193">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="5bb71-193">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="5bb71-194">このメッセージが属しているスレッドを表すバイナリ ID を含みます。</span><span class="sxs-lookup"><span data-stu-id="5bb71-194">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-195">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="5bb71-195">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="5bb71-196">会話識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-196">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-197">From</span><span class="sxs-lookup"><span data-stu-id="5bb71-197">From</span></span>](from.md) <br/> |<span data-ttu-id="5bb71-198">メッセージが送信された相手のアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-198">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-199">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="5bb71-199">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="5bb71-200">アイテムのインターネットメッセージ識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-200">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-201">IsRead</span><span class="sxs-lookup"><span data-stu-id="5bb71-201">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="5bb71-202">メッセージが開封されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-202">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-203">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="5bb71-203">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="5bb71-204">電子メールメッセージに対する応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-204">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-205">References</span><span class="sxs-lookup"><span data-stu-id="5bb71-205">References</span></span>](references.md) <br/> |<span data-ttu-id="5bb71-206">返信と元のメッセージを相互に関連付けるために使用される Usenet ヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-206">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-207">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="5bb71-207">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="5bb71-208">返信を送信する宛先のアドレスのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-208">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-209">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="5bb71-209">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="5bb71-210">[会議メッセージ](meetingmessage.md)に関連付けられている予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-210">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="5bb71-211">IsDelegated</span><span class="sxs-lookup"><span data-stu-id="5bb71-211">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="5bb71-212">代理人アクセス権を持つアカウントによって会議が処理されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-212">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-213">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="5bb71-213">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="5bb71-214">会議メッセージが古くなっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-214">Indicates whether a meeting message is out-of-date.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-215">Hasが処理されました</span><span class="sxs-lookup"><span data-stu-id="5bb71-215">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="5bb71-216">会議メッセージアイテムが処理されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-216">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-217">ResponseType</span><span class="sxs-lookup"><span data-stu-id="5bb71-217">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="5bb71-218">会議の受信者の応答の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-218">Represents the type of recipient response that is received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-219">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="5bb71-219">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="5bb71-220">アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5bb71-220">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="5bb71-221">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="5bb71-221">This element is read-only.</span></span> <span data-ttu-id="5bb71-222">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5bb71-222">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="5bb71-223">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="5bb71-223">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="5bb71-224">代理人アクセスシナリオの代理人を識別します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-224">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="5bb71-225">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5bb71-225">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-226">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="5bb71-226">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="5bb71-227">代理人アクセスシナリオのプリンシパルを識別します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-227">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="5bb71-228">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5bb71-228">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-229">UID</span><span class="sxs-lookup"><span data-stu-id="5bb71-229">UID</span></span>](uid.md) <br/> |<span data-ttu-id="5bb71-230">予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-230">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-231">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="5bb71-231">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="5bb71-232">定期的な予定表アイテムの特定のインスタンスを識別するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="5bb71-232">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-233">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="5bb71-233">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="5bb71-234">ICalendar オブジェクトのインスタンスが作成された日付と時刻を示します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-234">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5bb71-235">親要素</span><span class="sxs-lookup"><span data-stu-id="5bb71-235">Parent elements</span></span>

|<span data-ttu-id="5bb71-236">**要素**</span><span class="sxs-lookup"><span data-stu-id="5bb71-236">**Element**</span></span>|<span data-ttu-id="5bb71-237">**説明**</span><span class="sxs-lookup"><span data-stu-id="5bb71-237">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5bb71-238">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="5bb71-238">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="5bb71-239">会議の時刻に隣接しているすべての予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-239">Identifies all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-240">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="5bb71-240">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="5bb71-241">[Updateitem 操作](updateitem-operation.md)中に、アイテムの1つのプロパティに追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-241">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="5bb71-242">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="5bb71-242">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="5bb71-243">会議の時間と競合するすべてのアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-243">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-244">Create (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="5bb71-244">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="5bb71-245">ローカルクライアントストアに作成する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-245">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-246">Items</span><span class="sxs-lookup"><span data-stu-id="5bb71-246">Items</span></span>](items.md) <br/> |<span data-ttu-id="5bb71-247">項目の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-247">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-248">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="5bb71-248">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="5bb71-249">作成するアイテムの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-249">Contains an array of items to create.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-250">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="5bb71-250">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="5bb71-251">別の Exchange アイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-251">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="5bb71-252">SetItemField</span><span class="sxs-lookup"><span data-stu-id="5bb71-252">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="5bb71-253">[Updateitem 操作](updateitem-operation.md)のアイテムの1つのプロパティに対する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-253">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="5bb71-254">Update (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="5bb71-254">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="5bb71-255">ローカルクライアントストアで更新する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="5bb71-255">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5bb71-256">注釈</span><span class="sxs-lookup"><span data-stu-id="5bb71-256">Remarks</span></span>

<span data-ttu-id="5bb71-257">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5bb71-257">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5bb71-258">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5bb71-258">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5bb71-259">Namespace</span><span class="sxs-lookup"><span data-stu-id="5bb71-259">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5bb71-260">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5bb71-260">Schema Name</span></span>  <br/> |<span data-ttu-id="5bb71-261">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="5bb71-261">Types schema</span></span>  <br/> |
|<span data-ttu-id="5bb71-262">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5bb71-262">Validation File</span></span>  <br/> |<span data-ttu-id="5bb71-263">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="5bb71-263">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5bb71-264">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5bb71-264">Can be Empty</span></span>  <br/> |<span data-ttu-id="5bb71-265">正しくない</span><span class="sxs-lookup"><span data-stu-id="5bb71-265">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5bb71-266">関連項目</span><span class="sxs-lookup"><span data-stu-id="5bb71-266">See also</span></span>



- [<span data-ttu-id="5bb71-267">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5bb71-267">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


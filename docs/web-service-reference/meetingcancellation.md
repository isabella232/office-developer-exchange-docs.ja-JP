---
title: MeetingCancellation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingCancellation
api_type:
- schema
ms.assetid: a9c61f7f-2ecd-4b21-9dce-24d9f61aeeea
description: MeetingCancellation 要素は、Exchange ストア内の会議の取り消し通知を表します。
ms.openlocfilehash: b68135e2743c675bed92c54172369c2ef21f1a6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832447"
---
# <a name="meetingcancellation"></a><span data-ttu-id="79813-103">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="79813-103">MeetingCancellation</span></span>

<span data-ttu-id="79813-104">**MeetingCancellation**要素は、Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="79813-104">The **MeetingCancellation** element represents a meeting cancellation in the Exchange store.</span></span> 
  
```xml
<MeetingCancellation>
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
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
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
</MeetingCancellation>
```

 <span data-ttu-id="79813-105">**MeetingCancellationMessageType**</span><span class="sxs-lookup"><span data-stu-id="79813-105">**MeetingCancellationMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="79813-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="79813-106">Attributes and elements</span></span>

<span data-ttu-id="79813-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="79813-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79813-108">属性</span><span class="sxs-lookup"><span data-stu-id="79813-108">Attributes</span></span>

<span data-ttu-id="79813-109">なし。</span><span class="sxs-lookup"><span data-stu-id="79813-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79813-110">子要素</span><span class="sxs-lookup"><span data-stu-id="79813-110">Child elements</span></span>

|<span data-ttu-id="79813-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="79813-111">**Element**</span></span>|<span data-ttu-id="79813-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="79813-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79813-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="79813-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="79813-114">Base64Binary の形式で表されるオブジェクトのネイティブの MIME ストリームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="79813-114">Contains the native MIME stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="79813-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="79813-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="79813-116">Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="79813-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="79813-117">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="79813-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="79813-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="79813-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="79813-119">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="79813-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="79813-120">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="79813-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="79813-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="79813-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="79813-122">アイテムのメッセージ クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="79813-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="79813-123">Subject</span><span class="sxs-lookup"><span data-stu-id="79813-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="79813-124">Exchange ストアのアイテムおよび応答オブジェクトのサブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="79813-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="79813-125">件名は、255 文字までに制限されています。</span><span class="sxs-lookup"><span data-stu-id="79813-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="79813-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="79813-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="79813-127">アイテムの秘密度レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="79813-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="79813-128">Body/本文</span><span class="sxs-lookup"><span data-stu-id="79813-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="79813-129">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="79813-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="79813-130">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="79813-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="79813-131">アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="79813-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="79813-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="79813-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="79813-133">メールボックス内のアイテムを受信したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="79813-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="79813-134">Size</span><span class="sxs-lookup"><span data-stu-id="79813-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="79813-135">アイテムのバイト単位のサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="79813-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="79813-136">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="79813-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="79813-137">Categories</span><span class="sxs-lookup"><span data-stu-id="79813-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="79813-138">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="79813-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="79813-139">Importance</span><span class="sxs-lookup"><span data-stu-id="79813-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="79813-140">アイテムの重要性をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="79813-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="79813-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="79813-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="79813-142">このアイテムの返信するアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="79813-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="79813-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="79813-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="79813-144">アイテムが [送信トレイ] 既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79813-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="79813-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="79813-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="79813-146">アイテムはまだ送信されていないかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="79813-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="79813-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="79813-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="79813-148">ユーザーが彼または彼女自身にアイテムを送信するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79813-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="79813-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="79813-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="79813-150">アイテムが以前送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79813-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="79813-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="79813-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="79813-152">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79813-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="79813-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="79813-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="79813-154">メールボックス内のアイテムに含まれているすべてのインターネット メッセージ ヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="79813-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="79813-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="79813-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="79813-156">メールボックス内のアイテムが送信された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="79813-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="79813-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="79813-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="79813-158">メールボックス内の特定のアイテムが作成された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="79813-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="79813-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="79813-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="79813-160">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="79813-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="79813-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="79813-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="79813-162">イベントが発生したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="79813-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="79813-163">[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によってアラームが表示されたときを決定する使用されます。</span><span class="sxs-lookup"><span data-stu-id="79813-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="79813-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="79813-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="79813-165">Exchange ストアのアイテムのアラームが設定されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79813-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="79813-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="79813-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="79813-167">分前アラームが表示されているイベントに、の数を表します。</span><span class="sxs-lookup"><span data-stu-id="79813-167">Represents the number of minutes before an event that a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="79813-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="79813-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="79813-169">[Cc] ボックスの内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="79813-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="79813-170">これは、すべての Cc 受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="79813-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="79813-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="79813-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="79813-172">ボックスの内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="79813-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="79813-173">これは、すべての受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="79813-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="79813-174">添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="79813-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="79813-175">アイテムに表示されている 1 つ以上の添付ファイルがある場合に**true**に設定されているプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="79813-175">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="79813-176">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="79813-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="79813-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="79813-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="79813-178">フォルダーおよびアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="79813-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="79813-179">カルチャ</span><span class="sxs-lookup"><span data-stu-id="79813-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="79813-180">メールボックス内の指定したアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="79813-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="79813-181">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="79813-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="79813-182">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="79813-182">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="79813-183">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="79813-183">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="79813-184">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="79813-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="79813-185">最後の項目を変更するのにはユーザーの表示名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="79813-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="79813-186">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="79813-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="79813-187">アイテムが最後に修正された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="79813-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="79813-188">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="79813-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="79813-189">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79813-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="79813-190">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="79813-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="79813-191">Outlook Web App 内の項目を参照するのには Microsoft Office Outlook の Web アプリケーションのエンドポイントを結合するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="79813-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="79813-192">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="79813-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="79813-193">Outlook Web App 内の項目を編集するのには Outlook Web App エンドポイントへの連結に URL を表します。</span><span class="sxs-lookup"><span data-stu-id="79813-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="79813-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="79813-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="79813-195">アイテムや会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="79813-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="79813-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="79813-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="79813-197">このスレッドの一意の本文を表すテキストまたは HTML フラグメントを表します。</span><span class="sxs-lookup"><span data-stu-id="79813-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="79813-198">送信者</span><span class="sxs-lookup"><span data-stu-id="79813-198">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="79813-199">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="79813-199">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="79813-200">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="79813-200">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="79813-201">一連メッセージの受信者にはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="79813-201">Contains a set of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="79813-202">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="79813-202">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="79813-203">メッセージのコピーを受け取る受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="79813-203">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="79813-204">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="79813-204">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="79813-205">電子メールのブラインド カーボン コピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="79813-205">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="79813-206">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="79813-206">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="79813-207">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79813-207">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="79813-208">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="79813-208">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="79813-209">アイテムの送信者が配信済みメッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79813-209">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="79813-210">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="79813-210">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="79813-211">このメッセージが属するスレッドを表すバイナリの ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="79813-211">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="79813-212">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="79813-212">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="79813-213">会話 id を表します。</span><span class="sxs-lookup"><span data-stu-id="79813-213">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="79813-214">From</span><span class="sxs-lookup"><span data-stu-id="79813-214">From</span></span>](from.md) <br/> |<span data-ttu-id="79813-215">メッセージの送信元アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="79813-215">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="79813-216">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="79813-216">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="79813-217">アイテムのインターネット メッセージ id を表します。</span><span class="sxs-lookup"><span data-stu-id="79813-217">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="79813-218">IsRead</span><span class="sxs-lookup"><span data-stu-id="79813-218">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="79813-219">メッセージが読み取られたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79813-219">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="79813-220">IsResponseRequested</span><span class="sxs-lookup"><span data-stu-id="79813-220">IsResponseRequested</span></span>](isresponserequested.md) <br/> |<span data-ttu-id="79813-221">電子メール メッセージへの応答が要求されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79813-221">Indicates whether a response to an e-mail message is requested.</span></span>  <br/> |
|[<span data-ttu-id="79813-222">参照資料</span><span class="sxs-lookup"><span data-stu-id="79813-222">References</span></span>](references.md) <br/> |<span data-ttu-id="79813-223">元のメッセージに応答を関連付けるために使用する Usenet ヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="79813-223">Represents the Usenet header that is used to correlate replies with their original messages.</span></span>  <br/> |
|[<span data-ttu-id="79813-224">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="79813-224">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="79813-225">応答を送信するアドレスのセットを識別します。</span><span class="sxs-lookup"><span data-stu-id="79813-225">Identifies a set of addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="79813-226">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="79813-226">AssociatedCalendarItemId</span></span>](associatedcalendaritemid.md) <br/> |<span data-ttu-id="79813-227">の[MeetingMessage](meetingmessage.md)に関連付けられている予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="79813-227">Represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md).</span></span>  <br/> |
|[<span data-ttu-id="79813-228">IsDelegated</span><span class="sxs-lookup"><span data-stu-id="79813-228">IsDelegated</span></span>](isdelegated.md) <br/> |<span data-ttu-id="79813-229">会議は、代理人アクセスを持つアカウントによって処理されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79813-229">Indicates whether a meeting was handled by an account with delegate access.</span></span>  <br/> |
|[<span data-ttu-id="79813-230">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="79813-230">IsOutOfDate</span></span>](isoutofdate.md) <br/> |<span data-ttu-id="79813-231">会議メッセージが期限切れかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79813-231">Indicates whether a meeting message is out-of-date.</span></span>  <br/> |
|[<span data-ttu-id="79813-232">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="79813-232">HasBeenProcessed</span></span>](hasbeenprocessed.md) <br/> |<span data-ttu-id="79813-233">かどうか、会議出席依頼アイテムが処理されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="79813-233">Indicates whether a meeting message item has been processed.</span></span>  <br/> |
|[<span data-ttu-id="79813-234">ResponseType</span><span class="sxs-lookup"><span data-stu-id="79813-234">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="79813-235">会議の受信者の応答の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="79813-235">Represents the type of recipient response received for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="79813-236">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="79813-236">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="79813-237">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="79813-237">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="79813-238">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="79813-238">This element is read-only.</span></span> <span data-ttu-id="79813-239">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="79813-239">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="79813-240">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="79813-240">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="79813-241">代理人アクセス シナリオでは、デリゲートを識別します。</span><span class="sxs-lookup"><span data-stu-id="79813-241">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="79813-242">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="79813-242">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="79813-243">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="79813-243">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="79813-244">代理人アクセスのシナリオでプリンシパルを識別します。</span><span class="sxs-lookup"><span data-stu-id="79813-244">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="79813-245">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="79813-245">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="79813-246">UID</span><span class="sxs-lookup"><span data-stu-id="79813-246">UID</span></span>](uid.md) <br/> |<span data-ttu-id="79813-247">予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="79813-247">Identifies a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="79813-248">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="79813-248">RecurrenceId</span></span>](recurrenceid.md) <br/> |<span data-ttu-id="79813-249">定期的な予定表アイテムの特定のインスタンスを識別するために使用します。</span><span class="sxs-lookup"><span data-stu-id="79813-249">Used to identify a specific instance of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="79813-250">DateTimeStamp</span><span class="sxs-lookup"><span data-stu-id="79813-250">DateTimeStamp</span></span>](datetimestamp.md) <br/> |<span data-ttu-id="79813-251">ICalendar オブジェクトのインスタンスが作成された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="79813-251">Indicates the date and time that an instance of an iCalendar object was created.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="79813-252">親要素</span><span class="sxs-lookup"><span data-stu-id="79813-252">Parent elements</span></span>

|<span data-ttu-id="79813-253">**要素**</span><span class="sxs-lookup"><span data-stu-id="79813-253">**Element**</span></span>|<span data-ttu-id="79813-254">**説明**</span><span class="sxs-lookup"><span data-stu-id="79813-254">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79813-255">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="79813-255">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="79813-256">会議の時刻に隣接しているすべての予定表アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="79813-256">Identifies all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="79813-257">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="79813-257">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="79813-258">[UpdateItem 操作](updateitem-operation.md)中に 1 つのアイテムのプロパティを追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="79813-258">Identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="79813-259">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="79813-259">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="79813-260">会議の時間と競合するすべての項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="79813-260">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="79813-261">(ItemSync) を作成します。</span><span class="sxs-lookup"><span data-stu-id="79813-261">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="79813-262">ローカル クライアント ストアに作成する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="79813-262">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="79813-263">Items</span><span class="sxs-lookup"><span data-stu-id="79813-263">Items</span></span>](items.md) <br/> |<span data-ttu-id="79813-264">項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="79813-264">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="79813-265">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="79813-265">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="79813-266">作成する項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="79813-266">Contains an array of items to create.</span></span>  <br/> |
|[<span data-ttu-id="79813-267">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="79813-267">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="79813-268">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="79813-268">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="79813-269">SetItemField</span><span class="sxs-lookup"><span data-stu-id="79813-269">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="79813-270">[UpdateItem 操作](updateitem-operation.md)内の項目の 1 つのプロパティには、更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="79813-270">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="79813-271">更新プログラム (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="79813-271">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="79813-272">ローカル クライアント ストアで更新する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="79813-272">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="79813-273">テキスト値</span><span class="sxs-lookup"><span data-stu-id="79813-273">Text value</span></span>

<span data-ttu-id="79813-274">なし。</span><span class="sxs-lookup"><span data-stu-id="79813-274">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="79813-275">備考</span><span class="sxs-lookup"><span data-stu-id="79813-275">Remarks</span></span>

<span data-ttu-id="79813-276">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="79813-276">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="79813-277">要素情報</span><span class="sxs-lookup"><span data-stu-id="79813-277">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79813-278">名前空間</span><span class="sxs-lookup"><span data-stu-id="79813-278">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="79813-279">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="79813-279">Schema Name</span></span>  <br/> |<span data-ttu-id="79813-280">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="79813-280">Types schema</span></span>  <br/> |
|<span data-ttu-id="79813-281">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="79813-281">Validation File</span></span>  <br/> |<span data-ttu-id="79813-282">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="79813-282">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="79813-283">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="79813-283">Can be Empty</span></span>  <br/> |<span data-ttu-id="79813-284">False</span><span class="sxs-lookup"><span data-stu-id="79813-284">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="79813-285">関連項目</span><span class="sxs-lookup"><span data-stu-id="79813-285">See also</span></span>



- [<span data-ttu-id="79813-286">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="79813-286">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


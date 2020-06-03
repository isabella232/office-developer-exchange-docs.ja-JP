---
title: PostItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PostItem
api_type:
- schema
ms.assetid: 7727ed84-9591-4a1c-bb04-12129926499b
description: PostItem 要素は、Exchange ストア内の投稿アイテムを表します。
ms.openlocfilehash: 5fba1a9a6a3abc95ea2ce65cafa2b62bc7423f28
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528868"
---
# <a name="postitem"></a><span data-ttu-id="8dc78-103">PostItem</span><span class="sxs-lookup"><span data-stu-id="8dc78-103">PostItem</span></span>

<span data-ttu-id="8dc78-104">**Postitem**要素は、Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-104">The **PostItem** element represents a post item in the Exchange store.</span></span> 
  
```xml
<PostItem>
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
   <ConversationIndex/>
   <ConversationTopic/>
   <From/>
   <InternetMessageId/>
   <IsRead/>
   <PostedTime/>
   <References/>
   <Sender/>
</PostItem>
```

 <span data-ttu-id="8dc78-105">**PostItemType**</span><span class="sxs-lookup"><span data-stu-id="8dc78-105">**PostItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8dc78-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8dc78-106">Attributes and elements</span></span>

<span data-ttu-id="8dc78-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8dc78-108">属性</span><span class="sxs-lookup"><span data-stu-id="8dc78-108">Attributes</span></span>

<span data-ttu-id="8dc78-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8dc78-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8dc78-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8dc78-110">Child elements</span></span>

|<span data-ttu-id="8dc78-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="8dc78-111">**Element**</span></span>|<span data-ttu-id="8dc78-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="8dc78-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8dc78-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="8dc78-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="8dc78-114">Base64Binary 形式で表されるオブジェクトのネイティブな汎用インターネットメール内線 (MIME) ストリームが保存されています。</span><span class="sxs-lookup"><span data-stu-id="8dc78-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="8dc78-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="8dc78-116">Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8dc78-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="8dc78-117">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="8dc78-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="8dc78-119">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="8dc78-120">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="8dc78-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="8dc78-122">アイテムのメッセージクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-123">件名</span><span class="sxs-lookup"><span data-stu-id="8dc78-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="8dc78-124">Exchange ストアアイテムおよび応答オブジェクトの件名を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="8dc78-125">件名は255文字に制限されます。</span><span class="sxs-lookup"><span data-stu-id="8dc78-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="8dc78-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="8dc78-127">アイテムの秘密度レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-128">Body</span><span class="sxs-lookup"><span data-stu-id="8dc78-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="8dc78-129">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-130">Attachments</span><span class="sxs-lookup"><span data-stu-id="8dc78-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8dc78-131">Exchange ストア内のアイテムに添付されているアイテムまたはファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="8dc78-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="8dc78-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="8dc78-133">メールボックス内のアイテムが受信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-134">Size</span><span class="sxs-lookup"><span data-stu-id="8dc78-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="8dc78-135">アイテムのサイズ (バイト単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="8dc78-136">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-137">Categories</span><span class="sxs-lookup"><span data-stu-id="8dc78-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8dc78-138">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-138">Represents a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-139">Importance</span><span class="sxs-lookup"><span data-stu-id="8dc78-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="8dc78-140">アイテムの重要度について説明します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="8dc78-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="8dc78-142">このアイテムが返信であるアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="8dc78-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="8dc78-144">アイテムが送信トレイの既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="8dc78-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="8dc78-146">アイテムがまだ送信されていないかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="8dc78-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="8dc78-148">ユーザーが自分にアイテムを送信したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="8dc78-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="8dc78-150">アイテムが以前に送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="8dc78-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="8dc78-152">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="8dc78-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="8dc78-154">メールボックス内のアイテムに含まれるすべてのインターネットメッセージヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-154">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="8dc78-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="8dc78-156">メールボックス内のアイテムが送信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="8dc78-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="8dc78-158">メールボックス内の特定のアイテムが作成された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="8dc78-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="8dc78-160">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="8dc78-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="8dc78-162">イベントが発生した日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="8dc78-163">これは、アラームがいつ表示されるかを決定するために[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="8dc78-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="8dc78-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="8dc78-165">Exchange ストア内のアイテムにアラームが設定されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="8dc78-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="8dc78-167">アラームが表示されるイベントの前の時間 (分単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="8dc78-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="8dc78-169">[Cc] ボックスの内容に使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="8dc78-170">これは、すべての Cc 受信者表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="8dc78-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="8dc78-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="8dc78-172">[宛先] ボックスの内容に対して使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="8dc78-173">これは、すべての受信者の表示名の連結文字列です。</span><span class="sxs-lookup"><span data-stu-id="8dc78-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-174">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="8dc78-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="8dc78-175">アイテムに少なくとも1つの添付ファイルがある場合に**true**に設定されるプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-175">Represents a property that is set to **true** if an item has at least one attachment.</span></span> <span data-ttu-id="8dc78-176">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="8dc78-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="8dc78-178">フォルダーとアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-179">Culture</span><span class="sxs-lookup"><span data-stu-id="8dc78-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="8dc78-180">メールボックス内の特定のアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-181">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="8dc78-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="8dc78-182">アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8dc78-182">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="8dc78-183">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8dc78-183">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-184">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="8dc78-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="8dc78-185">アイテムを最後に変更したユーザーの表示名を含みます。</span><span class="sxs-lookup"><span data-stu-id="8dc78-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-186">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="8dc78-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="8dc78-187">アイテムが最後に変更された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-188">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="8dc78-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="8dc78-189">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-190">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="8dc78-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="8dc78-191">Outlook Web app のアイテムを読み取るために Microsoft Office Outlook Web App エンドポイントに連結する URL を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-192">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="8dc78-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="8dc78-193">Outlook web app エンドポイントに連結して Outlook Web App のアイテムを編集するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="8dc78-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="8dc78-195">アイテムまたは会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8dc78-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="8dc78-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="8dc78-197">この会話の一意の本文を表す HTML フラグメントまたはプレーンテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-198">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="8dc78-198">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="8dc78-199">このメッセージが属しているスレッドを表すバイナリ ID を含みます。</span><span class="sxs-lookup"><span data-stu-id="8dc78-199">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-200">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="8dc78-200">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="8dc78-201">会話識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-201">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-202">From</span><span class="sxs-lookup"><span data-stu-id="8dc78-202">From</span></span>](from.md) <br/> |<span data-ttu-id="8dc78-203">投稿アイテムの送信元のアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-203">Represents the address from which the post item was sent.</span></span> <span data-ttu-id="8dc78-204">**From**要素は、作成時にのみ設定できます。</span><span class="sxs-lookup"><span data-stu-id="8dc78-204">The **From** element can only be set at creation time.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-205">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="8dc78-205">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="8dc78-206">アイテムのインターネットメッセージ識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-206">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-207">IsRead</span><span class="sxs-lookup"><span data-stu-id="8dc78-207">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="8dc78-208">メッセージが開封されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-208">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-209">PostedTime</span><span class="sxs-lookup"><span data-stu-id="8dc78-209">PostedTime</span></span>](postedtime.md) <br/> |<span data-ttu-id="8dc78-210">[Postitem](postitem.md)が投稿された時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-210">Represents the time that a [PostItem](postitem.md) was posted.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-211">References</span><span class="sxs-lookup"><span data-stu-id="8dc78-211">References</span></span>](references.md) <br/> |<span data-ttu-id="8dc78-212">元のメッセージに返信を関連付けるために使用される Usenet ヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-212">Represents the Usenet header that is used to associate replies with the original messages.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-213">Sender</span><span class="sxs-lookup"><span data-stu-id="8dc78-213">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="8dc78-214">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-214">Identifies the sender of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8dc78-215">親要素</span><span class="sxs-lookup"><span data-stu-id="8dc78-215">Parent elements</span></span>

|<span data-ttu-id="8dc78-216">**要素**</span><span class="sxs-lookup"><span data-stu-id="8dc78-216">**Element**</span></span>|<span data-ttu-id="8dc78-217">**説明**</span><span class="sxs-lookup"><span data-stu-id="8dc78-217">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8dc78-218">SetItemField</span><span class="sxs-lookup"><span data-stu-id="8dc78-218">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="8dc78-219">UpdateItem 操作のアイテムの1つのプロパティに対する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-219">Represents an update to a single property of an item in an UpdateItem operation.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-220">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="8dc78-220">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="8dc78-221">[Updateitem 操作](updateitem-operation.md)中に、アイテムまたはフォルダーの1つのプロパティに追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-221">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="8dc78-222">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="8dc78-222">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="8dc78-223">別の Exchange アイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-223">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-224">Create (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="8dc78-224">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="8dc78-225">ローカルクライアントストアに作成する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-225">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-226">Update (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="8dc78-226">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="8dc78-227">ローカルクライアントストアで更新する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-227">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-228">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="8dc78-228">ReadFlagChange</span></span>](readflagchange.md) <br/> |<span data-ttu-id="8dc78-229">アイテムが読み取られたときの[Syncfolderitems](syncfolderitems.md)応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="8dc78-229">Returned in [SyncFolderItems](syncfolderitems.md) responses when an item has been read.</span></span> <span data-ttu-id="8dc78-230">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-230">This property is read-only.</span></span> <span data-ttu-id="8dc78-231">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8dc78-231">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-232">Items</span><span class="sxs-lookup"><span data-stu-id="8dc78-232">Items</span></span>](items.md) <br/> |<span data-ttu-id="8dc78-233">項目の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-233">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-234">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="8dc78-234">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="8dc78-235">会議の時間と競合するすべてのアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-235">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="8dc78-236">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="8dc78-236">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="8dc78-237">会議の時刻に隣接しているすべての予定表アイテムを説明します。</span><span class="sxs-lookup"><span data-stu-id="8dc78-237">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8dc78-238">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8dc78-238">Text value</span></span>

<span data-ttu-id="8dc78-239">なし。</span><span class="sxs-lookup"><span data-stu-id="8dc78-239">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8dc78-240">注釈</span><span class="sxs-lookup"><span data-stu-id="8dc78-240">Remarks</span></span>

<span data-ttu-id="8dc78-241">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8dc78-241">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8dc78-242">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8dc78-242">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8dc78-243">Namespace</span><span class="sxs-lookup"><span data-stu-id="8dc78-243">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8dc78-244">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8dc78-244">Schema Name</span></span>  <br/> |<span data-ttu-id="8dc78-245">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8dc78-245">Types schema</span></span>  <br/> |
|<span data-ttu-id="8dc78-246">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8dc78-246">Validation File</span></span>  <br/> |<span data-ttu-id="8dc78-247">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8dc78-247">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8dc78-248">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8dc78-248">Can be Empty</span></span>  <br/> |<span data-ttu-id="8dc78-249">正しくない</span><span class="sxs-lookup"><span data-stu-id="8dc78-249">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8dc78-250">関連項目</span><span class="sxs-lookup"><span data-stu-id="8dc78-250">See also</span></span>



- [<span data-ttu-id="8dc78-251">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8dc78-251">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


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
description: PostItem エレメントでは、Exchange ストア内の投稿アイテムを表します。
ms.openlocfilehash: 3fb6d6cfe334999c93ca0238547dd5aee8150a5f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832866"
---
# <a name="postitem"></a><span data-ttu-id="57d75-103">PostItem</span><span class="sxs-lookup"><span data-stu-id="57d75-103">PostItem</span></span>

<span data-ttu-id="57d75-104">**PostItem**エレメントでは、Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-104">The **PostItem** element represents a post item in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="57d75-105">**PostItemType**</span><span class="sxs-lookup"><span data-stu-id="57d75-105">**PostItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57d75-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="57d75-106">Attributes and elements</span></span>

<span data-ttu-id="57d75-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="57d75-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57d75-108">属性</span><span class="sxs-lookup"><span data-stu-id="57d75-108">Attributes</span></span>

<span data-ttu-id="57d75-109">なし。</span><span class="sxs-lookup"><span data-stu-id="57d75-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57d75-110">子要素</span><span class="sxs-lookup"><span data-stu-id="57d75-110">Child elements</span></span>

|<span data-ttu-id="57d75-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="57d75-111">**Element**</span></span>|<span data-ttu-id="57d75-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="57d75-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57d75-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="57d75-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="57d75-114">Base64Binary の形式で表されるオブジェクトのネイティブの多目的インターネット メール拡張 (MIME) ストリームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="57d75-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="57d75-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="57d75-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="57d75-116">Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="57d75-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="57d75-117">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="57d75-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="57d75-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="57d75-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="57d75-119">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="57d75-120">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="57d75-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="57d75-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="57d75-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="57d75-122">アイテムのメッセージ クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="57d75-123">Subject</span><span class="sxs-lookup"><span data-stu-id="57d75-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="57d75-124">Exchange ストアのアイテムおよび応答オブジェクトのサブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="57d75-125">件名は、255 文字までに制限されています。</span><span class="sxs-lookup"><span data-stu-id="57d75-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="57d75-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="57d75-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="57d75-127">アイテムの秘密度レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="57d75-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="57d75-128">Body/本文</span><span class="sxs-lookup"><span data-stu-id="57d75-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="57d75-129">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="57d75-130">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="57d75-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="57d75-131">アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="57d75-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="57d75-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="57d75-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="57d75-133">メールボックス内のアイテムを受信したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="57d75-134">Size</span><span class="sxs-lookup"><span data-stu-id="57d75-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="57d75-135">アイテムのバイト単位のサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="57d75-136">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="57d75-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="57d75-137">Categories</span><span class="sxs-lookup"><span data-stu-id="57d75-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="57d75-138">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-138">Represents a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="57d75-139">Importance</span><span class="sxs-lookup"><span data-stu-id="57d75-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="57d75-140">アイテムの重要性をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="57d75-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="57d75-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="57d75-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="57d75-142">このアイテムの返信するアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="57d75-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="57d75-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="57d75-144">アイテムが [送信トレイ] 既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="57d75-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="57d75-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="57d75-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="57d75-146">アイテムはまだ送信されていないかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="57d75-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="57d75-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="57d75-148">ユーザーが彼または彼女自身にアイテムを送信するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="57d75-148">Indicates whether a user sent an item to him or herself.</span></span>  <br/> |
|[<span data-ttu-id="57d75-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="57d75-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="57d75-150">アイテムが以前送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="57d75-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="57d75-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="57d75-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="57d75-152">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="57d75-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="57d75-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="57d75-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="57d75-154">メールボックス内のアイテムに含まれるすべてのインターネット メッセージ ヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-154">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="57d75-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="57d75-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="57d75-156">メールボックス内のアイテムが送信された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="57d75-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="57d75-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="57d75-158">メールボックス内の特定のアイテムが作成された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="57d75-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="57d75-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="57d75-160">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="57d75-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="57d75-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="57d75-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="57d75-162">イベントが発生したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="57d75-163">[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によってアラームが表示されたときを決定する使用されます。</span><span class="sxs-lookup"><span data-stu-id="57d75-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="57d75-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="57d75-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="57d75-165">Exchange ストアのアイテムのアラームが設定されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="57d75-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="57d75-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="57d75-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="57d75-167">分前にアラームが表示されるときに、イベントの数を表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="57d75-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="57d75-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="57d75-169">[Cc] ボックスの内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="57d75-170">これは、すべての Cc 受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="57d75-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="57d75-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="57d75-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="57d75-172">ボックスの内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="57d75-173">これは、すべての受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="57d75-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="57d75-174">添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="57d75-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="57d75-175">項目に 1 つ以上の添付ファイルがある場合に**true**に設定されているプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-175">Represents a property that is set to **true** if an item has at least one attachment.</span></span> <span data-ttu-id="57d75-176">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="57d75-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="57d75-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="57d75-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="57d75-178">フォルダーおよびアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="57d75-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="57d75-179">カルチャ</span><span class="sxs-lookup"><span data-stu-id="57d75-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="57d75-180">メールボックス内の指定したアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="57d75-181">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="57d75-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="57d75-182">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="57d75-182">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="57d75-183">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="57d75-183">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="57d75-184">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="57d75-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="57d75-185">最後の項目を変更するのにはユーザーの表示名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="57d75-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="57d75-186">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="57d75-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="57d75-187">アイテムが最後に修正された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="57d75-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="57d75-188">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="57d75-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="57d75-189">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="57d75-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="57d75-190">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="57d75-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="57d75-191">Outlook Web App 内の項目を参照するのには Microsoft Office Outlook の Web アプリケーションのエンドポイントを結合するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="57d75-192">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="57d75-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="57d75-193">Outlook Web App 内の項目を編集するのには Outlook Web App エンドポイントへの連結に URL を表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="57d75-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="57d75-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="57d75-195">アイテムや会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="57d75-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="57d75-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="57d75-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="57d75-197">このスレッドの一意の本文を表すテキストまたは HTML フラグメントを表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="57d75-198">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="57d75-198">ConversationIndex</span></span>](conversationindex.md) <br/> |<span data-ttu-id="57d75-199">このメッセージが属するスレッドを表すバイナリの ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="57d75-199">Contains a binary ID that represents the thread to which this message belongs.</span></span>  <br/> |
|[<span data-ttu-id="57d75-200">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="57d75-200">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="57d75-201">会話 id を表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-201">Represents the conversation identifier.</span></span>  <br/> |
|[<span data-ttu-id="57d75-202">From</span><span class="sxs-lookup"><span data-stu-id="57d75-202">From</span></span>](from.md) <br/> |<span data-ttu-id="57d75-203">投稿アイテムの送信元アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-203">Represents the address from which the post item was sent.</span></span> <span data-ttu-id="57d75-204">**** 要素は、作成時にのみ設定できます。</span><span class="sxs-lookup"><span data-stu-id="57d75-204">The **From** element can only be set at creation time.</span></span>  <br/> |
|[<span data-ttu-id="57d75-205">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="57d75-205">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="57d75-206">アイテムのインターネット メッセージ id を表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-206">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="57d75-207">IsRead</span><span class="sxs-lookup"><span data-stu-id="57d75-207">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="57d75-208">メッセージが読み取られたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="57d75-208">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="57d75-209">PostedTime</span><span class="sxs-lookup"><span data-stu-id="57d75-209">PostedTime</span></span>](postedtime.md) <br/> |<span data-ttu-id="57d75-210">[PostItem](postitem.md)転記された時間を表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-210">Represents the time that a [PostItem](postitem.md) was posted.</span></span>  <br/> |
|[<span data-ttu-id="57d75-211">参照資料</span><span class="sxs-lookup"><span data-stu-id="57d75-211">References</span></span>](references.md) <br/> |<span data-ttu-id="57d75-212">返信に元のメッセージを関連付けるために使用する Usenet ヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-212">Represents the Usenet header that is used to associate replies with the original messages.</span></span>  <br/> |
|[<span data-ttu-id="57d75-213">送信者</span><span class="sxs-lookup"><span data-stu-id="57d75-213">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="57d75-214">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="57d75-214">Identifies the sender of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="57d75-215">親要素</span><span class="sxs-lookup"><span data-stu-id="57d75-215">Parent elements</span></span>

|<span data-ttu-id="57d75-216">**要素**</span><span class="sxs-lookup"><span data-stu-id="57d75-216">**Element**</span></span>|<span data-ttu-id="57d75-217">**説明**</span><span class="sxs-lookup"><span data-stu-id="57d75-217">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57d75-218">SetItemField</span><span class="sxs-lookup"><span data-stu-id="57d75-218">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="57d75-219">UpdateItem 操作内の項目の 1 つのプロパティには、更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-219">Represents an update to a single property of an item in an UpdateItem operation.</span></span>  <br/> |
|[<span data-ttu-id="57d75-220">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="57d75-220">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="57d75-221">[UpdateItem 操作](updateitem-operation.md)中に 1 つのアイテムまたはフォルダーのプロパティを追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="57d75-221">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="57d75-222">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="57d75-222">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="57d75-223">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="57d75-223">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="57d75-224">(ItemSync) を作成します。</span><span class="sxs-lookup"><span data-stu-id="57d75-224">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="57d75-225">ローカル クライアント ストアに作成する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="57d75-225">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="57d75-226">更新プログラム (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="57d75-226">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="57d75-227">ローカル クライアント ストアで更新する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="57d75-227">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="57d75-228">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="57d75-228">ReadFlagChange</span></span>](readflagchange.md) <br/> |<span data-ttu-id="57d75-229">アイテムを開封したときに、 [SyncFolderItems](syncfolderitems.md)の応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="57d75-229">Returned in [SyncFolderItems](syncfolderitems.md) responses when an item has been read.</span></span> <span data-ttu-id="57d75-230">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="57d75-230">This property is read-only.</span></span> <span data-ttu-id="57d75-231">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="57d75-231">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="57d75-232">Items</span><span class="sxs-lookup"><span data-stu-id="57d75-232">Items</span></span>](items.md) <br/> |<span data-ttu-id="57d75-233">項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="57d75-233">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="57d75-234">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="57d75-234">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="57d75-235">会議の時間と競合するすべての項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="57d75-235">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="57d75-236">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="57d75-236">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="57d75-237">会議の時刻に隣接しているすべての予定表のアイテムについて説明します。</span><span class="sxs-lookup"><span data-stu-id="57d75-237">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="57d75-238">テキスト値</span><span class="sxs-lookup"><span data-stu-id="57d75-238">Text value</span></span>

<span data-ttu-id="57d75-239">なし。</span><span class="sxs-lookup"><span data-stu-id="57d75-239">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="57d75-240">備考</span><span class="sxs-lookup"><span data-stu-id="57d75-240">Remarks</span></span>

<span data-ttu-id="57d75-241">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="57d75-241">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57d75-242">要素情報</span><span class="sxs-lookup"><span data-stu-id="57d75-242">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57d75-243">名前空間</span><span class="sxs-lookup"><span data-stu-id="57d75-243">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="57d75-244">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="57d75-244">Schema Name</span></span>  <br/> |<span data-ttu-id="57d75-245">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="57d75-245">Types schema</span></span>  <br/> |
|<span data-ttu-id="57d75-246">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="57d75-246">Validation File</span></span>  <br/> |<span data-ttu-id="57d75-247">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="57d75-247">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="57d75-248">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="57d75-248">Can be Empty</span></span>  <br/> |<span data-ttu-id="57d75-249">False</span><span class="sxs-lookup"><span data-stu-id="57d75-249">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57d75-250">関連項目</span><span class="sxs-lookup"><span data-stu-id="57d75-250">See also</span></span>



- [<span data-ttu-id="57d75-251">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="57d75-251">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: Item
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Item
api_type:
- schema
ms.assetid: 4dfe8f48-e7b4-444d-bdf9-a34e180f598b
description: Item 要素は、Exchange ストア内の一般的な項目を表します。
ms.openlocfilehash: 7af8e063c3bfd77bd87b80463c11c58d996626b5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832143"
---
# <a name="item"></a><span data-ttu-id="1ddc2-103">Item</span><span class="sxs-lookup"><span data-stu-id="1ddc2-103">Item</span></span>

<span data-ttu-id="1ddc2-104">**Item**要素は、Exchange ストア内の一般的な項目を表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-104">The **Item** element represents a generic item in the Exchange store.</span></span> 
  
```xml
<Item>
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
</Item>
```

 <span data-ttu-id="1ddc2-105">**ItemType**</span><span class="sxs-lookup"><span data-stu-id="1ddc2-105">**ItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ddc2-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1ddc2-106">Attributes and elements</span></span>

<span data-ttu-id="1ddc2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ddc2-108">属性</span><span class="sxs-lookup"><span data-stu-id="1ddc2-108">Attributes</span></span>

<span data-ttu-id="1ddc2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1ddc2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1ddc2-110">Child elements</span></span>

|<span data-ttu-id="1ddc2-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="1ddc2-111">**Element**</span></span>|<span data-ttu-id="1ddc2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ddc2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ddc2-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="1ddc2-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="1ddc2-114">Base64Binary の形式で表されるオブジェクトのネイティブの多目的インターネット メール拡張 (MIME) ストリームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="1ddc2-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="1ddc2-116">Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="1ddc2-117">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-117">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-118">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="1ddc2-118">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="1ddc2-119">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-119">Represents the identifier of the parent folder that contains the item or folder.</span></span> <span data-ttu-id="1ddc2-120">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-120">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-121">ItemClass</span><span class="sxs-lookup"><span data-stu-id="1ddc2-121">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="1ddc2-122">アイテムのメッセージ クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-122">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-123">Subject</span><span class="sxs-lookup"><span data-stu-id="1ddc2-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="1ddc2-124">Exchange ストアのアイテムおよび応答オブジェクトのサブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-124">Represents the subject for Exchange store items and response objects.</span></span> <span data-ttu-id="1ddc2-125">件名は、255 文字までに制限されています。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-125">The subject is limited to 255 characters.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-126">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="1ddc2-126">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="1ddc2-127">アイテムの秘密度レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-127">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-128">Body/本文</span><span class="sxs-lookup"><span data-stu-id="1ddc2-128">Body</span></span>](body.md) <br/> |<span data-ttu-id="1ddc2-129">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-129">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-130">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="1ddc2-130">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1ddc2-131">アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-131">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-132">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="1ddc2-132">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="1ddc2-133">メールボックス内のアイテムを受信したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-133">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-134">Size</span><span class="sxs-lookup"><span data-stu-id="1ddc2-134">Size</span></span>](size.md) <br/> |<span data-ttu-id="1ddc2-135">アイテムのバイト単位のサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-135">Represents the size in bytes of an item.</span></span> <span data-ttu-id="1ddc2-136">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-136">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-137">Categories</span><span class="sxs-lookup"><span data-stu-id="1ddc2-137">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1ddc2-138">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-138">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-139">Importance</span><span class="sxs-lookup"><span data-stu-id="1ddc2-139">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="1ddc2-140">アイテムの重要性をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-140">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-141">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="1ddc2-141">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="1ddc2-142">このアイテムの返信するアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-142">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="1ddc2-143">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="1ddc2-144">アイテムが [送信トレイ] 既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-144">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-145">IsDraft</span><span class="sxs-lookup"><span data-stu-id="1ddc2-145">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="1ddc2-146">アイテムはまだ送信されていないかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-146">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-147">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="1ddc2-147">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="1ddc2-148">ユーザーが自身にアイテムを送信するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-148">Indicates whether a user sent an item to itself.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="1ddc2-149">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="1ddc2-150">アイテムが以前送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-150">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-151">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="1ddc2-151">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="1ddc2-152">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-152">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-153">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="1ddc2-153">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="1ddc2-154">メールボックス内のアイテムに含まれているすべてのインターネット メッセージ ヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-154">Represents the collection of all Internet message headers that are contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-155">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="1ddc2-155">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="1ddc2-156">メールボックス内のアイテムが送信された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-156">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-157">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="1ddc2-157">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="1ddc2-158">メールボックス内の特定のアイテムが作成された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-158">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-159">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="1ddc2-159">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="1ddc2-160">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-160">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-161">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="1ddc2-161">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="1ddc2-162">イベントが発生したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-162">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="1ddc2-163">[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によってアラームが表示されたときを決定する使用されます。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-163">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-164">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="1ddc2-164">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="1ddc2-165">Exchange ストアのアイテムのアラームが設定されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-165">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-166">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="1ddc2-166">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="1ddc2-167">分前にアラームが表示されるときに、イベントの数を表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-167">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-168">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="1ddc2-168">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="1ddc2-169">[Cc] ボックスの内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-169">Represents the display string that is used for the contents of the Cc box.</span></span> <span data-ttu-id="1ddc2-170">これは、すべての Cc 受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-170">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-171">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="1ddc2-171">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="1ddc2-172">ボックスの内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-172">Represents the display string that is used for the contents of the To box.</span></span> <span data-ttu-id="1ddc2-173">これは、すべての受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-173">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-174">添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="1ddc2-174">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="1ddc2-175">アイテムに添付ファイルがある場合に**true**に設定されているプロパティを表す 1 つ以上の表示されている添付ファイルです。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-175">Represents a property that is set to **true** if an item has attachments at least one visible attachment.</span></span> <span data-ttu-id="1ddc2-176">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-176">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-177">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="1ddc2-177">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="1ddc2-178">フォルダーおよびアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-178">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-179">カルチャ</span><span class="sxs-lookup"><span data-stu-id="1ddc2-179">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="1ddc2-180">メールボックス内の指定したアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-180">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-181">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="1ddc2-181">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="1ddc2-182">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-182">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="1ddc2-183">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-183">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-184">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="1ddc2-184">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="1ddc2-185">最後の項目を変更するのにはユーザーの表示名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-185">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-186">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="1ddc2-186">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="1ddc2-187">アイテムが最後に修正された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-187">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-188">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="1ddc2-188">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="1ddc2-189">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-189">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-190">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="1ddc2-190">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="1ddc2-191">Outlook Web App 内の項目を参照するのには Microsoft Office Outlook の Web アプリケーションのエンドポイントを結合するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-191">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-192">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="1ddc2-192">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="1ddc2-193">Outlook Web App 内の項目を編集するのには Outlook Web App エンドポイントへの連結に URL を表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-193">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-194">ConversationId</span><span class="sxs-lookup"><span data-stu-id="1ddc2-194">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="1ddc2-195">アイテムや会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-195">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-196">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="1ddc2-196">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="1ddc2-197">このスレッドの一意の本文を表すテキストまたは HTML フラグメントを表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-197">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1ddc2-198">親要素</span><span class="sxs-lookup"><span data-stu-id="1ddc2-198">Parent elements</span></span>

|<span data-ttu-id="1ddc2-199">**要素**</span><span class="sxs-lookup"><span data-stu-id="1ddc2-199">**Element**</span></span>|<span data-ttu-id="1ddc2-200">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ddc2-200">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ddc2-201">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="1ddc2-201">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="1ddc2-202">会議の時刻に隣接しているすべての予定表のアイテムについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-202">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-203">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="1ddc2-203">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="1ddc2-204">[UpdateItem 操作](updateitem-operation.md)中に、アイテムやフォルダーの 1 つのプロパティを追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-204">Identifies data to append to a single property of an item/folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-205">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="1ddc2-205">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="1ddc2-206">会議の時間と競合するすべての項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-206">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-207">(ItemSync) を作成します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-207">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="1ddc2-208">ローカル クライアント ストアに作成する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-208">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-209">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="1ddc2-209">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="1ddc2-210">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-210">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-211">Items</span><span class="sxs-lookup"><span data-stu-id="1ddc2-211">Items</span></span>](items.md) <br/> |<span data-ttu-id="1ddc2-212">項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-212">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-213">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="1ddc2-213">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="1ddc2-214">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で識別されるフォルダーを作成する項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-214">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-215">SetItemField</span><span class="sxs-lookup"><span data-stu-id="1ddc2-215">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="1ddc2-216">[UpdateItem 操作](updateitem-operation.md)内の項目の 1 つのプロパティには、更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-216">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="1ddc2-217">更新プログラム (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="1ddc2-217">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="1ddc2-218">ローカル クライアント ストアで更新する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-218">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1ddc2-219">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1ddc2-219">Text value</span></span>

<span data-ttu-id="1ddc2-220">なし。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-220">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1ddc2-221">備考</span><span class="sxs-lookup"><span data-stu-id="1ddc2-221">Remarks</span></span>

<span data-ttu-id="1ddc2-222">**ItemType**が[タスク](task.md)、[カレンダー項目](calendaritem.md)、[連絡先](contact.md)、 [DistributionList](distributionlist.md)、および[メッセージ](message-ex15websvcsotherref.md)の基本型であることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-222">It is important to note that **ItemType** is the base type for [Task](task.md), [CalendarItem](calendaritem.md), [Contact](contact.md), [DistributionList](distributionlist.md), and [Message](message-ex15websvcsotherref.md).</span></span>
  
<span data-ttu-id="1ddc2-223">[メッセージ](message-ex15websvcsotherref.md)要素は、電子メール メッセージ、Exchange Web サービス (EWS) スキーマが厳密に型指定されない他のすべての項目を表します。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-223">[Message](message-ex15websvcsotherref.md) elements represent e-mail messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="1ddc2-224">IPM などの項目です。共有し、IPM.InfoPath は、**メッセージ**の要素として返されます。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-224">Items such as IPM.Sharing and IPM.InfoPath are returned as **Message** elements.</span></span> <span data-ttu-id="1ddc2-225">Microsoft Exchange Server 2010 では、応答の基本要素の**項目**が返されません。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-225">Microsoft Exchange Server 2010 does not return the base **Item** element in responses.</span></span> 
  
<span data-ttu-id="1ddc2-226">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1ddc2-226">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ddc2-227">要素情報</span><span class="sxs-lookup"><span data-stu-id="1ddc2-227">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ddc2-228">名前空間</span><span class="sxs-lookup"><span data-stu-id="1ddc2-228">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1ddc2-229">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1ddc2-229">Schema Name</span></span>  <br/> |<span data-ttu-id="1ddc2-230">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1ddc2-230">Types schema</span></span>  <br/> |
|<span data-ttu-id="1ddc2-231">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1ddc2-231">Validation File</span></span>  <br/> |<span data-ttu-id="1ddc2-232">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1ddc2-232">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1ddc2-233">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1ddc2-233">Can be Empty</span></span>  <br/> |<span data-ttu-id="1ddc2-234">False</span><span class="sxs-lookup"><span data-stu-id="1ddc2-234">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ddc2-235">関連項目</span><span class="sxs-lookup"><span data-stu-id="1ddc2-235">See also</span></span>



- [<span data-ttu-id="1ddc2-236">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1ddc2-236">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
<span data-ttu-id="1ddc2-237">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="1ddc2-237">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>


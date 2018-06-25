---
title: DistributionList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistributionList
api_type:
- schema
ms.assetid: f65aea01-e870-44a2-8571-fa6c001341cc
description: DistributionList 要素は、配布リストを表します。
ms.openlocfilehash: 5edcc83eef6a5b16470e6c290aacd057ceecceb1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760135"
---
# <a name="distributionlist"></a><span data-ttu-id="45385-103">DistributionList</span><span class="sxs-lookup"><span data-stu-id="45385-103">DistributionList</span></span>

<span data-ttu-id="45385-104">**DistributionList**要素は、配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="45385-104">The **DistributionList** element represents a distribution list.</span></span> 
  
```xml
<DistributionList>
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
   <DisplayName/>
   <FileAs/>
   <ContactSource/>
   <Members/>
</DistributionList>
```

 <span data-ttu-id="45385-105">**DistributionListType**</span><span class="sxs-lookup"><span data-stu-id="45385-105">**DistributionListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="45385-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="45385-106">Attributes and elements</span></span>

<span data-ttu-id="45385-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="45385-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="45385-108">属性</span><span class="sxs-lookup"><span data-stu-id="45385-108">Attributes</span></span>

<span data-ttu-id="45385-109">なし。</span><span class="sxs-lookup"><span data-stu-id="45385-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="45385-110">子要素</span><span class="sxs-lookup"><span data-stu-id="45385-110">Child elements</span></span>

|<span data-ttu-id="45385-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="45385-111">**Element**</span></span>|<span data-ttu-id="45385-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="45385-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45385-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="45385-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="45385-114">Base64Binary の形式で表されるオブジェクトのネイティブの MIME ストリームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="45385-114">Contains the native MIME stream of an object represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="45385-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="45385-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="45385-116">Exchange ストア内の配布リスト アイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="45385-116">Contains the unique identifier and change key of a distribution list item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="45385-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="45385-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="45385-118">配布リスト アイテムを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="45385-118">Represents the identifier of the parent folder that contains the distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="45385-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="45385-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="45385-120">配布リストのアイテムのメッセージ クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="45385-120">Represents the message class of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="45385-121">Subject</span><span class="sxs-lookup"><span data-stu-id="45385-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="45385-122">Exchange ストアのアイテムおよび応答オブジェクトのサブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="45385-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="45385-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="45385-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="45385-124">配布リスト アイテムの秘密度の状態が含まれています。</span><span class="sxs-lookup"><span data-stu-id="45385-124">Contains the status for a distribution list item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="45385-125">Body/本文</span><span class="sxs-lookup"><span data-stu-id="45385-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="45385-126">配布リスト アイテムの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="45385-126">Represents the actual body content of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="45385-127">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="45385-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="45385-128">アイテムまたは Exchange ストア内の配布リスト アイテムに関連付けられているファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="45385-128">Contains the items or files that are attached to a distribution list item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="45385-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="45385-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="45385-130">メールボックス内の配布リストのアイテムを受信したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="45385-130">Represents the date and time that a distribution list item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="45385-131">Size</span><span class="sxs-lookup"><span data-stu-id="45385-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="45385-132">配布リストのアイテムのバイト単位でサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="45385-132">Represents the size, in bytes, of a distribution list item.</span></span> <span data-ttu-id="45385-133">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="45385-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="45385-134">Categories</span><span class="sxs-lookup"><span data-stu-id="45385-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="45385-135">メールボックス内の配布リストのアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="45385-135">Represents a collection of strings that identify to which categories a distribution list item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="45385-136">Importance</span><span class="sxs-lookup"><span data-stu-id="45385-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="45385-137">配布リストのアイテムの重要性をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="45385-137">Describes the importance of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="45385-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="45385-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="45385-139">このアイテムの返信であるアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="45385-139">Represents the identifier of the item which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="45385-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="45385-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="45385-141">アイテムが [送信トレイ] 既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="45385-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="45385-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="45385-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="45385-143">アイテムはまだ送信されていないかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="45385-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="45385-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="45385-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="45385-145">ユーザーが自身にアイテムを送信するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="45385-145">Indicates whether a user sent an item to itself.</span></span>  <br/> |
|[<span data-ttu-id="45385-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="45385-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="45385-147">アイテムが以前送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="45385-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="45385-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="45385-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="45385-149">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="45385-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="45385-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="45385-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="45385-151">メールボックス内のアイテムに含まれているすべてのインターネット メッセージ ヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="45385-151">Represents the collection of all Internet message headers contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="45385-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="45385-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="45385-153">メールボックス内のアイテムが送信された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="45385-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="45385-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="45385-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="45385-155">メールボックス内の特定のアイテムが作成された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="45385-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="45385-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="45385-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="45385-157">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="45385-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="45385-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="45385-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="45385-159">イベントが発生したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="45385-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="45385-160">[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によってアラームが表示されたときを決定する使用されます。</span><span class="sxs-lookup"><span data-stu-id="45385-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="45385-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="45385-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="45385-162">Exchange ストアのアイテムのアラームが設定されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="45385-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="45385-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="45385-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="45385-164">分前にアラームが表示されるときに、イベントの数を表します。</span><span class="sxs-lookup"><span data-stu-id="45385-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="45385-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="45385-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="45385-166">[Cc] 行の内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="45385-166">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="45385-167">これは、すべての Cc 受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="45385-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="45385-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="45385-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="45385-169">行の内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="45385-169">Represents the display string that is used for the contents of the To line.</span></span> <span data-ttu-id="45385-170">これは、すべての受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="45385-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="45385-171">添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="45385-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="45385-172">アイテムに表示されている 1 つ以上の添付ファイルがある場合に**true**に設定されているプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="45385-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="45385-173">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="45385-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="45385-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="45385-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="45385-175">配布リスト アイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="45385-175">Identifies extended properties on a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="45385-176">カルチャ</span><span class="sxs-lookup"><span data-stu-id="45385-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="45385-177">メールボックス内の配布リスト アイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="45385-177">Represents the culture for a distribution list item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="45385-178">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="45385-178">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="45385-179">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="45385-179">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="45385-180">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="45385-180">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="45385-181">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="45385-181">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="45385-182">最後の項目を変更するのにはユーザーの表示名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="45385-182">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="45385-183">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="45385-183">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="45385-184">アイテムが最後に修正された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="45385-184">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="45385-185">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="45385-185">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="45385-186">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="45385-186">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="45385-187">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="45385-187">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="45385-188">Outlook Web App 内の項目を参照するのには Microsoft Office Outlook の Web アプリケーションのエンドポイントを結合するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="45385-188">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="45385-189">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="45385-189">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="45385-190">Outlook Web App 内の項目を編集するのには Outlook Web App エンドポイントへの連結に URL を表します。</span><span class="sxs-lookup"><span data-stu-id="45385-190">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="45385-191">ConversationId</span><span class="sxs-lookup"><span data-stu-id="45385-191">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="45385-192">アイテムや会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="45385-192">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="45385-193">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="45385-193">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="45385-194">このスレッドの一意の本文を表すテキストまたは HTML フラグメントを表します。</span><span class="sxs-lookup"><span data-stu-id="45385-194">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="45385-195">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="45385-195">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="45385-196">配布リストの表示名を定義します。</span><span class="sxs-lookup"><span data-stu-id="45385-196">Defines the display name of a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="45385-197">表題</span><span class="sxs-lookup"><span data-stu-id="45385-197">FileAs</span></span>](fileas.md) <br/> |<span data-ttu-id="45385-198">配布リストを連絡先フォルダーにファイリングする方法を表します。</span><span class="sxs-lookup"><span data-stu-id="45385-198">Represents how a distribution list is filed in the Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="45385-199">ContactSource</span><span class="sxs-lookup"><span data-stu-id="45385-199">ContactSource</span></span>](contactsource.md) <br/> |<span data-ttu-id="45385-200">Exchange ストアまたは Active Directory ドメイン サービス (AD DS) の連絡先があるかどうかについて説明します。</span><span class="sxs-lookup"><span data-stu-id="45385-200">Describes whether the contact is located in the Exchange store or in Active Directory Domain Services (AD DS).</span></span>  <br/> |
|[<span data-ttu-id="45385-201">メンバー (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="45385-201">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="45385-202">配布リストのメンバーの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="45385-202">Contains a list of members of the distribution list.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="45385-203">親要素</span><span class="sxs-lookup"><span data-stu-id="45385-203">Parent elements</span></span>

|<span data-ttu-id="45385-204">**要素**</span><span class="sxs-lookup"><span data-stu-id="45385-204">**Element**</span></span>|<span data-ttu-id="45385-205">**説明**</span><span class="sxs-lookup"><span data-stu-id="45385-205">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45385-206">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="45385-206">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="45385-207">会議の時刻に隣接しているすべての予定表のアイテムについて説明します。</span><span class="sxs-lookup"><span data-stu-id="45385-207">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="45385-208">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="45385-208">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="45385-209">[UpdateItem 操作](updateitem-operation.md)中に 1 つの配布リストのプロパティを追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="45385-209">Identifies data to append to a single property of a distribution list during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="45385-210">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="45385-210">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="45385-211">会議の時間と競合するすべての項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="45385-211">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="45385-212">(ItemSync) を作成します。</span><span class="sxs-lookup"><span data-stu-id="45385-212">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="45385-213">ローカル クライアント ストアに作成する 1 つの配布リストを識別します。</span><span class="sxs-lookup"><span data-stu-id="45385-213">Identifies a single distribution list to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="45385-214">更新プログラム (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="45385-214">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="45385-215">ローカル クライアント ストアで更新するための 1 つの配布リストを識別します。</span><span class="sxs-lookup"><span data-stu-id="45385-215">Identifies a single distribution list to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="45385-216">Items</span><span class="sxs-lookup"><span data-stu-id="45385-216">Items</span></span>](items.md) <br/> |<span data-ttu-id="45385-217">項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="45385-217">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="45385-218">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="45385-218">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="45385-219">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で指定されたフォルダーに作成する項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="45385-219">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="45385-220">SetItemField</span><span class="sxs-lookup"><span data-stu-id="45385-220">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="45385-221">[UpdateItem 操作](updateitem-operation.md)では、配布リストのアイテムの 1 つのプロパティには、更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="45385-221">Represents an update to a single property of a distribution list item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="45385-222">テキスト値</span><span class="sxs-lookup"><span data-stu-id="45385-222">Text value</span></span>

<span data-ttu-id="45385-223">なし。</span><span class="sxs-lookup"><span data-stu-id="45385-223">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="45385-224">備考</span><span class="sxs-lookup"><span data-stu-id="45385-224">Remarks</span></span>

<span data-ttu-id="45385-225">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="45385-225">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="45385-226">要素情報</span><span class="sxs-lookup"><span data-stu-id="45385-226">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="45385-227">名前空間</span><span class="sxs-lookup"><span data-stu-id="45385-227">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="45385-228">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="45385-228">Schema Name</span></span>  <br/> |<span data-ttu-id="45385-229">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="45385-229">Types schema</span></span>  <br/> |
|<span data-ttu-id="45385-230">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="45385-230">Validation File</span></span>  <br/> |<span data-ttu-id="45385-231">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="45385-231">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="45385-232">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="45385-232">Can be Empty</span></span>  <br/> |<span data-ttu-id="45385-233">False</span><span class="sxs-lookup"><span data-stu-id="45385-233">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="45385-234">関連項目</span><span class="sxs-lookup"><span data-stu-id="45385-234">See also</span></span>

- [<span data-ttu-id="45385-235">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="45385-235">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


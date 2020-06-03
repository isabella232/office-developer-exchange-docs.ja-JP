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
ms.openlocfilehash: 5eb97bef349ca02848f65fa58370b9c81c6653d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457005"
---
# <a name="distributionlist"></a><span data-ttu-id="adcca-103">DistributionList</span><span class="sxs-lookup"><span data-stu-id="adcca-103">DistributionList</span></span>

<span data-ttu-id="adcca-104">**DistributionList**要素は、配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-104">The **DistributionList** element represents a distribution list.</span></span> 
  
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

 <span data-ttu-id="adcca-105">**DistributionListType**</span><span class="sxs-lookup"><span data-stu-id="adcca-105">**DistributionListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="adcca-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="adcca-106">Attributes and elements</span></span>

<span data-ttu-id="adcca-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="adcca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="adcca-108">属性</span><span class="sxs-lookup"><span data-stu-id="adcca-108">Attributes</span></span>

<span data-ttu-id="adcca-109">なし。</span><span class="sxs-lookup"><span data-stu-id="adcca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="adcca-110">子要素</span><span class="sxs-lookup"><span data-stu-id="adcca-110">Child elements</span></span>

|<span data-ttu-id="adcca-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="adcca-111">**Element**</span></span>|<span data-ttu-id="adcca-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="adcca-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="adcca-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="adcca-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="adcca-114">Base64Binary 形式で表されるオブジェクトのネイティブ MIME ストリームが格納されています。</span><span class="sxs-lookup"><span data-stu-id="adcca-114">Contains the native MIME stream of an object represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="adcca-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="adcca-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="adcca-116">Exchange ストア内の配布リストアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="adcca-116">Contains the unique identifier and change key of a distribution list item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="adcca-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="adcca-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="adcca-118">配布リストアイテムを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-118">Represents the identifier of the parent folder that contains the distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="adcca-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="adcca-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="adcca-120">配布リストアイテムのメッセージクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-120">Represents the message class of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="adcca-121">件名</span><span class="sxs-lookup"><span data-stu-id="adcca-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="adcca-122">Exchange ストアアイテムおよび応答オブジェクトの件名を表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="adcca-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="adcca-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="adcca-124">配布リストアイテムの秘密度の状態を格納します。</span><span class="sxs-lookup"><span data-stu-id="adcca-124">Contains the status for a distribution list item's sensitivity.</span></span>  <br/> |
|[<span data-ttu-id="adcca-125">Body</span><span class="sxs-lookup"><span data-stu-id="adcca-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="adcca-126">配布リストアイテムの実際の本文のコンテンツを表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-126">Represents the actual body content of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="adcca-127">Attachments</span><span class="sxs-lookup"><span data-stu-id="adcca-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="adcca-128">Exchange ストア内の配布リストアイテムに添付されているアイテムまたはファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="adcca-128">Contains the items or files that are attached to a distribution list item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="adcca-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="adcca-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="adcca-130">メールボックス内の配布リストアイテムが受信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-130">Represents the date and time that a distribution list item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="adcca-131">Size</span><span class="sxs-lookup"><span data-stu-id="adcca-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="adcca-132">配布リストアイテムのサイズ (バイト単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-132">Represents the size, in bytes, of a distribution list item.</span></span> <span data-ttu-id="adcca-133">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="adcca-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="adcca-134">Categories</span><span class="sxs-lookup"><span data-stu-id="adcca-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="adcca-135">メールボックス内の配布リストアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-135">Represents a collection of strings that identify to which categories a distribution list item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="adcca-136">Importance</span><span class="sxs-lookup"><span data-stu-id="adcca-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="adcca-137">配布リストアイテムの重要度について説明します。</span><span class="sxs-lookup"><span data-stu-id="adcca-137">Describes the importance of a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="adcca-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="adcca-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="adcca-139">このアイテムが返信であるアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-139">Represents the identifier of the item which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="adcca-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="adcca-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="adcca-141">アイテムが送信トレイの既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="adcca-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="adcca-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="adcca-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="adcca-143">アイテムがまだ送信されていないかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="adcca-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="adcca-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="adcca-145">ユーザーがアイテムを自分自身に送信したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="adcca-145">Indicates whether a user sent an item to itself.</span></span>  <br/> |
|[<span data-ttu-id="adcca-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="adcca-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="adcca-147">アイテムが以前に送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="adcca-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="adcca-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="adcca-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="adcca-149">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="adcca-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="adcca-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="adcca-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="adcca-151">メールボックス内のアイテム内に含まれるすべてのインターネットメッセージヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-151">Represents the collection of all Internet message headers contained within an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="adcca-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="adcca-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="adcca-153">メールボックス内のアイテムが送信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="adcca-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="adcca-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="adcca-155">メールボックス内の特定のアイテムが作成された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="adcca-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="adcca-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="adcca-157">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="adcca-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="adcca-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="adcca-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="adcca-159">イベントが発生した日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="adcca-160">これは、アラームがいつ表示されるかを決定するために[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="adcca-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="adcca-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="adcca-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="adcca-162">Exchange ストア内のアイテムにアラームが設定されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="adcca-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="adcca-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="adcca-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="adcca-164">アラームが表示されるイベントの前の時間 (分単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="adcca-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="adcca-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="adcca-166">[Cc] 行の内容として使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-166">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="adcca-167">これは、すべての Cc 受信者表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="adcca-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="adcca-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="adcca-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="adcca-169">To 行の内容として使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-169">Represents the display string that is used for the contents of the To line.</span></span> <span data-ttu-id="adcca-170">これは、すべての受信者の表示名の連結文字列です。</span><span class="sxs-lookup"><span data-stu-id="adcca-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="adcca-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="adcca-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="adcca-172">アイテムに少なくとも1つの添付ファイルがある場合に**true**に設定されるプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="adcca-173">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="adcca-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="adcca-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="adcca-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="adcca-175">配布リストアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="adcca-175">Identifies extended properties on a distribution list item.</span></span>  <br/> |
|[<span data-ttu-id="adcca-176">Culture</span><span class="sxs-lookup"><span data-stu-id="adcca-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="adcca-177">メールボックス内の配布リストアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-177">Represents the culture for a distribution list item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="adcca-178">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="adcca-178">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="adcca-179">アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="adcca-179">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="adcca-180">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="adcca-180">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="adcca-181">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="adcca-181">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="adcca-182">アイテムを最後に変更したユーザーの表示名を含みます。</span><span class="sxs-lookup"><span data-stu-id="adcca-182">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="adcca-183">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="adcca-183">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="adcca-184">アイテムが最後に変更された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="adcca-184">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="adcca-185">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="adcca-185">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="adcca-186">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="adcca-186">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="adcca-187">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="adcca-187">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="adcca-188">Outlook Web app のアイテムを読み取るために Microsoft Office Outlook Web App エンドポイントに連結する URL を表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-188">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="adcca-189">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="adcca-189">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="adcca-190">Outlook web app エンドポイントに連結して Outlook Web App のアイテムを編集するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-190">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="adcca-191">ConversationId</span><span class="sxs-lookup"><span data-stu-id="adcca-191">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="adcca-192">アイテムまたは会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="adcca-192">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="adcca-193">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="adcca-193">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="adcca-194">この会話の一意の本文を表す HTML フラグメントまたはプレーンテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-194">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="adcca-195">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="adcca-195">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="adcca-196">配布リストの表示名を定義します。</span><span class="sxs-lookup"><span data-stu-id="adcca-196">Defines the display name of a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="adcca-197">FileAs</span><span class="sxs-lookup"><span data-stu-id="adcca-197">FileAs</span></span>](fileas.md) <br/> |<span data-ttu-id="adcca-198">配布リストが連絡先フォルダーでどのようにファイリングされるかを表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-198">Represents how a distribution list is filed in the Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="adcca-199">ContactSource</span><span class="sxs-lookup"><span data-stu-id="adcca-199">ContactSource</span></span>](contactsource.md) <br/> |<span data-ttu-id="adcca-200">連絡先が Exchange ストアまたは Active Directory ドメインサービス (AD DS) に存在するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="adcca-200">Describes whether the contact is located in the Exchange store or in Active Directory Domain Services (AD DS).</span></span>  <br/> |
|[<span data-ttu-id="adcca-201">Members (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="adcca-201">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="adcca-202">配布リストのメンバーの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="adcca-202">Contains a list of members of the distribution list.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="adcca-203">親要素</span><span class="sxs-lookup"><span data-stu-id="adcca-203">Parent elements</span></span>

|<span data-ttu-id="adcca-204">**要素**</span><span class="sxs-lookup"><span data-stu-id="adcca-204">**Element**</span></span>|<span data-ttu-id="adcca-205">**説明**</span><span class="sxs-lookup"><span data-stu-id="adcca-205">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="adcca-206">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="adcca-206">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="adcca-207">会議の時刻に隣接しているすべての予定表アイテムを説明します。</span><span class="sxs-lookup"><span data-stu-id="adcca-207">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="adcca-208">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="adcca-208">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="adcca-209">[Updateitem 操作](updateitem-operation.md)中に、配布リストの1つのプロパティに追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="adcca-209">Identifies data to append to a single property of a distribution list during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="adcca-210">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="adcca-210">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="adcca-211">会議の時間と競合するすべてのアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="adcca-211">Identifies all items that conflict with a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="adcca-212">Create (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="adcca-212">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="adcca-213">ローカルクライアントストアに作成する1つの配布リストを識別します。</span><span class="sxs-lookup"><span data-stu-id="adcca-213">Identifies a single distribution list to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="adcca-214">Update (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="adcca-214">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="adcca-215">ローカルクライアントストアで更新する1つの配布リストを識別します。</span><span class="sxs-lookup"><span data-stu-id="adcca-215">Identifies a single distribution list to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="adcca-216">Items</span><span class="sxs-lookup"><span data-stu-id="adcca-216">Items</span></span>](items.md) <br/> |<span data-ttu-id="adcca-217">項目の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="adcca-217">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="adcca-218">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="adcca-218">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="adcca-219">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="adcca-219">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="adcca-220">SetItemField</span><span class="sxs-lookup"><span data-stu-id="adcca-220">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="adcca-221">[Updateitem 操作](updateitem-operation.md)の配布リストアイテムの1つのプロパティに対する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="adcca-221">Represents an update to a single property of a distribution list item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="adcca-222">テキスト値</span><span class="sxs-lookup"><span data-stu-id="adcca-222">Text value</span></span>

<span data-ttu-id="adcca-223">なし。</span><span class="sxs-lookup"><span data-stu-id="adcca-223">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="adcca-224">注釈</span><span class="sxs-lookup"><span data-stu-id="adcca-224">Remarks</span></span>

<span data-ttu-id="adcca-225">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="adcca-225">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="adcca-226">要素の情報</span><span class="sxs-lookup"><span data-stu-id="adcca-226">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="adcca-227">Namespace</span><span class="sxs-lookup"><span data-stu-id="adcca-227">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="adcca-228">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="adcca-228">Schema Name</span></span>  <br/> |<span data-ttu-id="adcca-229">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="adcca-229">Types schema</span></span>  <br/> |
|<span data-ttu-id="adcca-230">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="adcca-230">Validation File</span></span>  <br/> |<span data-ttu-id="adcca-231">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="adcca-231">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="adcca-232">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="adcca-232">Can be Empty</span></span>  <br/> |<span data-ttu-id="adcca-233">正しくない</span><span class="sxs-lookup"><span data-stu-id="adcca-233">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="adcca-234">関連項目</span><span class="sxs-lookup"><span data-stu-id="adcca-234">See also</span></span>

- [<span data-ttu-id="adcca-235">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="adcca-235">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


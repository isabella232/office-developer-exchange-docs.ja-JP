---
title: Contact
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contact
api_type:
- schema
ms.assetid: 66bfff50-7a91-4d81-b6a0-610b9962f677
description: Contact 要素は、Exchange ストア内の連絡先アイテムを表します。
ms.openlocfilehash: b5b4af211815dbbd09449ca2f3c6b6b2dfba6f93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44445651"
---
# <a name="contact"></a><span data-ttu-id="c0385-103">Contact</span><span class="sxs-lookup"><span data-stu-id="c0385-103">Contact</span></span>

<span data-ttu-id="c0385-104">**Contact**要素は、Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-104">The **Contact** element represents a contact item in the Exchange store.</span></span> 
  
```XML
<Contact>
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
   <FileAs/>
   <FileAsMapping/>
   <DisplayName/>
   <GivenName/>
   <Initials/>
   <MiddleName/>
   <Nickname/>
   <CompleteName/>
   <CompanyName/>
   <EmailAddresses/>
   <PhysicalAddresses/>
   <PhoneNumbers/>
   <AssistantName/>
   <Birthday/>
   <BusinessHomePage/>
   <Children/>
   <Companies/>
   <ContactSource/>
   <Department/>
   <Generation/>
   <ImAddresses/>
   <JobTitle/>
   <Manager/>
   <Mileage/>
   <OfficeLocation/>
   <PostalAddressIndex/>
   <Profession/>
   <SpouseName/>
   <Surname/>
   <WeddingAnniversary/>
   <HasPicture/>
   <PhoneticFullName/>
   <PhoneticFirstName/>
   <PhoneticLastName/>
   <Alias/>
   <Notes/>
   <Photo/>
   <UserSMIMECertificate/>
   <MSExchangeCertificate/>
   <DirectoryId/>
   <ManagerMailbox/>
   <DirectReports/>
</Contact>
```

 <span data-ttu-id="c0385-105">**ContactItemType**</span><span class="sxs-lookup"><span data-stu-id="c0385-105">**ContactItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c0385-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c0385-106">Attributes and elements</span></span>

<span data-ttu-id="c0385-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c0385-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0385-108">属性</span><span class="sxs-lookup"><span data-stu-id="c0385-108">Attributes</span></span>

<span data-ttu-id="c0385-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c0385-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c0385-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c0385-110">Child elements</span></span>

|<span data-ttu-id="c0385-111">**要素名**</span><span class="sxs-lookup"><span data-stu-id="c0385-111">**Element name**</span></span>|<span data-ttu-id="c0385-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="c0385-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0385-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="c0385-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="c0385-114">Base64Binary 形式で表されるオブジェクトのネイティブな汎用インターネットメール内線 (MIME) ストリームが保存されています。</span><span class="sxs-lookup"><span data-stu-id="c0385-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="c0385-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="c0385-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="c0385-116">Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0385-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c0385-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="c0385-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="c0385-118">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-118">Represents the identifier of the parent folder that contains the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="c0385-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="c0385-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="c0385-120">アイテムのメッセージクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-120">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="c0385-121">件名</span><span class="sxs-lookup"><span data-stu-id="c0385-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="c0385-122">Exchange ストアアイテムおよび応答オブジェクトの件名を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="c0385-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="c0385-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="c0385-124">アイテムの秘密度レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="c0385-124">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="c0385-125">Body</span><span class="sxs-lookup"><span data-stu-id="c0385-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="c0385-126">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-126">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="c0385-127">Attachments</span><span class="sxs-lookup"><span data-stu-id="c0385-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c0385-128">Exchange ストア内のアイテムに添付されているアイテムまたはファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="c0385-128">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c0385-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="c0385-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="c0385-130">メールボックス内のアイテムが受信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-130">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="c0385-131">Size</span><span class="sxs-lookup"><span data-stu-id="c0385-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="c0385-132">アイテムのサイズ (バイト単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-132">Represents the size in bytes of an item.</span></span> <span data-ttu-id="c0385-133">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="c0385-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="c0385-134">Categories</span><span class="sxs-lookup"><span data-stu-id="c0385-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c0385-135">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-135">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="c0385-136">Importance</span><span class="sxs-lookup"><span data-stu-id="c0385-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="c0385-137">アイテムの重要度について説明します。</span><span class="sxs-lookup"><span data-stu-id="c0385-137">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="c0385-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="c0385-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="c0385-139">このアイテムが返信であるアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-139">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="c0385-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="c0385-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="c0385-141">アイテムが送信トレイの既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c0385-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="c0385-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="c0385-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="c0385-143">アイテムがまだ送信されていないかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="c0385-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="c0385-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="c0385-145">ユーザーが自分にアイテムを送信したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c0385-145">Indicates whether a user sent an item to himself or herself.</span></span>  <br/> |
|[<span data-ttu-id="c0385-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="c0385-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="c0385-147">アイテムが以前に送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c0385-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="c0385-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="c0385-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="c0385-149">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c0385-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="c0385-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="c0385-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="c0385-151">メールボックス内のアイテムに含まれるすべてのインターネットメッセージヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-151">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c0385-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="c0385-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="c0385-153">メールボックス内のアイテムが送信された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="c0385-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="c0385-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="c0385-155">メールボックス内の特定のアイテムが作成された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="c0385-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="c0385-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="c0385-157">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="c0385-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c0385-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="c0385-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="c0385-159">イベントが発生した日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="c0385-160">これは、アラームがいつ表示されるかを決定するために[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="c0385-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="c0385-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="c0385-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="c0385-162">Exchange ストア内のアイテムにアラームが設定されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c0385-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c0385-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="c0385-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="c0385-164">アラームが表示されるイベントの前の時間 (分単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="c0385-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="c0385-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="c0385-166">[Cc] 行の内容として使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-166">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="c0385-167">これは、すべての Cc 受信者表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="c0385-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="c0385-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="c0385-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="c0385-169">To 行の内容として使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-169">Represents the display string that is used for the contents of the To line.</span></span> <span data-ttu-id="c0385-170">これは、すべての受信者の表示名の連結文字列です。</span><span class="sxs-lookup"><span data-stu-id="c0385-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="c0385-171">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="c0385-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="c0385-172">アイテムに少なくとも1つの添付ファイルがある場合に**true**に設定されるプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="c0385-173">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="c0385-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="c0385-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="c0385-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="c0385-175">フォルダーとアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="c0385-175">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="c0385-176">Culture</span><span class="sxs-lookup"><span data-stu-id="c0385-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="c0385-177">メールボックス内の特定のアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-177">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c0385-178">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="c0385-178">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="c0385-179">アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0385-179">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="c0385-180">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="c0385-180">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="c0385-181">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="c0385-181">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="c0385-182">アイテムを最後に変更したユーザーの表示名を含みます。</span><span class="sxs-lookup"><span data-stu-id="c0385-182">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="c0385-183">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="c0385-183">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="c0385-184">アイテムが最後に変更された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="c0385-184">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="c0385-185">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="c0385-185">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="c0385-186">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c0385-186">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="c0385-187">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="c0385-187">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="c0385-188">Outlook Web app のアイテムを読み取るために Microsoft Office Outlook Web App エンドポイントに連結する URL を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-188">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="c0385-189">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="c0385-189">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="c0385-190">Outlook web app エンドポイントに連結して Outlook Web App のアイテムを編集するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-190">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="c0385-191">ConversationId</span><span class="sxs-lookup"><span data-stu-id="c0385-191">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="c0385-192">アイテムまたは会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0385-192">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="c0385-193">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="c0385-193">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="c0385-194">この会話の一意の本文を表す HTML フラグメントまたはプレーンテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-194">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="c0385-195">FileAs</span><span class="sxs-lookup"><span data-stu-id="c0385-195">FileAs</span></span>](fileas.md) <br/> |<span data-ttu-id="c0385-196">連絡先フォルダーに連絡先をファイリングする方法を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-196">Represents how a contact is filed in the Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="c0385-197">FileAsMapping</span><span class="sxs-lookup"><span data-stu-id="c0385-197">FileAsMapping</span></span>](fileasmapping.md) <br/> |<span data-ttu-id="c0385-198">連絡先に対して表示される内容を作成する方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="c0385-198">Defines how to construct what is displayed for a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-199">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="c0385-199">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="c0385-200">連絡先の表示名を定義します。</span><span class="sxs-lookup"><span data-stu-id="c0385-200">Defines the display name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-201">GivenName</span><span class="sxs-lookup"><span data-stu-id="c0385-201">GivenName</span></span>](givenname.md) <br/> |<span data-ttu-id="c0385-202">連絡先の特定の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0385-202">Contains a contact's given name.</span></span>  <br/> |
|<span data-ttu-id="c0385-203">[[頭文字](initials.md)]</span><span class="sxs-lookup"><span data-stu-id="c0385-203">[Initials](initials.md)</span></span> <br/> |<span data-ttu-id="c0385-204">連絡先のイニシャルを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-204">Represents the initials of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-205">MiddleName</span><span class="sxs-lookup"><span data-stu-id="c0385-205">MiddleName</span></span>](middlename.md) <br/> |<span data-ttu-id="c0385-206">連絡先のミドルネームを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-206">Represents the middle name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-207">ニックネーム</span><span class="sxs-lookup"><span data-stu-id="c0385-207">Nickname</span></span>](nickname.md) <br/> |<span data-ttu-id="c0385-208">連絡先のニックネームを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-208">Represents the nickname of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-209">CompleteName</span><span class="sxs-lookup"><span data-stu-id="c0385-209">CompleteName</span></span>](completename.md) <br/> |<span data-ttu-id="c0385-210">連絡先の完全な名前を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-210">Represents the complete name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-211">CompanyName</span><span class="sxs-lookup"><span data-stu-id="c0385-211">CompanyName</span></span>](companyname.md) <br/> |<span data-ttu-id="c0385-212">連絡先に関連付けられている会社名を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-212">Represents the company name that is associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-213">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="c0385-213">EmailAddresses</span></span>](emailaddresses.md) <br/> |<span data-ttu-id="c0385-214">連絡先の電子メールアドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-214">Represents a collection of e-mail addresses for a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-215">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="c0385-215">PhysicalAddresses</span></span>](physicaladdresses.md) <br/> |<span data-ttu-id="c0385-216">連絡先に関連付けられている物理的な住所のコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="c0385-216">Contains a collection of physical addresses that are associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-217">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="c0385-217">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="c0385-218">連絡先の電話番号のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-218">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-219">AssistantName</span><span class="sxs-lookup"><span data-stu-id="c0385-219">AssistantName</span></span>](assistantname.md) <br/> |<span data-ttu-id="c0385-220">連絡先のアシスタントを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-220">Represents an assistant to a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-221">Birthday</span><span class="sxs-lookup"><span data-stu-id="c0385-221">Birthday</span></span>](birthday.md) <br/> |<span data-ttu-id="c0385-222">連絡先の生年月日を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-222">Represents the birth date of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-223">BusinessHomePage</span><span class="sxs-lookup"><span data-stu-id="c0385-223">BusinessHomePage</span></span>](businesshomepage.md) <br/> |<span data-ttu-id="c0385-224">連絡先のホームページ (Web アドレス) を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-224">Represents the Home page (Web address) for the contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-225">Children</span><span class="sxs-lookup"><span data-stu-id="c0385-225">Children</span></span>](children.md) <br/> |<span data-ttu-id="c0385-226">連絡先の子の名前を格納します。</span><span class="sxs-lookup"><span data-stu-id="c0385-226">Contains the names of a contact's children.</span></span>  <br/> |
|[<span data-ttu-id="c0385-227">Companies</span><span class="sxs-lookup"><span data-stu-id="c0385-227">Companies</span></span>](companies.md) <br/> |<span data-ttu-id="c0385-228">連絡先に関連付けられている会社のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-228">Represents the collection of companies that are associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-229">ContactSource</span><span class="sxs-lookup"><span data-stu-id="c0385-229">ContactSource</span></span>](contactsource.md) <br/> |<span data-ttu-id="c0385-230">連絡先が Exchange ストアまたは Active Directory ディレクトリサービスに存在するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c0385-230">Describes whether the contact is located in the Exchange store or the Active Directory directory service.</span></span>  <br/> |
|[<span data-ttu-id="c0385-231">Department</span><span class="sxs-lookup"><span data-stu-id="c0385-231">Department</span></span>](department.md) <br/> |<span data-ttu-id="c0385-232">作業中の連絡先の部署を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-232">Represents the contact's department at work.</span></span>  <br/> |
|[<span data-ttu-id="c0385-233">ジェネレーター</span><span class="sxs-lookup"><span data-stu-id="c0385-233">Generation</span></span>](generation.md) <br/> |<span data-ttu-id="c0385-234">連絡先の氏名の後の省略形を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-234">Represents a generational abbreviation that follows the full name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-235">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="c0385-235">ImAddresses</span></span>](imaddresses.md) <br/> |<span data-ttu-id="c0385-236">連絡先のインスタントメッセージアドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-236">Represents a collection of instant messaging addresses for a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-237">JobTitle</span><span class="sxs-lookup"><span data-stu-id="c0385-237">JobTitle</span></span>](jobtitle.md) <br/> |<span data-ttu-id="c0385-238">連絡先の役職を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-238">Represents the job title of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-239">Manager</span><span class="sxs-lookup"><span data-stu-id="c0385-239">Manager</span></span>](manager.md) <br/> |<span data-ttu-id="c0385-240">連絡先の上司を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-240">Represents a contact's manager.</span></span>  <br/> |
|[<span data-ttu-id="c0385-241">Mileage</span><span class="sxs-lookup"><span data-stu-id="c0385-241">Mileage</span></span>](mileage.md) <br/> |<span data-ttu-id="c0385-242">連絡先アイテムのマイレージを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-242">Represents mileage for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="c0385-243">OfficeLocation</span><span class="sxs-lookup"><span data-stu-id="c0385-243">OfficeLocation</span></span>](officelocation.md) <br/> |<span data-ttu-id="c0385-244">連絡先の勤務先の場所を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-244">Represents the office location of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-245">PostalAddressIndex</span><span class="sxs-lookup"><span data-stu-id="c0385-245">PostalAddressIndex</span></span>](postaladdressindex.md) <br/> |<span data-ttu-id="c0385-246">物理アドレスの表示の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-246">Represents the display types for physical addresses.</span></span>  <br/> |
|[<span data-ttu-id="c0385-247">Profession</span><span class="sxs-lookup"><span data-stu-id="c0385-247">Profession</span></span>](profession.md) <br/> |<span data-ttu-id="c0385-248">連絡先の職業を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-248">Represents the profession of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-249">SpouseName</span><span class="sxs-lookup"><span data-stu-id="c0385-249">SpouseName</span></span>](spousename.md) <br/> |<span data-ttu-id="c0385-250">連絡先の配偶者またはパートナーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-250">Represents the name of a contact's spouse/partner.</span></span>  <br/> |
|[<span data-ttu-id="c0385-251">姓</span><span class="sxs-lookup"><span data-stu-id="c0385-251">Surname</span></span>](surname.md) <br/> |<span data-ttu-id="c0385-252">連絡先の姓を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-252">Represents the surname of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-253">WeddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="c0385-253">WeddingAnniversary</span></span>](weddinganniversary.md) <br/> |<span data-ttu-id="c0385-254">連絡先の結婚記念日を含みます。</span><span class="sxs-lookup"><span data-stu-id="c0385-254">Contains the wedding anniversary of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-255">HasPicture</span><span class="sxs-lookup"><span data-stu-id="c0385-255">HasPicture</span></span>](haspicture.md) <br/> |<span data-ttu-id="c0385-256">連絡先アイテムに、連絡先の写真を表す添付ファイルがあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c0385-256">Indicates whether the contact item has a file attachment that represents the contact's picture.</span></span>  <br/> |
|[<span data-ttu-id="c0385-257">PhoneticFullName</span><span class="sxs-lookup"><span data-stu-id="c0385-257">PhoneticFullName</span></span>](phoneticfullname.md) <br/> |<span data-ttu-id="c0385-258">連絡先の氏名を含み、姓と名のスペルを入力します。</span><span class="sxs-lookup"><span data-stu-id="c0385-258">Contains the full name of a contact, including the first and last name, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="c0385-259">PhoneticFirstName</span><span class="sxs-lookup"><span data-stu-id="c0385-259">PhoneticFirstName</span></span>](phoneticfirstname.md) <br/> |<span data-ttu-id="c0385-260">連絡先の名の先頭にスペルを入力します。</span><span class="sxs-lookup"><span data-stu-id="c0385-260">Contains the first name of a contact, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="c0385-261">PhoneticLastName</span><span class="sxs-lookup"><span data-stu-id="c0385-261">PhoneticLastName</span></span>](phoneticlastname.md) <br/> |<span data-ttu-id="c0385-262">連絡先の姓が入力されています。</span><span class="sxs-lookup"><span data-stu-id="c0385-262">Contains the last name of a contact, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="c0385-263">Alias</span><span class="sxs-lookup"><span data-stu-id="c0385-263">Alias</span></span>](alias.md) <br/> |<span data-ttu-id="c0385-264">連絡先の電子メールエイリアスが保存されています。</span><span class="sxs-lookup"><span data-stu-id="c0385-264">Contains the email alias of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-265">メモ (連絡先)</span><span class="sxs-lookup"><span data-stu-id="c0385-265">Notes (Contact)</span></span>](notes-contact.md) <br/> |<span data-ttu-id="c0385-266">補足連絡先情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0385-266">Contains supplementary contact information.</span></span>  <br/> |
|[<span data-ttu-id="c0385-267">写真</span><span class="sxs-lookup"><span data-stu-id="c0385-267">Photo</span></span>](photo.md) <br/> |<span data-ttu-id="c0385-268">連絡先の写真をエンコードする値を格納します。</span><span class="sxs-lookup"><span data-stu-id="c0385-268">Contains a value that encodes the photo of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-269">UserSMIMECertificate</span><span class="sxs-lookup"><span data-stu-id="c0385-269">UserSMIMECertificate</span></span>](usersmimecertificate.md) <br/> |<span data-ttu-id="c0385-270">連絡先の SMIME 証明書をエンコードする値を格納します。</span><span class="sxs-lookup"><span data-stu-id="c0385-270">Contains a value that encodes the SMIME certificate of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-271">MSExchangeCertificate</span><span class="sxs-lookup"><span data-stu-id="c0385-271">MSExchangeCertificate</span></span>](msexchangecertificate.md) <br/> |<span data-ttu-id="c0385-272">連絡先の Microsoft Exchange 証明書をエンコードする値を格納します。</span><span class="sxs-lookup"><span data-stu-id="c0385-272">Contains a value that encodes the Microsoft Exchange certificate of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-273">DirectoryId</span><span class="sxs-lookup"><span data-stu-id="c0385-273">DirectoryId</span></span>](directoryid.md) <br/> |<span data-ttu-id="c0385-274">連絡先のディレクトリ ID を格納します。</span><span class="sxs-lookup"><span data-stu-id="c0385-274">Contains the directory ID of a contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-275">ManagerMailbox</span><span class="sxs-lookup"><span data-stu-id="c0385-275">ManagerMailbox</span></span>](managermailbox.md) <br/> |<span data-ttu-id="c0385-276">連絡先のマネージャーメールボックスを識別する SMTP 情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="c0385-276">Contains SMTP information that identifies the manager mailbox of the contact.</span></span>  <br/> |
|[<span data-ttu-id="c0385-277">DirectReports</span><span class="sxs-lookup"><span data-stu-id="c0385-277">DirectReports</span></span>](directreports.md) <br/> |<span data-ttu-id="c0385-278">連絡先の直属の部下を識別する SMTP 情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="c0385-278">Contains SMTP information that identifies the direct reports of a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c0385-279">親要素</span><span class="sxs-lookup"><span data-stu-id="c0385-279">Parent elements</span></span>

|<span data-ttu-id="c0385-280">**要素名**</span><span class="sxs-lookup"><span data-stu-id="c0385-280">**Element name**</span></span>|<span data-ttu-id="c0385-281">**説明**</span><span class="sxs-lookup"><span data-stu-id="c0385-281">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0385-282">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="c0385-282">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="c0385-283">会議の時刻に隣接しているすべての予定表アイテムを説明します。</span><span class="sxs-lookup"><span data-stu-id="c0385-283">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="c0385-284">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="c0385-284">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="c0385-285">[Updateitem 操作](updateitem-operation.md)中に、アイテムまたはフォルダーの1つのプロパティに追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="c0385-285">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="c0385-286">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="c0385-286">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="c0385-287">会議の時間と競合するすべてのアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="c0385-287">Identifies all items that conflict with a meeting time</span></span>  <br/> |
|[<span data-ttu-id="c0385-288">Create (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="c0385-288">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="c0385-289">ローカルクライアントストアに作成する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="c0385-289">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="c0385-290">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="c0385-290">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="c0385-291">別の Exchange アイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-291">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="c0385-292">Items</span><span class="sxs-lookup"><span data-stu-id="c0385-292">Items</span></span>](items.md) <br/> |<span data-ttu-id="c0385-293">項目の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="c0385-293">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="c0385-294">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="c0385-294">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="c0385-295">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0385-295">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="c0385-296">Resolution</span><span class="sxs-lookup"><span data-stu-id="c0385-296">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="c0385-297">1つの解決済みエンティティを含みます。</span><span class="sxs-lookup"><span data-stu-id="c0385-297">Contains a single resolved entity.</span></span>  <br/> |
|[<span data-ttu-id="c0385-298">SetItemField</span><span class="sxs-lookup"><span data-stu-id="c0385-298">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="c0385-299">[Updateitem 操作](updateitem-operation.md)のアイテムの1つのプロパティに対する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="c0385-299">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="c0385-300">Update (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="c0385-300">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="c0385-301">ローカルクライアントストアで更新する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="c0385-301">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c0385-302">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c0385-302">Text value</span></span>

<span data-ttu-id="c0385-303">なし。</span><span class="sxs-lookup"><span data-stu-id="c0385-303">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c0385-304">注釈</span><span class="sxs-lookup"><span data-stu-id="c0385-304">Remarks</span></span>

<span data-ttu-id="c0385-305">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c0385-305">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0385-306">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c0385-306">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0385-307">Namespace</span><span class="sxs-lookup"><span data-stu-id="c0385-307">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c0385-308">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c0385-308">Schema name</span></span>  <br/> |<span data-ttu-id="c0385-309">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c0385-309">Types schema</span></span>  <br/> |
|<span data-ttu-id="c0385-310">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c0385-310">Validation file</span></span>  <br/> |<span data-ttu-id="c0385-311">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c0385-311">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c0385-312">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c0385-312">Can be empty</span></span>  <br/> |<span data-ttu-id="c0385-313">正しくない</span><span class="sxs-lookup"><span data-stu-id="c0385-313">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c0385-314">関連項目</span><span class="sxs-lookup"><span data-stu-id="c0385-314">See also</span></span>



- [<span data-ttu-id="c0385-315">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c0385-315">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="c0385-316">連絡先の作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="c0385-316">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="c0385-317">連絡先の更新</span><span class="sxs-lookup"><span data-stu-id="c0385-317">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="c0385-318">連絡先の削除</span><span class="sxs-lookup"><span data-stu-id="c0385-318">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)


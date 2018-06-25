---
title: 連絡先
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
description: 連絡先の要素は、Exchange ストア内の連絡先アイテムを表します。
ms.openlocfilehash: 7b2e7c0197914c2a0a0ba3815dd05fca52a5f872
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759673"
---
# <a name="contact"></a><span data-ttu-id="a1e4a-103">連絡先</span><span class="sxs-lookup"><span data-stu-id="a1e4a-103">Contact</span></span>

<span data-ttu-id="a1e4a-104">**連絡**の要素は、Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-104">The **Contact** element represents a contact item in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="a1e4a-105">**ContactItemType**</span><span class="sxs-lookup"><span data-stu-id="a1e4a-105">**ContactItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a1e4a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a1e4a-106">Attributes and elements</span></span>

<span data-ttu-id="a1e4a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1e4a-108">属性</span><span class="sxs-lookup"><span data-stu-id="a1e4a-108">Attributes</span></span>

<span data-ttu-id="a1e4a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1e4a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a1e4a-110">Child elements</span></span>

|<span data-ttu-id="a1e4a-111">**要素名**</span><span class="sxs-lookup"><span data-stu-id="a1e4a-111">**Element name**</span></span>|<span data-ttu-id="a1e4a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a1e4a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1e4a-113">MimeContent</span><span class="sxs-lookup"><span data-stu-id="a1e4a-113">MimeContent</span></span>](mimecontent.md) <br/> |<span data-ttu-id="a1e4a-114">Base64Binary の形式で表されるオブジェクトのネイティブの多目的インターネット メール拡張 (MIME) ストリームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-114">Contains the native Multipurpose Internet Mail Extensions (MIME) stream of an object that is represented in base64Binary format.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="a1e4a-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="a1e4a-116">Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-117">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="a1e4a-117">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="a1e4a-118">アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-118">Represents the identifier of the parent folder that contains the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-119">ItemClass</span><span class="sxs-lookup"><span data-stu-id="a1e4a-119">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="a1e4a-120">アイテムのメッセージ クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-120">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-121">Subject</span><span class="sxs-lookup"><span data-stu-id="a1e4a-121">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="a1e4a-122">Exchange ストアのアイテムおよび応答オブジェクトのサブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-122">Represents the subject for Exchange store items and response objects.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-123">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="a1e4a-123">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="a1e4a-124">アイテムの秘密度レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-124">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-125">Body/本文</span><span class="sxs-lookup"><span data-stu-id="a1e4a-125">Body</span></span>](body.md) <br/> |<span data-ttu-id="a1e4a-126">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-126">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-127">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="a1e4a-127">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a1e4a-128">アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-128">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-129">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="a1e4a-129">DateTimeReceived</span></span>](datetimereceived.md) <br/> |<span data-ttu-id="a1e4a-130">メールボックス内のアイテムを受信したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-130">Represents the date and time that an item in a mailbox was received.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-131">Size</span><span class="sxs-lookup"><span data-stu-id="a1e4a-131">Size</span></span>](size.md) <br/> |<span data-ttu-id="a1e4a-132">アイテムのバイト単位のサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-132">Represents the size in bytes of an item.</span></span> <span data-ttu-id="a1e4a-133">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-133">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-134">Categories</span><span class="sxs-lookup"><span data-stu-id="a1e4a-134">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a1e4a-135">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-135">Represents a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-136">Importance</span><span class="sxs-lookup"><span data-stu-id="a1e4a-136">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="a1e4a-137">アイテムの重要性をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-137">Describes the importance of an item.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-138">InReplyTo</span><span class="sxs-lookup"><span data-stu-id="a1e4a-138">InReplyTo</span></span>](inreplyto.md) <br/> |<span data-ttu-id="a1e4a-139">このアイテムの返信するアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-139">Represents the identifier of the item to which this item is a reply.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-140">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="a1e4a-140">IsSubmitted</span></span>](issubmitted.md) <br/> |<span data-ttu-id="a1e4a-141">アイテムが [送信トレイ] 既定フォルダーに送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-141">Indicates whether an item has been submitted to the Outbox default folder.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-142">IsDraft</span><span class="sxs-lookup"><span data-stu-id="a1e4a-142">IsDraft</span></span>](isdraft.md) <br/> |<span data-ttu-id="a1e4a-143">アイテムはまだ送信されていないかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-143">Represents whether an item has not yet been sent.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-144">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="a1e4a-144">IsFromMe</span></span>](isfromme.md) <br/> |<span data-ttu-id="a1e4a-145">ユーザーが自分自身にアイテムを送信するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-145">Indicates whether a user sent an item to himself or herself.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="a1e4a-146">IsResend</span></span>](isresend.md) <br/> |<span data-ttu-id="a1e4a-147">アイテムが以前送信されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-147">Indicates whether the item had previously been sent.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-148">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="a1e4a-148">IsUnmodified</span></span>](isunmodified.md) <br/> |<span data-ttu-id="a1e4a-149">アイテムが変更されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-149">Indicates whether the item has been modified.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-150">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="a1e4a-150">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="a1e4a-151">メールボックス内のアイテムに含まれるすべてのインターネット メッセージ ヘッダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-151">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-152">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="a1e4a-152">DateTimeSent</span></span>](datetimesent.md) <br/> |<span data-ttu-id="a1e4a-153">メールボックス内のアイテムが送信された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-153">Represents the date and time that an item in a mailbox was sent.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-154">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="a1e4a-154">DateTimeCreated</span></span>](datetimecreated.md) <br/> |<span data-ttu-id="a1e4a-155">メールボックス内の特定のアイテムが作成された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-155">Represents the date and time that a given item in the mailbox was created.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-156">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="a1e4a-156">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="a1e4a-157">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-157">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-158">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="a1e4a-158">ReminderDueBy</span></span>](reminderdueby.md) <br/> |<span data-ttu-id="a1e4a-159">イベントが発生したときの日時を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-159">Represents the date and time when the event occurs.</span></span> <span data-ttu-id="a1e4a-160">[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によってアラームが表示されたときを決定する使用されます。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-160">This is used by the [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) element to determine when the reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-161">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="a1e4a-161">ReminderIsSet</span></span>](reminderisset.md) <br/> |<span data-ttu-id="a1e4a-162">Exchange ストアのアイテムのアラームが設定されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-162">Indicates whether a reminder has been set for an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-163">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="a1e4a-163">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md) <br/> |<span data-ttu-id="a1e4a-164">分前にアラームが表示されるときに、イベントの数を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-164">Represents the number of minutes before an event when a reminder is displayed.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-165">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="a1e4a-165">DisplayCc</span></span>](displaycc.md) <br/> |<span data-ttu-id="a1e4a-166">[Cc] 行の内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-166">Represents the display string that is used for the contents of the Cc line.</span></span> <span data-ttu-id="a1e4a-167">これは、すべての Cc 受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-167">This is the concatenated string of all Cc recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-168">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="a1e4a-168">DisplayTo</span></span>](displayto.md) <br/> |<span data-ttu-id="a1e4a-169">行の内容のために使用される表示文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-169">Represents the display string that is used for the contents of the To line.</span></span> <span data-ttu-id="a1e4a-170">これは、すべての受信者の表示名の連結された文字列です。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-170">This is the concatenated string of all To recipient display names.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-171">添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="a1e4a-171">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="a1e4a-172">アイテムに表示されている 1 つ以上の添付ファイルがある場合に**true**に設定されているプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-172">Represents a property that is set to **true** if an item has at least one visible attachment.</span></span> <span data-ttu-id="a1e4a-173">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-173">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-174">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="a1e4a-174">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="a1e4a-175">フォルダーおよびアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-175">Identifies extended properties on folders and items.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-176">カルチャ</span><span class="sxs-lookup"><span data-stu-id="a1e4a-176">Culture</span></span>](culture.md) <br/> |<span data-ttu-id="a1e4a-177">メールボックス内の指定したアイテムのカルチャを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-177">Represents the culture for a given item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-178">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="a1e4a-178">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="a1e4a-179">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-179">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="a1e4a-180">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-180">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-181">LastModifiedName</span><span class="sxs-lookup"><span data-stu-id="a1e4a-181">LastModifiedName</span></span>](lastmodifiedname.md) <br/> |<span data-ttu-id="a1e4a-182">最後の項目を変更するのにはユーザーの表示名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-182">Contains the display name of the last user to modify an item.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-183">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="a1e4a-183">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="a1e4a-184">アイテムが最後に修正された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-184">Indicates when an item was last modified.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-185">IsAssociated</span><span class="sxs-lookup"><span data-stu-id="a1e4a-185">IsAssociated</span></span>](isassociated.md) <br/> |<span data-ttu-id="a1e4a-186">アイテムがフォルダーに関連付けられているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-186">Indicates whether the item is associated with a folder.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-187">WebClientReadFormQueryString</span><span class="sxs-lookup"><span data-stu-id="a1e4a-187">WebClientReadFormQueryString</span></span>](webclientreadformquerystring.md) <br/> |<span data-ttu-id="a1e4a-188">Outlook Web App 内の項目を参照するのには Microsoft Office Outlook の Web アプリケーションのエンドポイントを結合するための URL を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-188">Represents a URL to concatenate to the Microsoft Office Outlook Web App endpoint to read an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-189">WebClientEditFormQueryString</span><span class="sxs-lookup"><span data-stu-id="a1e4a-189">WebClientEditFormQueryString</span></span>](webclienteditformquerystring.md) <br/> |<span data-ttu-id="a1e4a-190">Outlook Web App 内の項目を編集するのには Outlook Web App エンドポイントへの連結に URL を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-190">Represents a URL to concatenate to the Outlook Web App endpoint to edit an item in Outlook Web App.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-191">ConversationId</span><span class="sxs-lookup"><span data-stu-id="a1e4a-191">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="a1e4a-192">アイテムや会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-192">Contains the identifier of an item or conversation.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-193">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="a1e4a-193">UniqueBody</span></span>](uniquebody.md) <br/> |<span data-ttu-id="a1e4a-194">このスレッドの一意の本文を表すテキストまたは HTML フラグメントを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-194">Represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-195">表題</span><span class="sxs-lookup"><span data-stu-id="a1e4a-195">FileAs</span></span>](fileas.md) <br/> |<span data-ttu-id="a1e4a-196">連絡先フォルダーに連絡先を保存する方法を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-196">Represents how a contact is filed in the Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-197">FileAsMapping</span><span class="sxs-lookup"><span data-stu-id="a1e4a-197">FileAsMapping</span></span>](fileasmapping.md) <br/> |<span data-ttu-id="a1e4a-198">連絡先の表示内容を構築する方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-198">Defines how to construct what is displayed for a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-199">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="a1e4a-199">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="a1e4a-200">連絡先の表示名を定義します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-200">Defines the display name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-201">GivenName</span><span class="sxs-lookup"><span data-stu-id="a1e4a-201">GivenName</span></span>](givenname.md) <br/> |<span data-ttu-id="a1e4a-202">連絡先の指定された名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-202">Contains a contact's given name.</span></span>  <br/> |
|<span data-ttu-id="a1e4a-203">[[頭文字]](initials.md)</span><span class="sxs-lookup"><span data-stu-id="a1e4a-203">[Initials](initials.md)</span></span> <br/> |<span data-ttu-id="a1e4a-204">連絡先のイニシャルを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-204">Represents the initials of a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-205">ミドル ネーム</span><span class="sxs-lookup"><span data-stu-id="a1e4a-205">MiddleName</span></span>](middlename.md) <br/> |<span data-ttu-id="a1e4a-206">連絡先のミドル ネームを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-206">Represents the middle name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-207">ニックネーム</span><span class="sxs-lookup"><span data-stu-id="a1e4a-207">Nickname</span></span>](nickname.md) <br/> |<span data-ttu-id="a1e4a-208">連絡先のニックネームを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-208">Represents the nickname of a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-209">CompleteName</span><span class="sxs-lookup"><span data-stu-id="a1e4a-209">CompleteName</span></span>](completename.md) <br/> |<span data-ttu-id="a1e4a-210">連絡先の完全な名前を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-210">Represents the complete name of a contact.</span></span>  <br/> |
|<span data-ttu-id="a1e4a-211">[[得意先名]](companyname.md)</span><span class="sxs-lookup"><span data-stu-id="a1e4a-211">[CompanyName](companyname.md)</span></span> <br/> |<span data-ttu-id="a1e4a-212">連絡先に関連付けられている会社名を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-212">Represents the company name that is associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-213">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="a1e4a-213">EmailAddresses</span></span>](emailaddresses.md) <br/> |<span data-ttu-id="a1e4a-214">連絡先の電子メール アドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-214">Represents a collection of e-mail addresses for a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-215">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="a1e4a-215">PhysicalAddresses</span></span>](physicaladdresses.md) <br/> |<span data-ttu-id="a1e4a-216">連絡先に関連付けられている物理アドレスのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-216">Contains a collection of physical addresses that are associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-217">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="a1e4a-217">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="a1e4a-218">連絡先の電話番号のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-218">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-219">AssistantName</span><span class="sxs-lookup"><span data-stu-id="a1e4a-219">AssistantName</span></span>](assistantname.md) <br/> |<span data-ttu-id="a1e4a-220">連絡先にアシスタントを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-220">Represents an assistant to a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-221">Birthday</span><span class="sxs-lookup"><span data-stu-id="a1e4a-221">Birthday</span></span>](birthday.md) <br/> |<span data-ttu-id="a1e4a-222">連絡先の生年月日を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-222">Represents the birth date of a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-223">BusinessHomePage</span><span class="sxs-lookup"><span data-stu-id="a1e4a-223">BusinessHomePage</span></span>](businesshomepage.md) <br/> |<span data-ttu-id="a1e4a-224">連絡先のホーム ページ (Web アドレス) を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-224">Represents the Home page (Web address) for the contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-225">Children</span><span class="sxs-lookup"><span data-stu-id="a1e4a-225">Children</span></span>](children.md) <br/> |<span data-ttu-id="a1e4a-226">連絡先の子供の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-226">Contains the names of a contact's children.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-227">Companies</span><span class="sxs-lookup"><span data-stu-id="a1e4a-227">Companies</span></span>](companies.md) <br/> |<span data-ttu-id="a1e4a-228">連絡先に関連付けられている企業のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-228">Represents the collection of companies that are associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-229">ContactSource</span><span class="sxs-lookup"><span data-stu-id="a1e4a-229">ContactSource</span></span>](contactsource.md) <br/> |<span data-ttu-id="a1e4a-230">連絡先が Exchange ストアまたは Active Directory ディレクトリ サービス内にあるかどうかについて説明します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-230">Describes whether the contact is located in the Exchange store or the Active Directory directory service.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-231">Department</span><span class="sxs-lookup"><span data-stu-id="a1e4a-231">Department</span></span>](department.md) <br/> |<span data-ttu-id="a1e4a-232">職場の連絡先の部署を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-232">Represents the contact's department at work.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-233">生成</span><span class="sxs-lookup"><span data-stu-id="a1e4a-233">Generation</span></span>](generation.md) <br/> |<span data-ttu-id="a1e4a-234">連絡先の完全な名前を次世代の省略形を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-234">Represents a generational abbreviation that follows the full name of a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-235">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="a1e4a-235">ImAddresses</span></span>](imaddresses.md) <br/> |<span data-ttu-id="a1e4a-236">連絡先のインスタント メッセージング アドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-236">Represents a collection of instant messaging addresses for a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-237">役職</span><span class="sxs-lookup"><span data-stu-id="a1e4a-237">JobTitle</span></span>](jobtitle.md) <br/> |<span data-ttu-id="a1e4a-238">取引先担当者の役職名を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-238">Represents the job title of a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-239">マネージャー</span><span class="sxs-lookup"><span data-stu-id="a1e4a-239">Manager</span></span>](manager.md) <br/> |<span data-ttu-id="a1e4a-240">連絡先のマネージャーを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-240">Represents a contact's manager.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-241">マイレージ</span><span class="sxs-lookup"><span data-stu-id="a1e4a-241">Mileage</span></span>](mileage.md) <br/> |<span data-ttu-id="a1e4a-242">連絡先アイテムの経費情報を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-242">Represents mileage for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-243">事業所</span><span class="sxs-lookup"><span data-stu-id="a1e4a-243">OfficeLocation</span></span>](officelocation.md) <br/> |<span data-ttu-id="a1e4a-244">連絡先のオフィスの場所を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-244">Represents the office location of a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-245">PostalAddressIndex</span><span class="sxs-lookup"><span data-stu-id="a1e4a-245">PostalAddressIndex</span></span>](postaladdressindex.md) <br/> |<span data-ttu-id="a1e4a-246">物理アドレスの表示の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-246">Represents the display types for physical addresses.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-247">Profession</span><span class="sxs-lookup"><span data-stu-id="a1e4a-247">Profession</span></span>](profession.md) <br/> |<span data-ttu-id="a1e4a-248">連絡先の職業を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-248">Represents the profession of a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-249">SpouseName</span><span class="sxs-lookup"><span data-stu-id="a1e4a-249">SpouseName</span></span>](spousename.md) <br/> |<span data-ttu-id="a1e4a-250">連絡先の配偶者またはパートナーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-250">Represents the name of a contact's spouse/partner.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-251">姓</span><span class="sxs-lookup"><span data-stu-id="a1e4a-251">Surname</span></span>](surname.md) <br/> |<span data-ttu-id="a1e4a-252">連絡先の姓を表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-252">Represents the surname of a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-253">WeddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="a1e4a-253">WeddingAnniversary</span></span>](weddinganniversary.md) <br/> |<span data-ttu-id="a1e4a-254">取引先担当者の結婚記念日が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-254">Contains the wedding anniversary of a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-255">HasPicture</span><span class="sxs-lookup"><span data-stu-id="a1e4a-255">HasPicture</span></span>](haspicture.md) <br/> |<span data-ttu-id="a1e4a-256">連絡先アイテムが連絡先の画像を表す添付ファイルがあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-256">Indicates whether the contact item has a file attachment that represents the contact's picture.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-257">PhoneticFullName</span><span class="sxs-lookup"><span data-stu-id="a1e4a-257">PhoneticFullName</span></span>](phoneticfullname.md) <br/> |<span data-ttu-id="a1e4a-258">発音のスペルの最初と最後の名前を含む、連絡先の完全な名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-258">Contains the full name of a contact, including the first and last name, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-259">PhoneticFirstName</span><span class="sxs-lookup"><span data-stu-id="a1e4a-259">PhoneticFirstName</span></span>](phoneticfirstname.md) <br/> |<span data-ttu-id="a1e4a-260">連絡先の名前を含む発音のスペルします。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-260">Contains the first name of a contact, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-261">PhoneticLastName</span><span class="sxs-lookup"><span data-stu-id="a1e4a-261">PhoneticLastName</span></span>](phoneticlastname.md) <br/> |<span data-ttu-id="a1e4a-262">連絡先の姓が含まれている発音のスペルします。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-262">Contains the last name of a contact, spelled phonetically.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-263">エイリアス</span><span class="sxs-lookup"><span data-stu-id="a1e4a-263">Alias</span></span>](alias.md) <br/> |<span data-ttu-id="a1e4a-264">連絡先の電子メール エイリアスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-264">Contains the email alias of a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-265">ノート (連絡先)</span><span class="sxs-lookup"><span data-stu-id="a1e4a-265">Notes (Contact)</span></span>](notes-contact.md) <br/> |<span data-ttu-id="a1e4a-266">補足の連絡先情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-266">Contains supplementary contact information.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-267">Photo</span><span class="sxs-lookup"><span data-stu-id="a1e4a-267">Photo</span></span>](photo.md) <br/> |<span data-ttu-id="a1e4a-268">連絡先の写真をエンコードする値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-268">Contains a value that encodes the photo of a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-269">UserSMIMECertificate</span><span class="sxs-lookup"><span data-stu-id="a1e4a-269">UserSMIMECertificate</span></span>](usersmimecertificate.md) <br/> |<span data-ttu-id="a1e4a-270">連絡先の SMIME の証明書をエンコードする値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-270">Contains a value that encodes the SMIME certificate of a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-271">MSExchangeCertificate</span><span class="sxs-lookup"><span data-stu-id="a1e4a-271">MSExchangeCertificate</span></span>](msexchangecertificate.md) <br/> |<span data-ttu-id="a1e4a-272">連絡先の [Microsoft Exchange 証明書をエンコードする値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-272">Contains a value that encodes the Microsoft Exchange certificate of a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-273">DirectoryId</span><span class="sxs-lookup"><span data-stu-id="a1e4a-273">DirectoryId</span></span>](directoryid.md) <br/> |<span data-ttu-id="a1e4a-274">連絡先のディレクトリ ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-274">Contains the directory ID of a contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-275">ManagerMailbox</span><span class="sxs-lookup"><span data-stu-id="a1e4a-275">ManagerMailbox</span></span>](managermailbox.md) <br/> |<span data-ttu-id="a1e4a-276">連絡先のマネージャーのメールボックスを識別するための SMTP 情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-276">Contains SMTP information that identifies the manager mailbox of the contact.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-277">DirectReports</span><span class="sxs-lookup"><span data-stu-id="a1e4a-277">DirectReports</span></span>](directreports.md) <br/> |<span data-ttu-id="a1e4a-278">取引先担当者の直属の部下を識別するための SMTP 情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-278">Contains SMTP information that identifies the direct reports of a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a1e4a-279">親要素</span><span class="sxs-lookup"><span data-stu-id="a1e4a-279">Parent elements</span></span>

|<span data-ttu-id="a1e4a-280">**要素名**</span><span class="sxs-lookup"><span data-stu-id="a1e4a-280">**Element name**</span></span>|<span data-ttu-id="a1e4a-281">**説明**</span><span class="sxs-lookup"><span data-stu-id="a1e4a-281">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1e4a-282">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="a1e4a-282">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> |<span data-ttu-id="a1e4a-283">会議の時刻に隣接しているすべての予定表のアイテムについて説明します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-283">Describes all calendar items that are adjacent to a meeting time.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-284">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="a1e4a-284">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="a1e4a-285">[UpdateItem 操作](updateitem-operation.md)中に 1 つのアイテムまたはフォルダーのプロパティを追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-285">Identifies data to append to a single property of an item or folder during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-286">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="a1e4a-286">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> |<span data-ttu-id="a1e4a-287">会議の時間と競合するすべての項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-287">Identifies all items that conflict with a meeting time</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-288">(ItemSync) を作成します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-288">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="a1e4a-289">ローカル クライアント ストアに作成する 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-289">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-290">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="a1e4a-290">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="a1e4a-291">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-291">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-292">Items</span><span class="sxs-lookup"><span data-stu-id="a1e4a-292">Items</span></span>](items.md) <br/> |<span data-ttu-id="a1e4a-293">項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-293">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-294">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="a1e4a-294">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="a1e4a-295">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で識別されるフォルダーを作成する項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-295">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-296">解決策</span><span class="sxs-lookup"><span data-stu-id="a1e4a-296">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="a1e4a-297">解決された 1 つのエンティティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-297">Contains a single resolved entity.</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-298">SetItemField</span><span class="sxs-lookup"><span data-stu-id="a1e4a-298">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="a1e4a-299">[UpdateItem 操作](updateitem-operation.md)内の項目の 1 つのプロパティには、更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-299">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="a1e4a-300">更新プログラム (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="a1e4a-300">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="a1e4a-301">ローカル クライアント ストアで更新する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-301">Identifies a single item to update in the local client store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a1e4a-302">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a1e4a-302">Text value</span></span>

<span data-ttu-id="a1e4a-303">なし。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-303">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a1e4a-304">備考</span><span class="sxs-lookup"><span data-stu-id="a1e4a-304">Remarks</span></span>

<span data-ttu-id="a1e4a-305">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-305">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1e4a-306">要素情報</span><span class="sxs-lookup"><span data-stu-id="a1e4a-306">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1e4a-307">名前空間</span><span class="sxs-lookup"><span data-stu-id="a1e4a-307">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a1e4a-308">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a1e4a-308">Schema name</span></span>  <br/> |<span data-ttu-id="a1e4a-309">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a1e4a-309">Types schema</span></span>  <br/> |
|<span data-ttu-id="a1e4a-310">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a1e4a-310">Validation file</span></span>  <br/> |<span data-ttu-id="a1e4a-311">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a1e4a-311">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a1e4a-312">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-312">Can be empty</span></span>  <br/> |<span data-ttu-id="a1e4a-313">False</span><span class="sxs-lookup"><span data-stu-id="a1e4a-313">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a1e4a-314">関連項目</span><span class="sxs-lookup"><span data-stu-id="a1e4a-314">See also</span></span>



- [<span data-ttu-id="a1e4a-315">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a1e4a-315">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="a1e4a-316">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-316">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="a1e4a-317">連絡先を更新</span><span class="sxs-lookup"><span data-stu-id="a1e4a-317">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="a1e4a-318">連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="a1e4a-318">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)


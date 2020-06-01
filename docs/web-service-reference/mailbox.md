---
title: メールボックス
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Mailbox
api_type:
- schema
ms.assetid: befc70fd-51cb-4258-884c-80c9050f0e82
description: Mailbox 要素は、メールが有効な Active Directory オブジェクトを識別します。
ms.openlocfilehash: 284c3ff6f9fece57611169a4ec41eeaa273c6ad3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468202"
---
# <a name="mailbox"></a><span data-ttu-id="e98a2-103">メールボックス</span><span class="sxs-lookup"><span data-stu-id="e98a2-103">Mailbox</span></span>

<span data-ttu-id="e98a2-104">**Mailbox**要素は、メールが有効な Active Directory オブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-104">The **Mailbox** element identifies a mail-enabled Active Directory object.</span></span> 
  
```XML
<Mailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Mailbox>
```

<span data-ttu-id="e98a2-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="e98a2-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e98a2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e98a2-106">Attributes and elements</span></span>

<span data-ttu-id="e98a2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e98a2-108">属性</span><span class="sxs-lookup"><span data-stu-id="e98a2-108">Attributes</span></span>

<span data-ttu-id="e98a2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e98a2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e98a2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e98a2-110">Child elements</span></span>

|<span data-ttu-id="e98a2-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="e98a2-111">**Element**</span></span>|<span data-ttu-id="e98a2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e98a2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e98a2-113">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e98a2-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="e98a2-114">メールボックスユーザーの名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="e98a2-115">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="e98a2-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-116">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="e98a2-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="e98a2-117">メールボックスユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="e98a2-118">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="e98a2-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="e98a2-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="e98a2-120">メールボックスに使用されるルーティングを定義します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="e98a2-121">既定値は SMTP です。</span><span class="sxs-lookup"><span data-stu-id="e98a2-121">The default is SMTP.</span></span> <span data-ttu-id="e98a2-122">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="e98a2-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="e98a2-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="e98a2-124">メールボックスユーザーのメールボックスの種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="e98a2-125">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="e98a2-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="e98a2-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="e98a2-127">ユーザーの連絡先フォルダーにある受信者の連絡先またはプライベート配布リストのアイテム識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-127">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="e98a2-128">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="e98a2-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e98a2-129">親要素</span><span class="sxs-lookup"><span data-stu-id="e98a2-129">Parent elements</span></span>

|<span data-ttu-id="e98a2-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="e98a2-130">**Element**</span></span>|<span data-ttu-id="e98a2-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="e98a2-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e98a2-132">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="e98a2-132">ExpandDL</span></span>](expanddl.md) <br/> |<span data-ttu-id="e98a2-133">配布リストを展開するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-133">Defines a request to expand a distribution list.</span></span> <br/> <br/> <span data-ttu-id="e98a2-134">この要素の XPath 式を次に示します。` /ExpandDL `</span><span class="sxs-lookup"><span data-stu-id="e98a2-134">The following is the XPath expression to this element: ` /ExpandDL `</span></span> <br/> |
|[<span data-ttu-id="e98a2-135">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="e98a2-135">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="e98a2-136">アイテムの受信者の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-136">Contains an array of recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-137">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="e98a2-137">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="e98a2-138">メッセージのコピーを受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-138">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-139">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="e98a2-139">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="e98a2-140">電子メールのブラインドカーボンコピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-140">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-141">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="e98a2-141">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="e98a2-142">返信が送信される電子メールアドレスの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-142">Identifies an array of e-mail addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-143">Sender</span><span class="sxs-lookup"><span data-stu-id="e98a2-143">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="e98a2-144">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-144">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-145">From</span><span class="sxs-lookup"><span data-stu-id="e98a2-145">From</span></span>](from.md) <br/> |<span data-ttu-id="e98a2-146">メッセージが送信された相手のアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-146">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-147">Organizer</span><span class="sxs-lookup"><span data-stu-id="e98a2-147">Organizer</span></span>](organizer.md) <br/> |<span data-ttu-id="e98a2-148">会議の開催者を表します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-148">Represents the organizer of a meeting.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-149">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="e98a2-149">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> | <span data-ttu-id="e98a2-150">Microsoft Exchange Server 2007 の既定のフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-150">Identifies default Microsoft Exchange Server 2007 folders.</span></span>  <br/><br/>  <span data-ttu-id="e98a2-151">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e98a2-151">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[<span data-ttu-id="e98a2-152">Resolution</span><span class="sxs-lookup"><span data-stu-id="e98a2-152">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="e98a2-153">1つの解決済みエンティティを含みます。</span><span class="sxs-lookup"><span data-stu-id="e98a2-153">Contains a single resolved entity.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-154">DLExpansion 展開</span><span class="sxs-lookup"><span data-stu-id="e98a2-154">DLExpansion</span></span>](dlexpansion.md) <br/> |<span data-ttu-id="e98a2-155">配布リストに含まれているメールボックスの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-155">Contains an array of mailboxes that are contained in a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-156">出席者</span><span class="sxs-lookup"><span data-stu-id="e98a2-156">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="e98a2-157">予定表アイテムの出席者とリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-157">Represents attendees and resources for a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-158">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="e98a2-158">CreateManagedFolder</span></span>](createmanagedfolder.md) <br/> |<span data-ttu-id="e98a2-159">メールボックスに管理フォルダーを追加する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-159">Defines a request to add managed folders to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-160">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="e98a2-160">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="e98a2-161">メールボックスに代理人を追加するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-161">Defines a request to add delegates to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-162">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="e98a2-162">GetDelegate</span></span>](getdelegate.md) <br/> |<span data-ttu-id="e98a2-163">メールボックスへの代理人に関する情報を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-163">Defines a request to get information about delegates to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-164">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="e98a2-164">RemoveDelegate</span></span>](removedelegate.md) <br/> |<span data-ttu-id="e98a2-165">メールボックスから代理人を削除するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-165">Defines a request to remove delegates from a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-166">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="e98a2-166">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="e98a2-167">メールボックスの代理人を更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-167">Defines a request to update delegates in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-168">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="e98a2-168">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="e98a2-169">代理人アクセスのシナリオでのデリゲートについて説明します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-169">Describes the delegate in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-170">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="e98a2-170">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="e98a2-171">代理人アクセスシナリオのプリンシパルについて説明します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-171">Describes the principal in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="e98a2-172">メンバー</span><span class="sxs-lookup"><span data-stu-id="e98a2-172">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e98a2-173">配布リストのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-173">Represents a member of a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e98a2-174">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e98a2-174">Text value</span></span>

<span data-ttu-id="e98a2-175">なし。</span><span class="sxs-lookup"><span data-stu-id="e98a2-175">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e98a2-176">注釈</span><span class="sxs-lookup"><span data-stu-id="e98a2-176">Remarks</span></span>

<span data-ttu-id="e98a2-177">[EmailAddress (非 Emptystringtype)](emailaddress-nonemptystringtype.md)要素と[ItemId](itemid.md)要素は、メールボックスまたは配布リストを識別します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-177">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) and [ItemId](itemid.md) elements identify a mailbox or distribution list.</span></span> 

<span data-ttu-id="e98a2-178">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)要素は、SMTP アドレスによってメールボックスまたは配布リストを識別します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-178">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element identifies a mailbox or distribution list by SMTP address.</span></span> 

<span data-ttu-id="e98a2-179">[ItemId](itemid.md)要素は、特定のメールボックスに関連付けられているアイテムの識別子によってメールボックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-179">The [ItemId](itemid.md) element identifies a mailbox by an item identifier, which is associated with a particular mailbox.</span></span> 

<span data-ttu-id="e98a2-180">[ItemId](itemid.md)要素を使用して、配布リストまたはパブリック連絡先フォルダー内の連絡先にメッセージを送信することはできません。</span><span class="sxs-lookup"><span data-stu-id="e98a2-180">The [ItemId](itemid.md) element cannot be used for sending a message to a distribution list or a contact in a public contacts folder.</span></span> <span data-ttu-id="e98a2-181">CreateItem、UpdateItem、または SendItem 操作で、連絡先パブリックフォルダーの配布リストまたは連絡先にメッセージを送信しようとすると、エラーがスローされます。</span><span class="sxs-lookup"><span data-stu-id="e98a2-181">An error will be thrown if this is used in a CreateItem, UpdateItem, or SendItem operation when an attempt is made to send a message to a distribution list or contact in a contacts public folder.</span></span> <span data-ttu-id="e98a2-182">ExpandDL 操作を使用して SMTP アドレスを取得してから、 [ItemId](itemid.md)要素ではなく[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)要素を使用してメッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-182">Use the ExpandDL operation to get the SMTP address and then send the message by using the [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element instead of the [ItemId](itemid.md) element.</span></span> 
  
<span data-ttu-id="e98a2-183">もう1つの要素である[メールボックス (可用性)](mailbox-availability.md)は、可用性の運用に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="e98a2-183">Another element, [Mailbox (Availability)](mailbox-availability.md), provides information for availability operations.</span></span> 
  
<span data-ttu-id="e98a2-184">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e98a2-184">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e98a2-185">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e98a2-185">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e98a2-186">Namespace</span><span class="sxs-lookup"><span data-stu-id="e98a2-186">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e98a2-187">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e98a2-187">Schema Name</span></span>  <br/> |<span data-ttu-id="e98a2-188">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e98a2-188">Types schema</span></span>  <br/> |
|<span data-ttu-id="e98a2-189">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e98a2-189">Validation File</span></span>  <br/> |<span data-ttu-id="e98a2-190">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e98a2-190">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e98a2-191">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e98a2-191">Can be Empty</span></span>  <br/> |<span data-ttu-id="e98a2-192">正しくない</span><span class="sxs-lookup"><span data-stu-id="e98a2-192">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e98a2-193">関連項目</span><span class="sxs-lookup"><span data-stu-id="e98a2-193">See also</span></span>

- [<span data-ttu-id="e98a2-194">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e98a2-194">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


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
description: メールボックス要素では、メールが有効な Active Directory のオブジェクトを識別します。
ms.openlocfilehash: e9fa21f3678249a9ac13d567b88beaf0177f989f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832258"
---
# <a name="mailbox"></a><span data-ttu-id="f2b5a-103">メールボックス</span><span class="sxs-lookup"><span data-stu-id="f2b5a-103">Mailbox</span></span>

<span data-ttu-id="f2b5a-104">**メールボックス**要素では、メールが有効な Active Directory のオブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-104">The **Mailbox** element identifies a mail-enabled Active Directory object.</span></span> 
  
```XML
<Mailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Mailbox>
```

<span data-ttu-id="f2b5a-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="f2b5a-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f2b5a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f2b5a-106">Attributes and elements</span></span>

<span data-ttu-id="f2b5a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2b5a-108">属性</span><span class="sxs-lookup"><span data-stu-id="f2b5a-108">Attributes</span></span>

<span data-ttu-id="f2b5a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2b5a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f2b5a-110">Child elements</span></span>

|<span data-ttu-id="f2b5a-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="f2b5a-111">**Element**</span></span>|<span data-ttu-id="f2b5a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f2b5a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2b5a-113">名 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="f2b5a-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="f2b5a-114">メールボックス ユーザーの名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="f2b5a-115">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="f2b5a-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="f2b5a-117">メールボックスのユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="f2b5a-118">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="f2b5a-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="f2b5a-120">メールボックスに使用されるルーティングを定義します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="f2b5a-121">既定値は、SMTP です。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-121">The default is SMTP.</span></span> <span data-ttu-id="f2b5a-122">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="f2b5a-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="f2b5a-124">メールボックスのユーザーのメールボックスの種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="f2b5a-125">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="f2b5a-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="f2b5a-127">ユーザーのアドレス帳フォルダーから受信者の連絡先または個人用配布リストの項目の識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-127">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="f2b5a-128">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f2b5a-129">親要素</span><span class="sxs-lookup"><span data-stu-id="f2b5a-129">Parent elements</span></span>

|<span data-ttu-id="f2b5a-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="f2b5a-130">**Element**</span></span>|<span data-ttu-id="f2b5a-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="f2b5a-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2b5a-132">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="f2b5a-132">ExpandDL</span></span>](expanddl.md) <br/> |<span data-ttu-id="f2b5a-133">配布リストを展開するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-133">Defines a request to expand a distribution list.</span></span> <br/> <br/> <span data-ttu-id="f2b5a-134">この要素への XPath 式は、次のようにします。` /ExpandDL `</span><span class="sxs-lookup"><span data-stu-id="f2b5a-134">The following is the XPath expression to this element: ` /ExpandDL `</span></span> <br/> |
|[<span data-ttu-id="f2b5a-135">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="f2b5a-135">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="f2b5a-136">アイテムの受信者の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-136">Contains an array of recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-137">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="f2b5a-137">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="f2b5a-138">メッセージのコピーを受け取る受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-138">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-139">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="f2b5a-139">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="f2b5a-140">電子メールのブラインド カーボン コピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-140">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-141">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="f2b5a-141">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="f2b5a-142">応答を送信する電子メール アドレスの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-142">Identifies an array of e-mail addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-143">送信者</span><span class="sxs-lookup"><span data-stu-id="f2b5a-143">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="f2b5a-144">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-144">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-145">From</span><span class="sxs-lookup"><span data-stu-id="f2b5a-145">From</span></span>](from.md) <br/> |<span data-ttu-id="f2b5a-146">メッセージの送信元アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-146">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-147">Organizer</span><span class="sxs-lookup"><span data-stu-id="f2b5a-147">Organizer</span></span>](organizer.md) <br/> |<span data-ttu-id="f2b5a-148">会議の開催者を表します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-148">Represents the organizer of a meeting.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-149">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="f2b5a-149">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> | <span data-ttu-id="f2b5a-150">Microsoft Exchange Server 2007 の既定のフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-150">Identifies default Microsoft Exchange Server 2007 folders.</span></span>  <br/><br/>  <span data-ttu-id="f2b5a-151">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-151">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[<span data-ttu-id="f2b5a-152">解決策</span><span class="sxs-lookup"><span data-stu-id="f2b5a-152">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="f2b5a-153">解決された 1 つのエンティティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-153">Contains a single resolved entity.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-154">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="f2b5a-154">DLExpansion</span></span>](dlexpansion.md) <br/> |<span data-ttu-id="f2b5a-155">配布リストに含まれているメールボックスの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-155">Contains an array of mailboxes that are contained in a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-156">Attendee</span><span class="sxs-lookup"><span data-stu-id="f2b5a-156">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="f2b5a-157">出席者とリソースの予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-157">Represents attendees and resources for a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-158">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="f2b5a-158">CreateManagedFolder</span></span>](createmanagedfolder.md) <br/> |<span data-ttu-id="f2b5a-159">メールボックスに管理フォルダーを追加する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-159">Defines a request to add managed folders to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-160">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="f2b5a-160">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="f2b5a-161">メールボックスに代理人を追加する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-161">Defines a request to add delegates to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-162">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="f2b5a-162">GetDelegate</span></span>](getdelegate.md) <br/> |<span data-ttu-id="f2b5a-163">メールボックスに代理人についての情報を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-163">Defines a request to get information about delegates to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-164">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="f2b5a-164">RemoveDelegate</span></span>](removedelegate.md) <br/> |<span data-ttu-id="f2b5a-165">メールボックスからデリゲートを削除する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-165">Defines a request to remove delegates from a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-166">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="f2b5a-166">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="f2b5a-167">メールボックスに代理人を更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-167">Defines a request to update delegates in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-168">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="f2b5a-168">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="f2b5a-169">代理人アクセス シナリオでは、デリゲートをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-169">Describes the delegate in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-170">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="f2b5a-170">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="f2b5a-171">代理人アクセスのシナリオでプリンシパルについて説明します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-171">Describes the principal in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="f2b5a-172">メンバー</span><span class="sxs-lookup"><span data-stu-id="f2b5a-172">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f2b5a-173">配布リストのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-173">Represents a member of a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f2b5a-174">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f2b5a-174">Text value</span></span>

<span data-ttu-id="f2b5a-175">なし。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-175">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f2b5a-176">備考</span><span class="sxs-lookup"><span data-stu-id="f2b5a-176">Remarks</span></span>

<span data-ttu-id="f2b5a-177">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)と[アイテム Id](itemid.md)要素は、メールボックスまたは配布リストを識別します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-177">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) and [ItemId](itemid.md) elements identify a mailbox or distribution list.</span></span> 

<span data-ttu-id="f2b5a-178">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)の要素では、SMTP アドレスを使用してメールボックスまたは配布リストを識別します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-178">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element identifies a mailbox or distribution list by SMTP address.</span></span> 

<span data-ttu-id="f2b5a-179">[アイテム Id](itemid.md)要素は、特定のメールボックスに関連付けられている項目の識別子で、メールボックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-179">The [ItemId](itemid.md) element identifies a mailbox by an item identifier, which is associated with a particular mailbox.</span></span> 

<span data-ttu-id="f2b5a-180">[アイテム Id](itemid.md)要素は、配布リスト、またはパブリックの連絡先フォルダーの連絡先にメッセージを送信するのには使用できません。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-180">The [ItemId](itemid.md) element cannot be used for sending a message to a distribution list or a contact in a public contacts folder.</span></span> <span data-ttu-id="f2b5a-181">連絡先パブリック フォルダーの連絡先または配布リストにメッセージを送信しようとしましたがときに、createitem メソッド、UpdateItem、または SendItem 操作で使用される場合は、エラーがスローされます。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-181">An error will be thrown if this is used in a CreateItem, UpdateItem, or SendItem operation when an attempt is made to send a message to a distribution list or contact in a contacts public folder.</span></span> <span data-ttu-id="f2b5a-182">SMTP アドレスを取得し、[アイテム Id](itemid.md)の要素ではなく、 [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)の要素を使用してメッセージを送信するには、ExpandDL 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-182">Use the ExpandDL operation to get the SMTP address and then send the message by using the [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element instead of the [ItemId](itemid.md) element.</span></span> 
  
<span data-ttu-id="f2b5a-183">[(可用性) のメールボックス](mailbox-availability.md)、別の要素では、可用性の操作に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-183">Another element, [Mailbox (Availability)](mailbox-availability.md), provides information for availability operations.</span></span> 
  
<span data-ttu-id="f2b5a-184">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f2b5a-184">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2b5a-185">要素情報</span><span class="sxs-lookup"><span data-stu-id="f2b5a-185">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2b5a-186">名前空間</span><span class="sxs-lookup"><span data-stu-id="f2b5a-186">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f2b5a-187">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f2b5a-187">Schema Name</span></span>  <br/> |<span data-ttu-id="f2b5a-188">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f2b5a-188">Types schema</span></span>  <br/> |
|<span data-ttu-id="f2b5a-189">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f2b5a-189">Validation File</span></span>  <br/> |<span data-ttu-id="f2b5a-190">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f2b5a-190">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f2b5a-191">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f2b5a-191">Can be Empty</span></span>  <br/> |<span data-ttu-id="f2b5a-192">False</span><span class="sxs-lookup"><span data-stu-id="f2b5a-192">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2b5a-193">関連項目</span><span class="sxs-lookup"><span data-stu-id="f2b5a-193">See also</span></span>

- [<span data-ttu-id="f2b5a-194">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f2b5a-194">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


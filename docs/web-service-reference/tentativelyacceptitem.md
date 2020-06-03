---
title: TentativelyAcceptItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TentativelyAcceptItem
api_type:
- schema
ms.assetid: ce6f50ef-ad8a-47e4-915a-487b2ef7a2e0
description: TentativelyAcceptItem 要素は、会議出席依頼に対する仮承諾の返信を表します。
ms.openlocfilehash: 6d20ec2964c41dcbb786b1209b4597999e025609
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459498"
---
# <a name="tentativelyacceptitem"></a><span data-ttu-id="80136-103">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="80136-103">TentativelyAcceptItem</span></span>

<span data-ttu-id="80136-104">**TentativelyAcceptItem**要素は、会議出席依頼に対する仮承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="80136-104">The **TentativelyAcceptItem** element represents a Tentative reply to a meeting request.</span></span> 
  
```xml
<TentativelyAcceptItem>
   <ItemClass/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <InternetMessageHeaders/>
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ReferenceItemId/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
   <ProposedStart/>
   <ProposedEnd/>
</TentativelyAcceptItem>
```

 <span data-ttu-id="80136-105">**TentativelyAcceptItemType**</span><span class="sxs-lookup"><span data-stu-id="80136-105">**TentativelyAcceptItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="80136-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="80136-106">Attributes and elements</span></span>

<span data-ttu-id="80136-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="80136-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80136-108">属性</span><span class="sxs-lookup"><span data-stu-id="80136-108">Attributes</span></span>

<span data-ttu-id="80136-109">なし。</span><span class="sxs-lookup"><span data-stu-id="80136-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80136-110">子要素</span><span class="sxs-lookup"><span data-stu-id="80136-110">Child elements</span></span>

|<span data-ttu-id="80136-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="80136-111">**Element**</span></span>|<span data-ttu-id="80136-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="80136-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80136-113">ItemClass</span><span class="sxs-lookup"><span data-stu-id="80136-113">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="80136-114">アイテムのメッセージクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="80136-114">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="80136-115">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="80136-115">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="80136-116">アイテムの秘密度を識別します。</span><span class="sxs-lookup"><span data-stu-id="80136-116">Identifies the sensitivity of an item.</span></span>  <br/> |
|[<span data-ttu-id="80136-117">Body</span><span class="sxs-lookup"><span data-stu-id="80136-117">Body</span></span>](body.md) <br/> |<span data-ttu-id="80136-118">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="80136-118">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="80136-119">Attachments</span><span class="sxs-lookup"><span data-stu-id="80136-119">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="80136-120">Exchange ストア内のアイテムに添付されているアイテムまたはファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="80136-120">Contains the item or file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="80136-121">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="80136-121">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="80136-122">Headers コレクション内の指定されたヘッダーのインターネットメッセージヘッダー名を表します。</span><span class="sxs-lookup"><span data-stu-id="80136-122">Represents the Internet message header name for a given header within the headers collection.</span></span>  <br/> |
|[<span data-ttu-id="80136-123">Sender</span><span class="sxs-lookup"><span data-stu-id="80136-123">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="80136-124">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="80136-124">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="80136-125">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="80136-125">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="80136-126">アイテムの受信者のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="80136-126">Contains a set of recipients of an item.</span></span> <span data-ttu-id="80136-127">次に、アイテムのプライマリ受信者を示します。</span><span class="sxs-lookup"><span data-stu-id="80136-127">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="80136-128">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="80136-128">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="80136-129">メッセージのコピーを受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="80136-129">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="80136-130">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="80136-130">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="80136-131">電子メールのブラインドカーボンコピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="80136-131">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="80136-132">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="80136-132">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="80136-133">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80136-133">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="80136-134">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="80136-134">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="80136-135">アイテムの送信者が配信確認を要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80136-135">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="80136-136">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="80136-136">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="80136-137">Response オブジェクトが参照するアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="80136-137">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="80136-138">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="80136-138">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="80136-139">代理人アクセスシナリオの代理人を識別します。</span><span class="sxs-lookup"><span data-stu-id="80136-139">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="80136-140">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="80136-140">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="80136-141">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="80136-141">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="80136-142">代理人アクセスシナリオのプリンシパルを識別します。</span><span class="sxs-lookup"><span data-stu-id="80136-142">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="80136-143">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="80136-143">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="80136-144">ProposedStart</span><span class="sxs-lookup"><span data-stu-id="80136-144">ProposedStart</span></span>](proposedstart.md) <br/> |<span data-ttu-id="80136-145">会議出席依頼の提案された開始時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="80136-145">Specifies the proposed start time of the meeting request.</span></span>  <br/> |
|[<span data-ttu-id="80136-146">ProposedEnd</span><span class="sxs-lookup"><span data-stu-id="80136-146">ProposedEnd</span></span>](proposedend.md) <br/> |<span data-ttu-id="80136-147">会議出席依頼の提案された終了時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="80136-147">Specifies the proposed end time of the meeting request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="80136-148">親要素</span><span class="sxs-lookup"><span data-stu-id="80136-148">Parent elements</span></span>

|<span data-ttu-id="80136-149">**要素**</span><span class="sxs-lookup"><span data-stu-id="80136-149">**Element**</span></span>|<span data-ttu-id="80136-150">**説明**</span><span class="sxs-lookup"><span data-stu-id="80136-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80136-151">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="80136-151">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="80136-152">会議の時刻に隣接しているすべてのアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="80136-152">Describes all items that are adjacent to a meeting time.</span></span>  <br/> <br/> <span data-ttu-id="80136-153">この要素の XPath 式の一部を次に示します。</span><span class="sxs-lookup"><span data-stu-id="80136-153">The following are some of the XPath expressions to this element:</span></span>  <br/><br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="80136-154">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="80136-154">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="80136-155">会議の時間と競合するすべてのアイテムについて説明します。</span><span class="sxs-lookup"><span data-stu-id="80136-155">Describes all items that conflict with a meeting time.</span></span> <br/> <br/>  <span data-ttu-id="80136-156">この要素の XPath 式の一部を次に示します。</span><span class="sxs-lookup"><span data-stu-id="80136-156">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="80136-157">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="80136-157">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="80136-158">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="80136-158">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="80136-159">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="80136-159">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="80136-160">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="80136-160">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="80136-161">注釈</span><span class="sxs-lookup"><span data-stu-id="80136-161">Remarks</span></span>

<span data-ttu-id="80136-162">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="80136-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="80136-163">要素の情報</span><span class="sxs-lookup"><span data-stu-id="80136-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80136-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="80136-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="80136-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="80136-165">Schema Name</span></span>  <br/> |<span data-ttu-id="80136-166">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="80136-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="80136-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="80136-167">Validation File</span></span>  <br/> |<span data-ttu-id="80136-168">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="80136-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="80136-169">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="80136-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="80136-170">正しくない</span><span class="sxs-lookup"><span data-stu-id="80136-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="80136-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="80136-171">See also</span></span>

- [<span data-ttu-id="80136-172">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="80136-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


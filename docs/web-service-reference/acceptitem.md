---
title: AcceptItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AcceptItem
api_type:
- schema
ms.assetid: 05a15431-77e1-411a-a16b-5481d364d3cc
description: AcceptItem 要素は、会議出席依頼への返信の承諾を表します。
ms.openlocfilehash: 6f2197e9df8a095aec545e1a09a761f7e8e432d3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461717"
---
# <a name="acceptitem"></a><span data-ttu-id="dc1f4-103">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="dc1f4-103">AcceptItem</span></span>

<span data-ttu-id="dc1f4-104">**Acceptitem**要素は、会議出席依頼への返信の承諾を表します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-104">The **AcceptItem** element represents an Accept reply to a meeting request.</span></span> 
  
```xml
<AcceptItem>
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
</AcceptItem>
```

 <span data-ttu-id="dc1f4-105">**AcceptItemType**</span><span class="sxs-lookup"><span data-stu-id="dc1f4-105">**AcceptItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dc1f4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="dc1f4-106">Attributes and elements</span></span>

<span data-ttu-id="dc1f4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc1f4-108">属性</span><span class="sxs-lookup"><span data-stu-id="dc1f4-108">Attributes</span></span>

<span data-ttu-id="dc1f4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc1f4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dc1f4-110">Child elements</span></span>

|<span data-ttu-id="dc1f4-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="dc1f4-111">**Element**</span></span>|<span data-ttu-id="dc1f4-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="dc1f4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc1f4-113">ItemClass</span><span class="sxs-lookup"><span data-stu-id="dc1f4-113">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="dc1f4-114">アイテムのメッセージクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-114">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="dc1f4-115">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="dc1f4-115">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="dc1f4-116">アイテムの秘密度レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-116">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="dc1f4-117">Body</span><span class="sxs-lookup"><span data-stu-id="dc1f4-117">Body</span></span>](body.md) <br/> |<span data-ttu-id="dc1f4-118">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-118">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="dc1f4-119">Attachments</span><span class="sxs-lookup"><span data-stu-id="dc1f4-119">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="dc1f4-120">Exchange ストア内のアイテムに添付されているアイテムまたはファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-120">Contains the item or file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="dc1f4-121">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="dc1f4-121">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="dc1f4-122">Headers コレクション内の指定されたヘッダーのインターネットメッセージヘッダー名を表します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-122">Represents the Internet message header name for a given header within the headers collection.</span></span>  <br/> |
|[<span data-ttu-id="dc1f4-123">Sender</span><span class="sxs-lookup"><span data-stu-id="dc1f4-123">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="dc1f4-124">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-124">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="dc1f4-125">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="dc1f4-125">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="dc1f4-126">アイテムの受信者のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-126">Contains a set of recipients of an item.</span></span> <span data-ttu-id="dc1f4-127">次に、アイテムのプライマリ受信者を示します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-127">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="dc1f4-128">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="dc1f4-128">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="dc1f4-129">メッセージのコピーを受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-129">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="dc1f4-130">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="dc1f4-130">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="dc1f4-131">電子メールのブラインドカーボンコピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-131">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="dc1f4-132">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="dc1f4-132">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="dc1f4-133">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-133">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="dc1f4-134">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="dc1f4-134">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="dc1f4-135">アイテムの送信者が配信確認を要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-135">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="dc1f4-136">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="dc1f4-136">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="dc1f4-137">Response オブジェクトが参照するアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-137">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="dc1f4-138">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="dc1f4-138">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="dc1f4-139">代理人アクセスシナリオの代理人を識別します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-139">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="dc1f4-140">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-140">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="dc1f4-141">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="dc1f4-141">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="dc1f4-142">代理人アクセスシナリオのプリンシパルを識別します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-142">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="dc1f4-143">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-143">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="dc1f4-144">ProposedStart</span><span class="sxs-lookup"><span data-stu-id="dc1f4-144">ProposedStart</span></span>](proposedstart.md) <br/> |<span data-ttu-id="dc1f4-145">会議の提案された開始時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-145">Specifies the proposed start time of the meeting.</span></span>  <br/> |
|[<span data-ttu-id="dc1f4-146">ProposedEnd</span><span class="sxs-lookup"><span data-stu-id="dc1f4-146">ProposedEnd</span></span>](proposedend.md) <br/> |<span data-ttu-id="dc1f4-147">会議の終了時刻の提案を指定します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-147">Specifies the proposed end time of the meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dc1f4-148">親要素</span><span class="sxs-lookup"><span data-stu-id="dc1f4-148">Parent elements</span></span>

|<span data-ttu-id="dc1f4-149">**要素**</span><span class="sxs-lookup"><span data-stu-id="dc1f4-149">**Element**</span></span>|<span data-ttu-id="dc1f4-150">**説明**</span><span class="sxs-lookup"><span data-stu-id="dc1f4-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc1f4-151">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="dc1f4-151">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="dc1f4-152">会議の時刻に隣接しているすべてのアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-152">Describes all items that are adjacent to a meeting time.</span></span><br/><br/>  <span data-ttu-id="dc1f4-153">この要素の XPath 式の一部を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-153">The following are some of the XPath expressions to this element:</span></span><br/><br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="dc1f4-154">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="dc1f4-154">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="dc1f4-155">会議の時間と競合するすべてのアイテムについて説明します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-155">Describes all items that conflict with a meeting time.</span></span><br/><br/>  <span data-ttu-id="dc1f4-156">この要素の XPath 式の一部を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-156">The following are some of the XPath expressions to this element:</span></span><br/><br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="dc1f4-157">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="dc1f4-157">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="dc1f4-158">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-158">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="dc1f4-159">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="dc1f4-159">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="dc1f4-160">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-160">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dc1f4-161">注釈</span><span class="sxs-lookup"><span data-stu-id="dc1f4-161">Remarks</span></span>

<span data-ttu-id="dc1f4-162">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange サーバーの EWS ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="dc1f4-162">The schema that describes this element is located in the EWS directory of the Exchange server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc1f4-163">要素の情報</span><span class="sxs-lookup"><span data-stu-id="dc1f4-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc1f4-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="dc1f4-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dc1f4-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dc1f4-165">Schema Name</span></span>  <br/> |<span data-ttu-id="dc1f4-166">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="dc1f4-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="dc1f4-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dc1f4-167">Validation File</span></span>  <br/> |<span data-ttu-id="dc1f4-168">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="dc1f4-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dc1f4-169">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dc1f4-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="dc1f4-170">正しくない</span><span class="sxs-lookup"><span data-stu-id="dc1f4-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc1f4-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="dc1f4-171">See also</span></span>

- [<span data-ttu-id="dc1f4-172">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="dc1f4-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: ReplyAllToItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReplyAllToItem
api_type:
- schema
ms.assetid: 8ca970ca-ca73-40db-9233-7b271cc5f44f
description: ReplyToAllItem 要素には、Exchange ストア内のアイテムの識別されたすべての受信者と送信者への返信が含まれています。
ms.openlocfilehash: 99ee3427babba2c91c7c3b4ad5a750fddca6cbfd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833129"
---
# <a name="replyalltoitem"></a><span data-ttu-id="ff5e3-103">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="ff5e3-103">ReplyAllToItem</span></span>

<span data-ttu-id="ff5e3-104">**ReplyToAllItem**要素には、Exchange ストア内のアイテムの識別されたすべての受信者と送信者への返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-104">The **ReplyToAllItem** element contains a reply to the sender and all identified recipients of an item in the Exchange store.</span></span> 
  
```xml
<ReplyAllToItem>
   <Subject/>
   <Body/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <From/>
   <ReferenceItemId/>
   <NewBodyContent/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
</ReplyAllToItem>
```

 <span data-ttu-id="ff5e3-105">**ReplyAllToItemType**</span><span class="sxs-lookup"><span data-stu-id="ff5e3-105">**ReplyAllToItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff5e3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ff5e3-106">Attributes and elements</span></span>

<span data-ttu-id="ff5e3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff5e3-108">属性</span><span class="sxs-lookup"><span data-stu-id="ff5e3-108">Attributes</span></span>

<span data-ttu-id="ff5e3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff5e3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ff5e3-110">Child elements</span></span>

|<span data-ttu-id="ff5e3-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="ff5e3-111">**Element**</span></span>|<span data-ttu-id="ff5e3-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ff5e3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff5e3-113">Subject</span><span class="sxs-lookup"><span data-stu-id="ff5e3-113">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="ff5e3-114">Exchange ストアのアイテムの subject プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-114">Represents the subject property of Exchange store items.</span></span>  <br/> |
|[<span data-ttu-id="ff5e3-115">Body/本文</span><span class="sxs-lookup"><span data-stu-id="ff5e3-115">Body</span></span>](body.md) <br/> |<span data-ttu-id="ff5e3-116">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-116">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="ff5e3-117">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="ff5e3-117">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="ff5e3-118">アイテムの受信者のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-118">Contains a set of recipients of an item.</span></span> <span data-ttu-id="ff5e3-119">これらは、アイテムの主な受信者です。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-119">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="ff5e3-120">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="ff5e3-120">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="ff5e3-121">メッセージのコピーを受け取る受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-121">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="ff5e3-122">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="ff5e3-122">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="ff5e3-123">電子メール メッセージのブラインド カーボン コピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-123">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="ff5e3-124">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="ff5e3-124">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="ff5e3-125">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-125">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="ff5e3-126">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="ff5e3-126">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="ff5e3-127">アイテムの送信者が配信済みメッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-127">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="ff5e3-128">From</span><span class="sxs-lookup"><span data-stu-id="ff5e3-128">From</span></span>](from.md) <br/> |<span data-ttu-id="ff5e3-129">メッセージの送信元アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-129">Represents the address from which the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="ff5e3-130">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="ff5e3-130">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="ff5e3-131">応答オブジェクトが参照する項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-131">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="ff5e3-132">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="ff5e3-132">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="ff5e3-133">メッセージの新しい本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-133">Represents the new body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="ff5e3-134">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="ff5e3-134">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="ff5e3-135">代理人アクセス シナリオでは、デリゲートを識別します。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-135">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="ff5e3-136">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-136">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="ff5e3-137">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="ff5e3-137">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="ff5e3-138">代理人アクセスのシナリオでプリンシパルを識別します。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-138">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="ff5e3-139">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-139">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ff5e3-140">親要素</span><span class="sxs-lookup"><span data-stu-id="ff5e3-140">Parent elements</span></span>

|<span data-ttu-id="ff5e3-141">**要素**</span><span class="sxs-lookup"><span data-stu-id="ff5e3-141">**Element**</span></span>|<span data-ttu-id="ff5e3-142">**説明**</span><span class="sxs-lookup"><span data-stu-id="ff5e3-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff5e3-143">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="ff5e3-143">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="ff5e3-144">会議の時刻に隣接しているすべての項目について説明します。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-144">Describes all items that are adjacent to a meeting time.</span></span>  <br/><br/>  <span data-ttu-id="ff5e3-145">以下は、この要素への XPath 式の一部です。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-145">The following are some of the XPath expressions to this element:</span></span>  <br/><br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="ff5e3-146">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="ff5e3-146">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="ff5e3-147">会議の時間と競合するすべての項目について説明します。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-147">Describes all items that conflict with a meeting time.</span></span>  <br/><br/>  <span data-ttu-id="ff5e3-148">以下は、この要素への XPath 式の一部です。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-148">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="ff5e3-149">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="ff5e3-149">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="ff5e3-150">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-150">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ff5e3-151">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="ff5e3-151">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="ff5e3-152">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で指定されたフォルダーに作成する項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-152">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ff5e3-153">備考</span><span class="sxs-lookup"><span data-stu-id="ff5e3-153">Remarks</span></span>

<span data-ttu-id="ff5e3-154">要素[から](from.md)設定してください、プリンシパルの電子メール アドレスにアイテムが返信の場合代理人によって。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-154">The [From](from.md) element should be set to the e-mail address of the principal if an item is a reply by a delegate.</span></span> <span data-ttu-id="ff5e3-155">代理人が、 [From](from.md)プロパティを設定していない場合、代理人のメールボックスから直接送信されたアイテムが表示されます。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-155">If the delegate does not set the [From](from.md) property, the item will appear to have been sent directly from the delegate's mailbox.</span></span> 
  
<span data-ttu-id="ff5e3-156">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="ff5e3-156">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff5e3-157">要素情報</span><span class="sxs-lookup"><span data-stu-id="ff5e3-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff5e3-158">名前空間</span><span class="sxs-lookup"><span data-stu-id="ff5e3-158">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ff5e3-159">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ff5e3-159">Schema Name</span></span>  <br/> |<span data-ttu-id="ff5e3-160">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ff5e3-160">Types schema</span></span>  <br/> |
|<span data-ttu-id="ff5e3-161">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ff5e3-161">Validation File</span></span>  <br/> |<span data-ttu-id="ff5e3-162">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ff5e3-162">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ff5e3-163">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ff5e3-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="ff5e3-164">False</span><span class="sxs-lookup"><span data-stu-id="ff5e3-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff5e3-165">関連項目</span><span class="sxs-lookup"><span data-stu-id="ff5e3-165">See also</span></span>

- [<span data-ttu-id="ff5e3-166">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ff5e3-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


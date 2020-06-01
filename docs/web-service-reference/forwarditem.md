---
title: Forwarditem と
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ForwardItem
api_type:
- schema
ms.assetid: 97786086-8b91-4471-8af8-d21e8d66de87
description: Forwarditem と要素には、受信者に転送するための Exchange ストアアイテムが含まれています。
ms.openlocfilehash: dcc9a3eb2bf1cdd80680ef9142d22f5281437922
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461318"
---
# <a name="forwarditem"></a><span data-ttu-id="6ef5b-103">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="6ef5b-103">ForwardItem</span></span>

<span data-ttu-id="6ef5b-104">**Forwarditem と**要素には、受信者に転送するための Exchange ストアアイテムが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-104">The **ForwardItem** element contains an Exchange store item to forward to recipients.</span></span> 
  
```xml
<ForwardItem>
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
</ForwardItem>
```

<span data-ttu-id="6ef5b-105">**ForwardItemType**</span><span class="sxs-lookup"><span data-stu-id="6ef5b-105">**ForwardItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6ef5b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6ef5b-106">Attributes and elements</span></span>

<span data-ttu-id="6ef5b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ef5b-108">属性</span><span class="sxs-lookup"><span data-stu-id="6ef5b-108">Attributes</span></span>

<span data-ttu-id="6ef5b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6ef5b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6ef5b-110">Child elements</span></span>

|<span data-ttu-id="6ef5b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="6ef5b-111">**Element**</span></span>|<span data-ttu-id="6ef5b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6ef5b-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6ef5b-113">[[件名]](subject.md)</span><span class="sxs-lookup"><span data-stu-id="6ef5b-113">[Subject](subject.md)</span></span> <br/> |<span data-ttu-id="6ef5b-114">Exchange ストアアイテムの subject プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-114">Represents the subject property of Exchange store items.</span></span>  <br/> |
|[<span data-ttu-id="6ef5b-115">Body</span><span class="sxs-lookup"><span data-stu-id="6ef5b-115">Body</span></span>](body.md) <br/> |<span data-ttu-id="6ef5b-116">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-116">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="6ef5b-117">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="6ef5b-117">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="6ef5b-118">アイテムの受信者のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-118">Contains a set of recipients of an item.</span></span> <span data-ttu-id="6ef5b-119">次に、アイテムのプライマリ受信者を示します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-119">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="6ef5b-120">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="6ef5b-120">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="6ef5b-121">メッセージのコピーを受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-121">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="6ef5b-122">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="6ef5b-122">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="6ef5b-123">電子メールのブラインドカーボンコピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-123">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="6ef5b-124">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="6ef5b-124">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="6ef5b-125">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-125">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="6ef5b-126">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="6ef5b-126">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="6ef5b-127">アイテムの送信者が配信確認を要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-127">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="6ef5b-128">From</span><span class="sxs-lookup"><span data-stu-id="6ef5b-128">From</span></span>](from.md) <br/> |<span data-ttu-id="6ef5b-129">メッセージの送信元のアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-129">Represents the address from which the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="6ef5b-130">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="6ef5b-130">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="6ef5b-131">Response オブジェクトが参照するアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-131">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="6ef5b-132">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="6ef5b-132">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="6ef5b-133">メッセージの新しい本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-133">Represents the new body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="6ef5b-134">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="6ef5b-134">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="6ef5b-135">代理人アクセスシナリオの代理人を識別します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-135">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="6ef5b-136">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-136">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="6ef5b-137">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="6ef5b-137">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="6ef5b-138">代理人アクセスシナリオのプリンシパルを識別します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-138">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="6ef5b-139">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-139">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6ef5b-140">親要素</span><span class="sxs-lookup"><span data-stu-id="6ef5b-140">Parent elements</span></span>

|<span data-ttu-id="6ef5b-141">**要素**</span><span class="sxs-lookup"><span data-stu-id="6ef5b-141">**Element**</span></span>|<span data-ttu-id="6ef5b-142">**説明**</span><span class="sxs-lookup"><span data-stu-id="6ef5b-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ef5b-143">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="6ef5b-143">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="6ef5b-144">会議の時刻に隣接しているすべてのアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-144">Describes all items that are adjacent to a meeting time.</span></span>  <br/><br/>  <span data-ttu-id="6ef5b-145">この要素の XPath 式の一部を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-145">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="6ef5b-146">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="6ef5b-146">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="6ef5b-147">会議の時間と競合するすべてのアイテムについて説明します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-147">Describes all items that conflict with a meeting time.</span></span>  <br/><br/>  <span data-ttu-id="6ef5b-148">この要素の XPath 式の一部を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-148">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="6ef5b-149">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="6ef5b-149">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="6ef5b-150">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-150">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6ef5b-151">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="6ef5b-151">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="6ef5b-152">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-152">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6ef5b-153">注釈</span><span class="sxs-lookup"><span data-stu-id="6ef5b-153">Remarks</span></span>

<span data-ttu-id="6ef5b-154">アイテムが代理人によって転送される場合、 [From](from.md)要素はプリンシパルの電子メールアドレスに設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-154">The [From](from.md) element should be set to the e-mail address of the principal if an item is forwarded by a delegate.</span></span> <span data-ttu-id="6ef5b-155">代理人が[From](from.md)プロパティを設定しない場合、アイテムは代理人のメールボックスから直接送信されたように表示されます。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-155">If the delegate does not set the [From](from.md) property, the item will appear to have been sent directly from the delegate's mailbox.</span></span> 
  
<span data-ttu-id="6ef5b-156">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="6ef5b-156">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6ef5b-157">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6ef5b-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ef5b-158">Namespace</span><span class="sxs-lookup"><span data-stu-id="6ef5b-158">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6ef5b-159">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6ef5b-159">Schema Name</span></span>  <br/> |<span data-ttu-id="6ef5b-160">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6ef5b-160">Types schema</span></span>  <br/> |
|<span data-ttu-id="6ef5b-161">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6ef5b-161">Validation File</span></span>  <br/> |<span data-ttu-id="6ef5b-162">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6ef5b-162">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6ef5b-163">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6ef5b-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="6ef5b-164">正しくない</span><span class="sxs-lookup"><span data-stu-id="6ef5b-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6ef5b-165">関連項目</span><span class="sxs-lookup"><span data-stu-id="6ef5b-165">See also</span></span>

- [<span data-ttu-id="6ef5b-166">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6ef5b-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


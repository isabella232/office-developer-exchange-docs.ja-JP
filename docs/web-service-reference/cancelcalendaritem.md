---
title: CancelCalendarItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CancelCalendarItem
api_type:
- schema
ms.assetid: a2046402-a176-44d5-b4b3-adb696581935
description: CancelCalendarItem 要素は、会議の取り消しに使用される response オブジェクトを表します。
ms.openlocfilehash: 45ad76d19bd43e2081aa9b9eb63547e091014803
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462256"
---
# <a name="cancelcalendaritem"></a><span data-ttu-id="36c8c-103">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="36c8c-103">CancelCalendarItem</span></span>

<span data-ttu-id="36c8c-104">**Cancelcalendaritem**要素は、会議の取り消しに使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-104">The **CancelCalendarItem** element represents the response object that is used to cancel a meeting.</span></span> 
  
```xml
<CancelCalendarItem>
   <Subject/>
   <Body/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ReferenceItemId/>
   <NewBodyContent/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
</CancelCalendarItem>
```

 <span data-ttu-id="36c8c-105">**CancelCalendarItemType**</span><span class="sxs-lookup"><span data-stu-id="36c8c-105">**CancelCalendarItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36c8c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="36c8c-106">Attributes and elements</span></span>

<span data-ttu-id="36c8c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36c8c-108">属性</span><span class="sxs-lookup"><span data-stu-id="36c8c-108">Attributes</span></span>

<span data-ttu-id="36c8c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="36c8c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36c8c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="36c8c-110">Child elements</span></span>

|<span data-ttu-id="36c8c-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="36c8c-111">**Element**</span></span>|<span data-ttu-id="36c8c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="36c8c-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="36c8c-113">[[件名]](subject.md)</span><span class="sxs-lookup"><span data-stu-id="36c8c-113">[Subject](subject.md)</span></span> <br/> |<span data-ttu-id="36c8c-114">Exchange ストアアイテムの subject プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-114">Represents the subject property of Exchange store items.</span></span>  <br/> |
|[<span data-ttu-id="36c8c-115">Body</span><span class="sxs-lookup"><span data-stu-id="36c8c-115">Body</span></span>](body.md) <br/> |<span data-ttu-id="36c8c-116">**Cancelcalendaritem**では使用されません。</span><span class="sxs-lookup"><span data-stu-id="36c8c-116">Not used by **CancelCalendarItem**.</span></span> <span data-ttu-id="36c8c-117">本文のコンテンツを設定するには、 [Newbodycontent](newbodycontent.md)プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-117">Use the [NewBodyContent](newbodycontent.md) property to set the body content.</span></span>  <br/> |
|[<span data-ttu-id="36c8c-118">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="36c8c-118">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="36c8c-119">アイテムの受信者のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="36c8c-119">Contains a set of recipients of an item.</span></span> <span data-ttu-id="36c8c-120">次に、アイテムのプライマリ受信者を示します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-120">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="36c8c-121">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="36c8c-121">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="36c8c-122">メッセージのコピーを受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-122">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="36c8c-123">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="36c8c-123">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="36c8c-124">電子メールのブラインドカーボンコピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-124">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="36c8c-125">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="36c8c-125">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="36c8c-126">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-126">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="36c8c-127">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="36c8c-127">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="36c8c-128">アイテムの送信者が配信確認を要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-128">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="36c8c-129">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="36c8c-129">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="36c8c-130">Response オブジェクトが参照するアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-130">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="36c8c-131">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="36c8c-131">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="36c8c-132">メッセージの新しい本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-132">Represents the new body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="36c8c-133">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="36c8c-133">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="36c8c-134">代理人アクセスシナリオの代理人を識別します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-134">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="36c8c-135">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="36c8c-135">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="36c8c-136">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="36c8c-136">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="36c8c-137">代理人アクセスシナリオのプリンシパルを識別します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-137">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="36c8c-138">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="36c8c-138">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="36c8c-139">親要素</span><span class="sxs-lookup"><span data-stu-id="36c8c-139">Parent elements</span></span>

|<span data-ttu-id="36c8c-140">**要素**</span><span class="sxs-lookup"><span data-stu-id="36c8c-140">**Element**</span></span>|<span data-ttu-id="36c8c-141">**説明**</span><span class="sxs-lookup"><span data-stu-id="36c8c-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36c8c-142">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="36c8c-142">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="36c8c-143">会議の時刻に隣接しているすべてのアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-143">Describes all items that are adjacent to a meeting time.</span></span><br/><br/> <span data-ttu-id="36c8c-144">この要素の XPath 式の一部を次に示します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-144">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="36c8c-145">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="36c8c-145">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="36c8c-146">会議の時間と競合するすべてのアイテムについて説明します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-146">Describes all items that conflict with a meeting time.</span></span><br/><br/><span data-ttu-id="36c8c-147">この要素の XPath 式の一部を次に示します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-147">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="36c8c-148">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="36c8c-148">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="36c8c-149">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-149">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="36c8c-150">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="36c8c-150">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="36c8c-151">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="36c8c-151">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="36c8c-152">注釈</span><span class="sxs-lookup"><span data-stu-id="36c8c-152">Remarks</span></span>

<span data-ttu-id="36c8c-153">**Cancelcalendaritem**要素は、開催者によってのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="36c8c-153">The **CancelCalendarItem** element is only viewed by the organizer.</span></span> <span data-ttu-id="36c8c-154">開催者の予定表アイテムにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="36c8c-154">It only applies to the organizer's calendar item.</span></span> 
  
<span data-ttu-id="36c8c-155">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="36c8c-155">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36c8c-156">要素の情報</span><span class="sxs-lookup"><span data-stu-id="36c8c-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36c8c-157">Namespace</span><span class="sxs-lookup"><span data-stu-id="36c8c-157">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36c8c-158">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="36c8c-158">Schema Name</span></span>  <br/> |<span data-ttu-id="36c8c-159">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="36c8c-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="36c8c-160">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="36c8c-160">Validation File</span></span>  <br/> |<span data-ttu-id="36c8c-161">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="36c8c-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="36c8c-162">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="36c8c-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="36c8c-163">正しくない</span><span class="sxs-lookup"><span data-stu-id="36c8c-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36c8c-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="36c8c-164">See also</span></span>

- [<span data-ttu-id="36c8c-165">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="36c8c-165">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


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
description: CancelCalendarItem 要素は、会議をキャンセルするために使用される応答オブジェクトを表します。
ms.openlocfilehash: 262f60db33abac36156b069dc85e1fccb3522d5b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759606"
---
# <a name="cancelcalendaritem"></a><span data-ttu-id="f4cde-103">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="f4cde-103">CancelCalendarItem</span></span>

<span data-ttu-id="f4cde-104">**CancelCalendarItem**要素は、会議をキャンセルするために使用される応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="f4cde-104">The **CancelCalendarItem** element represents the response object that is used to cancel a meeting.</span></span> 
  
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

 <span data-ttu-id="f4cde-105">**CancelCalendarItemType**</span><span class="sxs-lookup"><span data-stu-id="f4cde-105">**CancelCalendarItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4cde-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f4cde-106">Attributes and elements</span></span>

<span data-ttu-id="f4cde-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f4cde-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4cde-108">属性</span><span class="sxs-lookup"><span data-stu-id="f4cde-108">Attributes</span></span>

<span data-ttu-id="f4cde-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f4cde-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4cde-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f4cde-110">Child elements</span></span>

|<span data-ttu-id="f4cde-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="f4cde-111">**Element**</span></span>|<span data-ttu-id="f4cde-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f4cde-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4cde-113">Subject</span><span class="sxs-lookup"><span data-stu-id="f4cde-113">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="f4cde-114">Exchange ストアのアイテムの subject プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="f4cde-114">Represents the subject property of Exchange store items.</span></span>  <br/> |
|[<span data-ttu-id="f4cde-115">Body/本文</span><span class="sxs-lookup"><span data-stu-id="f4cde-115">Body</span></span>](body.md) <br/> |<span data-ttu-id="f4cde-116">**CancelCalendarItem**では使用されません。</span><span class="sxs-lookup"><span data-stu-id="f4cde-116">Not used by **CancelCalendarItem**.</span></span> <span data-ttu-id="f4cde-117">本文の内容を設定するのには、 [NewBodyContent](newbodycontent.md)プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="f4cde-117">Use the [NewBodyContent](newbodycontent.md) property to set the body content.</span></span>  <br/> |
|[<span data-ttu-id="f4cde-118">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="f4cde-118">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="f4cde-119">アイテムの受信者のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f4cde-119">Contains a set of recipients of an item.</span></span> <span data-ttu-id="f4cde-120">これらは、アイテムの主な受信者です。</span><span class="sxs-lookup"><span data-stu-id="f4cde-120">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="f4cde-121">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="f4cde-121">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="f4cde-122">メッセージのコピーを受け取る受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="f4cde-122">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="f4cde-123">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="f4cde-123">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="f4cde-124">電子メールのブラインド カーボン コピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="f4cde-124">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="f4cde-125">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="f4cde-125">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="f4cde-126">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f4cde-126">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="f4cde-127">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="f4cde-127">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="f4cde-128">アイテムの送信者が配信済みメッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f4cde-128">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="f4cde-129">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="f4cde-129">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="f4cde-130">応答オブジェクトが参照する項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="f4cde-130">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="f4cde-131">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="f4cde-131">NewBodyContent</span></span>](newbodycontent.md) <br/> |<span data-ttu-id="f4cde-132">メッセージの新しい本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="f4cde-132">Represents the new body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="f4cde-133">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="f4cde-133">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="f4cde-134">代理人アクセス シナリオでは、デリゲートを識別します。</span><span class="sxs-lookup"><span data-stu-id="f4cde-134">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="f4cde-135">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f4cde-135">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="f4cde-136">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="f4cde-136">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="f4cde-137">代理人アクセスのシナリオでプリンシパルを識別します。</span><span class="sxs-lookup"><span data-stu-id="f4cde-137">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="f4cde-138">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f4cde-138">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f4cde-139">親要素</span><span class="sxs-lookup"><span data-stu-id="f4cde-139">Parent elements</span></span>

|<span data-ttu-id="f4cde-140">**要素**</span><span class="sxs-lookup"><span data-stu-id="f4cde-140">**Element**</span></span>|<span data-ttu-id="f4cde-141">**説明**</span><span class="sxs-lookup"><span data-stu-id="f4cde-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4cde-142">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="f4cde-142">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="f4cde-143">会議の時刻に隣接しているすべての項目について説明します。</span><span class="sxs-lookup"><span data-stu-id="f4cde-143">Describes all items that are adjacent to a meeting time.</span></span><br/><br/> <span data-ttu-id="f4cde-144">以下は、この要素への XPath 式の一部です。</span><span class="sxs-lookup"><span data-stu-id="f4cde-144">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="f4cde-145">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="f4cde-145">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="f4cde-146">会議の時間と競合するすべての項目について説明します。</span><span class="sxs-lookup"><span data-stu-id="f4cde-146">Describes all items that conflict with a meeting time.</span></span><br/><br/><span data-ttu-id="f4cde-147">以下は、この要素への XPath 式の一部です。</span><span class="sxs-lookup"><span data-stu-id="f4cde-147">The following are some of the XPath expressions to this element:</span></span><br/><br/>`/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="f4cde-148">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="f4cde-148">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="f4cde-149">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f4cde-149">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f4cde-150">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="f4cde-150">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="f4cde-151">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で指定されたフォルダーに作成する項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f4cde-151">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f4cde-152">備考</span><span class="sxs-lookup"><span data-stu-id="f4cde-152">Remarks</span></span>

<span data-ttu-id="f4cde-153">**CancelCalendarItem**要素は、開催者によってのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="f4cde-153">The **CancelCalendarItem** element is only viewed by the organizer.</span></span> <span data-ttu-id="f4cde-154">開催者の予定表アイテムにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="f4cde-154">It only applies to the organizer's calendar item.</span></span> 
  
<span data-ttu-id="f4cde-155">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="f4cde-155">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4cde-156">要素情報</span><span class="sxs-lookup"><span data-stu-id="f4cde-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4cde-157">名前空間</span><span class="sxs-lookup"><span data-stu-id="f4cde-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f4cde-158">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f4cde-158">Schema Name</span></span>  <br/> |<span data-ttu-id="f4cde-159">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f4cde-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="f4cde-160">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f4cde-160">Validation File</span></span>  <br/> |<span data-ttu-id="f4cde-161">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f4cde-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f4cde-162">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f4cde-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="f4cde-163">False</span><span class="sxs-lookup"><span data-stu-id="f4cde-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f4cde-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="f4cde-164">See also</span></span>

- [<span data-ttu-id="f4cde-165">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f4cde-165">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


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
description: AcceptItem 要素は、会議出席依頼、承諾の返信を表します。
ms.openlocfilehash: 532862fc5299364e51ed469047deaea058692e83
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760448"
---
# <a name="acceptitem"></a><span data-ttu-id="7239b-103">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="7239b-103">AcceptItem</span></span>

<span data-ttu-id="7239b-104">**AcceptItem**要素は、会議出席依頼、承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="7239b-104">The **AcceptItem** element represents an Accept reply to a meeting request.</span></span> 
  
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

 <span data-ttu-id="7239b-105">**AcceptItemType**</span><span class="sxs-lookup"><span data-stu-id="7239b-105">**AcceptItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7239b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7239b-106">Attributes and elements</span></span>

<span data-ttu-id="7239b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7239b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7239b-108">属性</span><span class="sxs-lookup"><span data-stu-id="7239b-108">Attributes</span></span>

<span data-ttu-id="7239b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7239b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7239b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7239b-110">Child elements</span></span>

|<span data-ttu-id="7239b-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="7239b-111">**Element**</span></span>|<span data-ttu-id="7239b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7239b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7239b-113">ItemClass</span><span class="sxs-lookup"><span data-stu-id="7239b-113">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="7239b-114">アイテムのメッセージ クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="7239b-114">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="7239b-115">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="7239b-115">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="7239b-116">アイテムの秘密度レベルを示します。</span><span class="sxs-lookup"><span data-stu-id="7239b-116">Indicates the sensitivity level of an item.</span></span>  <br/> |
|[<span data-ttu-id="7239b-117">Body/本文</span><span class="sxs-lookup"><span data-stu-id="7239b-117">Body</span></span>](body.md) <br/> |<span data-ttu-id="7239b-118">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="7239b-118">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="7239b-119">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="7239b-119">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7239b-120">アイテムまたは Exchange ストア内のアイテムに関連付けられているファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7239b-120">Contains the item or file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7239b-121">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="7239b-121">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="7239b-122">ヘッダー コレクション内の指定したヘッダーのインターネット メッセージ ヘッダーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="7239b-122">Represents the Internet message header name for a given header within the headers collection.</span></span>  <br/> |
|[<span data-ttu-id="7239b-123">送信者</span><span class="sxs-lookup"><span data-stu-id="7239b-123">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="7239b-124">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="7239b-124">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="7239b-125">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="7239b-125">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="7239b-126">アイテムの受信者のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7239b-126">Contains a set of recipients of an item.</span></span> <span data-ttu-id="7239b-127">これらは、アイテムの主な受信者です。</span><span class="sxs-lookup"><span data-stu-id="7239b-127">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="7239b-128">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="7239b-128">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="7239b-129">メッセージのコピーを受け取る受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="7239b-129">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="7239b-130">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="7239b-130">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="7239b-131">電子メールのブラインド カーボン コピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="7239b-131">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="7239b-132">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="7239b-132">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="7239b-133">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7239b-133">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="7239b-134">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="7239b-134">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="7239b-135">アイテムの送信者が配信済みメッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7239b-135">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="7239b-136">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="7239b-136">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="7239b-137">応答オブジェクトが参照する項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="7239b-137">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="7239b-138">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="7239b-138">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="7239b-139">代理人アクセス シナリオでは、デリゲートを識別します。</span><span class="sxs-lookup"><span data-stu-id="7239b-139">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="7239b-140">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7239b-140">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="7239b-141">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="7239b-141">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="7239b-142">代理人アクセスのシナリオでプリンシパルを識別します。</span><span class="sxs-lookup"><span data-stu-id="7239b-142">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="7239b-143">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7239b-143">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="7239b-144">ProposedStart</span><span class="sxs-lookup"><span data-stu-id="7239b-144">ProposedStart</span></span>](proposedstart.md) <br/> |<span data-ttu-id="7239b-145">会議の提案した開始時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="7239b-145">Specifies the proposed start time of the meeting.</span></span>  <br/> |
|[<span data-ttu-id="7239b-146">ProposedEnd</span><span class="sxs-lookup"><span data-stu-id="7239b-146">ProposedEnd</span></span>](proposedend.md) <br/> |<span data-ttu-id="7239b-147">会議の提案した終了時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="7239b-147">Specifies the proposed end time of the meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7239b-148">親要素</span><span class="sxs-lookup"><span data-stu-id="7239b-148">Parent elements</span></span>

|<span data-ttu-id="7239b-149">**要素**</span><span class="sxs-lookup"><span data-stu-id="7239b-149">**Element**</span></span>|<span data-ttu-id="7239b-150">**説明**</span><span class="sxs-lookup"><span data-stu-id="7239b-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7239b-151">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="7239b-151">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="7239b-152">会議の時刻に隣接しているすべての項目について説明します。</span><span class="sxs-lookup"><span data-stu-id="7239b-152">Describes all items that are adjacent to a meeting time.</span></span><br/><br/>  <span data-ttu-id="7239b-153">以下は、この要素への XPath 式の一部です。</span><span class="sxs-lookup"><span data-stu-id="7239b-153">The following are some of the XPath expressions to this element:</span></span><br/><br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="7239b-154">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="7239b-154">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="7239b-155">会議の時間と競合するすべての項目について説明します。</span><span class="sxs-lookup"><span data-stu-id="7239b-155">Describes all items that conflict with a meeting time.</span></span><br/><br/>  <span data-ttu-id="7239b-156">以下は、この要素への XPath 式の一部です。</span><span class="sxs-lookup"><span data-stu-id="7239b-156">The following are some of the XPath expressions to this element:</span></span><br/><br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="7239b-157">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="7239b-157">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="7239b-158">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7239b-158">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7239b-159">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="7239b-159">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="7239b-160">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で指定されたフォルダーに作成する項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7239b-160">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7239b-161">備考</span><span class="sxs-lookup"><span data-stu-id="7239b-161">Remarks</span></span>

<span data-ttu-id="7239b-162">この要素を記述するスキーマは、EWS のディレクトリにあるクライアント アクセス サーバーの役割がインストールされている Exchange サーバーです。</span><span class="sxs-lookup"><span data-stu-id="7239b-162">The schema that describes this element is located in the EWS directory of the Exchange server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7239b-163">要素情報</span><span class="sxs-lookup"><span data-stu-id="7239b-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7239b-164">名前空間</span><span class="sxs-lookup"><span data-stu-id="7239b-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7239b-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7239b-165">Schema Name</span></span>  <br/> |<span data-ttu-id="7239b-166">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7239b-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="7239b-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7239b-167">Validation File</span></span>  <br/> |<span data-ttu-id="7239b-168">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7239b-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7239b-169">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7239b-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="7239b-170">False</span><span class="sxs-lookup"><span data-stu-id="7239b-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7239b-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="7239b-171">See also</span></span>

- [<span data-ttu-id="7239b-172">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7239b-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


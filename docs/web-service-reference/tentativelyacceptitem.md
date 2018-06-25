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
description: TentativelyAcceptItem 要素は、会議出席依頼に返信する、仮の予定を表します。
ms.openlocfilehash: 203028aae2ec972e36209b2a97420e83d61ddd81
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839671"
---
# <a name="tentativelyacceptitem"></a><span data-ttu-id="ae310-103">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="ae310-103">TentativelyAcceptItem</span></span>

<span data-ttu-id="ae310-104">**TentativelyAcceptItem**要素は、会議出席依頼に返信する、仮の予定を表します。</span><span class="sxs-lookup"><span data-stu-id="ae310-104">The **TentativelyAcceptItem** element represents a Tentative reply to a meeting request.</span></span> 
  
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

 <span data-ttu-id="ae310-105">**TentativelyAcceptItemType**</span><span class="sxs-lookup"><span data-stu-id="ae310-105">**TentativelyAcceptItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ae310-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ae310-106">Attributes and elements</span></span>

<span data-ttu-id="ae310-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ae310-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae310-108">属性</span><span class="sxs-lookup"><span data-stu-id="ae310-108">Attributes</span></span>

<span data-ttu-id="ae310-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ae310-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae310-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ae310-110">Child elements</span></span>

|<span data-ttu-id="ae310-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="ae310-111">**Element**</span></span>|<span data-ttu-id="ae310-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ae310-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae310-113">ItemClass</span><span class="sxs-lookup"><span data-stu-id="ae310-113">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="ae310-114">アイテムのメッセージ クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="ae310-114">Represents the message class of an item.</span></span>  <br/> |
|[<span data-ttu-id="ae310-115">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="ae310-115">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="ae310-116">アイテムの秘密度を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae310-116">Identifies the sensitivity of an item.</span></span>  <br/> |
|[<span data-ttu-id="ae310-117">Body/本文</span><span class="sxs-lookup"><span data-stu-id="ae310-117">Body</span></span>](body.md) <br/> |<span data-ttu-id="ae310-118">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="ae310-118">Represents the actual body content of a message.</span></span>  <br/> |
|[<span data-ttu-id="ae310-119">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="ae310-119">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ae310-120">アイテムまたは Exchange ストア内のアイテムに関連付けられているファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ae310-120">Contains the item or file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ae310-121">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="ae310-121">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="ae310-122">ヘッダー コレクション内の指定したヘッダーのインターネット メッセージ ヘッダーの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="ae310-122">Represents the Internet message header name for a given header within the headers collection.</span></span>  <br/> |
|[<span data-ttu-id="ae310-123">送信者</span><span class="sxs-lookup"><span data-stu-id="ae310-123">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="ae310-124">アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="ae310-124">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="ae310-125">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="ae310-125">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="ae310-126">アイテムの受信者のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ae310-126">Contains a set of recipients of an item.</span></span> <span data-ttu-id="ae310-127">これらは、アイテムの主な受信者です。</span><span class="sxs-lookup"><span data-stu-id="ae310-127">These are the primary recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="ae310-128">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="ae310-128">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="ae310-129">メッセージのコピーを受け取る受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ae310-129">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="ae310-130">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="ae310-130">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="ae310-131">電子メールのブラインド カーボン コピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="ae310-131">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="ae310-132">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="ae310-132">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md) <br/> |<span data-ttu-id="ae310-133">アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ae310-133">Indicates whether the sender of an item requests a read receipt.</span></span>  <br/> |
|[<span data-ttu-id="ae310-134">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="ae310-134">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md) <br/> |<span data-ttu-id="ae310-135">アイテムの送信者が配信済みメッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ae310-135">Indicates whether the sender of an item requests a delivery receipt.</span></span>  <br/> |
|[<span data-ttu-id="ae310-136">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="ae310-136">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="ae310-137">応答オブジェクトが参照する項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="ae310-137">Identifies the item to which the response object refers.</span></span>  <br/> |
|[<span data-ttu-id="ae310-138">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="ae310-138">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="ae310-139">代理人アクセス シナリオでは、デリゲートを識別します。</span><span class="sxs-lookup"><span data-stu-id="ae310-139">Identifies the delegate in a delegate access scenario.</span></span> <span data-ttu-id="ae310-140">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ae310-140">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="ae310-141">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="ae310-141">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="ae310-142">代理人アクセスのシナリオでプリンシパルを識別します。</span><span class="sxs-lookup"><span data-stu-id="ae310-142">Identifies the principal in a delegate access scenario.</span></span> <span data-ttu-id="ae310-143">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ae310-143">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="ae310-144">ProposedStart</span><span class="sxs-lookup"><span data-stu-id="ae310-144">ProposedStart</span></span>](proposedstart.md) <br/> |<span data-ttu-id="ae310-145">会議出席依頼の提案された開始時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae310-145">Specifies the proposed start time of the meeting request.</span></span>  <br/> |
|[<span data-ttu-id="ae310-146">ProposedEnd</span><span class="sxs-lookup"><span data-stu-id="ae310-146">ProposedEnd</span></span>](proposedend.md) <br/> |<span data-ttu-id="ae310-147">会議出席依頼の提案した終了時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae310-147">Specifies the proposed end time of the meeting request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ae310-148">親要素</span><span class="sxs-lookup"><span data-stu-id="ae310-148">Parent elements</span></span>

|<span data-ttu-id="ae310-149">**要素**</span><span class="sxs-lookup"><span data-stu-id="ae310-149">**Element**</span></span>|<span data-ttu-id="ae310-150">**説明**</span><span class="sxs-lookup"><span data-stu-id="ae310-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae310-151">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="ae310-151">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="ae310-152">会議の時刻に隣接しているすべての項目について説明します。</span><span class="sxs-lookup"><span data-stu-id="ae310-152">Describes all items that are adjacent to a meeting time.</span></span>  <br/> <br/> <span data-ttu-id="ae310-153">以下は、この要素への XPath 式の一部です。</span><span class="sxs-lookup"><span data-stu-id="ae310-153">The following are some of the XPath expressions to this element:</span></span>  <br/><br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="ae310-154">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="ae310-154">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="ae310-155">会議の時間と競合するすべての項目について説明します。</span><span class="sxs-lookup"><span data-stu-id="ae310-155">Describes all items that conflict with a meeting time.</span></span> <br/> <br/>  <span data-ttu-id="ae310-156">以下は、この要素への XPath 式の一部です。</span><span class="sxs-lookup"><span data-stu-id="ae310-156">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="ae310-157">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="ae310-157">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="ae310-158">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ae310-158">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ae310-159">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="ae310-159">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="ae310-160">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で指定されたフォルダーに作成する項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ae310-160">Contains an array of items to create in the folder identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ae310-161">備考</span><span class="sxs-lookup"><span data-stu-id="ae310-161">Remarks</span></span>

<span data-ttu-id="ae310-162">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="ae310-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae310-163">要素情報</span><span class="sxs-lookup"><span data-stu-id="ae310-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae310-164">名前空間</span><span class="sxs-lookup"><span data-stu-id="ae310-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ae310-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ae310-165">Schema Name</span></span>  <br/> |<span data-ttu-id="ae310-166">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ae310-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="ae310-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ae310-167">Validation File</span></span>  <br/> |<span data-ttu-id="ae310-168">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ae310-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ae310-169">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ae310-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="ae310-170">False</span><span class="sxs-lookup"><span data-stu-id="ae310-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ae310-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="ae310-171">See also</span></span>

- [<span data-ttu-id="ae310-172">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ae310-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


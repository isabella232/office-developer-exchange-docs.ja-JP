---
title: アイテム (NonEmptyArrayOfAllItemsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Items
api_type:
- schema
ms.assetid: d61ef1cc-ddfc-480a-9625-7b436cb33ae0
description: 項目要素には、作成するアイテムのセットが含まれています。
ms.openlocfilehash: 3b1ce7092bb6d37f23792fbf1ecb1f77b63f2afd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832160"
---
# <a name="items-nonemptyarrayofallitemstype"></a><span data-ttu-id="623fb-103">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="623fb-103">Items (NonEmptyArrayOfAllItemsType)</span></span>

<span data-ttu-id="623fb-104">**項目**要素には、作成するアイテムのセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="623fb-104">The **Items** element contains a set of items to create.</span></span> 
  
```XML
<Items>
   <Item/>
   <Message/>
   <CalendarItem/>
   <Contact/>
   <DistributionList/>
   <MeetingMessage/>
   <MeetingRequest/>
   <MeetingResponse/>
   <MeetingCancellation/>
   <Task/>
   <ReplyToItem/>
   <ForwardItem/>
   <ReplyAllToItem/>
   <AcceptItem/>
   <TentativelyAcceptItem/>
   <DeclineItem/>
   <CancelCalendarItem/>
   <RemoveItem/>
   <PostReplyItem/>
   <SuppressReadReceipt/>
   <AcceptSharingInvitation/>
</Items>
```

 <span data-ttu-id="623fb-105">**NonEmptyArrayOfAllItemsType**</span><span class="sxs-lookup"><span data-stu-id="623fb-105">**NonEmptyArrayOfAllItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="623fb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="623fb-106">Attributes and elements</span></span>

<span data-ttu-id="623fb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="623fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="623fb-108">属性</span><span class="sxs-lookup"><span data-stu-id="623fb-108">Attributes</span></span>

<span data-ttu-id="623fb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="623fb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="623fb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="623fb-110">Child elements</span></span>

|<span data-ttu-id="623fb-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="623fb-111">**Element**</span></span>|<span data-ttu-id="623fb-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="623fb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="623fb-113">Item</span><span class="sxs-lookup"><span data-stu-id="623fb-113">Item</span></span>](item.md) <br/> |<span data-ttu-id="623fb-114">Exchange ストア内の項目を表します。</span><span class="sxs-lookup"><span data-stu-id="623fb-114">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="623fb-115">Message</span><span class="sxs-lookup"><span data-stu-id="623fb-115">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="623fb-116">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="623fb-116">Represents an Exchange email message.</span></span>  <br/> |
|[<span data-ttu-id="623fb-117">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="623fb-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="623fb-118">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="623fb-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="623fb-119">Contact</span><span class="sxs-lookup"><span data-stu-id="623fb-119">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="623fb-120">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="623fb-120">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="623fb-121">DistributionList</span><span class="sxs-lookup"><span data-stu-id="623fb-121">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="623fb-122">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="623fb-122">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="623fb-123">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="623fb-123">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="623fb-124">Exchange ストア内の会議のメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="623fb-124">Represents a meeting message in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="623fb-125">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="623fb-125">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="623fb-126">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="623fb-126">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="623fb-127">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="623fb-127">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="623fb-128">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="623fb-128">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="623fb-129">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="623fb-129">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="623fb-130">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="623fb-130">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="623fb-131">タスク</span><span class="sxs-lookup"><span data-stu-id="623fb-131">Task</span></span>](task.md) <br/> |<span data-ttu-id="623fb-132">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="623fb-132">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="623fb-133">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="623fb-133">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="623fb-134">Exchange ストア内のアイテムの送信者への返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="623fb-134">Contains a reply to the sender of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="623fb-135">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="623fb-135">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="623fb-136">受信者に転送するのには、Exchange ストアの項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="623fb-136">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="623fb-137">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="623fb-137">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="623fb-138">Exchange ストア内のアイテムの識別されたすべての受信者と送信者への返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="623fb-138">Contains a reply to the sender and all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="623fb-139">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="623fb-139">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="623fb-140">会議出席依頼、承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="623fb-140">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="623fb-141">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="623fb-141">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="623fb-142">仮の予定を表しますが、会議出席依頼に返信します。</span><span class="sxs-lookup"><span data-stu-id="623fb-142">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="623fb-143">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="623fb-143">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="623fb-144">会議出席依頼を辞退の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="623fb-144">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="623fb-145">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="623fb-145">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="623fb-146">会議をキャンセルするために使用される応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="623fb-146">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="623fb-147">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="623fb-147">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="623fb-148">MeetingCancellation メッセージを受信したとき、会議アイテムを削除するために使用される応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="623fb-148">Represents a response object that is used to remove a meeting item when a MeetingCancellation message is received.</span></span>  <br/> |
|[<span data-ttu-id="623fb-149">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="623fb-149">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="623fb-150">投稿アイテムへの返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="623fb-150">Contains a reply to a post item.</span></span>  <br/> |
|[<span data-ttu-id="623fb-151">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="623fb-151">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="623fb-152">開封確認メッセージを非表示にするために使用します。</span><span class="sxs-lookup"><span data-stu-id="623fb-152">Used to suppress read receipts.</span></span>  <br/> |
|[<span data-ttu-id="623fb-153">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="623fb-153">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="623fb-154">別のユーザーの予定表や連絡先のデータへのアクセスを可能にするための招待を承諾する場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="623fb-154">Used to accept an invitation that allows access to another user's calendar or contacts data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="623fb-155">親要素</span><span class="sxs-lookup"><span data-stu-id="623fb-155">Parent elements</span></span>

|<span data-ttu-id="623fb-156">**要素**</span><span class="sxs-lookup"><span data-stu-id="623fb-156">**Element**</span></span>|<span data-ttu-id="623fb-157">**説明**</span><span class="sxs-lookup"><span data-stu-id="623fb-157">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="623fb-158">CreateItem</span><span class="sxs-lookup"><span data-stu-id="623fb-158">CreateItem</span></span>](createitem.md) <br/> |<span data-ttu-id="623fb-159">Exchange ストア内のアイテムを作成する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="623fb-159">Defines the request to create an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="623fb-160">この要素への XPath 式は、次のようにします。`/CreateItem`</span><span class="sxs-lookup"><span data-stu-id="623fb-160">The following is the XPath expression to this element:  `/CreateItem`</span></span> <br/> |
|[<span data-ttu-id="623fb-161">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="623fb-161">ConversationNode</span></span>](conversationnode.md) <br/> |<span data-ttu-id="623fb-162">会話で 1 つのノードを識別します。</span><span class="sxs-lookup"><span data-stu-id="623fb-162">Identifies a single node in a conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="623fb-163">備考</span><span class="sxs-lookup"><span data-stu-id="623fb-163">Remarks</span></span>

<span data-ttu-id="623fb-164">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="623fb-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="623fb-165">要素情報</span><span class="sxs-lookup"><span data-stu-id="623fb-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="623fb-166">名前空間</span><span class="sxs-lookup"><span data-stu-id="623fb-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="623fb-167">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="623fb-167">Schema Name</span></span>  <br/> |<span data-ttu-id="623fb-168">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="623fb-168">Message schema</span></span>  <br/> |
|<span data-ttu-id="623fb-169">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="623fb-169">Validation File</span></span>  <br/> |<span data-ttu-id="623fb-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="623fb-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="623fb-171">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="623fb-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="623fb-172">False</span><span class="sxs-lookup"><span data-stu-id="623fb-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="623fb-173">関連項目</span><span class="sxs-lookup"><span data-stu-id="623fb-173">See also</span></span>



<span data-ttu-id="623fb-174">
  [CreateFolder 操作](createfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="623fb-174">[CreateFolder operation](createfolder-operation.md)</span></span>
  
<span data-ttu-id="623fb-175">
  [CreateItem 操作](createitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="623fb-175">[CreateItem operation](createitem-operation.md)</span></span>


[<span data-ttu-id="623fb-176">フォルダー (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="623fb-176">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)


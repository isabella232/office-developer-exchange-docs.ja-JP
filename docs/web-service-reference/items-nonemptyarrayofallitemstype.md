---
title: アイテム (非 Emptyarrayofallitemstype)
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
description: Items 要素には、作成する一連のアイテムが含まれています。
ms.openlocfilehash: 0f70f1fe4348b5b74cef6be6414618af1e3de260
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459855"
---
# <a name="items-nonemptyarrayofallitemstype"></a><span data-ttu-id="6b0f0-103">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="6b0f0-103">Items (NonEmptyArrayOfAllItemsType)</span></span>

<span data-ttu-id="6b0f0-104">**Items**要素には、作成する一連のアイテムが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-104">The **Items** element contains a set of items to create.</span></span> 
  
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

 <span data-ttu-id="6b0f0-105">**非 Emptyarrayofallitemstype**</span><span class="sxs-lookup"><span data-stu-id="6b0f0-105">**NonEmptyArrayOfAllItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b0f0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6b0f0-106">Attributes and elements</span></span>

<span data-ttu-id="6b0f0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b0f0-108">属性</span><span class="sxs-lookup"><span data-stu-id="6b0f0-108">Attributes</span></span>

<span data-ttu-id="6b0f0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b0f0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6b0f0-110">Child elements</span></span>

|<span data-ttu-id="6b0f0-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="6b0f0-111">**Element**</span></span>|<span data-ttu-id="6b0f0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6b0f0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b0f0-113">Item</span><span class="sxs-lookup"><span data-stu-id="6b0f0-113">Item</span></span>](item.md) <br/> |<span data-ttu-id="6b0f0-114">Exchange ストア内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-114">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-115">Message</span><span class="sxs-lookup"><span data-stu-id="6b0f0-115">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6b0f0-116">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-116">Represents an Exchange email message.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="6b0f0-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="6b0f0-118">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-119">Contact</span><span class="sxs-lookup"><span data-stu-id="6b0f0-119">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="6b0f0-120">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-120">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-121">DistributionList</span><span class="sxs-lookup"><span data-stu-id="6b0f0-121">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="6b0f0-122">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-122">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-123">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="6b0f0-123">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="6b0f0-124">Exchange ストア内の会議メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-124">Represents a meeting message in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-125">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="6b0f0-125">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="6b0f0-126">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-126">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-127">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="6b0f0-127">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="6b0f0-128">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-128">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-129">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="6b0f0-129">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="6b0f0-130">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-130">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-131">タスク</span><span class="sxs-lookup"><span data-stu-id="6b0f0-131">Task</span></span>](task.md) <br/> |<span data-ttu-id="6b0f0-132">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-132">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-133">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="6b0f0-133">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="6b0f0-134">Exchange ストア内のアイテムの送信者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-134">Contains a reply to the sender of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-135">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="6b0f0-135">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="6b0f0-136">受信者に転送するための Exchange ストアアイテムが保存されています。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-136">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-137">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="6b0f0-137">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="6b0f0-138">Exchange ストア内のアイテムの送信者および特定の受信者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-138">Contains a reply to the sender and all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-139">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="6b0f0-139">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="6b0f0-140">会議出席依頼への返信を承諾するかを表します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-140">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-141">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="6b0f0-141">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="6b0f0-142">会議出席依頼に対する仮の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-142">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-143">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="6b0f0-143">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="6b0f0-144">会議出席依頼への返信を拒否することを表します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-144">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-145">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="6b0f0-145">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="6b0f0-146">会議の取り消しに使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-146">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-147">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="6b0f0-147">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="6b0f0-148">会議の取り消しメッセージを受信したときに会議アイテムを削除するために使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-148">Represents a response object that is used to remove a meeting item when a MeetingCancellation message is received.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-149">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="6b0f0-149">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="6b0f0-150">投稿アイテムへの返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-150">Contains a reply to a post item.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-151">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="6b0f0-151">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="6b0f0-152">開封確認メッセージを抑制するために使用します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-152">Used to suppress read receipts.</span></span>  <br/> |
|[<span data-ttu-id="6b0f0-153">AcceptSharingInvitation 状</span><span class="sxs-lookup"><span data-stu-id="6b0f0-153">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="6b0f0-154">別のユーザーの予定表または連絡先データへのアクセスを許可する招待を承諾するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-154">Used to accept an invitation that allows access to another user's calendar or contacts data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6b0f0-155">親要素</span><span class="sxs-lookup"><span data-stu-id="6b0f0-155">Parent elements</span></span>

|<span data-ttu-id="6b0f0-156">**要素**</span><span class="sxs-lookup"><span data-stu-id="6b0f0-156">**Element**</span></span>|<span data-ttu-id="6b0f0-157">**説明**</span><span class="sxs-lookup"><span data-stu-id="6b0f0-157">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b0f0-158">CreateItem</span><span class="sxs-lookup"><span data-stu-id="6b0f0-158">CreateItem</span></span>](createitem.md) <br/> |<span data-ttu-id="6b0f0-159">Exchange ストアにアイテムを作成するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-159">Defines the request to create an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="6b0f0-160">この要素の XPath 式を次に示します。`/CreateItem`</span><span class="sxs-lookup"><span data-stu-id="6b0f0-160">The following is the XPath expression to this element:  `/CreateItem`</span></span> <br/> |
|[<span data-ttu-id="6b0f0-161">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="6b0f0-161">ConversationNode</span></span>](conversationnode.md) <br/> |<span data-ttu-id="6b0f0-162">会話内の1つのノードを識別します。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-162">Identifies a single node in a conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6b0f0-163">注釈</span><span class="sxs-lookup"><span data-stu-id="6b0f0-163">Remarks</span></span>

<span data-ttu-id="6b0f0-164">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6b0f0-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b0f0-165">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6b0f0-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b0f0-166">Namespace</span><span class="sxs-lookup"><span data-stu-id="6b0f0-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6b0f0-167">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6b0f0-167">Schema Name</span></span>  <br/> |<span data-ttu-id="6b0f0-168">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="6b0f0-168">Message schema</span></span>  <br/> |
|<span data-ttu-id="6b0f0-169">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6b0f0-169">Validation File</span></span>  <br/> |<span data-ttu-id="6b0f0-170">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="6b0f0-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6b0f0-171">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6b0f0-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="6b0f0-172">正しくない</span><span class="sxs-lookup"><span data-stu-id="6b0f0-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6b0f0-173">関連項目</span><span class="sxs-lookup"><span data-stu-id="6b0f0-173">See also</span></span>



[<span data-ttu-id="6b0f0-174">CreateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="6b0f0-174">CreateFolder operation</span></span>](createfolder-operation.md)
  
[<span data-ttu-id="6b0f0-175">CreateItem 操作</span><span class="sxs-lookup"><span data-stu-id="6b0f0-175">CreateItem operation</span></span>](createitem-operation.md)


[<span data-ttu-id="6b0f0-176">フォルダーの作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="6b0f0-176">Creating Folders (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)


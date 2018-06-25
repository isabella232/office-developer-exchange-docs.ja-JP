---
title: ResponseObjects
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseObjects
api_type:
- schema
ms.assetid: ad29e064-3f3d-4b7b-aa4c-9ec27326381d
description: ResponseObjects 要素には、Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。
ms.openlocfilehash: b1d95063439f5089665d2aad97d747665caef0ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833197"
---
# <a name="responseobjects"></a><span data-ttu-id="0dfa0-103">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="0dfa0-103">ResponseObjects</span></span>

<span data-ttu-id="0dfa0-104">**ResponseObjects**要素には、Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-104">The **ResponseObjects** element contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span> 
  
```XML
<ResponseObjects>
   <AcceptItem/>
   <TentativelyAcceptItem/>
   <DeclineItem/>
   <ReplyToItem/>
   <ForwardItem/>
   <ReplyAllToItem/>
   <CancelCalendarItem/>
   <RemoveItem/>
   <PostReplyItem/>
   <SuppressReadReceipt/>
   <AcceptSharingInvitation/>
</ResponseObjects>
```

 <span data-ttu-id="0dfa0-105">**NonEmptyArrayOfResponseObjectsType**</span><span class="sxs-lookup"><span data-stu-id="0dfa0-105">**NonEmptyArrayOfResponseObjectsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0dfa0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0dfa0-106">Attributes and elements</span></span>

<span data-ttu-id="0dfa0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0dfa0-108">属性</span><span class="sxs-lookup"><span data-stu-id="0dfa0-108">Attributes</span></span>

<span data-ttu-id="0dfa0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0dfa0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0dfa0-110">Child elements</span></span>

|<span data-ttu-id="0dfa0-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="0dfa0-111">**Element**</span></span>|<span data-ttu-id="0dfa0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0dfa0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0dfa0-113">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="0dfa0-113">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="0dfa0-114">会議出席依頼、承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-114">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-115">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="0dfa0-115">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="0dfa0-116">仮の予定を表しますが、会議出席依頼に返信します。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-116">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-117">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="0dfa0-117">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="0dfa0-118">会議出席依頼を辞退の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-118">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-119">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="0dfa0-119">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="0dfa0-120">Exchange ストア内のアイテムの作成者に返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-120">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-121">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="0dfa0-121">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="0dfa0-122">受信者に転送するのには、Exchange ストアの項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-122">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-123">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="0dfa0-123">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="0dfa0-124">Exchange ストア内のアイテムの識別されたすべての受信者への返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-124">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-125">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="0dfa0-125">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="0dfa0-126">会議をキャンセルするために使用する応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-126">Represents the response object used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-127">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="0dfa0-127">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="0dfa0-128">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-128">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-129">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="0dfa0-129">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="0dfa0-130">投稿アイテムへの返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-130">Contains a reply to a post item.</span></span> <span data-ttu-id="0dfa0-131">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-132">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="0dfa0-132">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="0dfa0-133">開封確認メッセージ要求を非表示に使用されます。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-133">Used to suppress read receipt requests.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-134">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="0dfa0-134">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="0dfa0-135">別のユーザーの予定表や連絡先のデータへのアクセスを可能にするための招待を承諾する場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-135">Used to accept an invitation that allows access to another user's calendar or contacts data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0dfa0-136">親要素</span><span class="sxs-lookup"><span data-stu-id="0dfa0-136">Parent elements</span></span>

|<span data-ttu-id="0dfa0-137">**要素**</span><span class="sxs-lookup"><span data-stu-id="0dfa0-137">**Element**</span></span>|<span data-ttu-id="0dfa0-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="0dfa0-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0dfa0-139">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="0dfa0-139">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="0dfa0-140">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-140">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-141">Contact</span><span class="sxs-lookup"><span data-stu-id="0dfa0-141">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="0dfa0-142">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-142">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-143">DistributionList</span><span class="sxs-lookup"><span data-stu-id="0dfa0-143">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="0dfa0-144">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-144">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-145">アイテム</span><span class="sxs-lookup"><span data-stu-id="0dfa0-145">Item</span></span>](item.md) <br/> |<span data-ttu-id="0dfa0-146">Exchange ストア内の項目を表します。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-146">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-147">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="0dfa0-147">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="0dfa0-148">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-148">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-149">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="0dfa0-149">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="0dfa0-150">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-150">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-151">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="0dfa0-151">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="0dfa0-152">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-152">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-153">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="0dfa0-153">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="0dfa0-154">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-154">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-155">Message</span><span class="sxs-lookup"><span data-stu-id="0dfa0-155">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0dfa0-156">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-156">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-157">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="0dfa0-157">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="0dfa0-158">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-158">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0dfa0-159">タスク</span><span class="sxs-lookup"><span data-stu-id="0dfa0-159">Task</span></span>](task.md) <br/> |<span data-ttu-id="0dfa0-160">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-160">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0dfa0-161">備考</span><span class="sxs-lookup"><span data-stu-id="0dfa0-161">Remarks</span></span>

<span data-ttu-id="0dfa0-162">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0dfa0-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0dfa0-163">要素情報</span><span class="sxs-lookup"><span data-stu-id="0dfa0-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0dfa0-164">名前空間</span><span class="sxs-lookup"><span data-stu-id="0dfa0-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0dfa0-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0dfa0-165">Schema Name</span></span>  <br/> |<span data-ttu-id="0dfa0-166">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="0dfa0-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="0dfa0-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0dfa0-167">Validation File</span></span>  <br/> |<span data-ttu-id="0dfa0-168">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0dfa0-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0dfa0-169">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0dfa0-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="0dfa0-170">False</span><span class="sxs-lookup"><span data-stu-id="0dfa0-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0dfa0-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="0dfa0-171">See also</span></span>



- [<span data-ttu-id="0dfa0-172">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0dfa0-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


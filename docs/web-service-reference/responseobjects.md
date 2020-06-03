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
description: ResponseObjects 要素には、Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションが含まれています。
ms.openlocfilehash: 675bfda4addb38535736efc0c790577ff4739108
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457439"
---
# <a name="responseobjects"></a><span data-ttu-id="fb3bf-103">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="fb3bf-103">ResponseObjects</span></span>

<span data-ttu-id="fb3bf-104">**Responseobjects**要素には、Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-104">The **ResponseObjects** element contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="fb3bf-105">**非 Emptyarrayofresponseobjectstype**</span><span class="sxs-lookup"><span data-stu-id="fb3bf-105">**NonEmptyArrayOfResponseObjectsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb3bf-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fb3bf-106">Attributes and elements</span></span>

<span data-ttu-id="fb3bf-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb3bf-108">属性</span><span class="sxs-lookup"><span data-stu-id="fb3bf-108">Attributes</span></span>

<span data-ttu-id="fb3bf-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb3bf-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fb3bf-110">Child elements</span></span>

|<span data-ttu-id="fb3bf-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="fb3bf-111">**Element**</span></span>|<span data-ttu-id="fb3bf-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb3bf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb3bf-113">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="fb3bf-113">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="fb3bf-114">会議出席依頼への返信を承諾するかを表します。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-114">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-115">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="fb3bf-115">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="fb3bf-116">会議出席依頼に対する仮の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-116">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-117">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="fb3bf-117">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="fb3bf-118">会議出席依頼への返信を拒否することを表します。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-118">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-119">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="fb3bf-119">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="fb3bf-120">Exchange ストア内のアイテムの作成者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-120">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-121">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="fb3bf-121">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="fb3bf-122">受信者に転送するための Exchange ストアアイテムが保存されています。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-122">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-123">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="fb3bf-123">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="fb3bf-124">Exchange ストア内のアイテムの特定の受信者全員への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-124">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-125">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="fb3bf-125">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="fb3bf-126">会議の取り消しに使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-126">Represents the response object used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-127">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="fb3bf-127">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="fb3bf-128">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-128">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-129">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="fb3bf-129">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="fb3bf-130">投稿アイテムへの返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-130">Contains a reply to a post item.</span></span> <span data-ttu-id="fb3bf-131">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-132">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="fb3bf-132">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="fb3bf-133">開封確認要求を抑制するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-133">Used to suppress read receipt requests.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-134">AcceptSharingInvitation 状</span><span class="sxs-lookup"><span data-stu-id="fb3bf-134">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="fb3bf-135">別のユーザーの予定表または連絡先データへのアクセスを許可する招待を承諾するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-135">Used to accept an invitation that allows access to another user's calendar or contacts data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fb3bf-136">親要素</span><span class="sxs-lookup"><span data-stu-id="fb3bf-136">Parent elements</span></span>

|<span data-ttu-id="fb3bf-137">**要素**</span><span class="sxs-lookup"><span data-stu-id="fb3bf-137">**Element**</span></span>|<span data-ttu-id="fb3bf-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb3bf-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb3bf-139">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="fb3bf-139">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="fb3bf-140">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-140">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-141">Contact</span><span class="sxs-lookup"><span data-stu-id="fb3bf-141">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="fb3bf-142">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-142">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-143">DistributionList</span><span class="sxs-lookup"><span data-stu-id="fb3bf-143">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="fb3bf-144">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-144">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-145">Item</span><span class="sxs-lookup"><span data-stu-id="fb3bf-145">Item</span></span>](item.md) <br/> |<span data-ttu-id="fb3bf-146">Exchange ストア内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-146">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-147">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="fb3bf-147">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="fb3bf-148">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-148">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-149">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="fb3bf-149">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="fb3bf-150">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-150">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-151">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="fb3bf-151">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="fb3bf-152">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-152">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-153">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="fb3bf-153">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="fb3bf-154">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-154">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-155">Message</span><span class="sxs-lookup"><span data-stu-id="fb3bf-155">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="fb3bf-156">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-156">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-157">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="fb3bf-157">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="fb3bf-158">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-158">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fb3bf-159">タスク</span><span class="sxs-lookup"><span data-stu-id="fb3bf-159">Task</span></span>](task.md) <br/> |<span data-ttu-id="fb3bf-160">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-160">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fb3bf-161">注釈</span><span class="sxs-lookup"><span data-stu-id="fb3bf-161">Remarks</span></span>

<span data-ttu-id="fb3bf-162">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fb3bf-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb3bf-163">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fb3bf-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb3bf-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="fb3bf-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fb3bf-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fb3bf-165">Schema Name</span></span>  <br/> |<span data-ttu-id="fb3bf-166">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="fb3bf-166">Types schema</span></span>  <br/> |
|<span data-ttu-id="fb3bf-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fb3bf-167">Validation File</span></span>  <br/> |<span data-ttu-id="fb3bf-168">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="fb3bf-168">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fb3bf-169">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fb3bf-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="fb3bf-170">正しくない</span><span class="sxs-lookup"><span data-stu-id="fb3bf-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb3bf-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="fb3bf-171">See also</span></span>



- [<span data-ttu-id="fb3bf-172">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="fb3bf-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


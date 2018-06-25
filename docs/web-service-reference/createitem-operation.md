---
title: CreateItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 78a52120-f1d0-4ed7-8748-436e554f75b6
description: CreateItem 操作は、Exchange ストア内のアイテムを作成します。
ms.openlocfilehash: 7e1808c685cdbaa1e8867aa7425b2cc52218d001
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759839"
---
# <a name="createitem-operation"></a><span data-ttu-id="584da-103">CreateItem 操作</span><span class="sxs-lookup"><span data-stu-id="584da-103">CreateItem operation</span></span>

<span data-ttu-id="584da-104">CreateItem 操作は、Exchange ストア内のアイテムを作成します。</span><span class="sxs-lookup"><span data-stu-id="584da-104">The CreateItem operation creates items in the Exchange store.</span></span>
  
## <a name="using-the-createitem-operation"></a><span data-ttu-id="584da-105">CreateItem 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="584da-105">Using the CreateItem Operation</span></span>

<span data-ttu-id="584da-106">CreateItem 操作を使用して、次を作成できます。</span><span class="sxs-lookup"><span data-stu-id="584da-106">You can use the CreateItem operation to create the following:</span></span>
  
- <span data-ttu-id="584da-107">予定表アイテム</span><span class="sxs-lookup"><span data-stu-id="584da-107">Calendar items</span></span>
    
- <span data-ttu-id="584da-108">電子メール メッセージ</span><span class="sxs-lookup"><span data-stu-id="584da-108">E-mail messages</span></span>
    
- <span data-ttu-id="584da-109">会議出席依頼</span><span class="sxs-lookup"><span data-stu-id="584da-109">Meeting requests</span></span>
    
- <span data-ttu-id="584da-110">タスク</span><span class="sxs-lookup"><span data-stu-id="584da-110">Tasks</span></span>
    
- <span data-ttu-id="584da-111">連絡先</span><span class="sxs-lookup"><span data-stu-id="584da-111">Contacts</span></span>
    
<span data-ttu-id="584da-112">詳細については、 [CreateItem 操作 (予定表アイテム)](createitem-operation-calendar-item.md)、 [CreateItem 操作 (電子メール メッセージ)](createitem-operation-email-message.md)、 [CreateItem 操作 (会議出席依頼)](createitem-operation-meeting-request.md)、 [CreateItem 操作 (タスク)](createitem-operation-task.md)、および[CreateItem 操作 (連絡先) を参照してください。](createitem-operation-contact.md).</span><span class="sxs-lookup"><span data-stu-id="584da-112">For more information, see [CreateItem operation (calendar item)](createitem-operation-calendar-item.md), [CreateItem operation (email message)](createitem-operation-email-message.md), [CreateItem operation (meeting request)](createitem-operation-meeting-request.md), [CreateItem operation (task)](createitem-operation-task.md), and [CreateItem operation (contact)](createitem-operation-contact.md).</span></span>
  
<span data-ttu-id="584da-113">CreateItem 操作には、応答オブジェクトの使用がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="584da-113">The CreateItem operation supports the use of response objects.</span></span> <span data-ttu-id="584da-114">応答オブジェクトは、承認と却下の会議と、標準の電子メール メッセージに含まれる返信ボタンの処理をサポートします。</span><span class="sxs-lookup"><span data-stu-id="584da-114">Response objects support the acceptance and rejection of meetings and the handling of voting buttons that are included in a standard e-mail message.</span></span> <span data-ttu-id="584da-115">次の表に、CreateItem 操作で処理される応答オブジェクトを示します。</span><span class="sxs-lookup"><span data-stu-id="584da-115">The following table lists the response objects that are handled in the CreateItem operation.</span></span>
  
|<span data-ttu-id="584da-116">**応答オブジェクト**</span><span class="sxs-lookup"><span data-stu-id="584da-116">**Response object**</span></span>|<span data-ttu-id="584da-117">**アクション**</span><span class="sxs-lookup"><span data-stu-id="584da-117">**Action**</span></span>|
|:-----|:-----|
|<span data-ttu-id="584da-118">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="584da-118">AcceptItem</span></span>  <br/> |<span data-ttu-id="584da-119">会議出席依頼を承諾します。</span><span class="sxs-lookup"><span data-stu-id="584da-119">Accept a meeting request.</span></span>  <br/> |
|<span data-ttu-id="584da-120">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="584da-120">CancelCalendarItem</span></span>  <br/> |<span data-ttu-id="584da-121">会議をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="584da-121">Cancel a meeting.</span></span> <span data-ttu-id="584da-122">これも、開催者の会議が削除されるので、すべての出席者を削除すると異なります。</span><span class="sxs-lookup"><span data-stu-id="584da-122">This differs from deleting all attendees because it deletes the meeting for the organizer also.</span></span>  <br/> |
|<span data-ttu-id="584da-123">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="584da-123">DeclineItem</span></span>  <br/> |<span data-ttu-id="584da-124">会議出席依頼を辞退します。</span><span class="sxs-lookup"><span data-stu-id="584da-124">Decline a meeting request.</span></span>  <br/> |
|<span data-ttu-id="584da-125">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="584da-125">ForwardItem</span></span>  <br/> |<span data-ttu-id="584da-126">他のユーザーに会議出席依頼と会議出席依頼を送信します。</span><span class="sxs-lookup"><span data-stu-id="584da-126">Send a meeting request to another person as a meeting request.</span></span>  <br/> |
|<span data-ttu-id="584da-127">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="584da-127">RemoveItem</span></span>  <br/> |<span data-ttu-id="584da-128">キャンセルされた会議を予定表から削除します。</span><span class="sxs-lookup"><span data-stu-id="584da-128">Remove a canceled meeting from the calendar.</span></span>  <br/> |
|<span data-ttu-id="584da-129">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="584da-129">ReplyAllToItem</span></span>  <br/> |<span data-ttu-id="584da-130">会議のすべての出席者に、元の会議出席依頼の本文を含むメッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="584da-130">Send a message that includes the body of the original meeting request to all attendees of the meeting.</span></span>  <br/> |
|<span data-ttu-id="584da-131">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="584da-131">ReplyToItem</span></span>  <br/> |<span data-ttu-id="584da-132">会議出席依頼の送信者に、元の会議出席依頼の本文を含むメッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="584da-132">Send a message that includes the body of the original meeting request to the sender of the meeting request.</span></span>  <br/> |
|<span data-ttu-id="584da-133">SendReadReceipt</span><span class="sxs-lookup"><span data-stu-id="584da-133">SendReadReceipt</span></span>  <br/> |<span data-ttu-id="584da-134">会議出席依頼の送信者に開封確認メッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="584da-134">Send a read receipt to the sender of the meeting request.</span></span>  <br/> |
|<span data-ttu-id="584da-135">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="584da-135">TentativelyAcceptItem</span></span>  <br/> |<span data-ttu-id="584da-136">会議出席依頼を仮承諾します。</span><span class="sxs-lookup"><span data-stu-id="584da-136">Tentatively accept a meeting request.</span></span>  <br/> |
   
<span data-ttu-id="584da-137">CreateItem 操作には、会議の他のオブジェクトもサポートしています。</span><span class="sxs-lookup"><span data-stu-id="584da-137">The CreateItem operation also supports additional meeting objects.</span></span> <span data-ttu-id="584da-138">CreateItem 操作をサポートする追加のオブジェクトを次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="584da-138">The following table lists additional objects that the CreateItem operation supports.</span></span>
  
|<span data-ttu-id="584da-139">**会議オブジェクト**</span><span class="sxs-lookup"><span data-stu-id="584da-139">**Meeting object**</span></span>|<span data-ttu-id="584da-140">**説明**</span><span class="sxs-lookup"><span data-stu-id="584da-140">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="584da-141">会議出席依頼</span><span class="sxs-lookup"><span data-stu-id="584da-141">Meeting Message</span></span>  <br/> |<span data-ttu-id="584da-142">Exchange ストア内の会議のメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="584da-142">Represents a meeting message in the Exchange store.</span></span> <span data-ttu-id="584da-143">これは、他の会議オブジェクトの基本オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="584da-143">This is the base object for the other meeting objects.</span></span>  <br/> |
|<span data-ttu-id="584da-144">会議出席依頼</span><span class="sxs-lookup"><span data-stu-id="584da-144">Meeting Request</span></span>  <br/> |<span data-ttu-id="584da-145">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="584da-145">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="584da-146">会議の返信</span><span class="sxs-lookup"><span data-stu-id="584da-146">Meeting Response</span></span>  <br/> |<span data-ttu-id="584da-147">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="584da-147">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="584da-148">会議の取り消し</span><span class="sxs-lookup"><span data-stu-id="584da-148">Meeting Cancellation</span></span>  <br/> |<span data-ttu-id="584da-149">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="584da-149">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="584da-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="584da-150">See also</span></span>



[<span data-ttu-id="584da-151">CreateItem 操作 (予定表アイテム)</span><span class="sxs-lookup"><span data-stu-id="584da-151">CreateItem operation (calendar item)</span></span>](createitem-operation-calendar-item.md)
  
[<span data-ttu-id="584da-152">CreateItem 操作 (連絡先)</span><span class="sxs-lookup"><span data-stu-id="584da-152">CreateItem operation (contact)</span></span>](createitem-operation-contact.md)
  
[<span data-ttu-id="584da-153">CreateItem 操作 (電子メール)</span><span class="sxs-lookup"><span data-stu-id="584da-153">CreateItem operation (email message)</span></span>](createitem-operation-email-message.md)
  
[<span data-ttu-id="584da-154">CreateItem 操作 (会議出席依頼)</span><span class="sxs-lookup"><span data-stu-id="584da-154">CreateItem operation (meeting request)</span></span>](createitem-operation-meeting-request.md)
  
[<span data-ttu-id="584da-155">CreateItem 操作 (タスク)</span><span class="sxs-lookup"><span data-stu-id="584da-155">CreateItem operation (task)</span></span>](createitem-operation-task.md)
  
 <span data-ttu-id="584da-156">**CreateItemType**</span><span class="sxs-lookup"><span data-stu-id="584da-156">**CreateItemType**</span></span>


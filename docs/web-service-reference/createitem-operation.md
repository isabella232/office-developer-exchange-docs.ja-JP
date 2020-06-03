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
description: CreateItem 操作は、Exchange ストアにアイテムを作成します。
ms.openlocfilehash: f6aaa9ed8e8257f19780492d6137fb015c1b6136
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458867"
---
# <a name="createitem-operation"></a><span data-ttu-id="28eb8-103">CreateItem 操作</span><span class="sxs-lookup"><span data-stu-id="28eb8-103">CreateItem operation</span></span>

<span data-ttu-id="28eb8-104">CreateItem 操作は、Exchange ストアにアイテムを作成します。</span><span class="sxs-lookup"><span data-stu-id="28eb8-104">The CreateItem operation creates items in the Exchange store.</span></span>
  
## <a name="using-the-createitem-operation"></a><span data-ttu-id="28eb8-105">CreateItem 操作の使用</span><span class="sxs-lookup"><span data-stu-id="28eb8-105">Using the CreateItem Operation</span></span>

<span data-ttu-id="28eb8-106">CreateItem 操作を使用して、次のものを作成できます。</span><span class="sxs-lookup"><span data-stu-id="28eb8-106">You can use the CreateItem operation to create the following:</span></span>
  
- <span data-ttu-id="28eb8-107">予定表アイテム</span><span class="sxs-lookup"><span data-stu-id="28eb8-107">Calendar items</span></span>
    
- <span data-ttu-id="28eb8-108">電子メール メッセージ</span><span class="sxs-lookup"><span data-stu-id="28eb8-108">E-mail messages</span></span>
    
- <span data-ttu-id="28eb8-109">会議出席依頼</span><span class="sxs-lookup"><span data-stu-id="28eb8-109">Meeting requests</span></span>
    
- <span data-ttu-id="28eb8-110">タスク</span><span class="sxs-lookup"><span data-stu-id="28eb8-110">Tasks</span></span>
    
- <span data-ttu-id="28eb8-111">連絡先</span><span class="sxs-lookup"><span data-stu-id="28eb8-111">Contacts</span></span>
    
<span data-ttu-id="28eb8-112">詳細については、「 [CreateItem 操作 (予定表アイテム)](createitem-operation-calendar-item.md)」、「 [CreateItem 操作 (電子メールメッセージ)](createitem-operation-email-message.md)」、「 [CreateItem operation (meeting request)](createitem-operation-meeting-request.md)、 [CreateItem operation (task)](createitem-operation-task.md)、 [CreateItem operation (contact)](createitem-operation-contact.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="28eb8-112">For more information, see [CreateItem operation (calendar item)](createitem-operation-calendar-item.md), [CreateItem operation (email message)](createitem-operation-email-message.md), [CreateItem operation (meeting request)](createitem-operation-meeting-request.md), [CreateItem operation (task)](createitem-operation-task.md), and [CreateItem operation (contact)](createitem-operation-contact.md).</span></span>
  
<span data-ttu-id="28eb8-113">CreateItem 操作では、response オブジェクトの使用がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="28eb8-113">The CreateItem operation supports the use of response objects.</span></span> <span data-ttu-id="28eb8-114">応答オブジェクトは、会議の承諾と却下、および標準の電子メールメッセージに含まれる投票ボタンの処理をサポートします。</span><span class="sxs-lookup"><span data-stu-id="28eb8-114">Response objects support the acceptance and rejection of meetings and the handling of voting buttons that are included in a standard e-mail message.</span></span> <span data-ttu-id="28eb8-115">次の表に、CreateItem 操作で処理される応答オブジェクトを示します。</span><span class="sxs-lookup"><span data-stu-id="28eb8-115">The following table lists the response objects that are handled in the CreateItem operation.</span></span>
  
|<span data-ttu-id="28eb8-116">**Response オブジェクト**</span><span class="sxs-lookup"><span data-stu-id="28eb8-116">**Response object**</span></span>|<span data-ttu-id="28eb8-117">**Action**</span><span class="sxs-lookup"><span data-stu-id="28eb8-117">**Action**</span></span>|
|:-----|:-----|
|<span data-ttu-id="28eb8-118">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="28eb8-118">AcceptItem</span></span>  <br/> |<span data-ttu-id="28eb8-119">会議出席依頼を承諾します。</span><span class="sxs-lookup"><span data-stu-id="28eb8-119">Accept a meeting request.</span></span>  <br/> |
|<span data-ttu-id="28eb8-120">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="28eb8-120">CancelCalendarItem</span></span>  <br/> |<span data-ttu-id="28eb8-121">会議をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="28eb8-121">Cancel a meeting.</span></span> <span data-ttu-id="28eb8-122">これは、開催者の会議も削除するため、すべての出席者を削除するのとは異なります。</span><span class="sxs-lookup"><span data-stu-id="28eb8-122">This differs from deleting all attendees because it deletes the meeting for the organizer also.</span></span>  <br/> |
|<span data-ttu-id="28eb8-123">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="28eb8-123">DeclineItem</span></span>  <br/> |<span data-ttu-id="28eb8-124">会議出席依頼を辞退します。</span><span class="sxs-lookup"><span data-stu-id="28eb8-124">Decline a meeting request.</span></span>  <br/> |
|<span data-ttu-id="28eb8-125">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="28eb8-125">ForwardItem</span></span>  <br/> |<span data-ttu-id="28eb8-126">会議出席依頼として他のユーザーに会議出席依頼を送信します。</span><span class="sxs-lookup"><span data-stu-id="28eb8-126">Send a meeting request to another person as a meeting request.</span></span>  <br/> |
|<span data-ttu-id="28eb8-127">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="28eb8-127">RemoveItem</span></span>  <br/> |<span data-ttu-id="28eb8-128">予定表からキャンセルされた会議を削除します。</span><span class="sxs-lookup"><span data-stu-id="28eb8-128">Remove a canceled meeting from the calendar.</span></span>  <br/> |
|<span data-ttu-id="28eb8-129">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="28eb8-129">ReplyAllToItem</span></span>  <br/> |<span data-ttu-id="28eb8-130">元の会議出席依頼の本文を含むメッセージを、会議のすべての出席者に送信します。</span><span class="sxs-lookup"><span data-stu-id="28eb8-130">Send a message that includes the body of the original meeting request to all attendees of the meeting.</span></span>  <br/> |
|<span data-ttu-id="28eb8-131">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="28eb8-131">ReplyToItem</span></span>  <br/> |<span data-ttu-id="28eb8-132">元の会議出席依頼の本文を含むメッセージを、会議出席依頼の送信者に送信します。</span><span class="sxs-lookup"><span data-stu-id="28eb8-132">Send a message that includes the body of the original meeting request to the sender of the meeting request.</span></span>  <br/> |
|<span data-ttu-id="28eb8-133">SendReadReceipt</span><span class="sxs-lookup"><span data-stu-id="28eb8-133">SendReadReceipt</span></span>  <br/> |<span data-ttu-id="28eb8-134">会議出席依頼の送信者に開封確認メッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="28eb8-134">Send a read receipt to the sender of the meeting request.</span></span>  <br/> |
|<span data-ttu-id="28eb8-135">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="28eb8-135">TentativelyAcceptItem</span></span>  <br/> |<span data-ttu-id="28eb8-136">会議出席依頼を仮承諾します。</span><span class="sxs-lookup"><span data-stu-id="28eb8-136">Tentatively accept a meeting request.</span></span>  <br/> |
   
<span data-ttu-id="28eb8-137">CreateItem 操作では、追加の会議オブジェクトもサポートされます。</span><span class="sxs-lookup"><span data-stu-id="28eb8-137">The CreateItem operation also supports additional meeting objects.</span></span> <span data-ttu-id="28eb8-138">次の表に、CreateItem 操作がサポートする追加のオブジェクトを示します。</span><span class="sxs-lookup"><span data-stu-id="28eb8-138">The following table lists additional objects that the CreateItem operation supports.</span></span>
  
|<span data-ttu-id="28eb8-139">**会議オブジェクト**</span><span class="sxs-lookup"><span data-stu-id="28eb8-139">**Meeting object**</span></span>|<span data-ttu-id="28eb8-140">**説明**</span><span class="sxs-lookup"><span data-stu-id="28eb8-140">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="28eb8-141">会議メッセージ</span><span class="sxs-lookup"><span data-stu-id="28eb8-141">Meeting Message</span></span>  <br/> |<span data-ttu-id="28eb8-142">Exchange ストア内の会議メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="28eb8-142">Represents a meeting message in the Exchange store.</span></span> <span data-ttu-id="28eb8-143">これは、その他の会議オブジェクトの基本オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="28eb8-143">This is the base object for the other meeting objects.</span></span>  <br/> |
|<span data-ttu-id="28eb8-144">会議出席依頼</span><span class="sxs-lookup"><span data-stu-id="28eb8-144">Meeting Request</span></span>  <br/> |<span data-ttu-id="28eb8-145">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="28eb8-145">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="28eb8-146">会議出席依頼の返信</span><span class="sxs-lookup"><span data-stu-id="28eb8-146">Meeting Response</span></span>  <br/> |<span data-ttu-id="28eb8-147">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="28eb8-147">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="28eb8-148">会議の取り消し</span><span class="sxs-lookup"><span data-stu-id="28eb8-148">Meeting Cancellation</span></span>  <br/> |<span data-ttu-id="28eb8-149">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="28eb8-149">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="28eb8-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="28eb8-150">See also</span></span>



[<span data-ttu-id="28eb8-151">CreateItem 操作 (予定表アイテム)</span><span class="sxs-lookup"><span data-stu-id="28eb8-151">CreateItem operation (calendar item)</span></span>](createitem-operation-calendar-item.md)
  
[<span data-ttu-id="28eb8-152">CreateItem 操作 (連絡先)</span><span class="sxs-lookup"><span data-stu-id="28eb8-152">CreateItem operation (contact)</span></span>](createitem-operation-contact.md)
  
[<span data-ttu-id="28eb8-153">CreateItem 操作 (電子メールメッセージ)</span><span class="sxs-lookup"><span data-stu-id="28eb8-153">CreateItem operation (email message)</span></span>](createitem-operation-email-message.md)
  
[<span data-ttu-id="28eb8-154">CreateItem 操作 (会議出席依頼)</span><span class="sxs-lookup"><span data-stu-id="28eb8-154">CreateItem operation (meeting request)</span></span>](createitem-operation-meeting-request.md)
  
[<span data-ttu-id="28eb8-155">CreateItem 操作 (タスク)</span><span class="sxs-lookup"><span data-stu-id="28eb8-155">CreateItem operation (task)</span></span>](createitem-operation-task.md)
  
 <span data-ttu-id="28eb8-156">**CreateItemType**</span><span class="sxs-lookup"><span data-stu-id="28eb8-156">**CreateItemType**</span></span>


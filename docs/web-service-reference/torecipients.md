---
title: ToRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ToRecipients
api_type:
- schema
ms.assetid: 72dc3be8-30bb-4ae1-acf4-fb94ff490631
description: ToRecipients 要素には、アイテムの受信者の配列が含まれています。 これらは、アイテムの主な受信者です。
ms.openlocfilehash: 2913705cad52c041809769fe58efc3d616f40462
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839727"
---
# <a name="torecipients"></a><span data-ttu-id="e07d5-104">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="e07d5-104">ToRecipients</span></span>

<span data-ttu-id="e07d5-105">**ToRecipients**要素には、アイテムの受信者の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e07d5-105">The **ToRecipients** element contains an array of recipients of an item.</span></span> <span data-ttu-id="e07d5-106">これらは、アイテムの主な受信者です。</span><span class="sxs-lookup"><span data-stu-id="e07d5-106">These are the primary recipients of an item.</span></span> 
  
```xml
<ToRecipients>
   <Mailbox/>
</ToRecipients>
```

 <span data-ttu-id="e07d5-107">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="e07d5-107">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e07d5-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e07d5-108">Attributes and elements</span></span>

<span data-ttu-id="e07d5-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e07d5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e07d5-110">属性</span><span class="sxs-lookup"><span data-stu-id="e07d5-110">Attributes</span></span>

<span data-ttu-id="e07d5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e07d5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e07d5-112">子要素</span><span class="sxs-lookup"><span data-stu-id="e07d5-112">Child elements</span></span>

|<span data-ttu-id="e07d5-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e07d5-113">**Element**</span></span>|<span data-ttu-id="e07d5-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e07d5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e07d5-115">メールボックス</span><span class="sxs-lookup"><span data-stu-id="e07d5-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="e07d5-116">メールが有効な Active Directory ディレクトリ サービス オブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="e07d5-116">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e07d5-117">親要素</span><span class="sxs-lookup"><span data-stu-id="e07d5-117">Parent elements</span></span>

|<span data-ttu-id="e07d5-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="e07d5-118">**Element**</span></span>|<span data-ttu-id="e07d5-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="e07d5-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e07d5-120">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="e07d5-120">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="e07d5-121">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="e07d5-121">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e07d5-122">Message</span><span class="sxs-lookup"><span data-stu-id="e07d5-122">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e07d5-123">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="e07d5-123">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="e07d5-124">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="e07d5-124">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="e07d5-125">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="e07d5-125">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e07d5-126">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="e07d5-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e07d5-127">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="e07d5-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e07d5-128">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="e07d5-128">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="e07d5-129">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="e07d5-129">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e07d5-130">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="e07d5-130">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="e07d5-131">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="e07d5-131">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e07d5-132">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="e07d5-132">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="e07d5-133">会議出席依頼、承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="e07d5-133">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="e07d5-134">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="e07d5-134">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="e07d5-135">仮の予定を表しますが、会議出席依頼に返信します。</span><span class="sxs-lookup"><span data-stu-id="e07d5-135">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="e07d5-136">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="e07d5-136">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="e07d5-137">会議出席依頼を辞退の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="e07d5-137">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="e07d5-138">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="e07d5-138">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="e07d5-139">Exchange ストア内のアイテムの作成者に返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e07d5-139">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e07d5-140">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="e07d5-140">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="e07d5-141">Exchange ストア内のアイテムの識別されたすべての受信者への返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e07d5-141">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e07d5-142">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="e07d5-142">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="e07d5-143">受信者に転送するのには、Exchange ストアの項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e07d5-143">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="e07d5-144">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="e07d5-144">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="e07d5-145">会議をキャンセルするために使用される応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="e07d5-145">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e07d5-146">備考</span><span class="sxs-lookup"><span data-stu-id="e07d5-146">Remarks</span></span>

<span data-ttu-id="e07d5-147">**ToRecipients**を FindItem 要求を使用して取得できません。</span><span class="sxs-lookup"><span data-stu-id="e07d5-147">You cannot get **ToRecipients** by using a FindItem request.</span></span> <span data-ttu-id="e07d5-148">**ToRecipients**を取得するのにには、GetItem 要求を使用します。</span><span class="sxs-lookup"><span data-stu-id="e07d5-148">Use a GetItem request to get the **ToRecipients**.</span></span>
  
<span data-ttu-id="e07d5-149">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="e07d5-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e07d5-150">要素情報</span><span class="sxs-lookup"><span data-stu-id="e07d5-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e07d5-151">名前空間</span><span class="sxs-lookup"><span data-stu-id="e07d5-151">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e07d5-152">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e07d5-152">Schema Name</span></span>  <br/> |<span data-ttu-id="e07d5-153">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e07d5-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="e07d5-154">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e07d5-154">Validation File</span></span>  <br/> |<span data-ttu-id="e07d5-155">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e07d5-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e07d5-156">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e07d5-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="e07d5-157">False</span><span class="sxs-lookup"><span data-stu-id="e07d5-157">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e07d5-158">関連項目</span><span class="sxs-lookup"><span data-stu-id="e07d5-158">See also</span></span>



- [<span data-ttu-id="e07d5-159">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e07d5-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


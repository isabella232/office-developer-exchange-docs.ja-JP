---
title: ReceivedBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReceivedBy
api_type:
- schema
ms.assetid: ac84c9c5-d2fe-4b6f-bf4d-0444131d835b
description: ReceivedBy 要素は、代理人アクセス シナリオでは、デリゲートを識別します。
ms.openlocfilehash: 7918fa3320223e5cf02dd225912adfae3181e29c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832969"
---
# <a name="receivedby"></a><span data-ttu-id="7e02b-103">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="7e02b-103">ReceivedBy</span></span>

<span data-ttu-id="7e02b-104">**ReceivedBy**要素は、代理人アクセス シナリオでは、デリゲートを識別します。</span><span class="sxs-lookup"><span data-stu-id="7e02b-104">The **ReceivedBy** element identifies the delegate in a delegate access scenario.</span></span> 
  
```xml
<ReceivedBy>
   <Mailbox/>
</ReceivedBy>
```

 <span data-ttu-id="7e02b-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="7e02b-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e02b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7e02b-106">Attributes and elements</span></span>

<span data-ttu-id="7e02b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7e02b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e02b-108">属性</span><span class="sxs-lookup"><span data-stu-id="7e02b-108">Attributes</span></span>

<span data-ttu-id="7e02b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7e02b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e02b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7e02b-110">Child elements</span></span>

|<span data-ttu-id="7e02b-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="7e02b-111">**Element**</span></span>|<span data-ttu-id="7e02b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e02b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e02b-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="7e02b-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="7e02b-114">メールが有効な Active Directory ディレクトリ サービス オブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="7e02b-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7e02b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="7e02b-115">Parent elements</span></span>

|<span data-ttu-id="7e02b-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="7e02b-116">**Element**</span></span>|<span data-ttu-id="7e02b-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e02b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e02b-118">Message</span><span class="sxs-lookup"><span data-stu-id="7e02b-118">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7e02b-119">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="7e02b-119">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="7e02b-120">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="7e02b-120">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="7e02b-121">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="7e02b-121">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7e02b-122">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="7e02b-122">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="7e02b-123">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="7e02b-123">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7e02b-124">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="7e02b-124">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="7e02b-125">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="7e02b-125">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7e02b-126">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="7e02b-126">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="7e02b-127">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="7e02b-127">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7e02b-128">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="7e02b-128">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="7e02b-129">会議出席依頼、承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="7e02b-129">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="7e02b-130">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="7e02b-130">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="7e02b-131">仮の予定を表しますが、会議出席依頼に返信します。</span><span class="sxs-lookup"><span data-stu-id="7e02b-131">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="7e02b-132">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="7e02b-132">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="7e02b-133">会議出席依頼を辞退の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="7e02b-133">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="7e02b-134">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="7e02b-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="7e02b-135">Exchange ストア内のアイテムの作成者に返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e02b-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7e02b-136">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="7e02b-136">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="7e02b-137">Exchange ストア内のアイテムの識別されたすべての受信者への返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e02b-137">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7e02b-138">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="7e02b-138">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="7e02b-139">受信者に転送するのには、Exchange ストアの項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e02b-139">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="7e02b-140">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="7e02b-140">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="7e02b-141">会議をキャンセルするために使用される応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="7e02b-141">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7e02b-142">備考</span><span class="sxs-lookup"><span data-stu-id="7e02b-142">Remarks</span></span>

<span data-ttu-id="7e02b-143">**ReceivedRepresenting**要素を使用して**から**とし、内の**ReceivedBy**要素は、アクセスのシナリオを委任します。</span><span class="sxs-lookup"><span data-stu-id="7e02b-143">The **ReceivedRepresenting** element is used together with the **From** and **ReceivedBy** elements in delegate access scenarios.</span></span> <span data-ttu-id="7e02b-144">次の表に、代理人アクセスのシナリオでこれらの要素を表すエンティティを示します。</span><span class="sxs-lookup"><span data-stu-id="7e02b-144">The following table lists the entities that these elements represent in a delegate access scenario.</span></span> 
  
<span data-ttu-id="7e02b-145">**代理人アクセスのシナリオ内の要素**</span><span class="sxs-lookup"><span data-stu-id="7e02b-145">**Elements in a delegate access scenario**</span></span>

|<span data-ttu-id="7e02b-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="7e02b-146">**Element**</span></span>|<span data-ttu-id="7e02b-147">**要素が表すエンティティ**</span><span class="sxs-lookup"><span data-stu-id="7e02b-147">**Entity that the element represent**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e02b-148">From</span><span class="sxs-lookup"><span data-stu-id="7e02b-148">From</span></span>](from.md) <br/> |<span data-ttu-id="7e02b-149">サード ・ パーティ</span><span class="sxs-lookup"><span data-stu-id="7e02b-149">ThirdParty</span></span>  <br/> |
|[<span data-ttu-id="7e02b-150">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="7e02b-150">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="7e02b-151">代理人</span><span class="sxs-lookup"><span data-stu-id="7e02b-151">Delegate</span></span>  <br/> |
|[<span data-ttu-id="7e02b-152">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="7e02b-152">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="7e02b-153">校長</span><span class="sxs-lookup"><span data-stu-id="7e02b-153">Principal</span></span>  <br/> |
   
<span data-ttu-id="7e02b-154">代理人アクセス シナリオでは、サード パーティーは、代理人を持っているプリンシパルに会議出席依頼を送信する場合、代理人が参照してください新しい会議出席依頼。</span><span class="sxs-lookup"><span data-stu-id="7e02b-154">In a delegate access scenario, if a ThirdParty sends a meeting request to a Principal who has a Delegate, the Delegate will see a new meeting request.</span></span> <span data-ttu-id="7e02b-155">これらの要素は、それらに直接送信されるメッセージと、デリゲートのルールを転送するために送信されるメッセージとを区別するための委任を有効にします。</span><span class="sxs-lookup"><span data-stu-id="7e02b-155">These elements enable delegates to distinguish between messages that are sent directly to them and messages that are sent to them because of a delegate forwarding rule.</span></span>
  
<span data-ttu-id="7e02b-156">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7e02b-156">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e02b-157">要素情報</span><span class="sxs-lookup"><span data-stu-id="7e02b-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e02b-158">名前空間</span><span class="sxs-lookup"><span data-stu-id="7e02b-158">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e02b-159">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7e02b-159">Schema Name</span></span>  <br/> |<span data-ttu-id="7e02b-160">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7e02b-160">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e02b-161">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7e02b-161">Validation File</span></span>  <br/> |<span data-ttu-id="7e02b-162">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7e02b-162">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e02b-163">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7e02b-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e02b-164">False</span><span class="sxs-lookup"><span data-stu-id="7e02b-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e02b-165">関連項目</span><span class="sxs-lookup"><span data-stu-id="7e02b-165">See also</span></span>



- [<span data-ttu-id="7e02b-166">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7e02b-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


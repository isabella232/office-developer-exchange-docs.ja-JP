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
description: ReceivedBy 要素は、代理人アクセスシナリオのデリゲートを識別します。
ms.openlocfilehash: 7cee996c15e81f77d71f42e052b14b1d21772ba1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468251"
---
# <a name="receivedby"></a><span data-ttu-id="5ec23-103">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="5ec23-103">ReceivedBy</span></span>

<span data-ttu-id="5ec23-104">**ReceivedBy**要素は、代理人アクセスシナリオのデリゲートを識別します。</span><span class="sxs-lookup"><span data-stu-id="5ec23-104">The **ReceivedBy** element identifies the delegate in a delegate access scenario.</span></span> 
  
```xml
<ReceivedBy>
   <Mailbox/>
</ReceivedBy>
```

 <span data-ttu-id="5ec23-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="5ec23-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5ec23-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5ec23-106">Attributes and elements</span></span>

<span data-ttu-id="5ec23-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5ec23-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5ec23-108">属性</span><span class="sxs-lookup"><span data-stu-id="5ec23-108">Attributes</span></span>

<span data-ttu-id="5ec23-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5ec23-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5ec23-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5ec23-110">Child elements</span></span>

|<span data-ttu-id="5ec23-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="5ec23-111">**Element**</span></span>|<span data-ttu-id="5ec23-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5ec23-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ec23-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="5ec23-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="5ec23-114">メールが有効な Active Directory ディレクトリサービスオブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="5ec23-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5ec23-115">親要素</span><span class="sxs-lookup"><span data-stu-id="5ec23-115">Parent elements</span></span>

|<span data-ttu-id="5ec23-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="5ec23-116">**Element**</span></span>|<span data-ttu-id="5ec23-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="5ec23-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ec23-118">Message</span><span class="sxs-lookup"><span data-stu-id="5ec23-118">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5ec23-119">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="5ec23-119">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="5ec23-120">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="5ec23-120">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="5ec23-121">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="5ec23-121">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5ec23-122">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="5ec23-122">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5ec23-123">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="5ec23-123">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5ec23-124">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="5ec23-124">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="5ec23-125">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="5ec23-125">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5ec23-126">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="5ec23-126">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="5ec23-127">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="5ec23-127">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5ec23-128">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="5ec23-128">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="5ec23-129">会議出席依頼への返信を承諾するかを表します。</span><span class="sxs-lookup"><span data-stu-id="5ec23-129">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="5ec23-130">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="5ec23-130">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="5ec23-131">会議出席依頼に対する仮の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="5ec23-131">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="5ec23-132">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="5ec23-132">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="5ec23-133">会議出席依頼への返信を拒否することを表します。</span><span class="sxs-lookup"><span data-stu-id="5ec23-133">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="5ec23-134">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="5ec23-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="5ec23-135">Exchange ストア内のアイテムの作成者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="5ec23-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5ec23-136">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="5ec23-136">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="5ec23-137">Exchange ストア内のアイテムの特定の受信者全員への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="5ec23-137">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5ec23-138">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="5ec23-138">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="5ec23-139">受信者に転送するための Exchange ストアアイテムが保存されています。</span><span class="sxs-lookup"><span data-stu-id="5ec23-139">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="5ec23-140">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="5ec23-140">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="5ec23-141">会議の取り消しに使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="5ec23-141">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5ec23-142">注釈</span><span class="sxs-lookup"><span data-stu-id="5ec23-142">Remarks</span></span>

<span data-ttu-id="5ec23-143">**ReceivedRepresenting**要素は、代理人アクセスのシナリオで**From**および**ReceivedBy**要素と共に使用されます。</span><span class="sxs-lookup"><span data-stu-id="5ec23-143">The **ReceivedRepresenting** element is used together with the **From** and **ReceivedBy** elements in delegate access scenarios.</span></span> <span data-ttu-id="5ec23-144">次の表に、これらの要素がデリゲートアクセスシナリオで表すエンティティを示します。</span><span class="sxs-lookup"><span data-stu-id="5ec23-144">The following table lists the entities that these elements represent in a delegate access scenario.</span></span> 
  
<span data-ttu-id="5ec23-145">**代理人アクセスシナリオの要素**</span><span class="sxs-lookup"><span data-stu-id="5ec23-145">**Elements in a delegate access scenario**</span></span>

|<span data-ttu-id="5ec23-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="5ec23-146">**Element**</span></span>|<span data-ttu-id="5ec23-147">**要素が表すエンティティ**</span><span class="sxs-lookup"><span data-stu-id="5ec23-147">**Entity that the element represent**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ec23-148">From</span><span class="sxs-lookup"><span data-stu-id="5ec23-148">From</span></span>](from.md) <br/> |<span data-ttu-id="5ec23-149">ThirdParty</span><span class="sxs-lookup"><span data-stu-id="5ec23-149">ThirdParty</span></span>  <br/> |
|[<span data-ttu-id="5ec23-150">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="5ec23-150">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="5ec23-151">代理人</span><span class="sxs-lookup"><span data-stu-id="5ec23-151">Delegate</span></span>  <br/> |
|[<span data-ttu-id="5ec23-152">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="5ec23-152">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="5ec23-153">Principal</span><span class="sxs-lookup"><span data-stu-id="5ec23-153">Principal</span></span>  <br/> |
   
<span data-ttu-id="5ec23-154">代理人アクセスのシナリオでは、ThirdParty が代理人を持つプリンシパルに会議出席依頼を送信すると、代理人には新しい会議出席依頼が表示されます。</span><span class="sxs-lookup"><span data-stu-id="5ec23-154">In a delegate access scenario, if a ThirdParty sends a meeting request to a Principal who has a Delegate, the Delegate will see a new meeting request.</span></span> <span data-ttu-id="5ec23-155">これらの要素によって、代理人が直接送信されたメッセージと、代理人の転送ルールによって送信されるメッセージを区別することができます。</span><span class="sxs-lookup"><span data-stu-id="5ec23-155">These elements enable delegates to distinguish between messages that are sent directly to them and messages that are sent to them because of a delegate forwarding rule.</span></span>
  
<span data-ttu-id="5ec23-156">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5ec23-156">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5ec23-157">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5ec23-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5ec23-158">Namespace</span><span class="sxs-lookup"><span data-stu-id="5ec23-158">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5ec23-159">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5ec23-159">Schema Name</span></span>  <br/> |<span data-ttu-id="5ec23-160">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="5ec23-160">Types schema</span></span>  <br/> |
|<span data-ttu-id="5ec23-161">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5ec23-161">Validation File</span></span>  <br/> |<span data-ttu-id="5ec23-162">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="5ec23-162">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5ec23-163">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5ec23-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="5ec23-164">正しくない</span><span class="sxs-lookup"><span data-stu-id="5ec23-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5ec23-165">関連項目</span><span class="sxs-lookup"><span data-stu-id="5ec23-165">See also</span></span>



- [<span data-ttu-id="5ec23-166">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5ec23-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: 送信元
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- From
api_type:
- schema
ms.assetid: 5a52d644-3677-4049-874c-12bd5c3080dc
description: From 要素は、メッセージの送信元のアドレスを表します。
ms.openlocfilehash: c0d655731677e56cc02c7c029264ffc96f0a18c2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459554"
---
# <a name="from"></a><span data-ttu-id="59943-103">送信元</span><span class="sxs-lookup"><span data-stu-id="59943-103">From</span></span>

<span data-ttu-id="59943-104">**From**要素は、メッセージの送信元のアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="59943-104">The **From** element represents the address from which the message was sent.</span></span> 
  
```xml
<From>
   <Mailbox/>
</From>
```

 <span data-ttu-id="59943-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="59943-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59943-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="59943-106">Attributes and elements</span></span>

<span data-ttu-id="59943-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="59943-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59943-108">属性</span><span class="sxs-lookup"><span data-stu-id="59943-108">Attributes</span></span>

<span data-ttu-id="59943-109">なし。</span><span class="sxs-lookup"><span data-stu-id="59943-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59943-110">子要素</span><span class="sxs-lookup"><span data-stu-id="59943-110">Child elements</span></span>

|<span data-ttu-id="59943-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="59943-111">**Element**</span></span>|<span data-ttu-id="59943-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="59943-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59943-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="59943-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="59943-114">メールが有効な Active Directory ディレクトリサービスオブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="59943-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="59943-115">親要素</span><span class="sxs-lookup"><span data-stu-id="59943-115">Parent elements</span></span>

|<span data-ttu-id="59943-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="59943-116">**Element**</span></span>|<span data-ttu-id="59943-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="59943-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59943-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="59943-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="59943-119">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="59943-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="59943-120">Message</span><span class="sxs-lookup"><span data-stu-id="59943-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="59943-121">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="59943-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="59943-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="59943-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="59943-123">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="59943-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="59943-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="59943-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="59943-125">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="59943-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="59943-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="59943-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="59943-127">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="59943-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="59943-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="59943-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="59943-129">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="59943-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="59943-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="59943-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="59943-131">会議出席依頼への返信を承諾するかを表します。</span><span class="sxs-lookup"><span data-stu-id="59943-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="59943-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="59943-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="59943-133">会議出席依頼に対する仮の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="59943-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="59943-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="59943-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="59943-135">会議出席依頼への返信を拒否することを表します。</span><span class="sxs-lookup"><span data-stu-id="59943-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="59943-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="59943-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="59943-137">Exchange ストア内のアイテムの作成者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="59943-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="59943-138">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="59943-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="59943-139">Exchange ストア内のアイテムの特定の受信者全員への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="59943-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="59943-140">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="59943-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="59943-141">受信者に転送するための Exchange ストアアイテムが保存されています。</span><span class="sxs-lookup"><span data-stu-id="59943-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="59943-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="59943-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="59943-143">会議の取り消しに使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="59943-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="59943-144">PostItem</span><span class="sxs-lookup"><span data-stu-id="59943-144">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="59943-145">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="59943-145">Represents a post item in the Exchange store.</span></span> <span data-ttu-id="59943-146">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="59943-146">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="59943-147">注釈</span><span class="sxs-lookup"><span data-stu-id="59943-147">Remarks</span></span>

<span data-ttu-id="59943-148">この要素は、"代理人として送信する" 電子メールに使用されます。</span><span class="sxs-lookup"><span data-stu-id="59943-148">This element is used for "send on behalf of" e-mails.</span></span>
  
<span data-ttu-id="59943-149">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="59943-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59943-150">要素の情報</span><span class="sxs-lookup"><span data-stu-id="59943-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59943-151">Namespace</span><span class="sxs-lookup"><span data-stu-id="59943-151">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="59943-152">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="59943-152">Schema Name</span></span>  <br/> |<span data-ttu-id="59943-153">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="59943-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="59943-154">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="59943-154">Validation File</span></span>  <br/> |<span data-ttu-id="59943-155">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="59943-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="59943-156">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="59943-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="59943-157">正しくない</span><span class="sxs-lookup"><span data-stu-id="59943-157">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59943-158">関連項目</span><span class="sxs-lookup"><span data-stu-id="59943-158">See also</span></span>



- [<span data-ttu-id="59943-159">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="59943-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


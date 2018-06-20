---
title: From
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
description: 要素は、メッセージの送信元アドレスを表します。
ms.openlocfilehash: 39c8c8ef84ff445e8f44ebb9f2285ccfc42353a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760612"
---
# <a name="from"></a><span data-ttu-id="de124-103">From</span><span class="sxs-lookup"><span data-stu-id="de124-103">From</span></span>

<span data-ttu-id="de124-104">**** 要素は、メッセージの送信元アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="de124-104">The **From** element represents the address from which the message was sent.</span></span> 
  
```xml
<From>
   <Mailbox/>
</From>
```

 <span data-ttu-id="de124-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="de124-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="de124-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="de124-106">Attributes and elements</span></span>

<span data-ttu-id="de124-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="de124-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de124-108">属性</span><span class="sxs-lookup"><span data-stu-id="de124-108">Attributes</span></span>

<span data-ttu-id="de124-109">なし。</span><span class="sxs-lookup"><span data-stu-id="de124-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="de124-110">子要素</span><span class="sxs-lookup"><span data-stu-id="de124-110">Child elements</span></span>

|<span data-ttu-id="de124-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="de124-111">**Element**</span></span>|<span data-ttu-id="de124-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="de124-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de124-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="de124-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="de124-114">メールが有効な Active Directory ディレクトリ サービス オブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="de124-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="de124-115">親要素</span><span class="sxs-lookup"><span data-stu-id="de124-115">Parent elements</span></span>

|<span data-ttu-id="de124-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="de124-116">**Element**</span></span>|<span data-ttu-id="de124-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="de124-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de124-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="de124-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="de124-119">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="de124-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="de124-120">Message</span><span class="sxs-lookup"><span data-stu-id="de124-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="de124-121">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="de124-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="de124-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="de124-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="de124-123">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="de124-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="de124-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="de124-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="de124-125">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="de124-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="de124-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="de124-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="de124-127">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="de124-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="de124-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="de124-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="de124-129">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="de124-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="de124-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="de124-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="de124-131">会議出席依頼、承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="de124-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="de124-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="de124-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="de124-133">仮の予定を表しますが、会議出席依頼に返信します。</span><span class="sxs-lookup"><span data-stu-id="de124-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="de124-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="de124-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="de124-135">会議出席依頼を辞退の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="de124-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="de124-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="de124-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="de124-137">Exchange ストア内のアイテムの作成者に返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de124-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="de124-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="de124-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="de124-139">Exchange ストア内のアイテムの識別されたすべての受信者への返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de124-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="de124-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="de124-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="de124-141">受信者に転送するのには、Exchange ストアの項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de124-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="de124-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="de124-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="de124-143">会議をキャンセルするために使用される応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="de124-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="de124-144">PostItem</span><span class="sxs-lookup"><span data-stu-id="de124-144">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="de124-145">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="de124-145">Represents a post item in the Exchange store.</span></span> <span data-ttu-id="de124-146">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="de124-146">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="de124-147">備考</span><span class="sxs-lookup"><span data-stu-id="de124-147">Remarks</span></span>

<span data-ttu-id="de124-148">メールの「代理送信」のこの要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="de124-148">This element is used for "send on behalf of" e-mails.</span></span>
  
<span data-ttu-id="de124-149">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="de124-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de124-150">要素情報</span><span class="sxs-lookup"><span data-stu-id="de124-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de124-151">名前空間</span><span class="sxs-lookup"><span data-stu-id="de124-151">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="de124-152">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="de124-152">Schema Name</span></span>  <br/> |<span data-ttu-id="de124-153">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="de124-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="de124-154">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="de124-154">Validation File</span></span>  <br/> |<span data-ttu-id="de124-155">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="de124-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="de124-156">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="de124-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="de124-157">False</span><span class="sxs-lookup"><span data-stu-id="de124-157">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="de124-158">関連項目</span><span class="sxs-lookup"><span data-stu-id="de124-158">See also</span></span>



- [<span data-ttu-id="de124-159">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="de124-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


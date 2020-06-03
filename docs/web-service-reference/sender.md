---
title: Sender
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Sender
api_type:
- schema
ms.assetid: 26d1a46e-e1d3-44b8-a02d-fa6f83aa5cda
description: Sender 要素は、アイテムの送信者を識別します。
ms.openlocfilehash: f056fefdd5c5832d4b5bf20416e07e376f6a03de
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530580"
---
# <a name="sender"></a><span data-ttu-id="9f5ba-103">Sender</span><span class="sxs-lookup"><span data-stu-id="9f5ba-103">Sender</span></span>

<span data-ttu-id="9f5ba-104">**Sender**要素は、アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-104">The **Sender** element identifies the sender of an item.</span></span> 
  
```xml
<Sender>
   <Mailbox/>
</Sender>
```

 <span data-ttu-id="9f5ba-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="9f5ba-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f5ba-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9f5ba-106">Attributes and elements</span></span>

<span data-ttu-id="9f5ba-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f5ba-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f5ba-108">Attributes</span></span>

<span data-ttu-id="9f5ba-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f5ba-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9f5ba-110">Child elements</span></span>

|<span data-ttu-id="9f5ba-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="9f5ba-111">**Element**</span></span>|<span data-ttu-id="9f5ba-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9f5ba-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f5ba-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="9f5ba-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="9f5ba-114">送信者を識別するメールが有効な Active Directory オブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-114">Identifies a mail enabled Active Directory object that identifies the sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f5ba-115">親要素</span><span class="sxs-lookup"><span data-stu-id="9f5ba-115">Parent elements</span></span>

|<span data-ttu-id="9f5ba-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="9f5ba-116">**Element**</span></span>|<span data-ttu-id="9f5ba-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="9f5ba-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f5ba-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="9f5ba-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="9f5ba-119">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9f5ba-120">Message</span><span class="sxs-lookup"><span data-stu-id="9f5ba-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9f5ba-121">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="9f5ba-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="9f5ba-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="9f5ba-123">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9f5ba-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="9f5ba-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="9f5ba-125">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9f5ba-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="9f5ba-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="9f5ba-127">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9f5ba-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="9f5ba-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="9f5ba-129">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9f5ba-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="9f5ba-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="9f5ba-131">会議出席依頼への返信を承諾するかを表します。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-131">Represents an accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="9f5ba-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="9f5ba-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="9f5ba-133">会議出席依頼に対する仮承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-133">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="9f5ba-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="9f5ba-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="9f5ba-135">会議出席依頼への返信を拒否することを表します。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-135">Represents a decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="9f5ba-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="9f5ba-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="9f5ba-137">Exchange ストア内のアイテムの作成者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9f5ba-138">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="9f5ba-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="9f5ba-139">Exchange ストア内のアイテムの特定の受信者全員への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9f5ba-140">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="9f5ba-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="9f5ba-141">受信者に転送するための Exchange ストアアイテムが保存されています。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="9f5ba-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="9f5ba-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="9f5ba-143">会議の取り消しに使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-143">Represents the response object used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="9f5ba-144">PostItem</span><span class="sxs-lookup"><span data-stu-id="9f5ba-144">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="9f5ba-145">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-145">Represents a post item in the Exchange store.</span></span> <span data-ttu-id="9f5ba-146">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-146">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9f5ba-147">注釈</span><span class="sxs-lookup"><span data-stu-id="9f5ba-147">Remarks</span></span>

<span data-ttu-id="9f5ba-148">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9f5ba-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f5ba-149">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9f5ba-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f5ba-150">Namespace</span><span class="sxs-lookup"><span data-stu-id="9f5ba-150">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9f5ba-151">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9f5ba-151">Schema Name</span></span>  <br/> |<span data-ttu-id="9f5ba-152">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9f5ba-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="9f5ba-153">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9f5ba-153">Validation File</span></span>  <br/> |<span data-ttu-id="9f5ba-154">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9f5ba-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9f5ba-155">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9f5ba-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="9f5ba-156">正しくない</span><span class="sxs-lookup"><span data-stu-id="9f5ba-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f5ba-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="9f5ba-157">See also</span></span>



- [<span data-ttu-id="9f5ba-158">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9f5ba-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


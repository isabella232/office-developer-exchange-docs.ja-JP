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
description: 送信者要素は、アイテムの送信者を識別します。
ms.openlocfilehash: a7b06543fadd7cf7ae05f7ae8f86122138e11076
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833323"
---
# <a name="sender"></a><span data-ttu-id="b6ef2-103">Sender</span><span class="sxs-lookup"><span data-stu-id="b6ef2-103">Sender</span></span>

<span data-ttu-id="b6ef2-104">**送信者**要素は、アイテムの送信者を識別します。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-104">The **Sender** element identifies the sender of an item.</span></span> 
  
```xml
<Sender>
   <Mailbox/>
</Sender>
```

 <span data-ttu-id="b6ef2-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="b6ef2-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6ef2-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b6ef2-106">Attributes and elements</span></span>

<span data-ttu-id="b6ef2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6ef2-108">属性</span><span class="sxs-lookup"><span data-stu-id="b6ef2-108">Attributes</span></span>

<span data-ttu-id="b6ef2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b6ef2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b6ef2-110">Child elements</span></span>

|<span data-ttu-id="b6ef2-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="b6ef2-111">**Element**</span></span>|<span data-ttu-id="b6ef2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b6ef2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6ef2-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="b6ef2-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="b6ef2-114">送信者を識別するメールが有効な Active Directory オブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-114">Identifies a mail enabled Active Directory object that identifies the sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b6ef2-115">親要素</span><span class="sxs-lookup"><span data-stu-id="b6ef2-115">Parent elements</span></span>

|<span data-ttu-id="b6ef2-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="b6ef2-116">**Element**</span></span>|<span data-ttu-id="b6ef2-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="b6ef2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6ef2-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="b6ef2-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="b6ef2-119">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b6ef2-120">Message</span><span class="sxs-lookup"><span data-stu-id="b6ef2-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b6ef2-121">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="b6ef2-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="b6ef2-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="b6ef2-123">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b6ef2-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b6ef2-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b6ef2-125">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b6ef2-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b6ef2-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="b6ef2-127">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b6ef2-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="b6ef2-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="b6ef2-129">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b6ef2-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="b6ef2-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="b6ef2-131">会議出席依頼、承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-131">Represents an accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="b6ef2-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="b6ef2-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="b6ef2-133">会議出席依頼に仮承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-133">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="b6ef2-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="b6ef2-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="b6ef2-135">会議出席依頼を辞退の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-135">Represents a decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="b6ef2-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="b6ef2-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="b6ef2-137">Exchange ストア内のアイテムの作成者に返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b6ef2-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="b6ef2-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="b6ef2-139">Exchange ストア内のアイテムの識別されたすべての受信者への返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b6ef2-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="b6ef2-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="b6ef2-141">受信者に転送するのには、Exchange ストアの項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="b6ef2-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="b6ef2-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="b6ef2-143">会議をキャンセルするために使用する応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-143">Represents the response object used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="b6ef2-144">PostItem</span><span class="sxs-lookup"><span data-stu-id="b6ef2-144">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="b6ef2-145">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-145">Represents a post item in the Exchange store.</span></span> <span data-ttu-id="b6ef2-146">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-146">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b6ef2-147">備考</span><span class="sxs-lookup"><span data-stu-id="b6ef2-147">Remarks</span></span>

<span data-ttu-id="b6ef2-148">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="b6ef2-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6ef2-149">要素情報</span><span class="sxs-lookup"><span data-stu-id="b6ef2-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6ef2-150">名前空間</span><span class="sxs-lookup"><span data-stu-id="b6ef2-150">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b6ef2-151">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b6ef2-151">Schema Name</span></span>  <br/> |<span data-ttu-id="b6ef2-152">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b6ef2-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="b6ef2-153">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b6ef2-153">Validation File</span></span>  <br/> |<span data-ttu-id="b6ef2-154">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b6ef2-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b6ef2-155">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b6ef2-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="b6ef2-156">False</span><span class="sxs-lookup"><span data-stu-id="b6ef2-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b6ef2-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="b6ef2-157">See also</span></span>



- [<span data-ttu-id="b6ef2-158">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b6ef2-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


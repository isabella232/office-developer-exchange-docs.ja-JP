---
title: ReplyTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReplyTo
api_type:
- schema
ms.assetid: 6b6ae792-e2c4-4aa0-95cb-b49b446f1e08
description: ReplyTo 要素は、応答の送信先となるアドレスの配列を指定します。
ms.openlocfilehash: 0ceb4f5edb75bbfe52a7a7156da3c2a328bea346
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833115"
---
# <a name="replyto"></a><span data-ttu-id="167f0-103">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="167f0-103">ReplyTo</span></span>

<span data-ttu-id="167f0-104">**ReplyTo**要素は、応答の送信先となるアドレスの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="167f0-104">The **ReplyTo** element identifies an array of addresses to which replies should be sent.</span></span> 
  
```xml
<ReplyTo>
   <Mailbox/>
</ReplyTo>
```

 <span data-ttu-id="167f0-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="167f0-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="167f0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="167f0-106">Attributes and elements</span></span>

<span data-ttu-id="167f0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="167f0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="167f0-108">属性</span><span class="sxs-lookup"><span data-stu-id="167f0-108">Attributes</span></span>

<span data-ttu-id="167f0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="167f0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="167f0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="167f0-110">Child elements</span></span>

|<span data-ttu-id="167f0-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="167f0-111">**Element**</span></span>|<span data-ttu-id="167f0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="167f0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="167f0-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="167f0-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="167f0-114">メールが有効な Active Directory ディレクトリ サービス オブジェクトの応答が送信されるを指定します。</span><span class="sxs-lookup"><span data-stu-id="167f0-114">Identifies a mail-enabled Active Directory directory service object to which a reply is sent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="167f0-115">親要素</span><span class="sxs-lookup"><span data-stu-id="167f0-115">Parent elements</span></span>

|<span data-ttu-id="167f0-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="167f0-116">**Element**</span></span>|<span data-ttu-id="167f0-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="167f0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="167f0-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="167f0-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="167f0-119">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="167f0-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="167f0-120">Message</span><span class="sxs-lookup"><span data-stu-id="167f0-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="167f0-121">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="167f0-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="167f0-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="167f0-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="167f0-123">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="167f0-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="167f0-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="167f0-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="167f0-125">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="167f0-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="167f0-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="167f0-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="167f0-127">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="167f0-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="167f0-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="167f0-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="167f0-129">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="167f0-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="167f0-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="167f0-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="167f0-131">会議出席依頼、承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="167f0-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="167f0-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="167f0-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="167f0-133">仮の予定を表しますが、会議出席依頼に返信します。</span><span class="sxs-lookup"><span data-stu-id="167f0-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="167f0-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="167f0-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="167f0-135">会議出席依頼を辞退の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="167f0-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="167f0-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="167f0-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="167f0-137">Exchange ストア内のアイテムの作成者に返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="167f0-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="167f0-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="167f0-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="167f0-139">Exchange ストア内のアイテムの識別されたすべての受信者への返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="167f0-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="167f0-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="167f0-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="167f0-141">受信者に転送するのには、Exchange ストアの項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="167f0-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="167f0-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="167f0-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="167f0-143">会議をキャンセルするために使用される応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="167f0-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="167f0-144">備考</span><span class="sxs-lookup"><span data-stu-id="167f0-144">Remarks</span></span>

<span data-ttu-id="167f0-145">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="167f0-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="167f0-146">要素情報</span><span class="sxs-lookup"><span data-stu-id="167f0-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="167f0-147">名前空間</span><span class="sxs-lookup"><span data-stu-id="167f0-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="167f0-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="167f0-148">Schema Name</span></span>  <br/> |<span data-ttu-id="167f0-149">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="167f0-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="167f0-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="167f0-150">Validation File</span></span>  <br/> |<span data-ttu-id="167f0-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="167f0-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="167f0-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="167f0-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="167f0-153">False</span><span class="sxs-lookup"><span data-stu-id="167f0-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="167f0-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="167f0-154">See also</span></span>



- [<span data-ttu-id="167f0-155">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="167f0-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


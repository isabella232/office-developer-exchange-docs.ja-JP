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
description: ReplyTo 要素は、返信が送信されるアドレスの配列を指定します。
ms.openlocfilehash: 08f9edce76fd01111922a2a07d1a63e288a0c1ee
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468328"
---
# <a name="replyto"></a><span data-ttu-id="ce0d2-103">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="ce0d2-103">ReplyTo</span></span>

<span data-ttu-id="ce0d2-104">**ReplyTo**要素は、返信が送信されるアドレスの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-104">The **ReplyTo** element identifies an array of addresses to which replies should be sent.</span></span> 
  
```xml
<ReplyTo>
   <Mailbox/>
</ReplyTo>
```

 <span data-ttu-id="ce0d2-105">**Arrayof受信者 Stype**</span><span class="sxs-lookup"><span data-stu-id="ce0d2-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce0d2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ce0d2-106">Attributes and elements</span></span>

<span data-ttu-id="ce0d2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce0d2-108">属性</span><span class="sxs-lookup"><span data-stu-id="ce0d2-108">Attributes</span></span>

<span data-ttu-id="ce0d2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ce0d2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ce0d2-110">Child elements</span></span>

|<span data-ttu-id="ce0d2-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="ce0d2-111">**Element**</span></span>|<span data-ttu-id="ce0d2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ce0d2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce0d2-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="ce0d2-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="ce0d2-114">返信が送信されるメールが有効な Active Directory ディレクトリサービスオブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-114">Identifies a mail-enabled Active Directory directory service object to which a reply is sent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ce0d2-115">親要素</span><span class="sxs-lookup"><span data-stu-id="ce0d2-115">Parent elements</span></span>

|<span data-ttu-id="ce0d2-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="ce0d2-116">**Element**</span></span>|<span data-ttu-id="ce0d2-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="ce0d2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce0d2-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="ce0d2-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="ce0d2-119">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce0d2-120">Message</span><span class="sxs-lookup"><span data-stu-id="ce0d2-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ce0d2-121">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="ce0d2-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="ce0d2-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="ce0d2-123">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce0d2-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ce0d2-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ce0d2-125">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce0d2-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="ce0d2-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="ce0d2-127">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce0d2-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="ce0d2-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="ce0d2-129">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce0d2-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="ce0d2-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="ce0d2-131">会議出席依頼への返信を承諾するかを表します。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="ce0d2-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="ce0d2-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="ce0d2-133">会議出席依頼に対する仮の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="ce0d2-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="ce0d2-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="ce0d2-135">会議出席依頼への返信を拒否することを表します。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="ce0d2-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="ce0d2-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="ce0d2-137">Exchange ストア内のアイテムの作成者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce0d2-138">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="ce0d2-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="ce0d2-139">Exchange ストア内のアイテムの特定の受信者全員への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce0d2-140">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="ce0d2-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="ce0d2-141">受信者に転送するための Exchange ストアアイテムが保存されています。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="ce0d2-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="ce0d2-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="ce0d2-143">会議の取り消しに使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ce0d2-144">注釈</span><span class="sxs-lookup"><span data-stu-id="ce0d2-144">Remarks</span></span>

<span data-ttu-id="ce0d2-145">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="ce0d2-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ce0d2-146">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ce0d2-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce0d2-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="ce0d2-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ce0d2-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ce0d2-148">Schema Name</span></span>  <br/> |<span data-ttu-id="ce0d2-149">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ce0d2-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="ce0d2-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ce0d2-150">Validation File</span></span>  <br/> |<span data-ttu-id="ce0d2-151">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ce0d2-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ce0d2-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ce0d2-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="ce0d2-153">正しくない</span><span class="sxs-lookup"><span data-stu-id="ce0d2-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ce0d2-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="ce0d2-154">See also</span></span>



- [<span data-ttu-id="ce0d2-155">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ce0d2-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


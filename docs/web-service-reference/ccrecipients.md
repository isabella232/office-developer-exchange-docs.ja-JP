---
title: CcRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CcRecipients
api_type:
- schema
ms.assetid: 5c20ec3a-0bee-4e67-b220-586ed0d601c9
description: CcRecipients "要素" は、メッセージのコピーを受信する受信者のコレクションを表します。
ms.openlocfilehash: 57d0e2d3b2c44fbd7bb30696002b27e83d1e274e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462207"
---
# <a name="ccrecipients"></a><span data-ttu-id="2914e-103">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="2914e-103">CcRecipients</span></span>

<span data-ttu-id="2914e-104">**Ccrecipients** "要素" は、メッセージのコピーを受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="2914e-104">The **CcRecipients** element represents a collection of recipients that will receive a copy of the message.</span></span> 
  
```xml
<CcRecipients>
   <Mailbox/>
</CcRecipients>
```

 <span data-ttu-id="2914e-105">**Arrayof受信者 Stype**</span><span class="sxs-lookup"><span data-stu-id="2914e-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2914e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2914e-106">Attributes and elements</span></span>

<span data-ttu-id="2914e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2914e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2914e-108">属性</span><span class="sxs-lookup"><span data-stu-id="2914e-108">Attributes</span></span>

<span data-ttu-id="2914e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2914e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2914e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2914e-110">Child elements</span></span>

|<span data-ttu-id="2914e-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="2914e-111">**Element**</span></span>|<span data-ttu-id="2914e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2914e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2914e-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="2914e-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="2914e-114">メールが有効な Active Directory ディレクトリサービスオブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="2914e-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2914e-115">親要素</span><span class="sxs-lookup"><span data-stu-id="2914e-115">Parent elements</span></span>

|<span data-ttu-id="2914e-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="2914e-116">**Element**</span></span>|<span data-ttu-id="2914e-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="2914e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2914e-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="2914e-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="2914e-119">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="2914e-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2914e-120">Message</span><span class="sxs-lookup"><span data-stu-id="2914e-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2914e-121">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="2914e-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="2914e-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="2914e-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="2914e-123">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="2914e-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2914e-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="2914e-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2914e-125">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="2914e-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2914e-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="2914e-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="2914e-127">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="2914e-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2914e-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="2914e-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="2914e-129">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="2914e-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2914e-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="2914e-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="2914e-131">会議出席依頼への返信を承諾するかを表します。</span><span class="sxs-lookup"><span data-stu-id="2914e-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="2914e-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="2914e-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="2914e-133">会議出席依頼に対する仮の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="2914e-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="2914e-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="2914e-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="2914e-135">会議出席依頼への返信を拒否することを表します。</span><span class="sxs-lookup"><span data-stu-id="2914e-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="2914e-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="2914e-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="2914e-137">Exchange ストア内のアイテムの作成者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="2914e-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2914e-138">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="2914e-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="2914e-139">Exchange ストア内のアイテムの特定の受信者全員への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="2914e-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2914e-140">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="2914e-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="2914e-141">受信者に転送するための Exchange ストアアイテムが保存されています。</span><span class="sxs-lookup"><span data-stu-id="2914e-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="2914e-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="2914e-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="2914e-143">会議の取り消しに使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="2914e-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2914e-144">注釈</span><span class="sxs-lookup"><span data-stu-id="2914e-144">Remarks</span></span>

<span data-ttu-id="2914e-145">FindItem 要求を使用して、 **Ccrecipients**メンバーを取得することはできません。</span><span class="sxs-lookup"><span data-stu-id="2914e-145">You cannot get **CcRecipients** by using a FindItem request.</span></span> <span data-ttu-id="2914e-146">GetItem 要求を使用して**Ccrecipients**メンバーを取得します。</span><span class="sxs-lookup"><span data-stu-id="2914e-146">Use a GetItem request to get **CcRecipients**.</span></span>
  
<span data-ttu-id="2914e-147">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2914e-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2914e-148">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2914e-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2914e-149">Namespace</span><span class="sxs-lookup"><span data-stu-id="2914e-149">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2914e-150">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2914e-150">Schema Name</span></span>  <br/> |<span data-ttu-id="2914e-151">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="2914e-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="2914e-152">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2914e-152">Validation File</span></span>  <br/> |<span data-ttu-id="2914e-153">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="2914e-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2914e-154">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2914e-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="2914e-155">正しくない</span><span class="sxs-lookup"><span data-stu-id="2914e-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2914e-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="2914e-156">See also</span></span>



- [<span data-ttu-id="2914e-157">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2914e-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


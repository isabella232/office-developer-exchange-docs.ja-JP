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
description: CcRecipients 要素は、メッセージのコピーを受け取る受信者のコレクションを表します。
ms.openlocfilehash: 0afe19cfae49dbf48c685296a83ab1330b631d04
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759614"
---
# <a name="ccrecipients"></a><span data-ttu-id="5a2b0-103">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="5a2b0-103">CcRecipients</span></span>

<span data-ttu-id="5a2b0-104">**CcRecipients**要素は、メッセージのコピーを受け取る受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-104">The **CcRecipients** element represents a collection of recipients that will receive a copy of the message.</span></span> 
  
```xml
<CcRecipients>
   <Mailbox/>
</CcRecipients>
```

 <span data-ttu-id="5a2b0-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="5a2b0-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a2b0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5a2b0-106">Attributes and elements</span></span>

<span data-ttu-id="5a2b0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a2b0-108">属性</span><span class="sxs-lookup"><span data-stu-id="5a2b0-108">Attributes</span></span>

<span data-ttu-id="5a2b0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a2b0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5a2b0-110">Child elements</span></span>

|<span data-ttu-id="5a2b0-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="5a2b0-111">**Element**</span></span>|<span data-ttu-id="5a2b0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5a2b0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a2b0-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="5a2b0-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="5a2b0-114">メールが有効な Active Directory ディレクトリ サービス オブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5a2b0-115">親要素</span><span class="sxs-lookup"><span data-stu-id="5a2b0-115">Parent elements</span></span>

|<span data-ttu-id="5a2b0-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="5a2b0-116">**Element**</span></span>|<span data-ttu-id="5a2b0-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="5a2b0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a2b0-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="5a2b0-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="5a2b0-119">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5a2b0-120">Message</span><span class="sxs-lookup"><span data-stu-id="5a2b0-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5a2b0-121">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="5a2b0-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="5a2b0-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="5a2b0-123">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5a2b0-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="5a2b0-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5a2b0-125">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5a2b0-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="5a2b0-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="5a2b0-127">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5a2b0-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="5a2b0-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="5a2b0-129">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5a2b0-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="5a2b0-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="5a2b0-131">会議出席依頼、承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="5a2b0-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="5a2b0-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="5a2b0-133">仮の予定を表しますが、会議出席依頼に返信します。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="5a2b0-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="5a2b0-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="5a2b0-135">会議出席依頼を辞退の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="5a2b0-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="5a2b0-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="5a2b0-137">Exchange ストア内のアイテムの作成者に返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5a2b0-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="5a2b0-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="5a2b0-139">Exchange ストア内のアイテムの識別されたすべての受信者への返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5a2b0-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="5a2b0-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="5a2b0-141">受信者に転送するのには、Exchange ストアの項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="5a2b0-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="5a2b0-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="5a2b0-143">会議をキャンセルするために使用される応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5a2b0-144">備考</span><span class="sxs-lookup"><span data-stu-id="5a2b0-144">Remarks</span></span>

<span data-ttu-id="5a2b0-145">**CcRecipients**を FindItem 要求を使用して取得できません。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-145">You cannot get **CcRecipients** by using a FindItem request.</span></span> <span data-ttu-id="5a2b0-146">**CcRecipients**を取得するのにには、GetItem 要求を使用します。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-146">Use a GetItem request to get **CcRecipients**.</span></span>
  
<span data-ttu-id="5a2b0-147">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="5a2b0-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a2b0-148">要素情報</span><span class="sxs-lookup"><span data-stu-id="5a2b0-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a2b0-149">名前空間</span><span class="sxs-lookup"><span data-stu-id="5a2b0-149">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5a2b0-150">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5a2b0-150">Schema Name</span></span>  <br/> |<span data-ttu-id="5a2b0-151">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5a2b0-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="5a2b0-152">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5a2b0-152">Validation File</span></span>  <br/> |<span data-ttu-id="5a2b0-153">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5a2b0-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5a2b0-154">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5a2b0-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="5a2b0-155">False</span><span class="sxs-lookup"><span data-stu-id="5a2b0-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a2b0-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="5a2b0-156">See also</span></span>



- [<span data-ttu-id="5a2b0-157">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5a2b0-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


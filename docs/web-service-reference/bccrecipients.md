---
title: BccRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BccRecipients
api_type:
- schema
ms.assetid: c4e05168-d36b-4740-a526-4b7da53553c1
description: BccRecipients 要素は、電子メール メッセージのブラインド カーボン コピー (Bcc) を受信する受信者のコレクションを表します。
ms.openlocfilehash: 858fe74c32cb7d1ed624888c06bba4ffe09d489e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759495"
---
# <a name="bccrecipients"></a><span data-ttu-id="8a56d-103">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="8a56d-103">BccRecipients</span></span>

<span data-ttu-id="8a56d-104">**BccRecipients**要素は、電子メール メッセージのブラインド カーボン コピー (Bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="8a56d-104">The **BccRecipients** element represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail message.</span></span> 
  
```xml
<BccRecipients>
   <Mailbox/>
</BccRecipients>
```

 <span data-ttu-id="8a56d-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="8a56d-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8a56d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8a56d-106">Attributes and elements</span></span>

<span data-ttu-id="8a56d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8a56d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a56d-108">属性</span><span class="sxs-lookup"><span data-stu-id="8a56d-108">Attributes</span></span>

<span data-ttu-id="8a56d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8a56d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8a56d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8a56d-110">Child elements</span></span>

|<span data-ttu-id="8a56d-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="8a56d-111">**Element**</span></span>|<span data-ttu-id="8a56d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="8a56d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a56d-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="8a56d-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="8a56d-114">メールが有効な Active Directory ディレクトリ サービス オブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="8a56d-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8a56d-115">親要素</span><span class="sxs-lookup"><span data-stu-id="8a56d-115">Parent elements</span></span>

|<span data-ttu-id="8a56d-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="8a56d-116">**Element**</span></span>|<span data-ttu-id="8a56d-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="8a56d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a56d-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="8a56d-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="8a56d-119">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="8a56d-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8a56d-120">Message</span><span class="sxs-lookup"><span data-stu-id="8a56d-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8a56d-121">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="8a56d-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="8a56d-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="8a56d-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="8a56d-123">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="8a56d-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8a56d-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="8a56d-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="8a56d-125">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="8a56d-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8a56d-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="8a56d-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="8a56d-127">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="8a56d-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8a56d-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="8a56d-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="8a56d-129">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="8a56d-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8a56d-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="8a56d-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="8a56d-131">会議出席依頼、承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="8a56d-131">Represents an accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="8a56d-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="8a56d-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="8a56d-133">会議出席依頼に仮承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="8a56d-133">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="8a56d-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="8a56d-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="8a56d-135">会議出席依頼を辞退の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="8a56d-135">Represents a decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="8a56d-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="8a56d-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="8a56d-137">Exchange ストア内のアイテムの作成者に返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8a56d-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8a56d-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="8a56d-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="8a56d-139">Exchange ストア内のアイテムの識別されたすべての受信者への返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8a56d-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8a56d-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="8a56d-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="8a56d-141">受信者に転送するのには、Exchange ストアの項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8a56d-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="8a56d-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="8a56d-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="8a56d-143">会議をキャンセルするために使用される応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="8a56d-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8a56d-144">備考</span><span class="sxs-lookup"><span data-stu-id="8a56d-144">Remarks</span></span>

<span data-ttu-id="8a56d-145">**BccRecipients**を FindItem 要求を使用して取得できません。</span><span class="sxs-lookup"><span data-stu-id="8a56d-145">You cannot get **BccRecipients** by using a FindItem request.</span></span> <span data-ttu-id="8a56d-146">**BccRecipients**を取得するのにには、GetItem 要求を使用します。</span><span class="sxs-lookup"><span data-stu-id="8a56d-146">Use a GetItem request to get **BccRecipients**.</span></span>
  
<span data-ttu-id="8a56d-147">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="8a56d-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8a56d-148">要素情報</span><span class="sxs-lookup"><span data-stu-id="8a56d-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a56d-149">名前空間</span><span class="sxs-lookup"><span data-stu-id="8a56d-149">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8a56d-150">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8a56d-150">Schema Name</span></span>  <br/> |<span data-ttu-id="8a56d-151">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8a56d-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="8a56d-152">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8a56d-152">Validation File</span></span>  <br/> |<span data-ttu-id="8a56d-153">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8a56d-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8a56d-154">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8a56d-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="8a56d-155">False</span><span class="sxs-lookup"><span data-stu-id="8a56d-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8a56d-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="8a56d-156">See also</span></span>



- [<span data-ttu-id="8a56d-157">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8a56d-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


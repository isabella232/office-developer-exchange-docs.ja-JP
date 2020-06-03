---
title: ToRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ToRecipients
api_type:
- schema
ms.assetid: 72dc3be8-30bb-4ae1-acf4-fb94ff490631
description: トーラス要素には、アイテムの受信者の配列が含まれています。 次に、アイテムのプライマリ受信者を示します。
ms.openlocfilehash: 39ee359e1eaf3d0b6455fb1734222e78054dc7f3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467544"
---
# <a name="torecipients"></a><span data-ttu-id="c9f8a-104">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="c9f8a-104">ToRecipients</span></span>

<span data-ttu-id="c9f8a-105">**トーラス**要素には、アイテムの受信者の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-105">The **ToRecipients** element contains an array of recipients of an item.</span></span> <span data-ttu-id="c9f8a-106">次に、アイテムのプライマリ受信者を示します。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-106">These are the primary recipients of an item.</span></span> 
  
```xml
<ToRecipients>
   <Mailbox/>
</ToRecipients>
```

 <span data-ttu-id="c9f8a-107">**Arrayof受信者 Stype**</span><span class="sxs-lookup"><span data-stu-id="c9f8a-107">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9f8a-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c9f8a-108">Attributes and elements</span></span>

<span data-ttu-id="c9f8a-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9f8a-110">属性</span><span class="sxs-lookup"><span data-stu-id="c9f8a-110">Attributes</span></span>

<span data-ttu-id="c9f8a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9f8a-112">子要素</span><span class="sxs-lookup"><span data-stu-id="c9f8a-112">Child elements</span></span>

|<span data-ttu-id="c9f8a-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="c9f8a-113">**Element**</span></span>|<span data-ttu-id="c9f8a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c9f8a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9f8a-115">メールボックス</span><span class="sxs-lookup"><span data-stu-id="c9f8a-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="c9f8a-116">メールが有効な Active Directory ディレクトリサービスオブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-116">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c9f8a-117">親要素</span><span class="sxs-lookup"><span data-stu-id="c9f8a-117">Parent elements</span></span>

|<span data-ttu-id="c9f8a-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="c9f8a-118">**Element**</span></span>|<span data-ttu-id="c9f8a-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="c9f8a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9f8a-120">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="c9f8a-120">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="c9f8a-121">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-121">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c9f8a-122">Message</span><span class="sxs-lookup"><span data-stu-id="c9f8a-122">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c9f8a-123">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-123">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="c9f8a-124">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="c9f8a-124">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="c9f8a-125">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-125">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c9f8a-126">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c9f8a-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c9f8a-127">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c9f8a-128">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="c9f8a-128">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="c9f8a-129">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-129">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c9f8a-130">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="c9f8a-130">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="c9f8a-131">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-131">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c9f8a-132">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="c9f8a-132">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="c9f8a-133">会議出席依頼への返信を承諾するかを表します。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-133">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="c9f8a-134">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="c9f8a-134">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="c9f8a-135">会議出席依頼に対する仮の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-135">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="c9f8a-136">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="c9f8a-136">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="c9f8a-137">会議出席依頼への返信を拒否することを表します。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-137">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="c9f8a-138">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="c9f8a-138">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="c9f8a-139">Exchange ストア内のアイテムの作成者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-139">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c9f8a-140">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="c9f8a-140">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="c9f8a-141">Exchange ストア内のアイテムの特定の受信者全員への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-141">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c9f8a-142">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="c9f8a-142">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="c9f8a-143">受信者に転送するための Exchange ストアアイテムが保存されています。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-143">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="c9f8a-144">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="c9f8a-144">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="c9f8a-145">会議の取り消しに使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-145">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c9f8a-146">注釈</span><span class="sxs-lookup"><span data-stu-id="c9f8a-146">Remarks</span></span>

<span data-ttu-id="c9f8a-147">FindItem 要求を使用して、**トーラスの piを**取得することはできません。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-147">You cannot get **ToRecipients** by using a FindItem request.</span></span> <span data-ttu-id="c9f8a-148">GetItem 要求を使用して、**トーラスの piを**取得します。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-148">Use a GetItem request to get the **ToRecipients**.</span></span>
  
<span data-ttu-id="c9f8a-149">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c9f8a-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9f8a-150">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c9f8a-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9f8a-151">Namespace</span><span class="sxs-lookup"><span data-stu-id="c9f8a-151">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c9f8a-152">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c9f8a-152">Schema Name</span></span>  <br/> |<span data-ttu-id="c9f8a-153">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c9f8a-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="c9f8a-154">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c9f8a-154">Validation File</span></span>  <br/> |<span data-ttu-id="c9f8a-155">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c9f8a-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c9f8a-156">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c9f8a-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="c9f8a-157">正しくない</span><span class="sxs-lookup"><span data-stu-id="c9f8a-157">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9f8a-158">関連項目</span><span class="sxs-lookup"><span data-stu-id="c9f8a-158">See also</span></span>



- [<span data-ttu-id="c9f8a-159">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c9f8a-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


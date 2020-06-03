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
description: BccRecipients 要素は、電子メールメッセージのブラインドカーボンコピー (Bcc) を受信する受信者のコレクションを表します。
ms.openlocfilehash: 96070415c6d92a893f6c560884d9d191c7d5f15b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529505"
---
# <a name="bccrecipients"></a><span data-ttu-id="56a49-103">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="56a49-103">BccRecipients</span></span>

<span data-ttu-id="56a49-104">**Bccrecipients**要素は、電子メールメッセージのブラインドカーボンコピー (bcc) を受信する受信者のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="56a49-104">The **BccRecipients** element represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail message.</span></span> 
  
```xml
<BccRecipients>
   <Mailbox/>
</BccRecipients>
```

 <span data-ttu-id="56a49-105">**Arrayof受信者 Stype**</span><span class="sxs-lookup"><span data-stu-id="56a49-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="56a49-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="56a49-106">Attributes and elements</span></span>

<span data-ttu-id="56a49-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="56a49-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56a49-108">属性</span><span class="sxs-lookup"><span data-stu-id="56a49-108">Attributes</span></span>

<span data-ttu-id="56a49-109">なし。</span><span class="sxs-lookup"><span data-stu-id="56a49-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="56a49-110">子要素</span><span class="sxs-lookup"><span data-stu-id="56a49-110">Child elements</span></span>

|<span data-ttu-id="56a49-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="56a49-111">**Element**</span></span>|<span data-ttu-id="56a49-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="56a49-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56a49-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="56a49-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="56a49-114">メールが有効な Active Directory ディレクトリサービスオブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="56a49-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="56a49-115">親要素</span><span class="sxs-lookup"><span data-stu-id="56a49-115">Parent elements</span></span>

|<span data-ttu-id="56a49-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="56a49-116">**Element**</span></span>|<span data-ttu-id="56a49-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="56a49-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56a49-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="56a49-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="56a49-119">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="56a49-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="56a49-120">Message</span><span class="sxs-lookup"><span data-stu-id="56a49-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="56a49-121">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="56a49-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="56a49-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="56a49-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="56a49-123">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="56a49-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="56a49-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="56a49-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="56a49-125">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="56a49-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="56a49-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="56a49-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="56a49-127">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="56a49-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="56a49-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="56a49-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="56a49-129">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="56a49-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="56a49-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="56a49-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="56a49-131">会議出席依頼への返信を承諾するかを表します。</span><span class="sxs-lookup"><span data-stu-id="56a49-131">Represents an accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="56a49-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="56a49-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="56a49-133">会議出席依頼に対する仮承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="56a49-133">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="56a49-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="56a49-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="56a49-135">会議出席依頼への返信を拒否することを表します。</span><span class="sxs-lookup"><span data-stu-id="56a49-135">Represents a decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="56a49-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="56a49-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="56a49-137">Exchange ストア内のアイテムの作成者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="56a49-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="56a49-138">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="56a49-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="56a49-139">Exchange ストア内のアイテムの特定の受信者全員への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="56a49-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="56a49-140">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="56a49-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="56a49-141">受信者に転送するための Exchange ストアアイテムが保存されています。</span><span class="sxs-lookup"><span data-stu-id="56a49-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="56a49-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="56a49-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="56a49-143">会議の取り消しに使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="56a49-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="56a49-144">注釈</span><span class="sxs-lookup"><span data-stu-id="56a49-144">Remarks</span></span>

<span data-ttu-id="56a49-145">FindItem 要求を使用して**Bccrecipients**れたイベントを取得することはできません。</span><span class="sxs-lookup"><span data-stu-id="56a49-145">You cannot get **BccRecipients** by using a FindItem request.</span></span> <span data-ttu-id="56a49-146">GetItem 要求を使用して、 **Bccrecipients**イベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="56a49-146">Use a GetItem request to get **BccRecipients**.</span></span>
  
<span data-ttu-id="56a49-147">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="56a49-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="56a49-148">要素の情報</span><span class="sxs-lookup"><span data-stu-id="56a49-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56a49-149">Namespace</span><span class="sxs-lookup"><span data-stu-id="56a49-149">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="56a49-150">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="56a49-150">Schema Name</span></span>  <br/> |<span data-ttu-id="56a49-151">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="56a49-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="56a49-152">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="56a49-152">Validation File</span></span>  <br/> |<span data-ttu-id="56a49-153">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="56a49-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="56a49-154">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="56a49-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="56a49-155">正しくない</span><span class="sxs-lookup"><span data-stu-id="56a49-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="56a49-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="56a49-156">See also</span></span>



- [<span data-ttu-id="56a49-157">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="56a49-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


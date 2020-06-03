---
title: IsDeliveryReceiptRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsDeliveryReceiptRequested
api_type:
- schema
ms.assetid: 97776b7e-942c-4663-8277-165d64364daa
description: IsDeliveryReceiptRequested 要素は、アイテムの送信者が配信確認を要求するかどうかを示します。
ms.openlocfilehash: 94bcb79df16e5ef1d8128f2e2d1e8536d9c31603
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458181"
---
# <a name="isdeliveryreceiptrequested"></a><span data-ttu-id="d11ea-103">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d11ea-103">IsDeliveryReceiptRequested</span></span>

<span data-ttu-id="d11ea-104">**IsDeliveryReceiptRequested**要素は、アイテムの送信者が配信確認を要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d11ea-104">The **IsDeliveryReceiptRequested** element indicates whether the sender of an item requests a delivery receipt.</span></span> 
  
```xml
<IsDeliveryReceiptRequested/>
```

 <span data-ttu-id="d11ea-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d11ea-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d11ea-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d11ea-106">Attributes and elements</span></span>

<span data-ttu-id="d11ea-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d11ea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d11ea-108">属性</span><span class="sxs-lookup"><span data-stu-id="d11ea-108">Attributes</span></span>

<span data-ttu-id="d11ea-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d11ea-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d11ea-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d11ea-110">Child elements</span></span>

<span data-ttu-id="d11ea-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d11ea-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d11ea-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d11ea-112">Parent elements</span></span>

|<span data-ttu-id="d11ea-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d11ea-113">**Element**</span></span>|<span data-ttu-id="d11ea-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d11ea-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d11ea-115">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="d11ea-115">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="d11ea-116">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="d11ea-116">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d11ea-117">Message</span><span class="sxs-lookup"><span data-stu-id="d11ea-117">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d11ea-118">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="d11ea-118">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="d11ea-119">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="d11ea-119">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="d11ea-120">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="d11ea-120">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d11ea-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d11ea-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d11ea-122">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="d11ea-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d11ea-123">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="d11ea-123">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="d11ea-124">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="d11ea-124">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d11ea-125">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="d11ea-125">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="d11ea-126">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="d11ea-126">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d11ea-127">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="d11ea-127">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="d11ea-128">会議出席依頼への返信を承諾するかを表します。</span><span class="sxs-lookup"><span data-stu-id="d11ea-128">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="d11ea-129">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="d11ea-129">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="d11ea-130">会議出席依頼に対する仮の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="d11ea-130">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="d11ea-131">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="d11ea-131">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="d11ea-132">会議出席依頼への返信を拒否することを表します。</span><span class="sxs-lookup"><span data-stu-id="d11ea-132">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="d11ea-133">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="d11ea-133">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="d11ea-134">Exchange ストア内のアイテムの作成者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="d11ea-134">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d11ea-135">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="d11ea-135">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="d11ea-136">Exchange ストア内のアイテムの特定の受信者全員への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="d11ea-136">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d11ea-137">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="d11ea-137">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="d11ea-138">受信者に転送するための Exchange ストアアイテムが保存されています。</span><span class="sxs-lookup"><span data-stu-id="d11ea-138">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="d11ea-139">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="d11ea-139">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="d11ea-140">会議の取り消しに使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="d11ea-140">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d11ea-141">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d11ea-141">Text value</span></span>

<span data-ttu-id="d11ea-142">テキスト値が**true の場合**は、アイテムの受信者から配信確認が要求されることを示します。</span><span class="sxs-lookup"><span data-stu-id="d11ea-142">A text value of **true** indicates that a delivery receipt is requested from the recipient of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d11ea-143">注釈</span><span class="sxs-lookup"><span data-stu-id="d11ea-143">Remarks</span></span>

<span data-ttu-id="d11ea-144">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="d11ea-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d11ea-145">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d11ea-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d11ea-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="d11ea-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d11ea-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d11ea-147">Schema Name</span></span>  <br/> |<span data-ttu-id="d11ea-148">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d11ea-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="d11ea-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d11ea-149">Validation File</span></span>  <br/> |<span data-ttu-id="d11ea-150">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d11ea-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d11ea-151">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d11ea-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="d11ea-152">正しくない</span><span class="sxs-lookup"><span data-stu-id="d11ea-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d11ea-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="d11ea-153">See also</span></span>



- [<span data-ttu-id="d11ea-154">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d11ea-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


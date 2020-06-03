---
title: IsReadReceiptRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsReadReceiptRequested
api_type:
- schema
ms.assetid: 7ab6edd5-c7ed-4701-8de3-d7dc7ecfa9c2
description: IsReadReceiptRequested 要素は、アイテムの送信者が開封確認メッセージを要求するかどうかを示します。
ms.openlocfilehash: ff0c512ef23b315d4de1194432408f5b408029d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457789"
---
# <a name="isreadreceiptrequested"></a><span data-ttu-id="b65bc-103">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="b65bc-103">IsReadReceiptRequested</span></span>

<span data-ttu-id="b65bc-104">**IsReadReceiptRequested**要素は、アイテムの送信者が開封確認メッセージを要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b65bc-104">The **IsReadReceiptRequested** element indicates whether the sender of an item requests a read receipt.</span></span> 
  
```xml
<IsReadReceiptRequested/>
```

 <span data-ttu-id="b65bc-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b65bc-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b65bc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b65bc-106">Attributes and elements</span></span>

<span data-ttu-id="b65bc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b65bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b65bc-108">属性</span><span class="sxs-lookup"><span data-stu-id="b65bc-108">Attributes</span></span>

<span data-ttu-id="b65bc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b65bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b65bc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b65bc-110">Child elements</span></span>

<span data-ttu-id="b65bc-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b65bc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b65bc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b65bc-112">Parent elements</span></span>

|<span data-ttu-id="b65bc-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b65bc-113">**Element**</span></span>|<span data-ttu-id="b65bc-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b65bc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b65bc-115">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="b65bc-115">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="b65bc-116">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="b65bc-116">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b65bc-117">Message</span><span class="sxs-lookup"><span data-stu-id="b65bc-117">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b65bc-118">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="b65bc-118">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="b65bc-119">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="b65bc-119">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="b65bc-120">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="b65bc-120">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b65bc-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b65bc-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b65bc-122">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="b65bc-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b65bc-123">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b65bc-123">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="b65bc-124">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="b65bc-124">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b65bc-125">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="b65bc-125">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="b65bc-126">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="b65bc-126">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b65bc-127">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="b65bc-127">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="b65bc-128">会議出席依頼への返信を承諾するかを表します。</span><span class="sxs-lookup"><span data-stu-id="b65bc-128">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="b65bc-129">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="b65bc-129">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="b65bc-130">会議出席依頼に対する仮の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="b65bc-130">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="b65bc-131">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="b65bc-131">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="b65bc-132">会議出席依頼への返信を拒否することを表します。</span><span class="sxs-lookup"><span data-stu-id="b65bc-132">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="b65bc-133">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="b65bc-133">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="b65bc-134">Exchange ストア内のアイテムの作成者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="b65bc-134">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b65bc-135">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="b65bc-135">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="b65bc-136">Exchange ストア内のアイテムの特定の受信者全員への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="b65bc-136">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b65bc-137">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="b65bc-137">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="b65bc-138">受信者に転送するための Exchange ストアアイテムが保存されています。</span><span class="sxs-lookup"><span data-stu-id="b65bc-138">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="b65bc-139">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="b65bc-139">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="b65bc-140">会議の取り消しに使用される response オブジェクト thatis を表します。</span><span class="sxs-lookup"><span data-stu-id="b65bc-140">Represents the response object thatis used to cancel a meeting.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b65bc-141">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b65bc-141">Text value</span></span>

<span data-ttu-id="b65bc-142">テキスト値が**true の場合**は、アイテムの受信者が開封確認メッセージを要求していることを示します。</span><span class="sxs-lookup"><span data-stu-id="b65bc-142">A text value of **true** indicates that a read receipt is requested from the recipient of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b65bc-143">注釈</span><span class="sxs-lookup"><span data-stu-id="b65bc-143">Remarks</span></span>

<span data-ttu-id="b65bc-144">**IsReadReceiptRequested**が**true**の場合、 [isread](isread.md)を**true**に設定すると開封確認メッセージが送信されます。</span><span class="sxs-lookup"><span data-stu-id="b65bc-144">If **IsReadReceiptRequested** is **true**, setting [IsRead](isread.md) to **true** sends a read receipt.</span></span> <span data-ttu-id="b65bc-145">受信者は、 **isread**プロパティを設定する前に、 [SuppressReadReceipt](suppressreadreceipt.md) response オブジェクトを送信することによって、開封確認メッセージを抑制することができます。</span><span class="sxs-lookup"><span data-stu-id="b65bc-145">The recipient can suppress read receipts by submitting the [SuppressReadReceipt](suppressreadreceipt.md) response object before setting the **IsRead** property.</span></span> 
  
<span data-ttu-id="b65bc-146">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b65bc-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b65bc-147">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b65bc-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b65bc-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="b65bc-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b65bc-149">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b65bc-149">Schema Name</span></span>  <br/> |<span data-ttu-id="b65bc-150">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b65bc-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="b65bc-151">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b65bc-151">Validation File</span></span>  <br/> |<span data-ttu-id="b65bc-152">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b65bc-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b65bc-153">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b65bc-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="b65bc-154">正しくない</span><span class="sxs-lookup"><span data-stu-id="b65bc-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b65bc-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="b65bc-155">See also</span></span>



- [<span data-ttu-id="b65bc-156">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b65bc-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


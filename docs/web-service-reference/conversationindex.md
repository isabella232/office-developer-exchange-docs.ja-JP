---
title: ConversationIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationIndex
api_type:
- schema
ms.assetid: fdf47e22-8d93-4ae4-883b-0c9f07f48724
description: ConversationIndex 要素には、このメッセージが属しているスレッドを表すバイナリ ID が含まれています。
ms.openlocfilehash: 03874c6462be6380e34c999bc2354c376a462882
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461437"
---
# <a name="conversationindex"></a><span data-ttu-id="64ceb-103">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="64ceb-103">ConversationIndex</span></span>

<span data-ttu-id="64ceb-104">**ConversationIndex**要素には、このメッセージが属しているスレッドを表すバイナリ ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="64ceb-104">The **ConversationIndex** element contains a binary ID that represents the thread to which this message belongs.</span></span> 
  
```xml
<ConversationIndex/>
```

 <span data-ttu-id="64ceb-105">**Base64Binary**</span><span class="sxs-lookup"><span data-stu-id="64ceb-105">**Base64Binary**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64ceb-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="64ceb-106">Attributes and elements</span></span>

<span data-ttu-id="64ceb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="64ceb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64ceb-108">属性</span><span class="sxs-lookup"><span data-stu-id="64ceb-108">Attributes</span></span>

<span data-ttu-id="64ceb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="64ceb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64ceb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="64ceb-110">Child elements</span></span>

<span data-ttu-id="64ceb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="64ceb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="64ceb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="64ceb-112">Parent elements</span></span>

|<span data-ttu-id="64ceb-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="64ceb-113">**Element**</span></span>|<span data-ttu-id="64ceb-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="64ceb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64ceb-115">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="64ceb-115">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="64ceb-116">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="64ceb-116">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="64ceb-117">Message</span><span class="sxs-lookup"><span data-stu-id="64ceb-117">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="64ceb-118">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="64ceb-118">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="64ceb-119">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="64ceb-119">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="64ceb-120">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="64ceb-120">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="64ceb-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="64ceb-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="64ceb-122">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="64ceb-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="64ceb-123">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="64ceb-123">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="64ceb-124">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="64ceb-124">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="64ceb-125">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="64ceb-125">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="64ceb-126">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="64ceb-126">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="64ceb-127">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="64ceb-127">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="64ceb-128">会議出席依頼への返信を承諾するかを表します。</span><span class="sxs-lookup"><span data-stu-id="64ceb-128">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="64ceb-129">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="64ceb-129">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="64ceb-130">会議出席依頼に対する仮承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="64ceb-130">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="64ceb-131">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="64ceb-131">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="64ceb-132">会議出席依頼への返信を拒否することを表します。</span><span class="sxs-lookup"><span data-stu-id="64ceb-132">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="64ceb-133">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="64ceb-133">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="64ceb-134">Exchange ストア内のアイテムの作成者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="64ceb-134">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="64ceb-135">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="64ceb-135">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="64ceb-136">Exchange ストア内のアイテムの特定の受信者全員への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="64ceb-136">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="64ceb-137">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="64ceb-137">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="64ceb-138">受信者に転送するための Exchange ストアアイテムが保存されています。</span><span class="sxs-lookup"><span data-stu-id="64ceb-138">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="64ceb-139">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="64ceb-139">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="64ceb-140">会議の取り消しに使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="64ceb-140">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="64ceb-141">PostItem</span><span class="sxs-lookup"><span data-stu-id="64ceb-141">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="64ceb-142">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="64ceb-142">Represents a post item in the Exchange store.</span></span> <span data-ttu-id="64ceb-143">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="64ceb-143">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="64ceb-144">テキスト値</span><span class="sxs-lookup"><span data-stu-id="64ceb-144">Text value</span></span>

<span data-ttu-id="64ceb-145">テキスト値は、 **Base64Binary**形式のバイナリ識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="64ceb-145">The text value represents a binary identifier in **Base64Binary** format.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="64ceb-146">注釈</span><span class="sxs-lookup"><span data-stu-id="64ceb-146">Remarks</span></span>

<span data-ttu-id="64ceb-147">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange サーバーの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="64ceb-147">The schema that describes this element is located in the EWS virtual directory of the Exchange server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64ceb-148">要素の情報</span><span class="sxs-lookup"><span data-stu-id="64ceb-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64ceb-149">Namespace</span><span class="sxs-lookup"><span data-stu-id="64ceb-149">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="64ceb-150">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="64ceb-150">Schema Name</span></span>  <br/> |<span data-ttu-id="64ceb-151">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="64ceb-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="64ceb-152">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="64ceb-152">Validation File</span></span>  <br/> |<span data-ttu-id="64ceb-153">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="64ceb-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="64ceb-154">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="64ceb-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="64ceb-155">正しくない</span><span class="sxs-lookup"><span data-stu-id="64ceb-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="64ceb-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="64ceb-156">See also</span></span>



- [<span data-ttu-id="64ceb-157">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="64ceb-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


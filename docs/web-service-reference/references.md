---
title: 参照資料
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- References
api_type:
- schema
ms.assetid: d78f9a48-cd24-452f-af65-4c01933227ce
description: 参照要素は、元のメッセージに応答を関連付けるために使用する Usenet ヘッダーを表します。
ms.openlocfilehash: bf9230107c1ec3d4a8eb025635ec48fdf8d4b341
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833035"
---
# <a name="references"></a><span data-ttu-id="5a6c1-103">参照資料</span><span class="sxs-lookup"><span data-stu-id="5a6c1-103">References</span></span>

<span data-ttu-id="5a6c1-104">**参照**要素は、元のメッセージに応答を関連付けるために使用する Usenet ヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-104">The **References** element represents the Usenet header that is used to associate replies with the original messages.</span></span> 
  
```xml
<References/>
```

 <span data-ttu-id="5a6c1-105">**string**</span><span class="sxs-lookup"><span data-stu-id="5a6c1-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a6c1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5a6c1-106">Attributes and elements</span></span>

<span data-ttu-id="5a6c1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a6c1-108">属性</span><span class="sxs-lookup"><span data-stu-id="5a6c1-108">Attributes</span></span>

<span data-ttu-id="5a6c1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a6c1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5a6c1-110">Child elements</span></span>

<span data-ttu-id="5a6c1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5a6c1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5a6c1-112">Parent elements</span></span>

|<span data-ttu-id="5a6c1-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5a6c1-113">**Element**</span></span>|<span data-ttu-id="5a6c1-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5a6c1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a6c1-115">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="5a6c1-115">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="5a6c1-116">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-116">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5a6c1-117">Message</span><span class="sxs-lookup"><span data-stu-id="5a6c1-117">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5a6c1-118">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-118">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="5a6c1-119">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="5a6c1-119">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="5a6c1-120">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-120">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5a6c1-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="5a6c1-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5a6c1-122">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5a6c1-123">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="5a6c1-123">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="5a6c1-124">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-124">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5a6c1-125">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="5a6c1-125">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="5a6c1-126">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-126">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5a6c1-127">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="5a6c1-127">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="5a6c1-128">会議出席依頼、承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-128">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="5a6c1-129">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="5a6c1-129">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="5a6c1-130">仮の予定を表しますが、会議出席依頼に返信します。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-130">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="5a6c1-131">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="5a6c1-131">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="5a6c1-132">会議出席依頼を辞退の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-132">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="5a6c1-133">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="5a6c1-133">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="5a6c1-134">Exchange ストア内のアイテムの作成者に返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-134">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5a6c1-135">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="5a6c1-135">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="5a6c1-136">Exchange ストア内のアイテムの識別されたすべての受信者への返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-136">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5a6c1-137">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="5a6c1-137">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="5a6c1-138">受信者に転送するのには、Exchange ストアの項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-138">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="5a6c1-139">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="5a6c1-139">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="5a6c1-140">会議をキャンセルするために使用される応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-140">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="5a6c1-141">PostItem</span><span class="sxs-lookup"><span data-stu-id="5a6c1-141">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="5a6c1-142">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-142">Represents a post item in the Exchange store.</span></span> <span data-ttu-id="5a6c1-143">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-143">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5a6c1-144">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5a6c1-144">Text value</span></span>

<span data-ttu-id="5a6c1-145">テキスト値は、Usenet ヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-145">The text value represents a Usenet header.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5a6c1-146">備考</span><span class="sxs-lookup"><span data-stu-id="5a6c1-146">Remarks</span></span>

<span data-ttu-id="5a6c1-147">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5a6c1-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a6c1-148">要素情報</span><span class="sxs-lookup"><span data-stu-id="5a6c1-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a6c1-149">名前空間</span><span class="sxs-lookup"><span data-stu-id="5a6c1-149">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5a6c1-150">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5a6c1-150">Schema Name</span></span>  <br/> |<span data-ttu-id="5a6c1-151">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5a6c1-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="5a6c1-152">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5a6c1-152">Validation File</span></span>  <br/> |<span data-ttu-id="5a6c1-153">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5a6c1-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5a6c1-154">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5a6c1-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="5a6c1-155">False</span><span class="sxs-lookup"><span data-stu-id="5a6c1-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a6c1-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="5a6c1-156">See also</span></span>



- [<span data-ttu-id="5a6c1-157">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5a6c1-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


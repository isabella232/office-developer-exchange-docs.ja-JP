---
title: 件名
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subject
api_type:
- schema
ms.assetid: c140d6c2-deb1-4f67-a908-9397197c4ae7
description: 主題要素は、Exchange ストアのアイテムの subject プロパティを表します。 件名は、255 文字までに制限されています。
ms.openlocfilehash: b93d64c6f517c1cc990d697061c8dad478eb3a3f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833612"
---
# <a name="subject"></a><span data-ttu-id="b964e-104">件名</span><span class="sxs-lookup"><span data-stu-id="b964e-104">Subject</span></span>

<span data-ttu-id="b964e-105">**主題**要素は、Exchange ストアのアイテムの subject プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="b964e-105">The **Subject** element represents the subject property of Exchange store items.</span></span> <span data-ttu-id="b964e-106">件名は、255 文字までに制限されています。</span><span class="sxs-lookup"><span data-stu-id="b964e-106">The subject is limited to 255 characters.</span></span> 
  
```XML
<Subject/>
```

 <span data-ttu-id="b964e-107">**string**</span><span class="sxs-lookup"><span data-stu-id="b964e-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b964e-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b964e-108">Attributes and elements</span></span>

<span data-ttu-id="b964e-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b964e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b964e-110">属性</span><span class="sxs-lookup"><span data-stu-id="b964e-110">Attributes</span></span>

<span data-ttu-id="b964e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b964e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b964e-112">子要素</span><span class="sxs-lookup"><span data-stu-id="b964e-112">Child elements</span></span>

<span data-ttu-id="b964e-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b964e-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b964e-114">親要素</span><span class="sxs-lookup"><span data-stu-id="b964e-114">Parent elements</span></span>

|<span data-ttu-id="b964e-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="b964e-115">**Element**</span></span>|<span data-ttu-id="b964e-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="b964e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b964e-117">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="b964e-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="b964e-118">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="b964e-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="b964e-119">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="b964e-119">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="b964e-120">[キャンセル] の予定表アイテムの応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="b964e-120">Represents a cancel calendar item response object.</span></span>  <br/> |
|[<span data-ttu-id="b964e-121">Contact</span><span class="sxs-lookup"><span data-stu-id="b964e-121">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="b964e-122">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="b964e-122">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="b964e-123">DistributionList</span><span class="sxs-lookup"><span data-stu-id="b964e-123">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="b964e-124">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="b964e-124">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="b964e-125">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b964e-125">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="b964e-126">検索するメッセージの種類の条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="b964e-126">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="b964e-127">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="b964e-127">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="b964e-128">転送されたアイテムの応答のスマート オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="b964e-128">Represents a forward item smart response object.</span></span>  <br/> |
|[<span data-ttu-id="b964e-129">アイテム</span><span class="sxs-lookup"><span data-stu-id="b964e-129">Item</span></span>](item.md) <br/> |<span data-ttu-id="b964e-130">Exchange ストア内の項目を表します。</span><span class="sxs-lookup"><span data-stu-id="b964e-130">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b964e-131">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="b964e-131">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="b964e-132">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="b964e-132">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b964e-133">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="b964e-133">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="b964e-134">Exchange ストア内の会議のメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="b964e-134">Represents a meeting message in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b964e-135">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b964e-135">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b964e-136">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="b964e-136">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b964e-137">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b964e-137">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="b964e-138">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="b964e-138">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b964e-139">Message</span><span class="sxs-lookup"><span data-stu-id="b964e-139">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b964e-140">Exchange ストアに電子メールを表します。</span><span class="sxs-lookup"><span data-stu-id="b964e-140">Represents an e-mail in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b964e-141">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b964e-141">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="b964e-142">[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)で返される 1 つのメッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b964e-142">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="b964e-143">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="b964e-143">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="b964e-144">[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md)要素の 1 つのメッセージの結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b964e-144">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
|[<span data-ttu-id="b964e-145">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="b964e-145">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="b964e-146">削除項目応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="b964e-146">Represents a remove item response object.</span></span>  <br/> |
|[<span data-ttu-id="b964e-147">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="b964e-147">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="b964e-148">全員に返信がスマート応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="b964e-148">Represents a reply-to-all smart response object.</span></span>  <br/> |
|[<span data-ttu-id="b964e-149">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="b964e-149">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="b964e-150">項目への応答にスマート応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="b964e-150">Represents a reply-to-item smart response object.</span></span>  <br/> |
|[<span data-ttu-id="b964e-151">タスク</span><span class="sxs-lookup"><span data-stu-id="b964e-151">Task</span></span>](task.md) <br/> |<span data-ttu-id="b964e-152">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="b964e-152">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b964e-153">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b964e-153">Text value</span></span>

<span data-ttu-id="b964e-154">Exchange アイテムの件名が含まれているテキスト値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="b964e-154">A text value that contains the subject of an Exchange item is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b964e-155">備考</span><span class="sxs-lookup"><span data-stu-id="b964e-155">Remarks</span></span>

<span data-ttu-id="b964e-156">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b964e-156">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b964e-157">要素情報</span><span class="sxs-lookup"><span data-stu-id="b964e-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b964e-158">名前空間</span><span class="sxs-lookup"><span data-stu-id="b964e-158">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b964e-159">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b964e-159">Schema Name</span></span>  <br/> |<span data-ttu-id="b964e-160">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b964e-160">Types schema</span></span>  <br/> |
|<span data-ttu-id="b964e-161">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b964e-161">Validation File</span></span>  <br/> |<span data-ttu-id="b964e-162">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b964e-162">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b964e-163">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b964e-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="b964e-164">False</span><span class="sxs-lookup"><span data-stu-id="b964e-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b964e-165">関連項目</span><span class="sxs-lookup"><span data-stu-id="b964e-165">See also</span></span>



[<span data-ttu-id="b964e-166">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="b964e-166">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="b964e-167">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b964e-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


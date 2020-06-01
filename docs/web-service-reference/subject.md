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
description: Subject 要素は、Exchange ストアアイテムの subject プロパティを表します。 件名は255文字に制限されます。
ms.openlocfilehash: c4d7c21ab70c21ceb63e53d008d25aebf8e22270
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458972"
---
# <a name="subject"></a><span data-ttu-id="7d0d7-104">件名</span><span class="sxs-lookup"><span data-stu-id="7d0d7-104">Subject</span></span>

<span data-ttu-id="7d0d7-105">**Subject**要素は、Exchange ストアアイテムの subject プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-105">The **Subject** element represents the subject property of Exchange store items.</span></span> <span data-ttu-id="7d0d7-106">件名は255文字に制限されます。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-106">The subject is limited to 255 characters.</span></span> 
  
```XML
<Subject/>
```

 <span data-ttu-id="7d0d7-107">**string**</span><span class="sxs-lookup"><span data-stu-id="7d0d7-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7d0d7-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7d0d7-108">Attributes and elements</span></span>

<span data-ttu-id="7d0d7-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d0d7-110">属性</span><span class="sxs-lookup"><span data-stu-id="7d0d7-110">Attributes</span></span>

<span data-ttu-id="7d0d7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d0d7-112">子要素</span><span class="sxs-lookup"><span data-stu-id="7d0d7-112">Child elements</span></span>

<span data-ttu-id="7d0d7-113">なし。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7d0d7-114">親要素</span><span class="sxs-lookup"><span data-stu-id="7d0d7-114">Parent elements</span></span>

|<span data-ttu-id="7d0d7-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="7d0d7-115">**Element**</span></span>|<span data-ttu-id="7d0d7-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="7d0d7-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d0d7-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="7d0d7-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="7d0d7-118">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7d0d7-119">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="7d0d7-119">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="7d0d7-120">予定表アイテムの応答の取り消しオブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-120">Represents a cancel calendar item response object.</span></span>  <br/> |
|[<span data-ttu-id="7d0d7-121">連絡先</span><span class="sxs-lookup"><span data-stu-id="7d0d7-121">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="7d0d7-122">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-122">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="7d0d7-123">DistributionList</span><span class="sxs-lookup"><span data-stu-id="7d0d7-123">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="7d0d7-124">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-124">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="7d0d7-125">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7d0d7-125">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="7d0d7-126">検索するメッセージの種類の条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-126">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="7d0d7-127">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="7d0d7-127">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="7d0d7-128">転送アイテムのスマート応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-128">Represents a forward item smart response object.</span></span>  <br/> |
|[<span data-ttu-id="7d0d7-129">アイテム</span><span class="sxs-lookup"><span data-stu-id="7d0d7-129">Item</span></span>](item.md) <br/> |<span data-ttu-id="7d0d7-130">Exchange ストア内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-130">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7d0d7-131">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="7d0d7-131">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="7d0d7-132">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-132">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7d0d7-133">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="7d0d7-133">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="7d0d7-134">Exchange ストア内の会議メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-134">Represents a meeting message in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7d0d7-135">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="7d0d7-135">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="7d0d7-136">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-136">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7d0d7-137">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="7d0d7-137">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="7d0d7-138">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-138">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7d0d7-139">Message</span><span class="sxs-lookup"><span data-stu-id="7d0d7-139">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7d0d7-140">Exchange ストア内の電子メールを表します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-140">Represents an e-mail in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7d0d7-141">および search-messagetrackingreport</span><span class="sxs-lookup"><span data-stu-id="7d0d7-141">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="7d0d7-142">[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)で返される1つのメッセージを格納します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-142">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="7d0d7-143">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="7d0d7-143">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="7d0d7-144">[Findmessagetrackingreportresponse](findmessagetrackingreportresponse.md)要素の単一メッセージ結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-144">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
|[<span data-ttu-id="7d0d7-145">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="7d0d7-145">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="7d0d7-146">アイテムの削除応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-146">Represents a remove item response object.</span></span>  <br/> |
|[<span data-ttu-id="7d0d7-147">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="7d0d7-147">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="7d0d7-148">応答のすべてのスマート応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-148">Represents a reply-to-all smart response object.</span></span>  <br/> |
|[<span data-ttu-id="7d0d7-149">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="7d0d7-149">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="7d0d7-150">返信先アイテムのスマート応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-150">Represents a reply-to-item smart response object.</span></span>  <br/> |
|[<span data-ttu-id="7d0d7-151">Task</span><span class="sxs-lookup"><span data-stu-id="7d0d7-151">Task</span></span>](task.md) <br/> |<span data-ttu-id="7d0d7-152">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-152">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7d0d7-153">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7d0d7-153">Text value</span></span>

<span data-ttu-id="7d0d7-154">Exchange アイテムの件名を含むテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-154">A text value that contains the subject of an Exchange item is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7d0d7-155">注釈</span><span class="sxs-lookup"><span data-stu-id="7d0d7-155">Remarks</span></span>

<span data-ttu-id="7d0d7-156">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7d0d7-156">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d0d7-157">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7d0d7-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d0d7-158">Namespace</span><span class="sxs-lookup"><span data-stu-id="7d0d7-158">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7d0d7-159">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7d0d7-159">Schema Name</span></span>  <br/> |<span data-ttu-id="7d0d7-160">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7d0d7-160">Types schema</span></span>  <br/> |
|<span data-ttu-id="7d0d7-161">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7d0d7-161">Validation File</span></span>  <br/> |<span data-ttu-id="7d0d7-162">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7d0d7-162">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7d0d7-163">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7d0d7-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="7d0d7-164">正しくない</span><span class="sxs-lookup"><span data-stu-id="7d0d7-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d0d7-165">関連項目</span><span class="sxs-lookup"><span data-stu-id="7d0d7-165">See also</span></span>



[<span data-ttu-id="7d0d7-166">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="7d0d7-166">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="7d0d7-167">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7d0d7-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


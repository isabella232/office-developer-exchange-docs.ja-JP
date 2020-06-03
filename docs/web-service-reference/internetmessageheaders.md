---
title: InternetMessageHeaders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternetMessageHeaders
api_type:
- schema
ms.assetid: 4dcf8671-96df-4a2d-9836-7e8e3a67e0db
description: InternetMessageHeaders 要素には、メールボックス内のアイテムに含まれるいくつかのインターネットメッセージヘッダーのコレクションが含まれています。 インターネットメッセージヘッダーのコレクション全体を取得するには、PR_TRANSPORT_MESSAGE_HEADERS プロパティを使用します。 EWS およびインターネットメッセージヘッダーの詳細については、「EWS、MIME、および不足しているインターネットメッセージヘッダー」の「インターネットメッセージヘッダーの取得」を参照してください。
ms.openlocfilehash: 4719050c02590e021b29173c234466de3fdc58a4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467327"
---
# <a name="internetmessageheaders"></a><span data-ttu-id="f7bb5-105">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="f7bb5-105">InternetMessageHeaders</span></span>

<span data-ttu-id="f7bb5-106">**Internetmessageheaders**要素には、メールボックス内のアイテムに含まれるいくつかのインターネットメッセージヘッダーのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-106">The **InternetMessageHeaders** element contains a collection of some of the Internet message headers that are contained in an item in a mailbox.</span></span> <span data-ttu-id="f7bb5-107">インターネットメッセージヘッダーのコレクション全体を取得するには、 **PR_TRANSPORT_MESSAGE_HEADERS**プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-107">To get the entire collection of Internet message headers, use the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> <span data-ttu-id="f7bb5-108">EWS およびインターネットメッセージヘッダーの詳細については、「 [ews、MIME、および不足しているインターネット](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)メッセージヘッダー」の「インターネットメッセージヘッダーを取得する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-108">For more information about EWS and Internet message headers, see "Getting Internet message headers" in [EWS, MIME, and the missing Internet message headers](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx).</span></span>
  
```XML
<InternetMessageHeaders>
   <InternetMessageHeader/>
</InternetMessageHeaders>
```

 <span data-ttu-id="f7bb5-109">**NonEmptyArrayOfInternetHeadersType**</span><span class="sxs-lookup"><span data-stu-id="f7bb5-109">**NonEmptyArrayOfInternetHeadersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7bb5-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f7bb5-110">Attributes and elements</span></span>

<span data-ttu-id="f7bb5-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7bb5-112">属性</span><span class="sxs-lookup"><span data-stu-id="f7bb5-112">Attributes</span></span>

<span data-ttu-id="f7bb5-113">なし。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7bb5-114">子要素</span><span class="sxs-lookup"><span data-stu-id="f7bb5-114">Child elements</span></span>

|<span data-ttu-id="f7bb5-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="f7bb5-115">**Element**</span></span>|<span data-ttu-id="f7bb5-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="f7bb5-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7bb5-117">InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="f7bb5-117">InternetMessageHeader</span></span>](internetmessageheader.md) <br/> |<span data-ttu-id="f7bb5-118">Headers コレクション内の指定されたヘッダーのインターネットメッセージヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-118">Represents the Internet message header for a given header within the headers collection.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f7bb5-119">親要素</span><span class="sxs-lookup"><span data-stu-id="f7bb5-119">Parent elements</span></span>

|<span data-ttu-id="f7bb5-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="f7bb5-120">**Element**</span></span>|<span data-ttu-id="f7bb5-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="f7bb5-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7bb5-122">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="f7bb5-122">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="f7bb5-123">会議出席依頼への返信を承諾するかを表します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-123">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="f7bb5-124">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="f7bb5-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="f7bb5-125">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="f7bb5-126">Contact</span><span class="sxs-lookup"><span data-stu-id="f7bb5-126">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="f7bb5-127">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-127">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="f7bb5-128">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="f7bb5-128">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="f7bb5-129">会議出席依頼への返信を拒否することを表します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-129">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="f7bb5-130">DistributionList</span><span class="sxs-lookup"><span data-stu-id="f7bb5-130">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="f7bb5-131">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-131">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="f7bb5-132">Item</span><span class="sxs-lookup"><span data-stu-id="f7bb5-132">Item</span></span>](item.md) <br/> |<span data-ttu-id="f7bb5-133">Exchange ストア内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-133">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f7bb5-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="f7bb5-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="f7bb5-135">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-135">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f7bb5-136">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="f7bb5-136">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="f7bb5-137">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-137">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f7bb5-138">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="f7bb5-138">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="f7bb5-139">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-139">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f7bb5-140">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="f7bb5-140">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="f7bb5-141">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-141">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f7bb5-142">Message</span><span class="sxs-lookup"><span data-stu-id="f7bb5-142">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f7bb5-143">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-143">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="f7bb5-144">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="f7bb5-144">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="f7bb5-145">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-145">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f7bb5-146">タスク</span><span class="sxs-lookup"><span data-stu-id="f7bb5-146">Task</span></span>](task.md) <br/> |<span data-ttu-id="f7bb5-147">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-147">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f7bb5-148">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="f7bb5-148">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="f7bb5-149">会議出席依頼に対する仮承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-149">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f7bb5-150">注釈</span><span class="sxs-lookup"><span data-stu-id="f7bb5-150">Remarks</span></span>

<span data-ttu-id="f7bb5-151">**PR_TRANSPORT_MESSAGE_HEADERS**プロパティの EWS マネージ API 拡張プロパティの定義を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-151">The following is the EWS Managed API extended property definition for the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

<span data-ttu-id="f7bb5-152">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f7bb5-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7bb5-153">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f7bb5-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7bb5-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="f7bb5-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f7bb5-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f7bb5-155">Schema Name</span></span>  <br/> |<span data-ttu-id="f7bb5-156">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f7bb5-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="f7bb5-157">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f7bb5-157">Validation File</span></span>  <br/> |<span data-ttu-id="f7bb5-158">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f7bb5-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f7bb5-159">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f7bb5-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="f7bb5-160">正しくない</span><span class="sxs-lookup"><span data-stu-id="f7bb5-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f7bb5-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="f7bb5-161">See also</span></span>



- [<span data-ttu-id="f7bb5-162">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f7bb5-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f7bb5-163">EWS、MIME、および欠落しているインターネット メッセージ ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f7bb5-163">EWS, MIME, and the missing Internet message headers</span></span>](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)


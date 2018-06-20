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
description: InternetMessageHeaders 要素には、いくつかのメールボックス内の項目に含まれているインターネット メッセージ ヘッダーのコレクションが含まれています。 インターネット メッセージ ヘッダーのコレクション全体を取得するには、PR_TRANSPORT_MESSAGE_HEADERS プロパティを使用します。 EWS およびインターネット メッセージ ヘッダー、seeGetting インターネット メッセージ headersin EWS、MIME、および不足しているインターネット メッセージ ヘッダーに関する詳細については。
ms.openlocfilehash: 2da529a8a3532cebb2791b285b7673c962a2a656
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831954"
---
# <a name="internetmessageheaders"></a><span data-ttu-id="d3402-105">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="d3402-105">InternetMessageHeaders</span></span>

<span data-ttu-id="d3402-106">**InternetMessageHeaders**要素には、いくつかのメールボックス内の項目に含まれているインターネット メッセージ ヘッダーのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d3402-106">The **InternetMessageHeaders** element contains a collection of some of the Internet message headers that are contained in an item in a mailbox.</span></span> <span data-ttu-id="d3402-107">インターネット メッセージ ヘッダーのコレクション全体を取得するには、 **PR_TRANSPORT_MESSAGE_HEADERS**プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="d3402-107">To get the entire collection of Internet message headers, use the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> <span data-ttu-id="d3402-108">EWS およびインターネット メッセージ ヘッダーの詳細については、 [EWS、MIME、および不足しているインターネット メッセージ ヘッダー](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx)の「取得のインターネット メッセージのヘッダー」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d3402-108">For more information about EWS and Internet message headers, see "Getting Internet message headers" in [EWS, MIME, and the missing Internet message headers](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx).</span></span>
  
```XML
<InternetMessageHeaders>
   <InternetMessageHeader/>
</InternetMessageHeaders>
```

 <span data-ttu-id="d3402-109">**NonEmptyArrayOfInternetHeadersType**</span><span class="sxs-lookup"><span data-stu-id="d3402-109">**NonEmptyArrayOfInternetHeadersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3402-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d3402-110">Attributes and elements</span></span>

<span data-ttu-id="d3402-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d3402-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3402-112">属性</span><span class="sxs-lookup"><span data-stu-id="d3402-112">Attributes</span></span>

<span data-ttu-id="d3402-113">なし。</span><span class="sxs-lookup"><span data-stu-id="d3402-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3402-114">子要素</span><span class="sxs-lookup"><span data-stu-id="d3402-114">Child elements</span></span>

|<span data-ttu-id="d3402-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="d3402-115">**Element**</span></span>|<span data-ttu-id="d3402-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="d3402-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3402-117">InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="d3402-117">InternetMessageHeader</span></span>](internetmessageheader.md) <br/> |<span data-ttu-id="d3402-118">ヘッダー コレクション内の指定したヘッダーのインターネット メッセージ ヘッダーを表します。</span><span class="sxs-lookup"><span data-stu-id="d3402-118">Represents the Internet message header for a given header within the headers collection.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3402-119">親要素</span><span class="sxs-lookup"><span data-stu-id="d3402-119">Parent elements</span></span>

|<span data-ttu-id="d3402-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="d3402-120">**Element**</span></span>|<span data-ttu-id="d3402-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="d3402-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3402-122">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="d3402-122">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="d3402-123">会議出席依頼、承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="d3402-123">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="d3402-124">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="d3402-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d3402-125">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d3402-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d3402-126">Contact</span><span class="sxs-lookup"><span data-stu-id="d3402-126">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="d3402-127">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d3402-127">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="d3402-128">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="d3402-128">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="d3402-129">会議出席依頼を辞退の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="d3402-129">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="d3402-130">DistributionList</span><span class="sxs-lookup"><span data-stu-id="d3402-130">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="d3402-131">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="d3402-131">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="d3402-132">アイテム</span><span class="sxs-lookup"><span data-stu-id="d3402-132">Item</span></span>](item.md) <br/> |<span data-ttu-id="d3402-133">Exchange ストア内の項目を表します。</span><span class="sxs-lookup"><span data-stu-id="d3402-133">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d3402-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="d3402-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="d3402-135">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="d3402-135">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d3402-136">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="d3402-136">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="d3402-137">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="d3402-137">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d3402-138">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d3402-138">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d3402-139">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="d3402-139">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d3402-140">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="d3402-140">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="d3402-141">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="d3402-141">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d3402-142">Message</span><span class="sxs-lookup"><span data-stu-id="d3402-142">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d3402-143">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="d3402-143">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="d3402-144">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="d3402-144">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="d3402-145">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="d3402-145">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d3402-146">タスク</span><span class="sxs-lookup"><span data-stu-id="d3402-146">Task</span></span>](task.md) <br/> |<span data-ttu-id="d3402-147">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="d3402-147">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d3402-148">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="d3402-148">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="d3402-149">会議出席依頼に仮承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="d3402-149">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d3402-150">備考</span><span class="sxs-lookup"><span data-stu-id="d3402-150">Remarks</span></span>

<span data-ttu-id="d3402-151">**PR_TRANSPORT_MESSAGE_HEADERS**プロパティのプロパティの定義を拡張する EWS マネージ API は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="d3402-151">The following is the EWS Managed API extended property definition for the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

<span data-ttu-id="d3402-152">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d3402-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3402-153">要素情報</span><span class="sxs-lookup"><span data-stu-id="d3402-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3402-154">名前空間</span><span class="sxs-lookup"><span data-stu-id="d3402-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d3402-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d3402-155">Schema Name</span></span>  <br/> |<span data-ttu-id="d3402-156">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d3402-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="d3402-157">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d3402-157">Validation File</span></span>  <br/> |<span data-ttu-id="d3402-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d3402-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d3402-159">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d3402-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="d3402-160">False</span><span class="sxs-lookup"><span data-stu-id="d3402-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3402-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="d3402-161">See also</span></span>



- [<span data-ttu-id="d3402-162">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d3402-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="d3402-163">EWS、MIME、および不足しているインターネット メッセージのヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3402-163">EWS, MIME, and the missing Internet message headers</span></span>](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx)


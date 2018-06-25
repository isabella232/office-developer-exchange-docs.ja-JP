---
title: 添付ファイル
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Attachments
api_type:
- schema
ms.assetid: b470e614-34bb-44f0-8790-7ddbdcbbd29d
description: 添付ファイルの要素には、アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。
ms.openlocfilehash: 8aa5c0849122f5ca83485459fce5d0fea449c974
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759456"
---
# <a name="attachments"></a><span data-ttu-id="b0ee8-103">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="b0ee8-103">Attachments</span></span>

<span data-ttu-id="b0ee8-104">**添付ファイル**の要素には、アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-104">The **Attachments** element contains the items or files that are attached to an item in the Exchange store.</span></span> 
  
```xml
<Attachments>
   <ItemAttachment/>
   <FileAttachment/>
</Attachments>
```

 <span data-ttu-id="b0ee8-105">**ArrayOfAttachmentsType**と**NonEmptyArrayOfAttachmentsType**</span><span class="sxs-lookup"><span data-stu-id="b0ee8-105">**ArrayOfAttachmentsType** and **NonEmptyArrayOfAttachmentsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0ee8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b0ee8-106">Attributes and elements</span></span>

<span data-ttu-id="b0ee8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0ee8-108">属性</span><span class="sxs-lookup"><span data-stu-id="b0ee8-108">Attributes</span></span>

<span data-ttu-id="b0ee8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0ee8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b0ee8-110">Child elements</span></span>

|<span data-ttu-id="b0ee8-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="b0ee8-111">**Element**</span></span>|<span data-ttu-id="b0ee8-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0ee8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0ee8-113">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="b0ee8-113">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="b0ee8-114">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-114">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="b0ee8-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="b0ee8-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="b0ee8-116">Exchange ストア内のアイテムに関連付けられているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0ee8-117">親要素</span><span class="sxs-lookup"><span data-stu-id="b0ee8-117">Parent elements</span></span>

|<span data-ttu-id="b0ee8-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="b0ee8-118">**Element**</span></span>|<span data-ttu-id="b0ee8-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0ee8-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0ee8-120">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="b0ee8-120">CreateAttachment</span></span>](createattachment.md) <br/> |<span data-ttu-id="b0ee8-121">Exchange ストア内のアイテムに添付ファイルを作成する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-121">Defines a request to create an attachment to an item in the Exchange store.</span></span><br/><br/> <span data-ttu-id="b0ee8-122">この要素への XPath 式は、次のようにします。`/CreateAttachment`</span><span class="sxs-lookup"><span data-stu-id="b0ee8-122">The following is the XPath expression to this element:  `/CreateAttachment`</span></span> <br/> |
|[<span data-ttu-id="b0ee8-123">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="b0ee8-123">AcceptItem</span></span>](acceptitem.md) <br/> | <span data-ttu-id="b0ee8-124">会議出席依頼、承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-124">Represents an Accept reply to a meeting request.</span></span><br/><br/><span data-ttu-id="b0ee8-125">以下は、この要素への XPath 式の一部です。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-125">The following are some of the XPath expressions to this element:</span></span><ul><li>`/CreateItem/Items`</li><li>`/MeetingRequest/ConflictingMeetings` </li><li>`/SetItemField/CalendarItem/ConflictingMeetings`</li><li>`/AppendToItemField/CalendarItem/ConflictingMeetings`</li><li>`/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings`</li><li>`/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li><li>`/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li></ul> |
|[<span data-ttu-id="b0ee8-126">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="b0ee8-126">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="b0ee8-127">会議出席依頼を辞退の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-127">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="b0ee8-128">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="b0ee8-128">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="b0ee8-129">仮の予定を表しますが、会議出席依頼に返信します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-129">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="b0ee8-130">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="b0ee8-130">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="b0ee8-131">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-131">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b0ee8-132">アイテム</span><span class="sxs-lookup"><span data-stu-id="b0ee8-132">Item</span></span>](item.md) <br/> |<span data-ttu-id="b0ee8-133">一般的な Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-133">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="b0ee8-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="b0ee8-134">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="b0ee8-135">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-135">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b0ee8-136">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b0ee8-136">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b0ee8-137">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-137">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b0ee8-138">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b0ee8-138">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="b0ee8-139">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-139">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b0ee8-140">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="b0ee8-140">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="b0ee8-141">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-141">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b0ee8-142">Message</span><span class="sxs-lookup"><span data-stu-id="b0ee8-142">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b0ee8-143">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-143">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="b0ee8-144">タスク</span><span class="sxs-lookup"><span data-stu-id="b0ee8-144">Task</span></span>](task.md) <br/> |<span data-ttu-id="b0ee8-145">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-145">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b0ee8-146">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="b0ee8-146">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="b0ee8-147">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-147">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="b0ee8-148">Contact</span><span class="sxs-lookup"><span data-stu-id="b0ee8-148">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="b0ee8-149">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-149">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="b0ee8-150">DistributionList</span><span class="sxs-lookup"><span data-stu-id="b0ee8-150">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="b0ee8-151">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-151">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="b0ee8-152">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b0ee8-152">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md) <br/> |<span data-ttu-id="b0ee8-153">状態および 1 つの CreateAttachment 要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-153">Contains the status and result of a single CreateAttachment request.</span></span>  <br/> |
|[<span data-ttu-id="b0ee8-154">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b0ee8-154">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md) <br/> |<span data-ttu-id="b0ee8-155">GetAttachment 要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-155">Contains the status and result of a GetAttachment request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b0ee8-156">備考</span><span class="sxs-lookup"><span data-stu-id="b0ee8-156">Remarks</span></span>

<span data-ttu-id="b0ee8-157">**添付ファイル**の要素が同じの子要素を持つが、さまざまな種類に基づいています: **ArrayOfAttachmentsType**と**NonEmptyArrayOfAttachmentsType**。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-157">The **Attachments** elements have the same child elements but are based on different types: **ArrayOfAttachmentsType** and **NonEmptyArrayOfAttachmentsType**.</span></span> <span data-ttu-id="b0ee8-158">型では、子要素が必要かどうかを定義します。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-158">The types define whether a child element is required.</span></span> <span data-ttu-id="b0ee8-159">**ArrayOfAttachmentsType**は、応答メッセージにのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-159">The **ArrayOfAttachmentsType** is only used in the response message.</span></span> <span data-ttu-id="b0ee8-160">メッセージと型の両方の名前空間でこれらの要素が発生することに注意する必要もします。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-160">It is also important to note that these elements occur in both the messages and types namespaces.</span></span> 
  
<span data-ttu-id="b0ee8-161">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="b0ee8-161">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0ee8-162">要素情報</span><span class="sxs-lookup"><span data-stu-id="b0ee8-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0ee8-163">名前空間</span><span class="sxs-lookup"><span data-stu-id="b0ee8-163">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b0ee8-164">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b0ee8-164">Schema Name</span></span>  <br/> |<span data-ttu-id="b0ee8-165">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b0ee8-165">Types schema</span></span>  <br/> |
|<span data-ttu-id="b0ee8-166">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b0ee8-166">Validation File</span></span>  <br/> |<span data-ttu-id="b0ee8-167">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b0ee8-167">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b0ee8-168">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b0ee8-168">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0ee8-169">False</span><span class="sxs-lookup"><span data-stu-id="b0ee8-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0ee8-170">関連項目</span><span class="sxs-lookup"><span data-stu-id="b0ee8-170">See also</span></span>

- [<span data-ttu-id="b0ee8-171">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b0ee8-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


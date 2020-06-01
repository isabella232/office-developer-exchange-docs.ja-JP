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
description: Attachments 要素には、Exchange ストア内のアイテムに添付されているアイテムまたはファイルが含まれます。
ms.openlocfilehash: a9f79cd79f19e6226703c99c53c91efed600f495
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461535"
---
# <a name="attachments"></a><span data-ttu-id="2c93a-103">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="2c93a-103">Attachments</span></span>

<span data-ttu-id="2c93a-104">**Attachments**要素には、Exchange ストア内のアイテムに添付されているアイテムまたはファイルが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2c93a-104">The **Attachments** element contains the items or files that are attached to an item in the Exchange store.</span></span> 
  
```xml
<Attachments>
   <ItemAttachment/>
   <FileAttachment/>
</Attachments>
```

 <span data-ttu-id="2c93a-105">**Arrayofattachmentstype**および**Nonemptyarrayofattachmentstype**</span><span class="sxs-lookup"><span data-stu-id="2c93a-105">**ArrayOfAttachmentsType** and **NonEmptyArrayOfAttachmentsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c93a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2c93a-106">Attributes and elements</span></span>

<span data-ttu-id="2c93a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c93a-108">属性</span><span class="sxs-lookup"><span data-stu-id="2c93a-108">Attributes</span></span>

<span data-ttu-id="2c93a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2c93a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2c93a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2c93a-110">Child elements</span></span>

|<span data-ttu-id="2c93a-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="2c93a-111">**Element**</span></span>|<span data-ttu-id="2c93a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2c93a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c93a-113">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="2c93a-113">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="2c93a-114">別の Exchange アイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-114">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="2c93a-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="2c93a-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="2c93a-116">Exchange ストア内のアイテムに添付されているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2c93a-117">親要素</span><span class="sxs-lookup"><span data-stu-id="2c93a-117">Parent elements</span></span>

|<span data-ttu-id="2c93a-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="2c93a-118">**Element**</span></span>|<span data-ttu-id="2c93a-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="2c93a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c93a-120">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="2c93a-120">CreateAttachment</span></span>](createattachment.md) <br/> |<span data-ttu-id="2c93a-121">Exchange ストア内のアイテムの添付ファイルを作成するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-121">Defines a request to create an attachment to an item in the Exchange store.</span></span><br/><br/> <span data-ttu-id="2c93a-122">この要素の XPath 式を次に示します。`/CreateAttachment`</span><span class="sxs-lookup"><span data-stu-id="2c93a-122">The following is the XPath expression to this element:  `/CreateAttachment`</span></span> <br/> |
|[<span data-ttu-id="2c93a-123">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="2c93a-123">AcceptItem</span></span>](acceptitem.md) <br/> | <span data-ttu-id="2c93a-124">会議出席依頼への返信を承諾するかを表します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-124">Represents an Accept reply to a meeting request.</span></span><br/><br/><span data-ttu-id="2c93a-125">この要素の XPath 式の一部を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-125">The following are some of the XPath expressions to this element:</span></span><ul><li>`/CreateItem/Items`</li><li>`/MeetingRequest/ConflictingMeetings` </li><li>`/SetItemField/CalendarItem/ConflictingMeetings`</li><li>`/AppendToItemField/CalendarItem/ConflictingMeetings`</li><li>`/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings`</li><li>`/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li><li>`/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li></ul> |
|[<span data-ttu-id="2c93a-126">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="2c93a-126">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="2c93a-127">会議出席依頼への返信を拒否することを表します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-127">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="2c93a-128">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="2c93a-128">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="2c93a-129">会議出席依頼に対する仮の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-129">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="2c93a-130">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="2c93a-130">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="2c93a-131">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-131">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2c93a-132">アイテム</span><span class="sxs-lookup"><span data-stu-id="2c93a-132">Item</span></span>](item.md) <br/> |<span data-ttu-id="2c93a-133">汎用の Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-133">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="2c93a-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="2c93a-134">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="2c93a-135">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-135">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2c93a-136">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="2c93a-136">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2c93a-137">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-137">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2c93a-138">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="2c93a-138">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="2c93a-139">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-139">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2c93a-140">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="2c93a-140">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="2c93a-141">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-141">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2c93a-142">Message</span><span class="sxs-lookup"><span data-stu-id="2c93a-142">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2c93a-143">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-143">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="2c93a-144">Task</span><span class="sxs-lookup"><span data-stu-id="2c93a-144">Task</span></span>](task.md) <br/> |<span data-ttu-id="2c93a-145">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-145">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2c93a-146">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="2c93a-146">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2c93a-147">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-147">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2c93a-148">連絡先</span><span class="sxs-lookup"><span data-stu-id="2c93a-148">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="2c93a-149">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-149">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="2c93a-150">DistributionList</span><span class="sxs-lookup"><span data-stu-id="2c93a-150">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="2c93a-151">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-151">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="2c93a-152">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2c93a-152">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md) <br/> |<span data-ttu-id="2c93a-153">1つの CreateAttachment 要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-153">Contains the status and result of a single CreateAttachment request.</span></span>  <br/> |
|[<span data-ttu-id="2c93a-154">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2c93a-154">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md) <br/> |<span data-ttu-id="2c93a-155">GetAttachment 要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-155">Contains the status and result of a GetAttachment request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2c93a-156">注釈</span><span class="sxs-lookup"><span data-stu-id="2c93a-156">Remarks</span></span>

<span data-ttu-id="2c93a-157">**Attachments**要素には同じ子要素がありますが、さまざまな種類に基づいています。 **Arrayofattachmentstype**および**Nonemptyarrayofattachmentstype**。</span><span class="sxs-lookup"><span data-stu-id="2c93a-157">The **Attachments** elements have the same child elements but are based on different types: **ArrayOfAttachmentsType** and **NonEmptyArrayOfAttachmentsType**.</span></span> <span data-ttu-id="2c93a-158">この型は、子要素が必要かどうかを定義します。</span><span class="sxs-lookup"><span data-stu-id="2c93a-158">The types define whether a child element is required.</span></span> <span data-ttu-id="2c93a-159">**Arrayofattachmentstype**は、応答メッセージでのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="2c93a-159">The **ArrayOfAttachmentsType** is only used in the response message.</span></span> <span data-ttu-id="2c93a-160">また、これらの要素は、メッセージと型の両方の名前空間で発生することに注意してください。</span><span class="sxs-lookup"><span data-stu-id="2c93a-160">It is also important to note that these elements occur in both the messages and types namespaces.</span></span> 
  
<span data-ttu-id="2c93a-161">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2c93a-161">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2c93a-162">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2c93a-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c93a-163">Namespace</span><span class="sxs-lookup"><span data-stu-id="2c93a-163">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2c93a-164">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2c93a-164">Schema Name</span></span>  <br/> |<span data-ttu-id="2c93a-165">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="2c93a-165">Types schema</span></span>  <br/> |
|<span data-ttu-id="2c93a-166">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2c93a-166">Validation File</span></span>  <br/> |<span data-ttu-id="2c93a-167">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="2c93a-167">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2c93a-168">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2c93a-168">Can be Empty</span></span>  <br/> |<span data-ttu-id="2c93a-169">正しくない</span><span class="sxs-lookup"><span data-stu-id="2c93a-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2c93a-170">関連項目</span><span class="sxs-lookup"><span data-stu-id="2c93a-170">See also</span></span>

- [<span data-ttu-id="2c93a-171">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2c93a-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: HasAttachments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HasAttachments
api_type:
- schema
ms.assetid: 538b7a85-11d7-4daa-8458-09b540760e8b
description: HasAttachments 要素は、アイテムに少なくとも1つの添付ファイルがある場合、または添付ファイルを持つアイテムが1つ以上含まれている場合に、true に設定されるプロパティを表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。
ms.openlocfilehash: cc4e4ec0eac1c749723facc8cd780da41b0d8150
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462923"
---
# <a name="hasattachments"></a><span data-ttu-id="70c40-104">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="70c40-104">HasAttachments</span></span>

<span data-ttu-id="70c40-105">**Hasattachments**要素は、アイテムに少なくとも1つの添付ファイルがある場合、または添付ファイルを持つアイテムが1つ以上含まれている場合に、 **true**に設定されるプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="70c40-105">The **HasAttachments** element represents a property that is set to **true** if an item has at least one visible attachment or if a conversation contains at least one item that has an attachment.</span></span> <span data-ttu-id="70c40-106">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="70c40-106">This property is read-only.</span></span> 
  
```XML
<HasAttachments/>
```

 <span data-ttu-id="70c40-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="70c40-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70c40-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="70c40-108">Attributes and elements</span></span>

<span data-ttu-id="70c40-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="70c40-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70c40-110">属性</span><span class="sxs-lookup"><span data-stu-id="70c40-110">Attributes</span></span>

<span data-ttu-id="70c40-111">なし。</span><span class="sxs-lookup"><span data-stu-id="70c40-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70c40-112">子要素</span><span class="sxs-lookup"><span data-stu-id="70c40-112">Child elements</span></span>

<span data-ttu-id="70c40-113">なし。</span><span class="sxs-lookup"><span data-stu-id="70c40-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="70c40-114">親要素</span><span class="sxs-lookup"><span data-stu-id="70c40-114">Parent elements</span></span>

|<span data-ttu-id="70c40-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="70c40-115">**Element**</span></span>|<span data-ttu-id="70c40-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="70c40-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70c40-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="70c40-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="70c40-118">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="70c40-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="70c40-119">条件</span><span class="sxs-lookup"><span data-stu-id="70c40-119">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="70c40-120">そのルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="70c40-120">Represents the conditions that, when fulfilled, will trigger the rule actions for that rule.</span></span>  <br/> |
|[<span data-ttu-id="70c40-121">Contact</span><span class="sxs-lookup"><span data-stu-id="70c40-121">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="70c40-122">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="70c40-122">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="70c40-123">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="70c40-123">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="70c40-124">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="70c40-124">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="70c40-125">DistributionList</span><span class="sxs-lookup"><span data-stu-id="70c40-125">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="70c40-126">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="70c40-126">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="70c40-127">例外</span><span class="sxs-lookup"><span data-stu-id="70c40-127">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="70c40-128">受信トレイルールの利用可能なすべてのルールの例外条件を表します。</span><span class="sxs-lookup"><span data-stu-id="70c40-128">Represents all the available rule exception conditions for the Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="70c40-129">Item</span><span class="sxs-lookup"><span data-stu-id="70c40-129">Item</span></span>](item.md) <br/> |<span data-ttu-id="70c40-130">Exchange ストア内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="70c40-130">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="70c40-131">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="70c40-131">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="70c40-132">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="70c40-132">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="70c40-133">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="70c40-133">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="70c40-134">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="70c40-134">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="70c40-135">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="70c40-135">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="70c40-136">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="70c40-136">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="70c40-137">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="70c40-137">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="70c40-138">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="70c40-138">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="70c40-139">Message</span><span class="sxs-lookup"><span data-stu-id="70c40-139">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="70c40-140">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="70c40-140">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="70c40-141">タスク</span><span class="sxs-lookup"><span data-stu-id="70c40-141">Task</span></span>](task.md) <br/> |<span data-ttu-id="70c40-142">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="70c40-142">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="70c40-143">テキスト値</span><span class="sxs-lookup"><span data-stu-id="70c40-143">Text value</span></span>

<span data-ttu-id="70c40-144">ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="70c40-144">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="70c40-145">値が**true**の場合は、アイテムまたはスレッドに表示されている添付ファイルが1つ以上あることを意味します。</span><span class="sxs-lookup"><span data-stu-id="70c40-145">A value of **true** means that the item or conversation has at least one visible attachment.</span></span> <span data-ttu-id="70c40-146">値が**false**の場合は、アイテムまたは会話に添付ファイルがないか、または添付ファイルのみが含まれていることを意味します。</span><span class="sxs-lookup"><span data-stu-id="70c40-146">A value of **false** means that the item or conversation either has no attachments or has only hidden attachments.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="70c40-147">注釈</span><span class="sxs-lookup"><span data-stu-id="70c40-147">Remarks</span></span>

<span data-ttu-id="70c40-148">**Hasattachments**プロパティは、ブール値の**AllAttachmentsHidden** MAPI プロパティから計算されます。</span><span class="sxs-lookup"><span data-stu-id="70c40-148">The **HasAttachments** property is calculated from the Boolean **AllAttachmentsHidden** MAPI property.</span></span> <span data-ttu-id="70c40-149">アイテムに添付ファイルがない場合、 **AllAttachmentsHidden**プロパティは存在しません。</span><span class="sxs-lookup"><span data-stu-id="70c40-149">If an item does not have an attachment, the **AllAttachmentsHidden** property does not exist.</span></span> <span data-ttu-id="70c40-150">アイテムのすべての添付ファイルが非表示になっている場合、 **AllAttachmentsHidden**プロパティは**true**になります。</span><span class="sxs-lookup"><span data-stu-id="70c40-150">If all the attachments on the item are hidden, the **AllAttachmentsHidden** property is **true**.</span></span> <span data-ttu-id="70c40-151">少なくとも1つの添付ファイルがあり、少なくとも1つの添付ファイルが表示されている場合、 **AllAttachmentsHidden**プロパティは**false**になります。</span><span class="sxs-lookup"><span data-stu-id="70c40-151">The **AllAttachmentsHidden** property is **false** if it has at least one attachment and at least one of the attachments is visible.</span></span> <span data-ttu-id="70c40-152">**AllAttachmentsHidden** MAPI プロパティを使用して、アイテムの検索、グループ化、および並べ替えを行います。</span><span class="sxs-lookup"><span data-stu-id="70c40-152">Use the **AllAttachmentsHidden** MAPI property for searching, grouping, and sorting items.</span></span> 
  
<span data-ttu-id="70c40-153">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="70c40-153">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70c40-154">要素の情報</span><span class="sxs-lookup"><span data-stu-id="70c40-154">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70c40-155">Namespace</span><span class="sxs-lookup"><span data-stu-id="70c40-155">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="70c40-156">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="70c40-156">Schema Name</span></span>  <br/> |<span data-ttu-id="70c40-157">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="70c40-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="70c40-158">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="70c40-158">Validation File</span></span>  <br/> |<span data-ttu-id="70c40-159">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="70c40-159">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="70c40-160">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="70c40-160">Can be Empty</span></span>  <br/> |<span data-ttu-id="70c40-161">正しくない</span><span class="sxs-lookup"><span data-stu-id="70c40-161">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="70c40-162">関連項目</span><span class="sxs-lookup"><span data-stu-id="70c40-162">See also</span></span>



- [<span data-ttu-id="70c40-163">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="70c40-163">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="70c40-164">Exchange 用 EWS リファレンス</span><span class="sxs-lookup"><span data-stu-id="70c40-164">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)


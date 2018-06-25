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
description: 添付ファイル付きの要素は、項目が、表示されている 1 つ以上の添付ファイルまたは添付ファイルのある場合は、テーマには、少なくとも 1 つの項目が含まれている場合、true に設定されているプロパティを表します。 このプロパティは値の取得のみ可能です。
ms.openlocfilehash: e76e0ecbb357396540f0d1649cf5062edfb18660
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831801"
---
# <a name="hasattachments"></a><span data-ttu-id="8ea1b-104">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="8ea1b-104">HasAttachments</span></span>

<span data-ttu-id="8ea1b-105">**添付ファイル付き**の要素は、項目が、表示されている 1 つ以上の添付ファイルまたは添付ファイルのある会話には、少なくとも 1 つの項目が含まれている場合に**true**に設定されているプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-105">The **HasAttachments** element represents a property that is set to **true** if an item has at least one visible attachment or if a conversation contains at least one item that has an attachment.</span></span> <span data-ttu-id="8ea1b-106">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-106">This property is read-only.</span></span> 
  
```XML
<HasAttachments/>
```

 <span data-ttu-id="8ea1b-107">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="8ea1b-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8ea1b-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8ea1b-108">Attributes and elements</span></span>

<span data-ttu-id="8ea1b-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ea1b-110">属性</span><span class="sxs-lookup"><span data-stu-id="8ea1b-110">Attributes</span></span>

<span data-ttu-id="8ea1b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ea1b-112">子要素</span><span class="sxs-lookup"><span data-stu-id="8ea1b-112">Child elements</span></span>

<span data-ttu-id="8ea1b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8ea1b-114">親要素</span><span class="sxs-lookup"><span data-stu-id="8ea1b-114">Parent elements</span></span>

|<span data-ttu-id="8ea1b-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="8ea1b-115">**Element**</span></span>|<span data-ttu-id="8ea1b-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="8ea1b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ea1b-117">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="8ea1b-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="8ea1b-118">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8ea1b-119">条件</span><span class="sxs-lookup"><span data-stu-id="8ea1b-119">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="8ea1b-120">条件を表しますが、満たされるとときに、そのルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-120">Represents the conditions that, when fulfilled, will trigger the rule actions for that rule.</span></span>  <br/> |
|[<span data-ttu-id="8ea1b-121">Contact</span><span class="sxs-lookup"><span data-stu-id="8ea1b-121">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="8ea1b-122">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-122">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="8ea1b-123">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="8ea1b-123">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="8ea1b-124">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-124">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="8ea1b-125">DistributionList</span><span class="sxs-lookup"><span data-stu-id="8ea1b-125">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="8ea1b-126">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-126">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="8ea1b-127">Exceptions</span><span class="sxs-lookup"><span data-stu-id="8ea1b-127">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="8ea1b-128">受信トレイ ルールの使用可能なルールの例外条件をすべてを表します。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-128">Represents all the available rule exception conditions for the Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="8ea1b-129">アイテム</span><span class="sxs-lookup"><span data-stu-id="8ea1b-129">Item</span></span>](item.md) <br/> |<span data-ttu-id="8ea1b-130">Exchange ストア内の項目を表します。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-130">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8ea1b-131">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="8ea1b-131">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="8ea1b-132">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-132">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8ea1b-133">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="8ea1b-133">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="8ea1b-134">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-134">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8ea1b-135">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="8ea1b-135">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="8ea1b-136">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-136">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8ea1b-137">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="8ea1b-137">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="8ea1b-138">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-138">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8ea1b-139">Message</span><span class="sxs-lookup"><span data-stu-id="8ea1b-139">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8ea1b-140">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-140">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="8ea1b-141">タスク</span><span class="sxs-lookup"><span data-stu-id="8ea1b-141">Task</span></span>](task.md) <br/> |<span data-ttu-id="8ea1b-142">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-142">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8ea1b-143">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8ea1b-143">Text value</span></span>

<span data-ttu-id="8ea1b-144">ブール値を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-144">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="8ea1b-145">**True**の場合は、会話または複数のアイテムが表示されている 1 つ以上の添付ファイルを持っているを意味します。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-145">A value of **true** means that the item or conversation has at least one visible attachment.</span></span> <span data-ttu-id="8ea1b-146">**False**の値は、アイテムまたは会話ことか、添付ファイルがないか、添付ファイルを非表示にのみを意味します。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-146">A value of **false** means that the item or conversation either has no attachments or has only hidden attachments.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8ea1b-147">備考</span><span class="sxs-lookup"><span data-stu-id="8ea1b-147">Remarks</span></span>

<span data-ttu-id="8ea1b-148">**添付ファイル付き**のプロパティは、ブール値の**AllAttachmentsHidden**の MAPI プロパティから計算されます。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-148">The **HasAttachments** property is calculated from the Boolean **AllAttachmentsHidden** MAPI property.</span></span> <span data-ttu-id="8ea1b-149">アイテムが添付ファイルを持たない場合、 **AllAttachmentsHidden**プロパティは存在しません。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-149">If an item does not have an attachment, the **AllAttachmentsHidden** property does not exist.</span></span> <span data-ttu-id="8ea1b-150">アイテムのすべての添付ファイルが表示されない場合は、 **AllAttachmentsHidden**プロパティが**true**です。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-150">If all the attachments on the item are hidden, the **AllAttachmentsHidden** property is **true**.</span></span> <span data-ttu-id="8ea1b-151">1 つ以上の添付ファイルがあり、1 つ以上の添付ファイルが表示されている場合、 **AllAttachmentsHidden**プロパティは**false**です。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-151">The **AllAttachmentsHidden** property is **false** if it has at least one attachment and at least one of the attachments is visible.</span></span> <span data-ttu-id="8ea1b-152">**AllAttachmentsHidden** MAPI プロパティを使用して、検索、グループ化、およびアイテムの並べ替えをします。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-152">Use the **AllAttachmentsHidden** MAPI property for searching, grouping, and sorting items.</span></span> 
  
<span data-ttu-id="8ea1b-153">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8ea1b-153">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8ea1b-154">要素情報</span><span class="sxs-lookup"><span data-stu-id="8ea1b-154">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ea1b-155">名前空間</span><span class="sxs-lookup"><span data-stu-id="8ea1b-155">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8ea1b-156">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8ea1b-156">Schema Name</span></span>  <br/> |<span data-ttu-id="8ea1b-157">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8ea1b-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="8ea1b-158">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8ea1b-158">Validation File</span></span>  <br/> |<span data-ttu-id="8ea1b-159">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8ea1b-159">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8ea1b-160">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8ea1b-160">Can be Empty</span></span>  <br/> |<span data-ttu-id="8ea1b-161">False</span><span class="sxs-lookup"><span data-stu-id="8ea1b-161">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8ea1b-162">関連項目</span><span class="sxs-lookup"><span data-stu-id="8ea1b-162">See also</span></span>



- [<span data-ttu-id="8ea1b-163">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8ea1b-163">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
<span data-ttu-id="8ea1b-164">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="8ea1b-164">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>


---
title: DeleteItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 055cdee8-3c7d-47db-9f27-740f4a674729
description: DeleteItem 要素は、Exchange ストア内のメールボックスからアイテムを削除する要求を定義します。
ms.openlocfilehash: de64787750c88c8a47bb69daddc0a1d2ebe8bde9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759990"
---
# <a name="deleteitem"></a><span data-ttu-id="bad8d-103">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="bad8d-103">DeleteItem</span></span>

<span data-ttu-id="bad8d-104">**DeleteItem**要素は、Exchange ストア内のメールボックスからアイテムを削除する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="bad8d-104">The **DeleteItem** element defines a request to delete an item from a mailbox in the Exchange store.</span></span> 
  
```XML
<DeleteItem DeleteType="" SendMeetingCancellations="" AffectedTaskOccurrences="" SuppressReadReceipts="">
   <ItemIds/>
</DeleteItem>
```

 <span data-ttu-id="bad8d-105">**DeleteItemType**</span><span class="sxs-lookup"><span data-stu-id="bad8d-105">**DeleteItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bad8d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bad8d-106">Attributes and elements</span></span>

<span data-ttu-id="bad8d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bad8d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bad8d-108">属性</span><span class="sxs-lookup"><span data-stu-id="bad8d-108">Attributes</span></span>

|<span data-ttu-id="bad8d-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="bad8d-109">**Attribute**</span></span>|<span data-ttu-id="bad8d-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="bad8d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bad8d-111">**削除の種類**</span><span class="sxs-lookup"><span data-stu-id="bad8d-111">**DeleteType**</span></span> <br/> |<span data-ttu-id="bad8d-112">アイテムを削除する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="bad8d-112">Describes how an item is deleted.</span></span> <span data-ttu-id="bad8d-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="bad8d-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="bad8d-114">**SendMeetingCancellations**</span><span class="sxs-lookup"><span data-stu-id="bad8d-114">**SendMeetingCancellations**</span></span> <br/> |<span data-ttu-id="bad8d-115">予定表アイテムの削除を参加者に伝達するかどうかについて説明します。</span><span class="sxs-lookup"><span data-stu-id="bad8d-115">Describes whether a calendar item deletion is communicated to attendees.</span></span> <span data-ttu-id="bad8d-116">予定表アイテムが削除されたとき、この属性が必要です。</span><span class="sxs-lookup"><span data-stu-id="bad8d-116">This attribute is required when calendar items are deleted.</span></span> <span data-ttu-id="bad8d-117">この属性は、非予定表アイテムが削除された場合は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="bad8d-117">This attribute is optional if non-calendar items are deleted.</span></span>  <br/> |
|<span data-ttu-id="bad8d-118">**AffectedTaskOccurrences**</span><span class="sxs-lookup"><span data-stu-id="bad8d-118">**AffectedTaskOccurrences**</span></span> <br/> |<span data-ttu-id="bad8d-119">[DeleteItem 操作](deleteitem-operation.md)によって、タスクのインスタンスまたはタスク マスターを削除するかどうかについて説明します。</span><span class="sxs-lookup"><span data-stu-id="bad8d-119">Describes whether a task instance or a task master is deleted by a [DeleteItem operation](deleteitem-operation.md).</span></span> <span data-ttu-id="bad8d-120">タスクが削除されるとき、この属性が必要です。</span><span class="sxs-lookup"><span data-stu-id="bad8d-120">This attribute is required when tasks are deleted.</span></span> <span data-ttu-id="bad8d-121">以外の項目が削除されたとき、この属性はオプションです。</span><span class="sxs-lookup"><span data-stu-id="bad8d-121">This attribute is optional when non-task items are deleted.</span></span>  <br/> |
|<span data-ttu-id="bad8d-122">**SuppressReadReceipts**</span><span class="sxs-lookup"><span data-stu-id="bad8d-122">**SuppressReadReceipts**</span></span> <br/> |<span data-ttu-id="bad8d-123">削除済みアイテムの開封確認メッセージを抑制するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bad8d-123">Indicates whether read receipts for the deleted item are suppressed.</span></span> <span data-ttu-id="bad8d-124">テキストの値**は true**では、開封確認のメッセージが抑制されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="bad8d-124">A text value of **true**, indicates that the read receipts are suppressed.</span></span> <span data-ttu-id="bad8d-125">**False**の値は、送信者に開封確認を送信することを示します。</span><span class="sxs-lookup"><span data-stu-id="bad8d-125">A value of **false** indicates that the read receipts are sent to the sender.</span></span> <span data-ttu-id="bad8d-126">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="bad8d-126">This attribute is optional.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="bad8d-127">削除の種類の属性</span><span class="sxs-lookup"><span data-stu-id="bad8d-127">DeleteType attribute</span></span>

|<span data-ttu-id="bad8d-128">**値**</span><span class="sxs-lookup"><span data-stu-id="bad8d-128">**Value**</span></span>|<span data-ttu-id="bad8d-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="bad8d-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bad8d-130">HardDelete</span><span class="sxs-lookup"><span data-stu-id="bad8d-130">HardDelete</span></span>  <br/> |<span data-ttu-id="bad8d-131">アイテムはストアから完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="bad8d-131">An item is permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="bad8d-132">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="bad8d-132">SoftDelete</span></span>  <br/> |<span data-ttu-id="bad8d-133">アイテムを移動、ごみ箱をあさる場合、収集を有効にします。</span><span class="sxs-lookup"><span data-stu-id="bad8d-133">An item is moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="bad8d-134">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="bad8d-134">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="bad8d-135">アイテムは、削除済みアイテム フォルダーに移動されます。</span><span class="sxs-lookup"><span data-stu-id="bad8d-135">An item is moved to the Deleted Items folder.</span></span>  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a><span data-ttu-id="bad8d-136">SendMeetingCancellations 属性</span><span class="sxs-lookup"><span data-stu-id="bad8d-136">SendMeetingCancellations attribute</span></span>

|<span data-ttu-id="bad8d-137">**値**</span><span class="sxs-lookup"><span data-stu-id="bad8d-137">**Value**</span></span>|<span data-ttu-id="bad8d-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="bad8d-138">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bad8d-139">SendToNone</span><span class="sxs-lookup"><span data-stu-id="bad8d-139">SendToNone</span></span>  <br/> |<span data-ttu-id="bad8d-140">取り消しメッセージを送信することがなく、予定表アイテムが削除されます。</span><span class="sxs-lookup"><span data-stu-id="bad8d-140">A calendar item is deleted without sending a cancellation message.</span></span>  <br/> |
|<span data-ttu-id="bad8d-141">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="bad8d-141">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="bad8d-142">予定表アイテムが削除され、すべての出席者にキャンセル通知が送信されます。</span><span class="sxs-lookup"><span data-stu-id="bad8d-142">A calendar item is deleted and a cancellation message is sent to all attendees.</span></span>  <br/> |
|<span data-ttu-id="bad8d-143">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="bad8d-143">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="bad8d-144">予定表アイテムが削除され、すべての出席者にキャンセル通知が送信されます。</span><span class="sxs-lookup"><span data-stu-id="bad8d-144">A calendar item is deleted and a cancellation message is sent to all attendees.</span></span> <span data-ttu-id="bad8d-145">取り消しについてのメッセージのコピーは、送信済みアイテム フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="bad8d-145">A copy of the cancellation message is saved in the Sent Items folder.</span></span>  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a><span data-ttu-id="bad8d-146">AffectedTaskOccurrences 属性</span><span class="sxs-lookup"><span data-stu-id="bad8d-146">AffectedTaskOccurrences attribute</span></span>

|<span data-ttu-id="bad8d-147">**値**</span><span class="sxs-lookup"><span data-stu-id="bad8d-147">**Value**</span></span>|<span data-ttu-id="bad8d-148">**説明**</span><span class="sxs-lookup"><span data-stu-id="bad8d-148">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bad8d-149">AllOccurrences</span><span class="sxs-lookup"><span data-stu-id="bad8d-149">AllOccurrences</span></span>  <br/> |<span data-ttu-id="bad8d-150">削除項目の要求は、マスターのタスクを削除し、したがってすべての定期的なタスクに関連付けられているマスターのタスクします。</span><span class="sxs-lookup"><span data-stu-id="bad8d-150">A delete item request deletes the master task, and therefore all recurring tasks that are associated with the master task.</span></span>  <br/> |
|<span data-ttu-id="bad8d-151">SpecifiedOccurrenceOnly</span><span class="sxs-lookup"><span data-stu-id="bad8d-151">SpecifiedOccurrenceOnly</span></span>  <br/> |<span data-ttu-id="bad8d-152">削除項目の要求では、タスクの特定の個所だけを削除します。</span><span class="sxs-lookup"><span data-stu-id="bad8d-152">A delete item request deletes only specific occurrences of a task.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bad8d-153">子要素</span><span class="sxs-lookup"><span data-stu-id="bad8d-153">Child elements</span></span>

|<span data-ttu-id="bad8d-154">**要素**</span><span class="sxs-lookup"><span data-stu-id="bad8d-154">**Element**</span></span>|<span data-ttu-id="bad8d-155">**説明**</span><span class="sxs-lookup"><span data-stu-id="bad8d-155">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bad8d-156">Itemid</span><span class="sxs-lookup"><span data-stu-id="bad8d-156">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="bad8d-157">アイテム、出現アイテム、および Exchange ストアのメールボックスから削除するのにはマスターの定期的なアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bad8d-157">Contains an array of items, occurrence items, and recurring master items to delete from a mailbox in the Exchange store.</span></span> <span data-ttu-id="bad8d-158">[DeleteItem の操作](deleteitem-operation.md)は、任意の項目の種類を実行できます。</span><span class="sxs-lookup"><span data-stu-id="bad8d-158">The [DeleteItem operation](deleteitem-operation.md) can be performed on any item type.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bad8d-159">親要素</span><span class="sxs-lookup"><span data-stu-id="bad8d-159">Parent elements</span></span>

<span data-ttu-id="bad8d-160">なし。</span><span class="sxs-lookup"><span data-stu-id="bad8d-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bad8d-161">備考</span><span class="sxs-lookup"><span data-stu-id="bad8d-161">Remarks</span></span>

<span data-ttu-id="bad8d-162">**MoveToDeletedItems**および**HardDelete**オプションは、時間によって、Web サービスの呼び出しが完了していることを意味する、トランザクション、データベースは削除済みアイテム フォルダーにアイテムを移動または Exchange データベースから項目を完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="bad8d-162">The **MoveToDeletedItems** and **HardDelete** options are transactional, which means that by the time a Web service call completes, the database has moved the item to the Deleted Items folder or permanently removed the item from the Exchange database.</span></span> <span data-ttu-id="bad8d-163">この現象は、MicrosoftExchange Server 2007 および Exchange Server 2010 と同じです。</span><span class="sxs-lookup"><span data-stu-id="bad8d-163">This behavior is the same for MicrosoftExchange Server 2007 and Exchange Server 2010.</span></span> 
  
<span data-ttu-id="bad8d-164">**SoftDelete**オプションの動作は別のターゲットのバージョンの Exchange で異なります。</span><span class="sxs-lookup"><span data-stu-id="bad8d-164">The **SoftDelete** option works differently for different target versions of Exchange.</span></span> <span data-ttu-id="bad8d-165">Exchange 2007 用の**SoftDelete**のビット設定項目を示す項目を移動する Exchange データベースに、ごみ箱をあさる時に、不確定な将来のフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bad8d-165">**SoftDelete** for Exchange 2007 sets a bit on the item that indicates to the Exchange database that the item will be moved to the dumpster folder at an indeterminate time in the future.</span></span> <span data-ttu-id="bad8d-166">Exchange 2010 の**SoftDelete**はすぐにアイテムを移動、ごみ箱をあさる。</span><span class="sxs-lookup"><span data-stu-id="bad8d-166">**SoftDelete** for Exchange 2010 immediately moves the item to the dumpster.</span></span> <span data-ttu-id="bad8d-167">**SoftDelete**は、フォルダーの削除のオプションではありません。</span><span class="sxs-lookup"><span data-stu-id="bad8d-167">**SoftDelete** is not an option for folder deletion.</span></span> <span data-ttu-id="bad8d-168">アイテムとフォルダーの**SoftDelete**の走査の検索では、結果は返されません。</span><span class="sxs-lookup"><span data-stu-id="bad8d-168">**SoftDelete** traversal searches for items and folders will not return any results.</span></span> 
  
<span data-ttu-id="bad8d-169">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="bad8d-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bad8d-170">要素情報</span><span class="sxs-lookup"><span data-stu-id="bad8d-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bad8d-171">名前空間</span><span class="sxs-lookup"><span data-stu-id="bad8d-171">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bad8d-172">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bad8d-172">Schema Name</span></span>  <br/> |<span data-ttu-id="bad8d-173">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="bad8d-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bad8d-174">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bad8d-174">Validation File</span></span>  <br/> |<span data-ttu-id="bad8d-175">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bad8d-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bad8d-176">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bad8d-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="bad8d-177">False</span><span class="sxs-lookup"><span data-stu-id="bad8d-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bad8d-178">関連項目</span><span class="sxs-lookup"><span data-stu-id="bad8d-178">See also</span></span>

- [<span data-ttu-id="bad8d-179">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="bad8d-179">DeleteItemResponse</span></span>](deleteitemresponse.md)  
- [<span data-ttu-id="bad8d-180">DeleteItem の操作</span><span class="sxs-lookup"><span data-stu-id="bad8d-180">DeleteItem operation</span></span>](deleteitem-operation.md)


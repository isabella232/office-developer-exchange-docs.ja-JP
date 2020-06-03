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
description: DeleteItem 要素は、Exchange ストア内のメールボックスからアイテムを削除するための要求を定義します。
ms.openlocfilehash: ed13ee32b487f49740aed80e8705257d3e2e6938
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529204"
---
# <a name="deleteitem"></a><span data-ttu-id="4fa65-103">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="4fa65-103">DeleteItem</span></span>

<span data-ttu-id="4fa65-104">**DeleteItem**要素は、Exchange ストア内のメールボックスからアイテムを削除するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="4fa65-104">The **DeleteItem** element defines a request to delete an item from a mailbox in the Exchange store.</span></span> 
  
```XML
<DeleteItem DeleteType="" SendMeetingCancellations="" AffectedTaskOccurrences="" SuppressReadReceipts="">
   <ItemIds/>
</DeleteItem>
```

 <span data-ttu-id="4fa65-105">**DeleteItemType**</span><span class="sxs-lookup"><span data-stu-id="4fa65-105">**DeleteItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4fa65-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4fa65-106">Attributes and elements</span></span>

<span data-ttu-id="4fa65-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4fa65-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4fa65-108">属性</span><span class="sxs-lookup"><span data-stu-id="4fa65-108">Attributes</span></span>

|<span data-ttu-id="4fa65-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="4fa65-109">**Attribute**</span></span>|<span data-ttu-id="4fa65-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="4fa65-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4fa65-111">**DeleteType**</span><span class="sxs-lookup"><span data-stu-id="4fa65-111">**DeleteType**</span></span> <br/> |<span data-ttu-id="4fa65-112">アイテムが削除される方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="4fa65-112">Describes how an item is deleted.</span></span> <span data-ttu-id="4fa65-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="4fa65-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="4fa65-114">**Send会議のキャンセル**</span><span class="sxs-lookup"><span data-stu-id="4fa65-114">**SendMeetingCancellations**</span></span> <br/> |<span data-ttu-id="4fa65-115">予定表アイテムの削除が出席者に伝達されるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4fa65-115">Describes whether a calendar item deletion is communicated to attendees.</span></span> <span data-ttu-id="4fa65-116">この属性は、予定表アイテムが削除されるときに必要になります。</span><span class="sxs-lookup"><span data-stu-id="4fa65-116">This attribute is required when calendar items are deleted.</span></span> <span data-ttu-id="4fa65-117">非予定表アイテムが削除された場合、この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="4fa65-117">This attribute is optional if non-calendar items are deleted.</span></span>  <br/> |
|<span data-ttu-id="4fa65-118">**AffectedTaskOccurrences**</span><span class="sxs-lookup"><span data-stu-id="4fa65-118">**AffectedTaskOccurrences**</span></span> <br/> |<span data-ttu-id="4fa65-119">[DeleteItem 操作](deleteitem-operation.md)によってタスクインスタンスまたはタスクマスターが削除されるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4fa65-119">Describes whether a task instance or a task master is deleted by a [DeleteItem operation](deleteitem-operation.md).</span></span> <span data-ttu-id="4fa65-120">この属性は、タスクを削除するときに必要になります。</span><span class="sxs-lookup"><span data-stu-id="4fa65-120">This attribute is required when tasks are deleted.</span></span> <span data-ttu-id="4fa65-121">非タスクアイテムが削除されている場合、この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="4fa65-121">This attribute is optional when non-task items are deleted.</span></span>  <br/> |
|<span data-ttu-id="4fa65-122">**SuppressReadReceipts**</span><span class="sxs-lookup"><span data-stu-id="4fa65-122">**SuppressReadReceipts**</span></span> <br/> |<span data-ttu-id="4fa65-123">削除済みアイテムの開封確認を抑制するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fa65-123">Indicates whether read receipts for the deleted item are suppressed.</span></span> <span data-ttu-id="4fa65-124">テキスト値が**true**の場合、開封確認が抑制されることを示します。</span><span class="sxs-lookup"><span data-stu-id="4fa65-124">A text value of **true**, indicates that the read receipts are suppressed.</span></span> <span data-ttu-id="4fa65-125">値が**false**の場合、開封確認が送信者に送信されることを示します。</span><span class="sxs-lookup"><span data-stu-id="4fa65-125">A value of **false** indicates that the read receipts are sent to the sender.</span></span> <span data-ttu-id="4fa65-126">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="4fa65-126">This attribute is optional.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="4fa65-127">DeleteType 属性</span><span class="sxs-lookup"><span data-stu-id="4fa65-127">DeleteType attribute</span></span>

|<span data-ttu-id="4fa65-128">**値**</span><span class="sxs-lookup"><span data-stu-id="4fa65-128">**Value**</span></span>|<span data-ttu-id="4fa65-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="4fa65-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4fa65-130">HardDelete</span><span class="sxs-lookup"><span data-stu-id="4fa65-130">HardDelete</span></span>  <br/> |<span data-ttu-id="4fa65-131">アイテムがストアから完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="4fa65-131">An item is permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="4fa65-132">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="4fa65-132">SoftDelete</span></span>  <br/> |<span data-ttu-id="4fa65-133">収集が有効になっている場合、アイテムは収集に移動されます。</span><span class="sxs-lookup"><span data-stu-id="4fa65-133">An item is moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="4fa65-134">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="4fa65-134">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="4fa65-135">アイテムが [削除済みアイテム] フォルダーに移動されます。</span><span class="sxs-lookup"><span data-stu-id="4fa65-135">An item is moved to the Deleted Items folder.</span></span>  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a><span data-ttu-id="4fa65-136">Send会議のキャンセル属性</span><span class="sxs-lookup"><span data-stu-id="4fa65-136">SendMeetingCancellations attribute</span></span>

|<span data-ttu-id="4fa65-137">**値**</span><span class="sxs-lookup"><span data-stu-id="4fa65-137">**Value**</span></span>|<span data-ttu-id="4fa65-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="4fa65-138">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4fa65-139">SendToNone</span><span class="sxs-lookup"><span data-stu-id="4fa65-139">SendToNone</span></span>  <br/> |<span data-ttu-id="4fa65-140">キャンセルメッセージを送信せずに予定表アイテムが削除されます。</span><span class="sxs-lookup"><span data-stu-id="4fa65-140">A calendar item is deleted without sending a cancellation message.</span></span>  <br/> |
|<span data-ttu-id="4fa65-141">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="4fa65-141">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="4fa65-142">予定表アイテムが削除され、すべての出席者に取り消しメッセージが送信されます。</span><span class="sxs-lookup"><span data-stu-id="4fa65-142">A calendar item is deleted and a cancellation message is sent to all attendees.</span></span>  <br/> |
|<span data-ttu-id="4fa65-143">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="4fa65-143">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="4fa65-144">予定表アイテムが削除され、すべての出席者に取り消しメッセージが送信されます。</span><span class="sxs-lookup"><span data-stu-id="4fa65-144">A calendar item is deleted and a cancellation message is sent to all attendees.</span></span> <span data-ttu-id="4fa65-145">取り消しメッセージのコピーが [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="4fa65-145">A copy of the cancellation message is saved in the Sent Items folder.</span></span>  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a><span data-ttu-id="4fa65-146">AffectedTaskOccurrences 属性</span><span class="sxs-lookup"><span data-stu-id="4fa65-146">AffectedTaskOccurrences attribute</span></span>

|<span data-ttu-id="4fa65-147">**値**</span><span class="sxs-lookup"><span data-stu-id="4fa65-147">**Value**</span></span>|<span data-ttu-id="4fa65-148">**説明**</span><span class="sxs-lookup"><span data-stu-id="4fa65-148">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4fa65-149">AllOccurrences</span><span class="sxs-lookup"><span data-stu-id="4fa65-149">AllOccurrences</span></span>  <br/> |<span data-ttu-id="4fa65-150">アイテムの削除要求は、マスタータスクを削除します。したがって、マスタータスクに関連付けられているすべての定期的なタスクを削除します。</span><span class="sxs-lookup"><span data-stu-id="4fa65-150">A delete item request deletes the master task, and therefore all recurring tasks that are associated with the master task.</span></span>  <br/> |
|<span data-ttu-id="4fa65-151">変数のみ</span><span class="sxs-lookup"><span data-stu-id="4fa65-151">SpecifiedOccurrenceOnly</span></span>  <br/> |<span data-ttu-id="4fa65-152">アイテムの削除要求では、タスクの特定のオカレンスのみが削除されます。</span><span class="sxs-lookup"><span data-stu-id="4fa65-152">A delete item request deletes only specific occurrences of a task.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4fa65-153">子要素</span><span class="sxs-lookup"><span data-stu-id="4fa65-153">Child elements</span></span>

|<span data-ttu-id="4fa65-154">**Element**</span><span class="sxs-lookup"><span data-stu-id="4fa65-154">**Element**</span></span>|<span data-ttu-id="4fa65-155">**説明**</span><span class="sxs-lookup"><span data-stu-id="4fa65-155">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fa65-156">ItemIds</span><span class="sxs-lookup"><span data-stu-id="4fa65-156">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="4fa65-157">Exchange ストア内のメールボックスから削除する項目、オカレンスアイテム、定期的なマスターアイテムの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="4fa65-157">Contains an array of items, occurrence items, and recurring master items to delete from a mailbox in the Exchange store.</span></span> <span data-ttu-id="4fa65-158">[DeleteItem 操作](deleteitem-operation.md)は、任意のアイテムの種類に対して実行できます。</span><span class="sxs-lookup"><span data-stu-id="4fa65-158">The [DeleteItem operation](deleteitem-operation.md) can be performed on any item type.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4fa65-159">親要素</span><span class="sxs-lookup"><span data-stu-id="4fa65-159">Parent elements</span></span>

<span data-ttu-id="4fa65-160">なし。</span><span class="sxs-lookup"><span data-stu-id="4fa65-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4fa65-161">注釈</span><span class="sxs-lookup"><span data-stu-id="4fa65-161">Remarks</span></span>

<span data-ttu-id="4fa65-162">**MoveToDeletedItems**および**ハード削除**オプションは、トランザクションであり、Web サービスの呼び出しが完了すると、データベースがアイテムを削除済みアイテムフォルダーに移動したか、または Exchange データベースからアイテムを完全に削除したことを意味します。</span><span class="sxs-lookup"><span data-stu-id="4fa65-162">The **MoveToDeletedItems** and **HardDelete** options are transactional, which means that by the time a Web service call completes, the database has moved the item to the Deleted Items folder or permanently removed the item from the Exchange database.</span></span> <span data-ttu-id="4fa65-163">この動作は、Microsoft Exchange Server 2007 および Exchange Server 2010 の場合と同じです。</span><span class="sxs-lookup"><span data-stu-id="4fa65-163">This behavior is the same for MicrosoftExchange Server 2007 and Exchange Server 2010.</span></span> 
  
<span data-ttu-id="4fa65-164">**Softdelete**オプションは、Exchange のターゲットバージョンによって動作が異なります。</span><span class="sxs-lookup"><span data-stu-id="4fa65-164">The **SoftDelete** option works differently for different target versions of Exchange.</span></span> <span data-ttu-id="4fa65-165">Exchange 2007 用の**Softdelete**は、今後、不確定な時点でアイテムが収集フォルダーに移動されることを exchange データベースに示すように、アイテムのビットを設定します。</span><span class="sxs-lookup"><span data-stu-id="4fa65-165">**SoftDelete** for Exchange 2007 sets a bit on the item that indicates to the Exchange database that the item will be moved to the dumpster folder at an indeterminate time in the future.</span></span> <span data-ttu-id="4fa65-166">Exchange 2010 用の**Softdelete**は、直ちにアイテムを収集に移動します。</span><span class="sxs-lookup"><span data-stu-id="4fa65-166">**SoftDelete** for Exchange 2010 immediately moves the item to the dumpster.</span></span> <span data-ttu-id="4fa65-167">**Softdelete**はフォルダー削除のオプションではありません。</span><span class="sxs-lookup"><span data-stu-id="4fa65-167">**SoftDelete** is not an option for folder deletion.</span></span> <span data-ttu-id="4fa65-168">**ソフト削除**によるアイテムとフォルダーの検索では、結果は返されません。</span><span class="sxs-lookup"><span data-stu-id="4fa65-168">**SoftDelete** traversal searches for items and folders will not return any results.</span></span> 
  
<span data-ttu-id="4fa65-169">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4fa65-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4fa65-170">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4fa65-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4fa65-171">Namespace</span><span class="sxs-lookup"><span data-stu-id="4fa65-171">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4fa65-172">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4fa65-172">Schema Name</span></span>  <br/> |<span data-ttu-id="4fa65-173">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="4fa65-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4fa65-174">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4fa65-174">Validation File</span></span>  <br/> |<span data-ttu-id="4fa65-175">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="4fa65-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4fa65-176">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4fa65-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="4fa65-177">正しくない</span><span class="sxs-lookup"><span data-stu-id="4fa65-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4fa65-178">関連項目</span><span class="sxs-lookup"><span data-stu-id="4fa65-178">See also</span></span>

- [<span data-ttu-id="4fa65-179">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="4fa65-179">DeleteItemResponse</span></span>](deleteitemresponse.md)  
- [<span data-ttu-id="4fa65-180">DeleteItem 操作</span><span class="sxs-lookup"><span data-stu-id="4fa65-180">DeleteItem operation</span></span>](deleteitem-operation.md)


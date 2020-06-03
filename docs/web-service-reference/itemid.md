---
title: ItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- ItemId
api_type:
- schema
ms.assetid: 3350b597-57a0-4961-8f44-8624946719b4
description: ItemId 要素には、Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。
localization_priority: Priority
ms.openlocfilehash: d5931702225c6864b1ca60a6f0753b65f65aca30
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44441563"
---
# <a name="itemid"></a><span data-ttu-id="c8c90-103">ItemId</span><span class="sxs-lookup"><span data-stu-id="c8c90-103">ItemId</span></span>

<span data-ttu-id="c8c90-104">**ItemId**要素には、Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c8c90-104">The **ItemId** element contains the unique identifier and change key of an item in the Exchange store.</span></span> 
  
```XML
<ItemId Id="" ChangeKey="" />
```

 <span data-ttu-id="c8c90-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="c8c90-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c8c90-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c8c90-106">Attributes and elements</span></span>

<span data-ttu-id="c8c90-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8c90-108">属性</span><span class="sxs-lookup"><span data-stu-id="c8c90-108">Attributes</span></span>

|<span data-ttu-id="c8c90-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="c8c90-109">**Attribute**</span></span>|<span data-ttu-id="c8c90-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="c8c90-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c8c90-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="c8c90-111">**Id**</span></span> <br/> |<span data-ttu-id="c8c90-112">Exchange ストア内の特定のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-112">Identifies a specific item in the Exchange store.</span></span> <span data-ttu-id="c8c90-113">**Id**は大文字と小文字を区別します。そのため、 **id**間の比較には、大文字と小文字を区別するか、バイナリにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8c90-113">**Id** is case-sensitive; therefore, comparisons between **Ids** must be case-sensitive or binary.</span></span>  <br/> |
|<span data-ttu-id="c8c90-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="c8c90-114">**ChangeKey**</span></span> <br/> | <span data-ttu-id="c8c90-115">特定のバージョンのアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-115">Identifies a specific version of an item.</span></span> <br/><br/><span data-ttu-id="c8c90-116">次のシナリオでは、 **Changekey**が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8c90-116">A **ChangeKey** is required for the following scenarios:</span></span> <br/> <br/><span data-ttu-id="c8c90-117">- **ConflictResolution**属性が自動解決に設定されている場合、 [updateitem](updateitem.md)要素には**changekey**が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8c90-117">-  The [UpdateItem](updateitem.md) element requires a **ChangeKey** if the **ConflictResolution** attribute is set to AutoResolve.</span></span> <span data-ttu-id="c8c90-118">自動解決は既定値です。</span><span class="sxs-lookup"><span data-stu-id="c8c90-118">AutoResolve is a default value.</span></span> <span data-ttu-id="c8c90-119">**Changekey**属性が含まれていない場合、応答は、 **Errorchangekeyrequired**に[等しい値を](responsecode.md)返します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-119">If the **ChangeKey** attribute is not included, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorChangeKeyRequired**.</span></span>  <br/><br/><span data-ttu-id="c8c90-120">- [SendItem](senditem.md)要素には、試行された操作がアイテムの最新バージョンに対して動作するかどうかをテストするための**changekey**が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8c90-120">-  The [SendItem](senditem.md) element requires a **ChangeKey** to test whether the attempted operation will act upon the most recent version of an item.</span></span> <span data-ttu-id="c8c90-121">**Changekey**属性が**ItemId**に含まれていない場合、または**changekey**が空の場合は、応答は**ErrorStaleObject**に等しい、応答し[た値を](responsecode.md)返します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-121">If the **ChangeKey** attribute is not included in the **ItemId** or if the **ChangeKey** is empty, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorStaleObject**.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c8c90-122">子要素</span><span class="sxs-lookup"><span data-stu-id="c8c90-122">Child elements</span></span>

<span data-ttu-id="c8c90-123">なし。</span><span class="sxs-lookup"><span data-stu-id="c8c90-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c8c90-124">親要素</span><span class="sxs-lookup"><span data-stu-id="c8c90-124">Parent elements</span></span>

|<span data-ttu-id="c8c90-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="c8c90-125">**Element**</span></span>|<span data-ttu-id="c8c90-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="c8c90-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8c90-127">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="c8c90-127">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c8c90-128">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-128">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-129">Contact</span><span class="sxs-lookup"><span data-stu-id="c8c90-129">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="c8c90-130">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-130">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-131">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="c8c90-131">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="c8c90-132">アイテムまたはフォルダーがコピーされるときのイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-132">Represents an event when an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-133">対する createdevent</span><span class="sxs-lookup"><span data-stu-id="c8c90-133">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="c8c90-134">アイテムまたはフォルダーが作成されたときのイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-134">Represents an event when an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-135">削除 (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="c8c90-135">Delete (ItemSync)</span></span>](delete-itemsync.md) <br/> |<span data-ttu-id="c8c90-136">ローカルクライアントストアで削除する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-136">Identifies a single item to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-137">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="c8c90-137">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="c8c90-138">アイテムまたはフォルダーが削除されたときのイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-138">Represents an event when an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-139">DistributionList</span><span class="sxs-lookup"><span data-stu-id="c8c90-139">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="c8c90-140">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-140">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-141">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c8c90-141">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md) <br/> |<span data-ttu-id="c8c90-142">1つのメールボックスアイテムをエクスポートする要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-142">Contains the status and results of a request to export a single mailbox item.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-143">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="c8c90-143">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="c8c90-144">定期的な予定表アイテムの最初の出現を表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-144">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-145">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="c8c90-145">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="c8c90-146">メールボックス内のすべての会話アイテムのアイテム識別子のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c8c90-146">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-147">無視</span><span class="sxs-lookup"><span data-stu-id="c8c90-147">Ignore</span></span>](ignore.md) <br/> |<span data-ttu-id="c8c90-148">同期中にスキップするアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-148">Identifies items to skip during synchronization.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-149">Item</span><span class="sxs-lookup"><span data-stu-id="c8c90-149">Item</span></span>](item.md) <br/> |<span data-ttu-id="c8c90-150">汎用の Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-150">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-151">Item (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="c8c90-151">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="c8c90-152">メールボックスにアップロードする単一のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-152">Represents a single item to upload into a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-153">ItemChange</span><span class="sxs-lookup"><span data-stu-id="c8c90-153">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="c8c90-154">アイテム識別子と、アイテムに適用する更新を含みます。</span><span class="sxs-lookup"><span data-stu-id="c8c90-154">Contains an item identifier and the updates to apply to the item.</span></span>  <br/><br/> <span data-ttu-id="c8c90-155">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-155">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[<span data-ttu-id="c8c90-156">ItemIds</span><span class="sxs-lookup"><span data-stu-id="c8c90-156">ItemIds</span></span>](itemids.md) <br/> | <span data-ttu-id="c8c90-157">Exchange ストア内のアイテムの削除、送信、取得、移動、またはコピーに使用するアイテム、オカレンスアイテム、定期的なマスターアイテムの一意の id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c8c90-157">Contains the unique identities of items, occurrence items, and recurring master items used to delete, send, get, move, or copy items in the Exchange store.</span></span> <br/> <br/>  <span data-ttu-id="c8c90-158">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c8c90-158">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
|[<span data-ttu-id="c8c90-159">ItemIds (非 Emptyarrayofitemidstype)</span><span class="sxs-lookup"><span data-stu-id="c8c90-159">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md) <br/> |<span data-ttu-id="c8c90-160">メールボックスからエクスポートするアイテムを識別するアイテム識別子の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-160">Contains an array of item identifiers that identify the items to export from a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-161">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="c8c90-161">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="c8c90-162">定期的な予定表アイテムの最後の発生を表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-162">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-163">メールボックス</span><span class="sxs-lookup"><span data-stu-id="c8c90-163">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="c8c90-164">メールが有効な Active Directory ディレクトリサービスオブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-164">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-165">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="c8c90-165">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="c8c90-166">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-166">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-167">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="c8c90-167">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="c8c90-168">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-168">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-169">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c8c90-169">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c8c90-170">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-170">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-171">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="c8c90-171">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="c8c90-172">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-172">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-173">Message</span><span class="sxs-lookup"><span data-stu-id="c8c90-173">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c8c90-174">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-174">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-175">対する modifiedevent</span><span class="sxs-lookup"><span data-stu-id="c8c90-175">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="c8c90-176">アイテムが変更されたときに発生するイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-176">Represents an event that occurs when an item is modified.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-177">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="c8c90-177">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="c8c90-178">ある親フォルダーから別の親フォルダーにアイテムが移動されたときに発生するイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-178">Represents an event that occurs when an item is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-179">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="c8c90-179">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="c8c90-180">メールボックス内の新しいメールアイテムによってトリガーされるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-180">Represents an event that is triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-181">発生</span><span class="sxs-lookup"><span data-stu-id="c8c90-181">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="c8c90-182">定期的な予定表アイテムの1つの変更されたアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-182">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-183">PlayOnPhone (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="c8c90-183">PlayOnPhone (Exchange Web Services)</span></span>](playonphone-exchange-web-services.md) <br/> |<span data-ttu-id="c8c90-184">電話のアイテムを読み取るための要求を表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-184">Represents a request to read an item on a telephone.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-185">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="c8c90-185">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="c8c90-186">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-186">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-187">RoomList</span><span class="sxs-lookup"><span data-stu-id="c8c90-187">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="c8c90-188">会議室の一覧を識別する電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-188">Represents an e-mail address that identifies a list of meeting rooms.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-189">タスク</span><span class="sxs-lookup"><span data-stu-id="c8c90-189">Task</span></span>](task.md) <br/> |<span data-ttu-id="c8c90-190">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-190">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-191">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c8c90-191">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md) <br/> |<span data-ttu-id="c8c90-192">1つのメールボックスアイテムをアップロードする要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-192">Contains the status and results of a request to upload a single mailbox item.</span></span>  <br/> |
|[<span data-ttu-id="c8c90-193">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="c8c90-193">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="c8c90-194">1つのユーザー構成オブジェクトを定義します。</span><span class="sxs-lookup"><span data-stu-id="c8c90-194">Defines a single user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c8c90-195">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c8c90-195">Text value</span></span>

<span data-ttu-id="c8c90-196">なし。</span><span class="sxs-lookup"><span data-stu-id="c8c90-196">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c8c90-197">注釈</span><span class="sxs-lookup"><span data-stu-id="c8c90-197">Remarks</span></span>

<span data-ttu-id="c8c90-198">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c8c90-198">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c8c90-199">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c8c90-199">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c8c90-200">Namespace</span><span class="sxs-lookup"><span data-stu-id="c8c90-200">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c8c90-201">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c8c90-201">Schema Name</span></span>  <br/> |<span data-ttu-id="c8c90-202">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c8c90-202">Types schema</span></span>  <br/> |
|<span data-ttu-id="c8c90-203">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c8c90-203">Validation File</span></span>  <br/> |<span data-ttu-id="c8c90-204">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c8c90-204">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c8c90-205">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c8c90-205">Can be Empty</span></span>  <br/> |<span data-ttu-id="c8c90-206">正しくない</span><span class="sxs-lookup"><span data-stu-id="c8c90-206">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c8c90-207">関連項目</span><span class="sxs-lookup"><span data-stu-id="c8c90-207">See also</span></span>

- [<span data-ttu-id="c8c90-208">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="c8c90-208">ExportItems operation</span></span>](exportitems-operation.md)
- [<span data-ttu-id="c8c90-209">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="c8c90-209">UploadItems operation</span></span>](uploaditems-operation.md) 
- [<span data-ttu-id="c8c90-210">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="c8c90-210">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="c8c90-211">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c8c90-211">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


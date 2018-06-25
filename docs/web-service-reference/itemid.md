---
title: ItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemId
api_type:
- schema
ms.assetid: 3350b597-57a0-4961-8f44-8624946719b4
description: ItemId の要素には、Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。
ms.openlocfilehash: 9c5d71a23e1e4b77d2a50016aa4d765d872d04cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832157"
---
# <a name="itemid"></a><span data-ttu-id="c2e95-103">ItemId</span><span class="sxs-lookup"><span data-stu-id="c2e95-103">ItemId</span></span>

<span data-ttu-id="c2e95-104">**ItemId**の要素には、Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c2e95-104">The **ItemId** element contains the unique identifier and change key of an item in the Exchange store.</span></span> 
  
```XML
<ItemId Id="" ChangeKey="" />
```

 <span data-ttu-id="c2e95-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="c2e95-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2e95-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c2e95-106">Attributes and elements</span></span>

<span data-ttu-id="c2e95-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2e95-108">属性</span><span class="sxs-lookup"><span data-stu-id="c2e95-108">Attributes</span></span>

|<span data-ttu-id="c2e95-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="c2e95-109">**Attribute**</span></span>|<span data-ttu-id="c2e95-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2e95-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c2e95-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="c2e95-111">**Id**</span></span> <br/> |<span data-ttu-id="c2e95-112">Exchange ストア内の特定の項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-112">Identifies a specific item in the Exchange store.</span></span> <span data-ttu-id="c2e95-113">**Id**は大文字小文字を区別します。したがって、 **Id**の間の比較は大文字小文字を区別またはバイナリをする必要があります。</span><span class="sxs-lookup"><span data-stu-id="c2e95-113">**Id** is case-sensitive; therefore, comparisons between **Ids** must be case-sensitive or binary.</span></span>  <br/> |
|<span data-ttu-id="c2e95-114">**変更キー**</span><span class="sxs-lookup"><span data-stu-id="c2e95-114">**ChangeKey**</span></span> <br/> | <span data-ttu-id="c2e95-115">アイテムの特定のバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-115">Identifies a specific version of an item.</span></span> <br/><br/><span data-ttu-id="c2e95-116">の**変更キー**は、次のシナリオで必要です。</span><span class="sxs-lookup"><span data-stu-id="c2e95-116">A **ChangeKey** is required for the following scenarios:</span></span> <br/> <br/><span data-ttu-id="c2e95-117">- [UpdateItem](updateitem.md)要素では、自動解決する**ConflictResolution**属性が設定されている場合に、**変更キー**が必要です。</span><span class="sxs-lookup"><span data-stu-id="c2e95-117">-  The [UpdateItem](updateitem.md) element requires a **ChangeKey** if the **ConflictResolution** attribute is set to AutoResolve.</span></span> <span data-ttu-id="c2e95-118">自動解決は、既定値です。</span><span class="sxs-lookup"><span data-stu-id="c2e95-118">AutoResolve is a default value.</span></span> <span data-ttu-id="c2e95-119">**変更キー**属性が含まれていない場合は、応答が値を返す[ResponseCode](responsecode.md) **ErrorChangeKeyRequired**に等しい。</span><span class="sxs-lookup"><span data-stu-id="c2e95-119">If the **ChangeKey** attribute is not included, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorChangeKeyRequired**.</span></span>  <br/><br/><span data-ttu-id="c2e95-120">[SendItem](senditem.md)要素には、試行した操作は、項目の最新バージョンに対して機能するかどうかをテストするための**変更キー**が必要です。</span><span class="sxs-lookup"><span data-stu-id="c2e95-120">-  The [SendItem](senditem.md) element requires a **ChangeKey** to test whether the attempted operation will act upon the most recent version of an item.</span></span> <span data-ttu-id="c2e95-121">**アイテム Id**の**変更キー**の属性が含まれていない場合、または**変更キー**が空の場合は、応答が値を返す[ResponseCode](responsecode.md) **ErrorStaleObject**に等しい。</span><span class="sxs-lookup"><span data-stu-id="c2e95-121">If the **ChangeKey** attribute is not included in the **ItemId** or if the **ChangeKey** is empty, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorStaleObject**.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c2e95-122">子要素</span><span class="sxs-lookup"><span data-stu-id="c2e95-122">Child elements</span></span>

<span data-ttu-id="c2e95-123">なし。</span><span class="sxs-lookup"><span data-stu-id="c2e95-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c2e95-124">親要素</span><span class="sxs-lookup"><span data-stu-id="c2e95-124">Parent elements</span></span>

|<span data-ttu-id="c2e95-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="c2e95-125">**Element**</span></span>|<span data-ttu-id="c2e95-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2e95-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2e95-127">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="c2e95-127">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c2e95-128">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-128">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-129">Contact</span><span class="sxs-lookup"><span data-stu-id="c2e95-129">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="c2e95-130">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-130">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-131">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="c2e95-131">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="c2e95-132">アイテムまたはフォルダーがコピーされるときにイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-132">Represents an event when an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-133">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="c2e95-133">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="c2e95-134">アイテムまたはフォルダーが作成されたときにイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-134">Represents an event when an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-135">(ItemSync) を削除します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-135">Delete (ItemSync)</span></span>](delete-itemsync.md) <br/> |<span data-ttu-id="c2e95-136">ローカル クライアント ストアで削除するのには 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-136">Identifies a single item to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-137">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="c2e95-137">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="c2e95-138">アイテムまたはフォルダーが削除されたときにイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-138">Represents an event when an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-139">DistributionList</span><span class="sxs-lookup"><span data-stu-id="c2e95-139">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="c2e95-140">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-140">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-141">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c2e95-141">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md) <br/> |<span data-ttu-id="c2e95-142">状態および 1 つのメールボックス アイテムをエクスポートするのには要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c2e95-142">Contains the status and results of a request to export a single mailbox item.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-143">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="c2e95-143">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="c2e95-144">定期的な予定表アイテムが最初に見つかった位置を表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-144">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-145">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="c2e95-145">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="c2e95-146">メールボックス内のすべての会話項目の項目の識別子のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c2e95-146">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-147">Ignore</span><span class="sxs-lookup"><span data-stu-id="c2e95-147">Ignore</span></span>](ignore.md) <br/> |<span data-ttu-id="c2e95-148">同期中にスキップする項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-148">Identifies items to skip during synchronization.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-149">アイテム</span><span class="sxs-lookup"><span data-stu-id="c2e95-149">Item</span></span>](item.md) <br/> |<span data-ttu-id="c2e95-150">一般的な Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-150">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-151">項目 (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="c2e95-151">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="c2e95-152">メールボックスにアップロードする 1 つの項目を表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-152">Represents a single item to upload into a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-153">ItemChange</span><span class="sxs-lookup"><span data-stu-id="c2e95-153">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="c2e95-154">アイテム識別子と、アイテムに適用する更新プログラムが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c2e95-154">Contains an item identifier and the updates to apply to the item.</span></span>  <br/><br/> <span data-ttu-id="c2e95-155">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="c2e95-155">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[<span data-ttu-id="c2e95-156">Itemid</span><span class="sxs-lookup"><span data-stu-id="c2e95-156">ItemIds</span></span>](itemids.md) <br/> | <span data-ttu-id="c2e95-157">アイテム、出現アイテム、および削除、送信、取得、移動、または Exchange ストア内のアイテムをコピーするに使用されるマスターの定期的なアイテムの一意の id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c2e95-157">Contains the unique identities of items, occurrence items, and recurring master items used to delete, send, get, move, or copy items in the Exchange store.</span></span> <br/> <br/>  <span data-ttu-id="c2e95-158">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="c2e95-158">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
|[<span data-ttu-id="c2e95-159">Itemid (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="c2e95-159">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md) <br/> |<span data-ttu-id="c2e95-160">メールボックスからエクスポートする項目を識別する項目 id の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c2e95-160">Contains an array of item identifiers that identify the items to export from a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-161">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="c2e95-161">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="c2e95-162">定期的な予定表アイテムが最後に見つかった位置を表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-162">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-163">メールボックス</span><span class="sxs-lookup"><span data-stu-id="c2e95-163">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="c2e95-164">メールが有効な Active Directory ディレクトリ サービス オブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-164">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-165">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="c2e95-165">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="c2e95-166">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-166">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-167">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="c2e95-167">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="c2e95-168">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-168">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-169">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c2e95-169">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c2e95-170">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-170">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-171">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="c2e95-171">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="c2e95-172">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-172">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-173">Message</span><span class="sxs-lookup"><span data-stu-id="c2e95-173">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c2e95-174">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-174">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-175">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="c2e95-175">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="c2e95-176">アイテムが変更されたときに発生するイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-176">Represents an event that occurs when an item is modified.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-177">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="c2e95-177">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="c2e95-178">1 つの親フォルダーから別の親フォルダーにアイテムが移動したときに発生するイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-178">Represents an event that occurs when an item is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-179">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="c2e95-179">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="c2e95-180">メールボックス内の新しいメール アイテムによって発生するイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-180">Represents an event that is triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-181">出現</span><span class="sxs-lookup"><span data-stu-id="c2e95-181">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="c2e95-182">定期的な予定表アイテムの 1 つの変更されたアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-182">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-183">PlayOnPhone (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="c2e95-183">PlayOnPhone (Exchange Web Services)</span></span>](playonphone-exchange-web-services.md) <br/> |<span data-ttu-id="c2e95-184">電話上のアイテムの読み取り要求を表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-184">Represents a request to read an item on a telephone.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-185">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="c2e95-185">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="c2e95-186">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-186">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-187">RoomList</span><span class="sxs-lookup"><span data-stu-id="c2e95-187">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="c2e95-188">会議室の一覧を識別する電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-188">Represents an e-mail address that identifies a list of meeting rooms.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-189">タスク</span><span class="sxs-lookup"><span data-stu-id="c2e95-189">Task</span></span>](task.md) <br/> |<span data-ttu-id="c2e95-190">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-190">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-191">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c2e95-191">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md) <br/> |<span data-ttu-id="c2e95-192">状態および 1 つのメールボックス アイテムをアップロードするための要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c2e95-192">Contains the status and results of a request to upload a single mailbox item.</span></span>  <br/> |
|[<span data-ttu-id="c2e95-193">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="c2e95-193">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="c2e95-194">1 人のユーザーの構成オブジェクトを定義します。</span><span class="sxs-lookup"><span data-stu-id="c2e95-194">Defines a single user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c2e95-195">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c2e95-195">Text value</span></span>

<span data-ttu-id="c2e95-196">なし。</span><span class="sxs-lookup"><span data-stu-id="c2e95-196">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c2e95-197">備考</span><span class="sxs-lookup"><span data-stu-id="c2e95-197">Remarks</span></span>

<span data-ttu-id="c2e95-198">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c2e95-198">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2e95-199">要素情報</span><span class="sxs-lookup"><span data-stu-id="c2e95-199">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2e95-200">名前空間</span><span class="sxs-lookup"><span data-stu-id="c2e95-200">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c2e95-201">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c2e95-201">Schema Name</span></span>  <br/> |<span data-ttu-id="c2e95-202">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c2e95-202">Types schema</span></span>  <br/> |
|<span data-ttu-id="c2e95-203">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c2e95-203">Validation File</span></span>  <br/> |<span data-ttu-id="c2e95-204">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c2e95-204">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c2e95-205">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c2e95-205">Can be Empty</span></span>  <br/> |<span data-ttu-id="c2e95-206">False</span><span class="sxs-lookup"><span data-stu-id="c2e95-206">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2e95-207">関連項目</span><span class="sxs-lookup"><span data-stu-id="c2e95-207">See also</span></span>

- [<span data-ttu-id="c2e95-208">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="c2e95-208">ExportItems operation</span></span>](exportitems-operation.md)
- [<span data-ttu-id="c2e95-209">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="c2e95-209">UploadItems operation</span></span>](uploaditems-operation.md) 
- <span data-ttu-id="c2e95-210">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="c2e95-210">[FindConversation operation](findconversation-operation.md)</span></span>
- [<span data-ttu-id="c2e95-211">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c2e95-211">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: UpdateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 34643d58-2743-45b0-a08d-bff6dc1da61d
description: UpdateItem 要素では、メールボックス内のアイテムを更新する要求を定義します。
ms.openlocfilehash: 7b9b5f1dcffb95eb127572cb91f92d961c05a77e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/15/2018
ms.locfileid: "19839869"
---
# <a name="updateitem"></a><span data-ttu-id="52378-103">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="52378-103">UpdateItem</span></span>

<span data-ttu-id="52378-104">**UpdateItem**要素では、メールボックス内のアイテムを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="52378-104">The **UpdateItem** element defines a request to update an item in a mailbox.</span></span> 
  
```XML
<UpdateItem ConflictResolution="" MessageDisposition="" SendMeetingInvitationsOrCancellations="" SuppressReadReceipts="">
   <SavedItemFolderId/>
   <ItemChanges/>
</UpdateItem>
```

 <span data-ttu-id="52378-105">**UpdateItemType**</span><span class="sxs-lookup"><span data-stu-id="52378-105">**UpdateItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="52378-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="52378-106">Attributes and elements</span></span>

<span data-ttu-id="52378-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="52378-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="52378-108">属性</span><span class="sxs-lookup"><span data-stu-id="52378-108">Attributes</span></span>

|<span data-ttu-id="52378-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="52378-109">**Attribute**</span></span>|<span data-ttu-id="52378-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="52378-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="52378-111">**ConflictResolution**</span><span class="sxs-lookup"><span data-stu-id="52378-111">**ConflictResolution**</span></span> <br/> |<span data-ttu-id="52378-112">更新中に競合の解決の種類を識別します。</span><span class="sxs-lookup"><span data-stu-id="52378-112">Identifies the type of conflict resolution to try during an update.</span></span> <span data-ttu-id="52378-113">既定値は、自動解決します。</span><span class="sxs-lookup"><span data-stu-id="52378-113">The default value is AutoResolve.</span></span>  <br/> |
|<span data-ttu-id="52378-114">**MessageDisposition**</span><span class="sxs-lookup"><span data-stu-id="52378-114">**MessageDisposition**</span></span> <br/> |<span data-ttu-id="52378-115">更新後のアイテムの処理方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="52378-115">Describes how the item will be handled after it is updated.</span></span> <span data-ttu-id="52378-116">**MessageDisposition**属性は、メッセージ アイテム、会議の取り消し、会議出席依頼、会議出席依頼など、会議のメッセージを含む必要があります。</span><span class="sxs-lookup"><span data-stu-id="52378-116">The **MessageDisposition** attribute is required for message items, including meeting messages such as meeting cancellations, meeting requests, and meeting responses.</span></span>  <br/> |
|<span data-ttu-id="52378-117">**SendMeetingInvitationsOrCancellations**</span><span class="sxs-lookup"><span data-stu-id="52378-117">**SendMeetingInvitationsOrCancellations**</span></span> <br/> |<span data-ttu-id="52378-118">予定表アイテムが更新された後に会議の更新を通知する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="52378-118">Describes how meeting updates are communicated after a calendar item is updated.</span></span> <span data-ttu-id="52378-119">この属性は、予定表アイテム、予定表アイテムの出現する必要があります。</span><span class="sxs-lookup"><span data-stu-id="52378-119">This attribute is required for calendar items and calendar item occurrences.</span></span>  <br/> |
|<span data-ttu-id="52378-120">**SuppressReadReceipts**</span><span class="sxs-lookup"><span data-stu-id="52378-120">**SuppressReadReceipts**</span></span> <br/> |<span data-ttu-id="52378-121">更新されたアイテムの開封確認メッセージを抑制するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="52378-121">Indicates whether read receipts for the updated item should be suppressed.</span></span> <span data-ttu-id="52378-122">**True**の場合、テキスト値では、読み取り確認メッセージを抑制するかを示します。</span><span class="sxs-lookup"><span data-stu-id="52378-122">A text value of **true** indicates that read receipts should be suppressed.</span></span> <span data-ttu-id="52378-123">**False**の値は、送信者に開封確認が送信されることを示します。</span><span class="sxs-lookup"><span data-stu-id="52378-123">A value of **false** indicates that the read receipts will be sent to the sender.</span></span> <span data-ttu-id="52378-124">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="52378-124">This attribute is optional.</span></span>  <br/> <span data-ttu-id="52378-125">この属性は、Exchange Server 2013 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="52378-125">This attribute was introduced in Exchange Server 2013 SP1.</span></span>  <br/> |
   
#### <a name="conflictresolution-attribute"></a><span data-ttu-id="52378-126">ConflictResolution 属性</span><span class="sxs-lookup"><span data-stu-id="52378-126">ConflictResolution Attribute</span></span>

|<span data-ttu-id="52378-127">**値**</span><span class="sxs-lookup"><span data-stu-id="52378-127">**Value**</span></span>|<span data-ttu-id="52378-128">**説明**</span><span class="sxs-lookup"><span data-stu-id="52378-128">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="52378-129">NeverOverwrite</span><span class="sxs-lookup"><span data-stu-id="52378-129">NeverOverwrite</span></span>  <br/> |<span data-ttu-id="52378-130">競合がある場合は、更新操作は失敗し、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="52378-130">If there is a conflict, the update operation fails and an error is returned.</span></span>  <br/> |
|<span data-ttu-id="52378-131">自動解決</span><span class="sxs-lookup"><span data-stu-id="52378-131">AutoResolve</span></span>  <br/> |<span data-ttu-id="52378-132">更新操作は、自動的にすべての競合を解決します。</span><span class="sxs-lookup"><span data-stu-id="52378-132">The update operation automatically resolves any conflict.</span></span>  <br/> |
|<span data-ttu-id="52378-133">AlwaysOverwrite</span><span class="sxs-lookup"><span data-stu-id="52378-133">AlwaysOverwrite</span></span>  <br/> |<span data-ttu-id="52378-134">競合がある場合は、更新操作には情報が上書きされます。</span><span class="sxs-lookup"><span data-stu-id="52378-134">If there is a conflict, the update operation will overwrite information.</span></span>  <br/> |
   
#### <a name="messagedisposition-attribute"></a><span data-ttu-id="52378-135">MessageDisposition 属性</span><span class="sxs-lookup"><span data-stu-id="52378-135">MessageDisposition Attribute</span></span>

|<span data-ttu-id="52378-136">**値**</span><span class="sxs-lookup"><span data-stu-id="52378-136">**Value**</span></span>|<span data-ttu-id="52378-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="52378-137">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="52378-138">SaveOnly</span><span class="sxs-lookup"><span data-stu-id="52378-138">SaveOnly</span></span>  <br/> |<span data-ttu-id="52378-139">アイテムが更新され、現在のフォルダーに保存します。</span><span class="sxs-lookup"><span data-stu-id="52378-139">The item is updated and saved back to its current folder.</span></span>  <br/> |
|<span data-ttu-id="52378-140">SendOnly</span><span class="sxs-lookup"><span data-stu-id="52378-140">SendOnly</span></span>  <br/> |<span data-ttu-id="52378-141">アイテムが更新され、送信されたが、コピーは保存されません。</span><span class="sxs-lookup"><span data-stu-id="52378-141">The item is updated and sent but no copy is saved.</span></span>  <br/> |
|<span data-ttu-id="52378-142">SendAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="52378-142">SendAndSaveCopy</span></span>  <br/> |<span data-ttu-id="52378-143">アイテムを更新し、 [SavedItemFolderId](saveditemfolderid.md)要素で指定されたフォルダーにコピーを保存します。</span><span class="sxs-lookup"><span data-stu-id="52378-143">The item is updated and a copy is saved in the folder identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a><span data-ttu-id="52378-144">SendMeetingInvitationsOrCancellations 属性</span><span class="sxs-lookup"><span data-stu-id="52378-144">SendMeetingInvitationsOrCancellations Attribute</span></span>

|<span data-ttu-id="52378-145">**値**</span><span class="sxs-lookup"><span data-stu-id="52378-145">**Value**</span></span>|<span data-ttu-id="52378-146">**説明**</span><span class="sxs-lookup"><span data-stu-id="52378-146">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="52378-147">SendToNone</span><span class="sxs-lookup"><span data-stu-id="52378-147">SendToNone</span></span>  <br/> |<span data-ttu-id="52378-148">予定表アイテムが更新されますが、更新が出席者に送信されません。</span><span class="sxs-lookup"><span data-stu-id="52378-148">The calendar item is updated but updates are not sent to attendees.</span></span>  <br/> |
|<span data-ttu-id="52378-149">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="52378-149">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="52378-150">予定表アイテムが更新され、会議の更新は、すべての出席者に送信されますが、送信済みアイテム フォルダーには保存されません。</span><span class="sxs-lookup"><span data-stu-id="52378-150">The calendar item is updated and the meeting update is sent to all attendees but is not saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="52378-151">SendOnlyToChanged</span><span class="sxs-lookup"><span data-stu-id="52378-151">SendOnlyToChanged</span></span>  <br/> |<span data-ttu-id="52378-152">予定表アイテムが更新され、会議の更新は、会議の変更の影響を受けるための出席者にのみ送信します。</span><span class="sxs-lookup"><span data-stu-id="52378-152">The calendar item is updated and the meeting update is sent only to attendees that are affected by the change in the meeting.</span></span>  <br/> |
|<span data-ttu-id="52378-153">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="52378-153">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="52378-154">予定表アイテムが更新され、すべての出席者に会議の更新が送信されるコピーが [送信済みアイテム フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="52378-154">The calendar item is updated, the meeting update is sent to all attendees, and a copy is saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="52378-155">SendToChangedAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="52378-155">SendToChangedAndSaveCopy</span></span>  <br/> |<span data-ttu-id="52378-156">予定表アイテムが更新され、会議の変更の影響を受けるすべての出席者に会議の更新が送信されるコピーが [送信済みアイテム フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="52378-156">The calendar item is updated, the meeting update is sent to all attendees that are affected by the change in the meeting, and a copy is saved in the Sent Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="52378-157">子要素</span><span class="sxs-lookup"><span data-stu-id="52378-157">Child elements</span></span>

|<span data-ttu-id="52378-158">**要素**</span><span class="sxs-lookup"><span data-stu-id="52378-158">**Element**</span></span>|<span data-ttu-id="52378-159">**説明**</span><span class="sxs-lookup"><span data-stu-id="52378-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52378-160">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="52378-160">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="52378-161">更新、送信、および Exchange ストア内の項目を作成する操作のターゲット フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="52378-161">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="52378-162">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="52378-162">ItemChanges</span></span>](itemchanges.md) <br/> |<span data-ttu-id="52378-163">アイテムと、アイテムに適用する更新プログラムを識別する[ItemChange](itemchange.md)要素の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="52378-163">Contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="52378-164">親要素</span><span class="sxs-lookup"><span data-stu-id="52378-164">Parent elements</span></span>

<span data-ttu-id="52378-165">なし。</span><span class="sxs-lookup"><span data-stu-id="52378-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="52378-166">備考</span><span class="sxs-lookup"><span data-stu-id="52378-166">Remarks</span></span>

<span data-ttu-id="52378-167">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="52378-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="52378-168">要素情報</span><span class="sxs-lookup"><span data-stu-id="52378-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="52378-169">名前空間</span><span class="sxs-lookup"><span data-stu-id="52378-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="52378-170">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="52378-170">Schema Name</span></span>  <br/> |<span data-ttu-id="52378-171">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="52378-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="52378-172">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="52378-172">Validation File</span></span>  <br/> |<span data-ttu-id="52378-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="52378-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="52378-174">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="52378-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="52378-175">False</span><span class="sxs-lookup"><span data-stu-id="52378-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="52378-176">関連項目</span><span class="sxs-lookup"><span data-stu-id="52378-176">See also</span></span>



<span data-ttu-id="52378-177">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="52378-177">[UpdateItem operation](updateitem-operation.md)</span></span>


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
description: UpdateItem 要素は、メールボックス内のアイテムを更新する要求を定義します。
ms.openlocfilehash: 43821db58457ffce22be918a7ba6427f57230010
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466571"
---
# <a name="updateitem"></a><span data-ttu-id="f6cce-103">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="f6cce-103">UpdateItem</span></span>

<span data-ttu-id="f6cce-104">**Updateitem**要素は、メールボックス内のアイテムを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="f6cce-104">The **UpdateItem** element defines a request to update an item in a mailbox.</span></span> 
  
```XML
<UpdateItem ConflictResolution="" MessageDisposition="" SendMeetingInvitationsOrCancellations="" SuppressReadReceipts="">
   <SavedItemFolderId/>
   <ItemChanges/>
</UpdateItem>
```

 <span data-ttu-id="f6cce-105">**UpdateItemType**</span><span class="sxs-lookup"><span data-stu-id="f6cce-105">**UpdateItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6cce-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f6cce-106">Attributes and elements</span></span>

<span data-ttu-id="f6cce-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f6cce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6cce-108">属性</span><span class="sxs-lookup"><span data-stu-id="f6cce-108">Attributes</span></span>

|<span data-ttu-id="f6cce-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="f6cce-109">**Attribute**</span></span>|<span data-ttu-id="f6cce-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="f6cce-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f6cce-111">**ConflictResolution**</span><span class="sxs-lookup"><span data-stu-id="f6cce-111">**ConflictResolution**</span></span> <br/> |<span data-ttu-id="f6cce-112">更新中に試行する競合解決の種類を識別します。</span><span class="sxs-lookup"><span data-stu-id="f6cce-112">Identifies the type of conflict resolution to try during an update.</span></span> <span data-ttu-id="f6cce-113">既定値は自動解決です。</span><span class="sxs-lookup"><span data-stu-id="f6cce-113">The default value is AutoResolve.</span></span>  <br/> |
|<span data-ttu-id="f6cce-114">**MessageDisposition**</span><span class="sxs-lookup"><span data-stu-id="f6cce-114">**MessageDisposition**</span></span> <br/> |<span data-ttu-id="f6cce-115">アイテムが更新された後の処理方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="f6cce-115">Describes how the item will be handled after it is updated.</span></span> <span data-ttu-id="f6cce-116">**MessageDisposition**属性は、会議の取り消し、会議出席依頼、会議の返信などの会議メッセージを含む、メッセージアイテムに必要です。</span><span class="sxs-lookup"><span data-stu-id="f6cce-116">The **MessageDisposition** attribute is required for message items, including meeting messages such as meeting cancellations, meeting requests, and meeting responses.</span></span>  <br/> |
|<span data-ttu-id="f6cce-117">**SendMeetingInvitationsOrCancellations**</span><span class="sxs-lookup"><span data-stu-id="f6cce-117">**SendMeetingInvitationsOrCancellations**</span></span> <br/> |<span data-ttu-id="f6cce-118">予定表アイテムが更新された後に、会議の更新が伝達される方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="f6cce-118">Describes how meeting updates are communicated after a calendar item is updated.</span></span> <span data-ttu-id="f6cce-119">この属性は、予定表アイテムと予定表アイテムの出現に必要です。</span><span class="sxs-lookup"><span data-stu-id="f6cce-119">This attribute is required for calendar items and calendar item occurrences.</span></span>  <br/> |
|<span data-ttu-id="f6cce-120">**SuppressReadReceipts**</span><span class="sxs-lookup"><span data-stu-id="f6cce-120">**SuppressReadReceipts**</span></span> <br/> |<span data-ttu-id="f6cce-121">更新されたアイテムの開封確認を抑制するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f6cce-121">Indicates whether read receipts for the updated item should be suppressed.</span></span> <span data-ttu-id="f6cce-122">テキスト値が**true の場合**、開封確認を抑制する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="f6cce-122">A text value of **true** indicates that read receipts should be suppressed.</span></span> <span data-ttu-id="f6cce-123">値が**false**の場合、開封確認が送信者に送信されることを示します。</span><span class="sxs-lookup"><span data-stu-id="f6cce-123">A value of **false** indicates that the read receipts will be sent to the sender.</span></span> <span data-ttu-id="f6cce-124">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="f6cce-124">This attribute is optional.</span></span>  <br/> <span data-ttu-id="f6cce-125">この属性は、Exchange Server 2013 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f6cce-125">This attribute was introduced in Exchange Server 2013 SP1.</span></span>  <br/> |
   
#### <a name="conflictresolution-attribute"></a><span data-ttu-id="f6cce-126">ConflictResolution 属性</span><span class="sxs-lookup"><span data-stu-id="f6cce-126">ConflictResolution Attribute</span></span>

|<span data-ttu-id="f6cce-127">**値**</span><span class="sxs-lookup"><span data-stu-id="f6cce-127">**Value**</span></span>|<span data-ttu-id="f6cce-128">**説明**</span><span class="sxs-lookup"><span data-stu-id="f6cce-128">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f6cce-129">NeverOverwrite</span><span class="sxs-lookup"><span data-stu-id="f6cce-129">NeverOverwrite</span></span>  <br/> |<span data-ttu-id="f6cce-130">競合がある場合は、更新操作が失敗し、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="f6cce-130">If there is a conflict, the update operation fails and an error is returned.</span></span>  <br/> |
|<span data-ttu-id="f6cce-131">解決</span><span class="sxs-lookup"><span data-stu-id="f6cce-131">AutoResolve</span></span>  <br/> |<span data-ttu-id="f6cce-132">Update 操作は、競合を自動的に解決します。</span><span class="sxs-lookup"><span data-stu-id="f6cce-132">The update operation automatically resolves any conflict.</span></span>  <br/> |
|<span data-ttu-id="f6cce-133">AlwaysOverwrite</span><span class="sxs-lookup"><span data-stu-id="f6cce-133">AlwaysOverwrite</span></span>  <br/> |<span data-ttu-id="f6cce-134">競合がある場合は、更新操作によって情報が上書きされます。</span><span class="sxs-lookup"><span data-stu-id="f6cce-134">If there is a conflict, the update operation will overwrite information.</span></span>  <br/> |
   
#### <a name="messagedisposition-attribute"></a><span data-ttu-id="f6cce-135">MessageDisposition 属性</span><span class="sxs-lookup"><span data-stu-id="f6cce-135">MessageDisposition Attribute</span></span>

|<span data-ttu-id="f6cce-136">**値**</span><span class="sxs-lookup"><span data-stu-id="f6cce-136">**Value**</span></span>|<span data-ttu-id="f6cce-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="f6cce-137">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f6cce-138">SaveOnly</span><span class="sxs-lookup"><span data-stu-id="f6cce-138">SaveOnly</span></span>  <br/> |<span data-ttu-id="f6cce-139">アイテムが更新され、現在のフォルダーに戻されます。</span><span class="sxs-lookup"><span data-stu-id="f6cce-139">The item is updated and saved back to its current folder.</span></span>  <br/> |
|<span data-ttu-id="f6cce-140">SendOnly</span><span class="sxs-lookup"><span data-stu-id="f6cce-140">SendOnly</span></span>  <br/> |<span data-ttu-id="f6cce-141">アイテムは更新されて送信されますが、コピーは保存されません。</span><span class="sxs-lookup"><span data-stu-id="f6cce-141">The item is updated and sent but no copy is saved.</span></span>  <br/> |
|<span data-ttu-id="f6cce-142">SendAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="f6cce-142">SendAndSaveCopy</span></span>  <br/> |<span data-ttu-id="f6cce-143">アイテムが更新され、 [SavedItemFolderId](saveditemfolderid.md)要素によって識別されるフォルダーにコピーが保存されます。</span><span class="sxs-lookup"><span data-stu-id="f6cce-143">The item is updated and a copy is saved in the folder identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a><span data-ttu-id="f6cce-144">SendMeetingInvitationsOrCancellations 属性</span><span class="sxs-lookup"><span data-stu-id="f6cce-144">SendMeetingInvitationsOrCancellations Attribute</span></span>

|<span data-ttu-id="f6cce-145">**値**</span><span class="sxs-lookup"><span data-stu-id="f6cce-145">**Value**</span></span>|<span data-ttu-id="f6cce-146">**説明**</span><span class="sxs-lookup"><span data-stu-id="f6cce-146">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f6cce-147">SendToNone</span><span class="sxs-lookup"><span data-stu-id="f6cce-147">SendToNone</span></span>  <br/> |<span data-ttu-id="f6cce-148">予定表アイテムは更新されますが、更新プログラムは出席者に送信されません。</span><span class="sxs-lookup"><span data-stu-id="f6cce-148">The calendar item is updated but updates are not sent to attendees.</span></span>  <br/> |
|<span data-ttu-id="f6cce-149">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="f6cce-149">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="f6cce-150">予定表アイテムが更新され、会議の更新がすべての出席者に送信されますが、[送信済みアイテム] フォルダーには保存されません。</span><span class="sxs-lookup"><span data-stu-id="f6cce-150">The calendar item is updated and the meeting update is sent to all attendees but is not saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="f6cce-151">SendOnlyToChanged</span><span class="sxs-lookup"><span data-stu-id="f6cce-151">SendOnlyToChanged</span></span>  <br/> |<span data-ttu-id="f6cce-152">予定表アイテムが更新され、会議の変更の影響を受ける出席者にのみ会議の更新が送信されます。</span><span class="sxs-lookup"><span data-stu-id="f6cce-152">The calendar item is updated and the meeting update is sent only to attendees that are affected by the change in the meeting.</span></span>  <br/> |
|<span data-ttu-id="f6cce-153">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="f6cce-153">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="f6cce-154">予定表アイテムが更新されると、会議の更新はすべての出席者に送信され、コピーは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="f6cce-154">The calendar item is updated, the meeting update is sent to all attendees, and a copy is saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="f6cce-155">SendToChangedAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="f6cce-155">SendToChangedAndSaveCopy</span></span>  <br/> |<span data-ttu-id="f6cce-156">予定表アイテムが更新されると、会議の変更の影響を受けるすべての出席者に会議の更新が送信され、[送信済みアイテム] フォルダーにコピーが保存されます。</span><span class="sxs-lookup"><span data-stu-id="f6cce-156">The calendar item is updated, the meeting update is sent to all attendees that are affected by the change in the meeting, and a copy is saved in the Sent Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f6cce-157">子要素</span><span class="sxs-lookup"><span data-stu-id="f6cce-157">Child elements</span></span>

|<span data-ttu-id="f6cce-158">**Element**</span><span class="sxs-lookup"><span data-stu-id="f6cce-158">**Element**</span></span>|<span data-ttu-id="f6cce-159">**説明**</span><span class="sxs-lookup"><span data-stu-id="f6cce-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6cce-160">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="f6cce-160">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="f6cce-161">Exchange ストア内のアイテムを更新、送信、および作成する操作のターゲットフォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="f6cce-161">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6cce-162">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="f6cce-162">ItemChanges</span></span>](itemchanges.md) <br/> |<span data-ttu-id="f6cce-163">アイテムとアイテムに適用する更新を識別する[Itemchange](itemchange.md)要素の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f6cce-163">Contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f6cce-164">親要素</span><span class="sxs-lookup"><span data-stu-id="f6cce-164">Parent elements</span></span>

<span data-ttu-id="f6cce-165">なし。</span><span class="sxs-lookup"><span data-stu-id="f6cce-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f6cce-166">注釈</span><span class="sxs-lookup"><span data-stu-id="f6cce-166">Remarks</span></span>

<span data-ttu-id="f6cce-167">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f6cce-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6cce-168">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f6cce-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6cce-169">Namespace</span><span class="sxs-lookup"><span data-stu-id="f6cce-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f6cce-170">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f6cce-170">Schema Name</span></span>  <br/> |<span data-ttu-id="f6cce-171">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="f6cce-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f6cce-172">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f6cce-172">Validation File</span></span>  <br/> |<span data-ttu-id="f6cce-173">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="f6cce-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f6cce-174">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f6cce-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="f6cce-175">正しくない</span><span class="sxs-lookup"><span data-stu-id="f6cce-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6cce-176">関連項目</span><span class="sxs-lookup"><span data-stu-id="f6cce-176">See also</span></span>



<span data-ttu-id="f6cce-177">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="f6cce-177">[UpdateItem operation](updateitem-operation.md)</span></span>


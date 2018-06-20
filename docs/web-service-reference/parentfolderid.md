---
title: ParentFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 258f4b1f-367e-4c7d-9c29-eb775a2398c7
description: ParentFolderId 要素は、アイテムまたはフォルダーを含む親フォルダーの識別子を表します。
ms.openlocfilehash: 3f60e8adb62fbf464a58af4169fbcd83910877cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832687"
---
# <a name="parentfolderid"></a><span data-ttu-id="76924-103">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="76924-103">ParentFolderId</span></span>

<span data-ttu-id="76924-104">**ParentFolderId**要素は、アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="76924-104">The **ParentFolderId** element represents the identifier of the parent folder that contains the item or folder.</span></span> 
  
```XML
<ParentFolderId Id="" ChangeKey=""/>
```

<span data-ttu-id="76924-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="76924-105">**FolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="76924-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="76924-106">Attributes and elements</span></span>

<span data-ttu-id="76924-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="76924-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76924-108">属性</span><span class="sxs-lookup"><span data-stu-id="76924-108">Attributes</span></span>

|<span data-ttu-id="76924-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="76924-109">**Attribute**</span></span>|<span data-ttu-id="76924-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="76924-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="76924-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="76924-111">**Id**</span></span> <br/> |<span data-ttu-id="76924-112">Exchange ストア内のフォルダーを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="76924-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="76924-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="76924-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="76924-114">**変更キー**</span><span class="sxs-lookup"><span data-stu-id="76924-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="76924-115">**Id**属性によって識別されるフォルダーのバージョンを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="76924-115">Contains a string that identifies a version of a folder that is identified by the **Id** attribute.</span></span> <span data-ttu-id="76924-116">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="76924-116">This attribute is optional.</span></span> <span data-ttu-id="76924-117">フォルダーの正しいバージョンを使用するかどうかを確認するには、この属性を使用します。</span><span class="sxs-lookup"><span data-stu-id="76924-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="76924-118">子要素</span><span class="sxs-lookup"><span data-stu-id="76924-118">Child elements</span></span>

<span data-ttu-id="76924-119">なし。</span><span class="sxs-lookup"><span data-stu-id="76924-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="76924-120">親要素</span><span class="sxs-lookup"><span data-stu-id="76924-120">Parent elements</span></span>

|<span data-ttu-id="76924-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="76924-121">**Element**</span></span>|<span data-ttu-id="76924-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="76924-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76924-123">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="76924-123">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="76924-124">メールボックスの予定表フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-124">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="76924-125">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="76924-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="76924-126">メールボックス内の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-126">Represents a calendar item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="76924-127">Contact</span><span class="sxs-lookup"><span data-stu-id="76924-127">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="76924-128">メールボックス内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-128">Represents a contact item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="76924-129">メッセージ</span><span class="sxs-lookup"><span data-stu-id="76924-129">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="76924-130">メールボックスの連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-130">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="76924-131">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="76924-131">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="76924-132">アイテムまたはフォルダーのコピー先のイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-132">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="76924-133">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="76924-133">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="76924-134">アイテムまたはフォルダーが作成されているイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-134">Represents an event in which an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="76924-135">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="76924-135">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="76924-136">アイテムまたはフォルダーが削除されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-136">Represents an event in which an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="76924-137">DistributionList</span><span class="sxs-lookup"><span data-stu-id="76924-137">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="76924-138">メールボックス内の個人用配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-138">Represents a private distribution list in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="76924-139">Folder</span><span class="sxs-lookup"><span data-stu-id="76924-139">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="76924-140">メールボックス内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-140">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="76924-141">アイテム</span><span class="sxs-lookup"><span data-stu-id="76924-141">Item</span></span>](item.md) <br/> |<span data-ttu-id="76924-142">一般的な Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-142">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="76924-143">項目 (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="76924-143">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="76924-144">メールボックスにアップロードする 1 つの項目を表します。</span><span class="sxs-lookup"><span data-stu-id="76924-144">Represents a single item to upload into a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="76924-145">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="76924-145">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="76924-146">メールボックスで会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="76924-146">Represents a meeting cancellation in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="76924-147">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="76924-147">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="76924-148">メールボックス内の会議のメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-148">Represents a meeting message in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="76924-149">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="76924-149">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="76924-150">メールボックスで会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="76924-150">Represents a meeting request in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="76924-151">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="76924-151">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="76924-152">メールボックスで会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="76924-152">Represents a meeting response in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="76924-153">Message</span><span class="sxs-lookup"><span data-stu-id="76924-153">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="76924-154">メールボックスで電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-154">Represents an e-mail message in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="76924-155">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="76924-155">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="76924-156">アイテムまたはフォルダーが変更されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-156">Represents an event in which an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="76924-157">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="76924-157">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="76924-158">アイテムまたはフォルダーが 1 つの親フォルダー間で移動して別の親フォルダー イベントを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-158">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="76924-159">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="76924-159">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="76924-160">メールボックス内の新しいメール アイテムによって発生するイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-160">Represents an event that is triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="76924-161">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="76924-161">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="76924-162">会議出席依頼、承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="76924-162">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="76924-163">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="76924-163">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="76924-164">仮の予定を表しますが、会議出席依頼に返信します。</span><span class="sxs-lookup"><span data-stu-id="76924-164">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="76924-165">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="76924-165">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="76924-166">会議出席依頼を辞退の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="76924-166">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="76924-167">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="76924-167">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="76924-168">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="76924-168">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="76924-169">タスク</span><span class="sxs-lookup"><span data-stu-id="76924-169">Task</span></span>](task.md) <br/> |<span data-ttu-id="76924-170">メールボックス内の作業項目を表します。</span><span class="sxs-lookup"><span data-stu-id="76924-170">Represents a task item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="76924-171">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="76924-171">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="76924-172">Exchange ストア内のアイテムの作成者に返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="76924-172">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="76924-173">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="76924-173">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="76924-174">Exchange ストア内のアイテムの識別されたすべての受信者への返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="76924-174">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="76924-175">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="76924-175">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="76924-176">受信者に転送するのには、Exchange ストアの項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="76924-176">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="76924-177">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="76924-177">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="76924-178">会議をキャンセルするために使用される応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-178">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="76924-179">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="76924-179">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="76924-180">メールボックス内のタスク フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-180">Represents a task folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="76924-181">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="76924-181">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="76924-182">メールボックス内の検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="76924-182">Represents a search folder in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="76924-183">備考</span><span class="sxs-lookup"><span data-stu-id="76924-183">Remarks</span></span>

<span data-ttu-id="76924-184">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="76924-184">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76924-185">要素情報</span><span class="sxs-lookup"><span data-stu-id="76924-185">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76924-186">名前空間</span><span class="sxs-lookup"><span data-stu-id="76924-186">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="76924-187">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="76924-187">Schema Name</span></span>  <br/> |<span data-ttu-id="76924-188">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="76924-188">Types schema</span></span>  <br/> |
|<span data-ttu-id="76924-189">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="76924-189">Validation File</span></span>  <br/> |<span data-ttu-id="76924-190">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="76924-190">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="76924-191">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="76924-191">Can be Empty</span></span>  <br/> |<span data-ttu-id="76924-192">False</span><span class="sxs-lookup"><span data-stu-id="76924-192">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76924-193">関連項目</span><span class="sxs-lookup"><span data-stu-id="76924-193">See also</span></span>

- [<span data-ttu-id="76924-194">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="76924-194">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


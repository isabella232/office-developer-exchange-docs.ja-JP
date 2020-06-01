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
ms.openlocfilehash: 3bad638aa21019472df8f487f1e065d2e725e750
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465752"
---
# <a name="parentfolderid"></a><span data-ttu-id="3d3aa-103">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="3d3aa-103">ParentFolderId</span></span>

<span data-ttu-id="3d3aa-104">**ParentFolderId**要素は、アイテムまたはフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-104">The **ParentFolderId** element represents the identifier of the parent folder that contains the item or folder.</span></span> 
  
```XML
<ParentFolderId Id="" ChangeKey=""/>
```

<span data-ttu-id="3d3aa-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="3d3aa-105">**FolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3d3aa-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3d3aa-106">Attributes and elements</span></span>

<span data-ttu-id="3d3aa-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3d3aa-108">属性</span><span class="sxs-lookup"><span data-stu-id="3d3aa-108">Attributes</span></span>

|<span data-ttu-id="3d3aa-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="3d3aa-109">**Attribute**</span></span>|<span data-ttu-id="3d3aa-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="3d3aa-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3d3aa-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="3d3aa-111">**Id**</span></span> <br/> |<span data-ttu-id="3d3aa-112">Exchange ストア内のフォルダーを識別する文字列を格納します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="3d3aa-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="3d3aa-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="3d3aa-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="3d3aa-115">**Id**属性によって識別されるフォルダーのバージョンを識別する文字列を格納します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-115">Contains a string that identifies a version of a folder that is identified by the **Id** attribute.</span></span> <span data-ttu-id="3d3aa-116">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-116">This attribute is optional.</span></span> <span data-ttu-id="3d3aa-117">この属性を使用して、適切なバージョンのフォルダーが使用されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3d3aa-118">子要素</span><span class="sxs-lookup"><span data-stu-id="3d3aa-118">Child elements</span></span>

<span data-ttu-id="3d3aa-119">なし。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3d3aa-120">親要素</span><span class="sxs-lookup"><span data-stu-id="3d3aa-120">Parent elements</span></span>

|<span data-ttu-id="3d3aa-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="3d3aa-121">**Element**</span></span>|<span data-ttu-id="3d3aa-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="3d3aa-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3d3aa-123">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="3d3aa-123">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="3d3aa-124">メールボックス内の予定表フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-124">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-125">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="3d3aa-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="3d3aa-126">メールボックス内の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-126">Represents a calendar item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-127">連絡先</span><span class="sxs-lookup"><span data-stu-id="3d3aa-127">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="3d3aa-128">メールボックス内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-128">Represents a contact item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-129">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="3d3aa-129">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="3d3aa-130">メールボックス内の連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-130">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-131">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="3d3aa-131">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="3d3aa-132">アイテムまたはフォルダーがコピーされるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-132">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-133">対する createdevent</span><span class="sxs-lookup"><span data-stu-id="3d3aa-133">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="3d3aa-134">アイテムまたはフォルダーが作成されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-134">Represents an event in which an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-135">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="3d3aa-135">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="3d3aa-136">アイテムまたはフォルダーが削除されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-136">Represents an event in which an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-137">DistributionList</span><span class="sxs-lookup"><span data-stu-id="3d3aa-137">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="3d3aa-138">メールボックス内のプライベート配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-138">Represents a private distribution list in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-139">Folder</span><span class="sxs-lookup"><span data-stu-id="3d3aa-139">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="3d3aa-140">メールボックス内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-140">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-141">アイテム</span><span class="sxs-lookup"><span data-stu-id="3d3aa-141">Item</span></span>](item.md) <br/> |<span data-ttu-id="3d3aa-142">汎用の Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-142">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-143">Item (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="3d3aa-143">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="3d3aa-144">メールボックスにアップロードする単一のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-144">Represents a single item to upload into a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-145">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="3d3aa-145">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="3d3aa-146">メールボックス内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-146">Represents a meeting cancellation in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-147">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="3d3aa-147">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="3d3aa-148">メールボックス内の会議メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-148">Represents a meeting message in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-149">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="3d3aa-149">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="3d3aa-150">メールボックス内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-150">Represents a meeting request in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-151">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="3d3aa-151">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="3d3aa-152">メールボックス内の会議出席依頼の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-152">Represents a meeting response in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-153">Message</span><span class="sxs-lookup"><span data-stu-id="3d3aa-153">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3d3aa-154">メールボックス内の電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-154">Represents an e-mail message in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-155">対する modifiedevent</span><span class="sxs-lookup"><span data-stu-id="3d3aa-155">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="3d3aa-156">アイテムまたはフォルダーが変更されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-156">Represents an event in which an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-157">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="3d3aa-157">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="3d3aa-158">ある親フォルダーから別の親フォルダーにアイテムまたはフォルダーを移動するイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-158">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-159">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="3d3aa-159">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="3d3aa-160">メールボックス内の新しいメールアイテムによってトリガーされるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-160">Represents an event that is triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-161">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="3d3aa-161">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="3d3aa-162">会議出席依頼への返信を承諾するかを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-162">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-163">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="3d3aa-163">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="3d3aa-164">会議出席依頼に対する仮の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-164">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-165">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="3d3aa-165">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="3d3aa-166">会議出席依頼への返信を拒否することを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-166">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-167">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="3d3aa-167">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="3d3aa-168">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-168">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-169">Task</span><span class="sxs-lookup"><span data-stu-id="3d3aa-169">Task</span></span>](task.md) <br/> |<span data-ttu-id="3d3aa-170">メールボックス内のタスクアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-170">Represents a task item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-171">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="3d3aa-171">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="3d3aa-172">Exchange ストア内のアイテムの作成者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-172">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-173">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="3d3aa-173">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="3d3aa-174">Exchange ストア内のアイテムの特定の受信者全員への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-174">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-175">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="3d3aa-175">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="3d3aa-176">受信者に転送するための Exchange ストアアイテムが保存されています。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-176">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-177">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="3d3aa-177">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="3d3aa-178">会議の取り消しに使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-178">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-179">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="3d3aa-179">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="3d3aa-180">メールボックス内のタスクフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-180">Represents a task folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3d3aa-181">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="3d3aa-181">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="3d3aa-182">メールボックス内の検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-182">Represents a search folder in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3d3aa-183">注釈</span><span class="sxs-lookup"><span data-stu-id="3d3aa-183">Remarks</span></span>

<span data-ttu-id="3d3aa-184">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="3d3aa-184">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3d3aa-185">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3d3aa-185">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3d3aa-186">Namespace</span><span class="sxs-lookup"><span data-stu-id="3d3aa-186">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3d3aa-187">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3d3aa-187">Schema Name</span></span>  <br/> |<span data-ttu-id="3d3aa-188">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="3d3aa-188">Types schema</span></span>  <br/> |
|<span data-ttu-id="3d3aa-189">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3d3aa-189">Validation File</span></span>  <br/> |<span data-ttu-id="3d3aa-190">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="3d3aa-190">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3d3aa-191">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3d3aa-191">Can be Empty</span></span>  <br/> |<span data-ttu-id="3d3aa-192">正しくない</span><span class="sxs-lookup"><span data-stu-id="3d3aa-192">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3d3aa-193">関連項目</span><span class="sxs-lookup"><span data-stu-id="3d3aa-193">See also</span></span>

- [<span data-ttu-id="3d3aa-194">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3d3aa-194">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


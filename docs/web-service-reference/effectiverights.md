---
title: EffectiveRights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EffectiveRights
api_type:
- schema
ms.assetid: bf5278eb-3a1a-4d27-9d16-b8be043bb023
description: EffectiveRights 要素には、アイテムまたはフォルダーのアクセス許可の設定に基づいてクライアントの権限が含まれています。 この要素は値の取得のみ可能です。
ms.openlocfilehash: 3055eb73056750508b48ead29136b56e7ce97ee9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459245"
---
# <a name="effectiverights"></a><span data-ttu-id="98bd0-104">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="98bd0-104">EffectiveRights</span></span>

<span data-ttu-id="98bd0-105">**EffectiveRights**要素には、アイテムまたはフォルダーのアクセス許可の設定に基づいてクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="98bd0-105">The **EffectiveRights** element contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="98bd0-106">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="98bd0-106">This element is read-only.</span></span> 
  
```XML
<EffectiveRights>
   <CreateAssociated/>
   <CreateContents/>
   <CreateHierarchy/>
   <Delete/>
   <Modify/>
   <Read/>
   <ViewPrivateItems/>
</EffectiveRights>
```

 <span data-ttu-id="98bd0-107">**EffectiveRightsType**</span><span class="sxs-lookup"><span data-stu-id="98bd0-107">**EffectiveRightsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98bd0-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="98bd0-108">Attributes and elements</span></span>

<span data-ttu-id="98bd0-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98bd0-110">属性</span><span class="sxs-lookup"><span data-stu-id="98bd0-110">Attributes</span></span>

<span data-ttu-id="98bd0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="98bd0-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="98bd0-112">子要素</span><span class="sxs-lookup"><span data-stu-id="98bd0-112">Child elements</span></span>

|<span data-ttu-id="98bd0-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="98bd0-113">**Element**</span></span>|<span data-ttu-id="98bd0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="98bd0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98bd0-115">CreateAssociated</span><span class="sxs-lookup"><span data-stu-id="98bd0-115">CreateAssociated</span></span>](createassociated.md) <br/> |<span data-ttu-id="98bd0-116">クライアントが関連するコンテンツテーブルを作成できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-116">Indicates whether a client can create an associated contents table.</span></span> <span data-ttu-id="98bd0-117">このプロパティは、folder オブジェクトに対してのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="98bd0-117">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-118">CreateContents</span><span class="sxs-lookup"><span data-stu-id="98bd0-118">CreateContents</span></span>](createcontents.md) <br/> |<span data-ttu-id="98bd0-119">クライアントがコンテンツテーブルを作成できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-119">Indicates whether a client can create a contents table.</span></span> <span data-ttu-id="98bd0-120">このプロパティは、folder オブジェクトに対してのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="98bd0-120">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-121">CreateHierarchy</span><span class="sxs-lookup"><span data-stu-id="98bd0-121">CreateHierarchy</span></span>](createhierarchy.md) <br/> |<span data-ttu-id="98bd0-122">クライアントが階層テーブルを作成できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-122">Indicates whether a client can create a hierarchy table.</span></span> <span data-ttu-id="98bd0-123">このプロパティは、folder オブジェクトに対してのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="98bd0-123">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-124">Delete</span><span class="sxs-lookup"><span data-stu-id="98bd0-124">Delete</span></span>](delete.md) <br/> |<span data-ttu-id="98bd0-125">クライアントがフォルダーまたはアイテムを削除できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-125">Indicates whether a client can delete a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-126">Modify</span><span class="sxs-lookup"><span data-stu-id="98bd0-126">Modify</span></span>](modify.md) <br/> |<span data-ttu-id="98bd0-127">クライアントがフォルダーまたはアイテムを変更できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-127">Indicates whether a client can modify a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-128">読み取り</span><span class="sxs-lookup"><span data-stu-id="98bd0-128">Read</span></span>](read.md) <br/> |<span data-ttu-id="98bd0-129">クライアントがフォルダーまたはアイテムを読み取ることができるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-129">Indicates whether a client can read a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-130">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="98bd0-130">ViewPrivateItems</span></span>](viewprivateitems.md) <br/> |<span data-ttu-id="98bd0-131">プライベートアイテムを表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-131">Indicates whether a private item can be viewed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="98bd0-132">親要素</span><span class="sxs-lookup"><span data-stu-id="98bd0-132">Parent elements</span></span>

|<span data-ttu-id="98bd0-133">**要素**</span><span class="sxs-lookup"><span data-stu-id="98bd0-133">**Element**</span></span>|<span data-ttu-id="98bd0-134">**説明**</span><span class="sxs-lookup"><span data-stu-id="98bd0-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98bd0-135">Folder</span><span class="sxs-lookup"><span data-stu-id="98bd0-135">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="98bd0-136">メールボックス内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-136">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-137">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="98bd0-137">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="98bd0-138">メールボックス内のタスクフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-138">Represents a tasks folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-139">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="98bd0-139">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="98bd0-140">メールボックス内の連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-140">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-141">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="98bd0-141">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="98bd0-142">メールボックス内の予定表フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-142">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-143">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="98bd0-143">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="98bd0-144">メールボックス内の検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-144">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-145">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="98bd0-145">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="98bd0-146">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-146">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-147">Contact</span><span class="sxs-lookup"><span data-stu-id="98bd0-147">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="98bd0-148">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-148">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-149">DistributionList</span><span class="sxs-lookup"><span data-stu-id="98bd0-149">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="98bd0-150">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-150">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-151">Item</span><span class="sxs-lookup"><span data-stu-id="98bd0-151">Item</span></span>](item.md) <br/> |<span data-ttu-id="98bd0-152">汎用の Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-152">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-153">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="98bd0-153">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="98bd0-154">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-154">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-155">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="98bd0-155">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="98bd0-156">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-156">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-157">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="98bd0-157">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="98bd0-158">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-158">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-159">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="98bd0-159">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="98bd0-160">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-160">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-161">Message</span><span class="sxs-lookup"><span data-stu-id="98bd0-161">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="98bd0-162">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-162">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-163">タスク</span><span class="sxs-lookup"><span data-stu-id="98bd0-163">Task</span></span>](task.md) <br/> |<span data-ttu-id="98bd0-164">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-164">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="98bd0-165">PostItem</span><span class="sxs-lookup"><span data-stu-id="98bd0-165">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="98bd0-166">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-166">Represents a post item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="98bd0-167">テキスト値</span><span class="sxs-lookup"><span data-stu-id="98bd0-167">Text value</span></span>

<span data-ttu-id="98bd0-168">なし。</span><span class="sxs-lookup"><span data-stu-id="98bd0-168">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="98bd0-169">注釈</span><span class="sxs-lookup"><span data-stu-id="98bd0-169">Remarks</span></span>

<span data-ttu-id="98bd0-170">**EffectiveRights**は、Getfolder、GetItem、Findfolder、FindItem、SyncFolderHierarchy、および Syncfolderhierarchy 応答でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="98bd0-170">**EffectiveRights** is supported in the GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy, and SyncFolderItems responses.</span></span> <span data-ttu-id="98bd0-171">**EffectiveRights**プロパティは、フォルダーとアイテムの**allproperties**図形に公開されます。</span><span class="sxs-lookup"><span data-stu-id="98bd0-171">The **EffectiveRights** property is exposed in the **AllProperties** shape for folders and items.</span></span> 
  
<span data-ttu-id="98bd0-172">この**EffectiveRights**プロパティは、 **PR_ACCESS MAPI**プロパティで提供されるものと同じ情報へのアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="98bd0-172">This **EffectiveRights** property provides access to the same information that is provided in the **PR_ACCESS MAPI** property.</span></span> 
  
<span data-ttu-id="98bd0-173">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="98bd0-173">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="98bd0-174">要素の情報</span><span class="sxs-lookup"><span data-stu-id="98bd0-174">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98bd0-175">Namespace</span><span class="sxs-lookup"><span data-stu-id="98bd0-175">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="98bd0-176">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="98bd0-176">Schema Name</span></span>  <br/> |<span data-ttu-id="98bd0-177">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="98bd0-177">Types schema</span></span>  <br/> |
|<span data-ttu-id="98bd0-178">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="98bd0-178">Validation File</span></span>  <br/> |<span data-ttu-id="98bd0-179">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="98bd0-179">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="98bd0-180">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="98bd0-180">Can be Empty</span></span>  <br/> |<span data-ttu-id="98bd0-181">正しくない</span><span class="sxs-lookup"><span data-stu-id="98bd0-181">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="98bd0-182">関連項目</span><span class="sxs-lookup"><span data-stu-id="98bd0-182">See also</span></span>

- [<span data-ttu-id="98bd0-183">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="98bd0-183">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="98bd0-184">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="98bd0-184">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)


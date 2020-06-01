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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459245"
---
# <a name="effectiverights"></a><span data-ttu-id="2a8c6-104">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="2a8c6-104">EffectiveRights</span></span>

<span data-ttu-id="2a8c6-105">**EffectiveRights**要素には、アイテムまたはフォルダーのアクセス許可の設定に基づいてクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-105">The **EffectiveRights** element contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="2a8c6-106">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-106">This element is read-only.</span></span> 
  
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

 <span data-ttu-id="2a8c6-107">**EffectiveRightsType**</span><span class="sxs-lookup"><span data-stu-id="2a8c6-107">**EffectiveRightsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2a8c6-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2a8c6-108">Attributes and elements</span></span>

<span data-ttu-id="2a8c6-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a8c6-110">属性</span><span class="sxs-lookup"><span data-stu-id="2a8c6-110">Attributes</span></span>

<span data-ttu-id="2a8c6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2a8c6-112">子要素</span><span class="sxs-lookup"><span data-stu-id="2a8c6-112">Child elements</span></span>

|<span data-ttu-id="2a8c6-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="2a8c6-113">**Element**</span></span>|<span data-ttu-id="2a8c6-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="2a8c6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a8c6-115">CreateAssociated</span><span class="sxs-lookup"><span data-stu-id="2a8c6-115">CreateAssociated</span></span>](createassociated.md) <br/> |<span data-ttu-id="2a8c6-116">クライアントが関連するコンテンツテーブルを作成できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-116">Indicates whether a client can create an associated contents table.</span></span> <span data-ttu-id="2a8c6-117">このプロパティは、folder オブジェクトに対してのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-117">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-118">CreateContents</span><span class="sxs-lookup"><span data-stu-id="2a8c6-118">CreateContents</span></span>](createcontents.md) <br/> |<span data-ttu-id="2a8c6-119">クライアントがコンテンツテーブルを作成できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-119">Indicates whether a client can create a contents table.</span></span> <span data-ttu-id="2a8c6-120">このプロパティは、folder オブジェクトに対してのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-120">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-121">CreateHierarchy</span><span class="sxs-lookup"><span data-stu-id="2a8c6-121">CreateHierarchy</span></span>](createhierarchy.md) <br/> |<span data-ttu-id="2a8c6-122">クライアントが階層テーブルを作成できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-122">Indicates whether a client can create a hierarchy table.</span></span> <span data-ttu-id="2a8c6-123">このプロパティは、folder オブジェクトに対してのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-123">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-124">Delete</span><span class="sxs-lookup"><span data-stu-id="2a8c6-124">Delete</span></span>](delete.md) <br/> |<span data-ttu-id="2a8c6-125">クライアントがフォルダーまたはアイテムを削除できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-125">Indicates whether a client can delete a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-126">Modify</span><span class="sxs-lookup"><span data-stu-id="2a8c6-126">Modify</span></span>](modify.md) <br/> |<span data-ttu-id="2a8c6-127">クライアントがフォルダーまたはアイテムを変更できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-127">Indicates whether a client can modify a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-128">読み取り</span><span class="sxs-lookup"><span data-stu-id="2a8c6-128">Read</span></span>](read.md) <br/> |<span data-ttu-id="2a8c6-129">クライアントがフォルダーまたはアイテムを読み取ることができるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-129">Indicates whether a client can read a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-130">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="2a8c6-130">ViewPrivateItems</span></span>](viewprivateitems.md) <br/> |<span data-ttu-id="2a8c6-131">プライベートアイテムを表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-131">Indicates whether a private item can be viewed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2a8c6-132">親要素</span><span class="sxs-lookup"><span data-stu-id="2a8c6-132">Parent elements</span></span>

|<span data-ttu-id="2a8c6-133">**要素**</span><span class="sxs-lookup"><span data-stu-id="2a8c6-133">**Element**</span></span>|<span data-ttu-id="2a8c6-134">**説明**</span><span class="sxs-lookup"><span data-stu-id="2a8c6-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a8c6-135">Folder</span><span class="sxs-lookup"><span data-stu-id="2a8c6-135">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="2a8c6-136">メールボックス内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-136">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-137">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="2a8c6-137">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="2a8c6-138">メールボックス内のタスクフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-138">Represents a tasks folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-139">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="2a8c6-139">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="2a8c6-140">メールボックス内の連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-140">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-141">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="2a8c6-141">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="2a8c6-142">メールボックス内の予定表フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-142">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-143">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="2a8c6-143">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="2a8c6-144">メールボックス内の検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-144">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-145">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="2a8c6-145">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2a8c6-146">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-146">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-147">連絡先</span><span class="sxs-lookup"><span data-stu-id="2a8c6-147">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="2a8c6-148">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-148">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-149">DistributionList</span><span class="sxs-lookup"><span data-stu-id="2a8c6-149">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="2a8c6-150">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-150">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-151">アイテム</span><span class="sxs-lookup"><span data-stu-id="2a8c6-151">Item</span></span>](item.md) <br/> |<span data-ttu-id="2a8c6-152">汎用の Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-152">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-153">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="2a8c6-153">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="2a8c6-154">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-154">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-155">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="2a8c6-155">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="2a8c6-156">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-156">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-157">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="2a8c6-157">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2a8c6-158">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-158">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-159">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="2a8c6-159">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="2a8c6-160">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-160">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-161">Message</span><span class="sxs-lookup"><span data-stu-id="2a8c6-161">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2a8c6-162">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-162">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-163">Task</span><span class="sxs-lookup"><span data-stu-id="2a8c6-163">Task</span></span>](task.md) <br/> |<span data-ttu-id="2a8c6-164">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-164">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2a8c6-165">PostItem</span><span class="sxs-lookup"><span data-stu-id="2a8c6-165">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="2a8c6-166">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-166">Represents a post item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2a8c6-167">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2a8c6-167">Text value</span></span>

<span data-ttu-id="2a8c6-168">なし。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-168">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2a8c6-169">注釈</span><span class="sxs-lookup"><span data-stu-id="2a8c6-169">Remarks</span></span>

<span data-ttu-id="2a8c6-170">**EffectiveRights**は、Getfolder、GetItem、Findfolder、FindItem、SyncFolderHierarchy、および Syncfolderhierarchy 応答でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-170">**EffectiveRights** is supported in the GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy, and SyncFolderItems responses.</span></span> <span data-ttu-id="2a8c6-171">**EffectiveRights**プロパティは、フォルダーとアイテムの**allproperties**図形に公開されます。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-171">The **EffectiveRights** property is exposed in the **AllProperties** shape for folders and items.</span></span> 
  
<span data-ttu-id="2a8c6-172">この**EffectiveRights**プロパティは、 **PR_ACCESS MAPI**プロパティで提供されるものと同じ情報へのアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-172">This **EffectiveRights** property provides access to the same information that is provided in the **PR_ACCESS MAPI** property.</span></span> 
  
<span data-ttu-id="2a8c6-173">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2a8c6-173">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2a8c6-174">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2a8c6-174">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2a8c6-175">Namespace</span><span class="sxs-lookup"><span data-stu-id="2a8c6-175">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2a8c6-176">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2a8c6-176">Schema Name</span></span>  <br/> |<span data-ttu-id="2a8c6-177">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="2a8c6-177">Types schema</span></span>  <br/> |
|<span data-ttu-id="2a8c6-178">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2a8c6-178">Validation File</span></span>  <br/> |<span data-ttu-id="2a8c6-179">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="2a8c6-179">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2a8c6-180">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2a8c6-180">Can be Empty</span></span>  <br/> |<span data-ttu-id="2a8c6-181">正しくない</span><span class="sxs-lookup"><span data-stu-id="2a8c6-181">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2a8c6-182">関連項目</span><span class="sxs-lookup"><span data-stu-id="2a8c6-182">See also</span></span>

- [<span data-ttu-id="2a8c6-183">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2a8c6-183">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="2a8c6-184">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="2a8c6-184">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)


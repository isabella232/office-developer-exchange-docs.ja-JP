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
description: EffectiveRights 要素には、アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。 この要素は、読み取り専用です。
ms.openlocfilehash: 610d9e214a8de648ece667799bb5e67dfcc358f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760204"
---
# <a name="effectiverights"></a><span data-ttu-id="8e857-104">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="8e857-104">EffectiveRights</span></span>

<span data-ttu-id="8e857-105">**EffectiveRights**要素には、アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8e857-105">The **EffectiveRights** element contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="8e857-106">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8e857-106">This element is read-only.</span></span> 
  
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

 <span data-ttu-id="8e857-107">**EffectiveRightsType**</span><span class="sxs-lookup"><span data-stu-id="8e857-107">**EffectiveRightsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8e857-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8e857-108">Attributes and elements</span></span>

<span data-ttu-id="8e857-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8e857-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e857-110">属性</span><span class="sxs-lookup"><span data-stu-id="8e857-110">Attributes</span></span>

<span data-ttu-id="8e857-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8e857-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8e857-112">子要素</span><span class="sxs-lookup"><span data-stu-id="8e857-112">Child elements</span></span>

|<span data-ttu-id="8e857-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8e857-113">**Element**</span></span>|<span data-ttu-id="8e857-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8e857-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e857-115">CreateAssociated</span><span class="sxs-lookup"><span data-stu-id="8e857-115">CreateAssociated</span></span>](createassociated.md) <br/> |<span data-ttu-id="8e857-116">クライアントが、関連付けられている内容のテーブルを作成できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8e857-116">Indicates whether a client can create an associated contents table.</span></span> <span data-ttu-id="8e857-117">Folder オブジェクトに対してこのプロパティは使用のみ。</span><span class="sxs-lookup"><span data-stu-id="8e857-117">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="8e857-118">CreateContents</span><span class="sxs-lookup"><span data-stu-id="8e857-118">CreateContents</span></span>](createcontents.md) <br/> |<span data-ttu-id="8e857-119">クライアントに内容テーブルを作成できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8e857-119">Indicates whether a client can create a contents table.</span></span> <span data-ttu-id="8e857-120">Folder オブジェクトに対してこのプロパティは使用のみ。</span><span class="sxs-lookup"><span data-stu-id="8e857-120">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="8e857-121">CreateHierarchy</span><span class="sxs-lookup"><span data-stu-id="8e857-121">CreateHierarchy</span></span>](createhierarchy.md) <br/> |<span data-ttu-id="8e857-122">クライアントが階層テーブルを作成できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8e857-122">Indicates whether a client can create a hierarchy table.</span></span> <span data-ttu-id="8e857-123">Folder オブジェクトに対してこのプロパティは使用のみ。</span><span class="sxs-lookup"><span data-stu-id="8e857-123">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="8e857-124">Delete</span><span class="sxs-lookup"><span data-stu-id="8e857-124">Delete</span></span>](delete.md) <br/> |<span data-ttu-id="8e857-125">クライアントがフォルダーまたはアイテムを削除できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8e857-125">Indicates whether a client can delete a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="8e857-126">変更</span><span class="sxs-lookup"><span data-stu-id="8e857-126">Modify</span></span>](modify.md) <br/> |<span data-ttu-id="8e857-127">クライアントがフォルダーまたはアイテムを変更できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8e857-127">Indicates whether a client can modify a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="8e857-128">Read</span><span class="sxs-lookup"><span data-stu-id="8e857-128">Read</span></span>](read.md) <br/> |<span data-ttu-id="8e857-129">クライアントがフォルダーまたはアイテムを読み取ることができるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8e857-129">Indicates whether a client can read a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="8e857-130">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="8e857-130">ViewPrivateItems</span></span>](viewprivateitems.md) <br/> |<span data-ttu-id="8e857-131">プライベートなアイテムを表示できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8e857-131">Indicates whether a private item can be viewed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8e857-132">親要素</span><span class="sxs-lookup"><span data-stu-id="8e857-132">Parent elements</span></span>

|<span data-ttu-id="8e857-133">**要素**</span><span class="sxs-lookup"><span data-stu-id="8e857-133">**Element**</span></span>|<span data-ttu-id="8e857-134">**説明**</span><span class="sxs-lookup"><span data-stu-id="8e857-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e857-135">Folder</span><span class="sxs-lookup"><span data-stu-id="8e857-135">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="8e857-136">メールボックス内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="8e857-136">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8e857-137">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="8e857-137">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="8e857-138">メールボックス内のタスク フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="8e857-138">Represents a tasks folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8e857-139">メッセージ</span><span class="sxs-lookup"><span data-stu-id="8e857-139">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="8e857-140">メールボックスの連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="8e857-140">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8e857-141">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="8e857-141">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="8e857-142">メールボックスの予定表フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="8e857-142">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8e857-143">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="8e857-143">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="8e857-144">メールボックス内の検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="8e857-144">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8e857-145">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="8e857-145">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="8e857-146">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="8e857-146">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8e857-147">Contact</span><span class="sxs-lookup"><span data-stu-id="8e857-147">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="8e857-148">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="8e857-148">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="8e857-149">DistributionList</span><span class="sxs-lookup"><span data-stu-id="8e857-149">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="8e857-150">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="8e857-150">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="8e857-151">アイテム</span><span class="sxs-lookup"><span data-stu-id="8e857-151">Item</span></span>](item.md) <br/> |<span data-ttu-id="8e857-152">一般的な Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="8e857-152">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="8e857-153">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="8e857-153">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="8e857-154">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="8e857-154">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8e857-155">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="8e857-155">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="8e857-156">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="8e857-156">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8e857-157">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="8e857-157">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="8e857-158">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="8e857-158">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8e857-159">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="8e857-159">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="8e857-160">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="8e857-160">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8e857-161">Message</span><span class="sxs-lookup"><span data-stu-id="8e857-161">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8e857-162">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="8e857-162">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="8e857-163">タスク</span><span class="sxs-lookup"><span data-stu-id="8e857-163">Task</span></span>](task.md) <br/> |<span data-ttu-id="8e857-164">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="8e857-164">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8e857-165">PostItem</span><span class="sxs-lookup"><span data-stu-id="8e857-165">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="8e857-166">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="8e857-166">Represents a post item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8e857-167">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8e857-167">Text value</span></span>

<span data-ttu-id="8e857-168">なし。</span><span class="sxs-lookup"><span data-stu-id="8e857-168">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8e857-169">備考</span><span class="sxs-lookup"><span data-stu-id="8e857-169">Remarks</span></span>

<span data-ttu-id="8e857-170">**EffectiveRights**は、GetFolder、GetItem、FindFolder、FindItem、SyncFolderHierarchy、および SyncFolderItems の応答でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="8e857-170">**EffectiveRights** is supported in the GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy, and SyncFolderItems responses.</span></span> <span data-ttu-id="8e857-171">**EffectiveRights**プロパティは、フォルダーおよびアイテムの [ **AllProperties** ] 図形内に公開されます。</span><span class="sxs-lookup"><span data-stu-id="8e857-171">The **EffectiveRights** property is exposed in the **AllProperties** shape for folders and items.</span></span> 
  
<span data-ttu-id="8e857-172">この**EffectiveRights**プロパティは、 **MAPI の PR_ACCESS**プロパティで提供されている同じ情報へのアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="8e857-172">This **EffectiveRights** property provides access to the same information that is provided in the **PR_ACCESS MAPI** property.</span></span> 
  
<span data-ttu-id="8e857-173">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8e857-173">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e857-174">要素情報</span><span class="sxs-lookup"><span data-stu-id="8e857-174">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e857-175">名前空間</span><span class="sxs-lookup"><span data-stu-id="8e857-175">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8e857-176">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8e857-176">Schema Name</span></span>  <br/> |<span data-ttu-id="8e857-177">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8e857-177">Types schema</span></span>  <br/> |
|<span data-ttu-id="8e857-178">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8e857-178">Validation File</span></span>  <br/> |<span data-ttu-id="8e857-179">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8e857-179">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8e857-180">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8e857-180">Can be Empty</span></span>  <br/> |<span data-ttu-id="8e857-181">False</span><span class="sxs-lookup"><span data-stu-id="8e857-181">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8e857-182">関連項目</span><span class="sxs-lookup"><span data-stu-id="8e857-182">See also</span></span>

- [<span data-ttu-id="8e857-183">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8e857-183">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="8e857-184">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="8e857-184">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)


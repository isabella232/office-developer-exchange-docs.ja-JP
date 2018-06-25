---
title: フォルダー Id
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderId
api_type:
- schema
ms.assetid: 00d14e3e-4365-4f21-8f88-eaeea73b9bf7
description: フォルダー Id 要素には、フォルダーの識別子と変更キーが含まれています。
ms.openlocfilehash: 5764a164d5af183b8f313955ace5274dc6023a6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760567"
---
# <a name="folderid"></a><span data-ttu-id="536a5-103">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="536a5-103">FolderId</span></span>

<span data-ttu-id="536a5-104">**フォルダー Id**要素には、フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="536a5-104">The **FolderId** element contains the identifier and change key of a folder.</span></span> 
  
```XML
<FolderId Id="" ChangeKey="" />
```

 <span data-ttu-id="536a5-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="536a5-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="536a5-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="536a5-106">Attributes and elements</span></span>

<span data-ttu-id="536a5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="536a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="536a5-108">属性</span><span class="sxs-lookup"><span data-stu-id="536a5-108">Attributes</span></span>

|<span data-ttu-id="536a5-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="536a5-109">**Attribute**</span></span>|<span data-ttu-id="536a5-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="536a5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="536a5-111">ID</span><span class="sxs-lookup"><span data-stu-id="536a5-111">Id</span></span>  <br/> |<span data-ttu-id="536a5-112">Exchange ストア内のフォルダーを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="536a5-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="536a5-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="536a5-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="536a5-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="536a5-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="536a5-115">Id 属性によって識別されるフォルダーのバージョンを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="536a5-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="536a5-116">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="536a5-116">This attribute is optional.</span></span> <span data-ttu-id="536a5-117">フォルダーの正しいバージョンを使用するかどうかを確認するには、この属性を使用します。</span><span class="sxs-lookup"><span data-stu-id="536a5-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="536a5-118">子要素</span><span class="sxs-lookup"><span data-stu-id="536a5-118">Child elements</span></span>

<span data-ttu-id="536a5-119">なし。</span><span class="sxs-lookup"><span data-stu-id="536a5-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="536a5-120">親要素</span><span class="sxs-lookup"><span data-stu-id="536a5-120">Parent elements</span></span>

|<span data-ttu-id="536a5-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="536a5-121">**Element**</span></span>|<span data-ttu-id="536a5-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="536a5-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="536a5-123">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="536a5-123">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="536a5-124">フォルダーを使用する操作を対象としているフォルダーを示します。</span><span class="sxs-lookup"><span data-stu-id="536a5-124">Indicates the folder that is targeted for actions that use folders.</span></span>  <br/> |
|[<span data-ttu-id="536a5-125">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="536a5-125">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="536a5-126">アイテムまたはフォルダーのコピー先のイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="536a5-126">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="536a5-127">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="536a5-127">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="536a5-128">コピー先のフォルダーを指定し、アクションを移動します。</span><span class="sxs-lookup"><span data-stu-id="536a5-128">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="536a5-129">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="536a5-129">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> | <span data-ttu-id="536a5-130">新しいフォルダーまたはアイテムを作成するフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="536a5-130">Identifies the folder where a new folder or item is created.</span></span>  <br/><br/>  <span data-ttu-id="536a5-131">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="536a5-131">The following are the XPath expressions to this element:</span></span><br/>  <br/> `/CreateItem/ParentFolderId` <br/><br/>  `/CreateFolder/ParentFolderId` <br/> |
|[<span data-ttu-id="536a5-132">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="536a5-132">BaseFolderIds</span></span>](basefolderids.md) <br/> |<span data-ttu-id="536a5-133">検索フォルダーの内容を判断するためにマイニングするフォルダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="536a5-133">Represents the collection of folders that will be mined to determine the contents of a search folder.</span></span>  <br/> |
|[<span data-ttu-id="536a5-134">(集合的) を削除します。</span><span class="sxs-lookup"><span data-stu-id="536a5-134">Delete (FolderSync)</span></span>](delete-foldersync.md) <br/> |<span data-ttu-id="536a5-135">ローカル クライアント ストアで削除するのには 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="536a5-135">Identifies a single folder to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="536a5-136">Folder</span><span class="sxs-lookup"><span data-stu-id="536a5-136">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="536a5-137">メールボックス内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="536a5-137">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="536a5-138">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="536a5-138">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="536a5-139">メールボックスの予定表フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="536a5-139">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="536a5-140">FolderChange</span><span class="sxs-lookup"><span data-stu-id="536a5-140">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="536a5-141">1 つのフォルダーで実行される変更のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="536a5-141">Represents a collection of changes to be performed on a single folder.</span></span>  <br/> <span data-ttu-id="536a5-142">この要素への XPath 式は、次のようにします。`/UpdateFolder/FolderChanges/FolderChange`</span><span class="sxs-lookup"><span data-stu-id="536a5-142">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange`</span></span> <br/> |
|[<span data-ttu-id="536a5-143">メッセージ</span><span class="sxs-lookup"><span data-stu-id="536a5-143">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="536a5-144">メールボックスの連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="536a5-144">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="536a5-145">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="536a5-145">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="536a5-146">メールボックス内の検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="536a5-146">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="536a5-147">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="536a5-147">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="536a5-148">メールボックス内のタスク フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="536a5-148">Represents a task folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="536a5-149">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="536a5-149">ToFolderId</span></span>](tofolderid.md) <br/> | <span data-ttu-id="536a5-150">先のフォルダーにコピーまたは移動されたアイテムまたはフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="536a5-150">Represents the destination folder for a copied or moved item or folder.</span></span> <br/> <br/>  <span data-ttu-id="536a5-151">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="536a5-151">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/MoveFolder/ToFolderId` <br/> <br/> `/CopyFolder/ToFolderId` <br/> <br/> `/MoveItem/ToFolderId`<br/> <br/>  `/CopyItem/ToFolderId` <br/> |
|[<span data-ttu-id="536a5-152">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="536a5-152">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> | <span data-ttu-id="536a5-153">更新、送信、および Exchange ストア内の項目を作成する操作のターゲット フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="536a5-153">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/><br/>  <span data-ttu-id="536a5-154">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="536a5-154">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/CreateItem/SavedItemFolderId` <br/><br/>  `/UpdateItem/SavedItemFolderId` <br/><br/>  `/SendItem/SavedItemFolderId` <br/> |
|[<span data-ttu-id="536a5-155">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="536a5-155">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="536a5-156">同期する項目を含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="536a5-156">Represents the folder that contains the items to synchronize.</span></span>  <br/> |
|[<span data-ttu-id="536a5-157">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="536a5-157">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="536a5-158">ユーザーの構成オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="536a5-158">Represents the name of a user configuration object.</span></span> <span data-ttu-id="536a5-159">ユーザーの構成オブジェクトの名前は、ユーザーの構成オブジェクトの識別子です。</span><span class="sxs-lookup"><span data-stu-id="536a5-159">The user configuration object name is the identifier for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="536a5-160">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="536a5-160">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="536a5-161">電子メール アイテムをコピーするフォルダーの ID を識別します。</span><span class="sxs-lookup"><span data-stu-id="536a5-161">Identifies the ID of the folder that e-mail items will be copied to.</span></span>  <br/> |
|[<span data-ttu-id="536a5-162">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="536a5-162">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="536a5-163">電子メール アイテムに移動するフォルダーの ID を識別します。</span><span class="sxs-lookup"><span data-stu-id="536a5-163">Identifies the ID of the folder that e-mail items will be moved to.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="536a5-164">テキスト値</span><span class="sxs-lookup"><span data-stu-id="536a5-164">Text value</span></span>

<span data-ttu-id="536a5-165">なし。</span><span class="sxs-lookup"><span data-stu-id="536a5-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="536a5-166">備考</span><span class="sxs-lookup"><span data-stu-id="536a5-166">Remarks</span></span>

<span data-ttu-id="536a5-167">**フォルダー Id**のすべての要素は、 **FolderIdType**タイプです。</span><span class="sxs-lookup"><span data-stu-id="536a5-167">All **FolderId** elements are of the **FolderIdType** type.</span></span> <span data-ttu-id="536a5-168">**BaseFolderType**を拡張する型を持つ要素を除くすべての場合に**フォルダー Id**の要素が必要か、**フォルダー Id**要素は、選択肢の一部です。</span><span class="sxs-lookup"><span data-stu-id="536a5-168">The **FolderId** element is required in every case except in elements whose type extends the **BaseFolderType** or where the **FolderId** element is a part of a choice.</span></span> <span data-ttu-id="536a5-169">詳細についてはスキーマを参照してください。</span><span class="sxs-lookup"><span data-stu-id="536a5-169">Review the schema for more information.</span></span> 
  
<span data-ttu-id="536a5-170">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="536a5-170">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="536a5-171">要素情報</span><span class="sxs-lookup"><span data-stu-id="536a5-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="536a5-172">名前空間</span><span class="sxs-lookup"><span data-stu-id="536a5-172">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="536a5-173">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="536a5-173">Schema Name</span></span>  <br/> |<span data-ttu-id="536a5-174">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="536a5-174">Types schema</span></span>  <br/> |
|<span data-ttu-id="536a5-175">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="536a5-175">Validation File</span></span>  <br/> |<span data-ttu-id="536a5-176">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="536a5-176">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="536a5-177">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="536a5-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="536a5-178">False</span><span class="sxs-lookup"><span data-stu-id="536a5-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="536a5-179">関連項目</span><span class="sxs-lookup"><span data-stu-id="536a5-179">See also</span></span>

- [<span data-ttu-id="536a5-180">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="536a5-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="536a5-181">フォルダー (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="536a5-181">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)


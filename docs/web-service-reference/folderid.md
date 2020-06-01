---
title: FolderId
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
description: FolderId 要素には、フォルダーの識別子と変更キーが含まれています。
ms.openlocfilehash: 7aa5070fa7a2c51303c7159de04fe277f909a874
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461388"
---
# <a name="folderid"></a><span data-ttu-id="41aed-103">FolderId</span><span class="sxs-lookup"><span data-stu-id="41aed-103">FolderId</span></span>

<span data-ttu-id="41aed-104">**FolderId**要素には、フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="41aed-104">The **FolderId** element contains the identifier and change key of a folder.</span></span> 
  
```XML
<FolderId Id="" ChangeKey="" />
```

 <span data-ttu-id="41aed-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="41aed-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="41aed-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="41aed-106">Attributes and elements</span></span>

<span data-ttu-id="41aed-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="41aed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41aed-108">属性</span><span class="sxs-lookup"><span data-stu-id="41aed-108">Attributes</span></span>

|<span data-ttu-id="41aed-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="41aed-109">**Attribute**</span></span>|<span data-ttu-id="41aed-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="41aed-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="41aed-111">ID</span><span class="sxs-lookup"><span data-stu-id="41aed-111">Id</span></span>  <br/> |<span data-ttu-id="41aed-112">Exchange ストア内のフォルダーを識別する文字列を格納します。</span><span class="sxs-lookup"><span data-stu-id="41aed-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="41aed-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="41aed-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="41aed-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="41aed-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="41aed-115">Id 属性によって識別されるフォルダーのバージョンを識別する文字列を格納します。</span><span class="sxs-lookup"><span data-stu-id="41aed-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="41aed-116">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="41aed-116">This attribute is optional.</span></span> <span data-ttu-id="41aed-117">この属性を使用して、適切なバージョンのフォルダーが使用されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="41aed-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="41aed-118">子要素</span><span class="sxs-lookup"><span data-stu-id="41aed-118">Child elements</span></span>

<span data-ttu-id="41aed-119">なし。</span><span class="sxs-lookup"><span data-stu-id="41aed-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="41aed-120">親要素</span><span class="sxs-lookup"><span data-stu-id="41aed-120">Parent elements</span></span>

|<span data-ttu-id="41aed-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="41aed-121">**Element**</span></span>|<span data-ttu-id="41aed-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="41aed-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41aed-123">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="41aed-123">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="41aed-124">フォルダーを使用する操作を対象とするフォルダーを示します。</span><span class="sxs-lookup"><span data-stu-id="41aed-124">Indicates the folder that is targeted for actions that use folders.</span></span>  <br/> |
|[<span data-ttu-id="41aed-125">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="41aed-125">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="41aed-126">アイテムまたはフォルダーがコピーされるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="41aed-126">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="41aed-127">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="41aed-127">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="41aed-128">コピー操作と移動操作の宛先フォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="41aed-128">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="41aed-129">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="41aed-129">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> | <span data-ttu-id="41aed-130">新しいフォルダーまたはアイテムを作成するフォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="41aed-130">Identifies the folder where a new folder or item is created.</span></span>  <br/><br/>  <span data-ttu-id="41aed-131">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="41aed-131">The following are the XPath expressions to this element:</span></span><br/>  <br/> `/CreateItem/ParentFolderId` <br/><br/>  `/CreateFolder/ParentFolderId` <br/> |
|[<span data-ttu-id="41aed-132">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="41aed-132">BaseFolderIds</span></span>](basefolderids.md) <br/> |<span data-ttu-id="41aed-133">検索フォルダーのコンテンツを特定するためにマイニングされるフォルダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="41aed-133">Represents the collection of folders that will be mined to determine the contents of a search folder.</span></span>  <br/> |
|[<span data-ttu-id="41aed-134">Delete (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="41aed-134">Delete (FolderSync)</span></span>](delete-foldersync.md) <br/> |<span data-ttu-id="41aed-135">ローカルクライアントストアで削除する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="41aed-135">Identifies a single folder to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="41aed-136">Folder</span><span class="sxs-lookup"><span data-stu-id="41aed-136">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="41aed-137">メールボックス内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="41aed-137">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="41aed-138">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="41aed-138">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="41aed-139">メールボックス内の予定表フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="41aed-139">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="41aed-140">FolderChange</span><span class="sxs-lookup"><span data-stu-id="41aed-140">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="41aed-141">1つのフォルダーに対して実行される変更のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="41aed-141">Represents a collection of changes to be performed on a single folder.</span></span>  <br/> <span data-ttu-id="41aed-142">この要素の XPath 式を次に示します。`/UpdateFolder/FolderChanges/FolderChange`</span><span class="sxs-lookup"><span data-stu-id="41aed-142">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange`</span></span> <br/> |
|[<span data-ttu-id="41aed-143">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="41aed-143">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="41aed-144">メールボックス内の連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="41aed-144">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="41aed-145">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="41aed-145">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="41aed-146">メールボックス内の検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="41aed-146">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="41aed-147">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="41aed-147">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="41aed-148">メールボックス内のタスクフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="41aed-148">Represents a task folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="41aed-149">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="41aed-149">ToFolderId</span></span>](tofolderid.md) <br/> | <span data-ttu-id="41aed-150">コピーまたは移動されたアイテムまたはフォルダーの移動先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="41aed-150">Represents the destination folder for a copied or moved item or folder.</span></span> <br/> <br/>  <span data-ttu-id="41aed-151">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="41aed-151">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/MoveFolder/ToFolderId` <br/> <br/> `/CopyFolder/ToFolderId` <br/> <br/> `/MoveItem/ToFolderId`<br/> <br/>  `/CopyItem/ToFolderId` <br/> |
|[<span data-ttu-id="41aed-152">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="41aed-152">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> | <span data-ttu-id="41aed-153">Exchange ストア内のアイテムを更新、送信、および作成する操作のターゲットフォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="41aed-153">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/><br/>  <span data-ttu-id="41aed-154">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="41aed-154">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/CreateItem/SavedItemFolderId` <br/><br/>  `/UpdateItem/SavedItemFolderId` <br/><br/>  `/SendItem/SavedItemFolderId` <br/> |
|[<span data-ttu-id="41aed-155">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="41aed-155">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="41aed-156">同期するアイテムを含むフォルダを表します。</span><span class="sxs-lookup"><span data-stu-id="41aed-156">Represents the folder that contains the items to synchronize.</span></span>  <br/> |
|[<span data-ttu-id="41aed-157">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="41aed-157">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="41aed-158">ユーザー構成オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="41aed-158">Represents the name of a user configuration object.</span></span> <span data-ttu-id="41aed-159">ユーザー構成オブジェクトの名前は、ユーザー構成オブジェクトの識別子です。</span><span class="sxs-lookup"><span data-stu-id="41aed-159">The user configuration object name is the identifier for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="41aed-160">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="41aed-160">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="41aed-161">電子メールアイテムがコピーされるフォルダーの ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="41aed-161">Identifies the ID of the folder that e-mail items will be copied to.</span></span>  <br/> |
|[<span data-ttu-id="41aed-162">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="41aed-162">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="41aed-163">電子メールアイテムの移動先フォルダーの ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="41aed-163">Identifies the ID of the folder that e-mail items will be moved to.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="41aed-164">テキスト値</span><span class="sxs-lookup"><span data-stu-id="41aed-164">Text value</span></span>

<span data-ttu-id="41aed-165">なし。</span><span class="sxs-lookup"><span data-stu-id="41aed-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="41aed-166">注釈</span><span class="sxs-lookup"><span data-stu-id="41aed-166">Remarks</span></span>

<span data-ttu-id="41aed-167">すべての**FolderId**要素は、 **folderidtype**型です。</span><span class="sxs-lookup"><span data-stu-id="41aed-167">All **FolderId** elements are of the **FolderIdType** type.</span></span> <span data-ttu-id="41aed-168">**FolderId**要素は、すべての場合に必要です。ただし、Type が**basefoldertype**を拡張する要素、または**FolderId**要素が選択範囲の一部である場合を除きます。</span><span class="sxs-lookup"><span data-stu-id="41aed-168">The **FolderId** element is required in every case except in elements whose type extends the **BaseFolderType** or where the **FolderId** element is a part of a choice.</span></span> <span data-ttu-id="41aed-169">詳細については、「スキーマ」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41aed-169">Review the schema for more information.</span></span> 
  
<span data-ttu-id="41aed-170">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="41aed-170">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="41aed-171">要素の情報</span><span class="sxs-lookup"><span data-stu-id="41aed-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41aed-172">Namespace</span><span class="sxs-lookup"><span data-stu-id="41aed-172">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="41aed-173">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="41aed-173">Schema Name</span></span>  <br/> |<span data-ttu-id="41aed-174">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="41aed-174">Types schema</span></span>  <br/> |
|<span data-ttu-id="41aed-175">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="41aed-175">Validation File</span></span>  <br/> |<span data-ttu-id="41aed-176">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="41aed-176">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="41aed-177">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="41aed-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="41aed-178">正しくない</span><span class="sxs-lookup"><span data-stu-id="41aed-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="41aed-179">関連項目</span><span class="sxs-lookup"><span data-stu-id="41aed-179">See also</span></span>

- [<span data-ttu-id="41aed-180">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="41aed-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="41aed-181">フォルダーの作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="41aed-181">Creating Folders (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)


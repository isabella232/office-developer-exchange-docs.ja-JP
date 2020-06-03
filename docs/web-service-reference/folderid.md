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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461388"
---
# <a name="folderid"></a><span data-ttu-id="06dd1-103">FolderId</span><span class="sxs-lookup"><span data-stu-id="06dd1-103">FolderId</span></span>

<span data-ttu-id="06dd1-104">**FolderId**要素には、フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="06dd1-104">The **FolderId** element contains the identifier and change key of a folder.</span></span> 
  
```XML
<FolderId Id="" ChangeKey="" />
```

 <span data-ttu-id="06dd1-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="06dd1-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06dd1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="06dd1-106">Attributes and elements</span></span>

<span data-ttu-id="06dd1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06dd1-108">属性</span><span class="sxs-lookup"><span data-stu-id="06dd1-108">Attributes</span></span>

|<span data-ttu-id="06dd1-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="06dd1-109">**Attribute**</span></span>|<span data-ttu-id="06dd1-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="06dd1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="06dd1-111">ID</span><span class="sxs-lookup"><span data-stu-id="06dd1-111">Id</span></span>  <br/> |<span data-ttu-id="06dd1-112">Exchange ストア内のフォルダーを識別する文字列を格納します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="06dd1-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="06dd1-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="06dd1-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="06dd1-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="06dd1-115">Id 属性によって識別されるフォルダーのバージョンを識別する文字列を格納します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="06dd1-116">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="06dd1-116">This attribute is optional.</span></span> <span data-ttu-id="06dd1-117">この属性を使用して、適切なバージョンのフォルダーが使用されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="06dd1-118">子要素</span><span class="sxs-lookup"><span data-stu-id="06dd1-118">Child elements</span></span>

<span data-ttu-id="06dd1-119">なし。</span><span class="sxs-lookup"><span data-stu-id="06dd1-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="06dd1-120">親要素</span><span class="sxs-lookup"><span data-stu-id="06dd1-120">Parent elements</span></span>

|<span data-ttu-id="06dd1-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="06dd1-121">**Element**</span></span>|<span data-ttu-id="06dd1-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="06dd1-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06dd1-123">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="06dd1-123">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="06dd1-124">フォルダーを使用する操作を対象とするフォルダーを示します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-124">Indicates the folder that is targeted for actions that use folders.</span></span>  <br/> |
|[<span data-ttu-id="06dd1-125">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="06dd1-125">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="06dd1-126">アイテムまたはフォルダーがコピーされるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-126">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="06dd1-127">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="06dd1-127">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="06dd1-128">コピー操作と移動操作の宛先フォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-128">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="06dd1-129">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="06dd1-129">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> | <span data-ttu-id="06dd1-130">新しいフォルダーまたはアイテムを作成するフォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-130">Identifies the folder where a new folder or item is created.</span></span>  <br/><br/>  <span data-ttu-id="06dd1-131">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="06dd1-131">The following are the XPath expressions to this element:</span></span><br/>  <br/> `/CreateItem/ParentFolderId` <br/><br/>  `/CreateFolder/ParentFolderId` <br/> |
|[<span data-ttu-id="06dd1-132">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="06dd1-132">BaseFolderIds</span></span>](basefolderids.md) <br/> |<span data-ttu-id="06dd1-133">検索フォルダーのコンテンツを特定するためにマイニングされるフォルダーのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-133">Represents the collection of folders that will be mined to determine the contents of a search folder.</span></span>  <br/> |
|[<span data-ttu-id="06dd1-134">Delete (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="06dd1-134">Delete (FolderSync)</span></span>](delete-foldersync.md) <br/> |<span data-ttu-id="06dd1-135">ローカルクライアントストアで削除する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-135">Identifies a single folder to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="06dd1-136">Folder</span><span class="sxs-lookup"><span data-stu-id="06dd1-136">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="06dd1-137">メールボックス内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-137">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="06dd1-138">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="06dd1-138">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="06dd1-139">メールボックス内の予定表フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-139">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="06dd1-140">FolderChange</span><span class="sxs-lookup"><span data-stu-id="06dd1-140">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="06dd1-141">1つのフォルダーに対して実行される変更のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-141">Represents a collection of changes to be performed on a single folder.</span></span>  <br/> <span data-ttu-id="06dd1-142">この要素の XPath 式を次に示します。`/UpdateFolder/FolderChanges/FolderChange`</span><span class="sxs-lookup"><span data-stu-id="06dd1-142">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange`</span></span> <br/> |
|[<span data-ttu-id="06dd1-143">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="06dd1-143">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="06dd1-144">メールボックス内の連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-144">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="06dd1-145">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="06dd1-145">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="06dd1-146">メールボックス内の検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-146">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="06dd1-147">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="06dd1-147">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="06dd1-148">メールボックス内のタスクフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-148">Represents a task folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="06dd1-149">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="06dd1-149">ToFolderId</span></span>](tofolderid.md) <br/> | <span data-ttu-id="06dd1-150">コピーまたは移動されたアイテムまたはフォルダーの移動先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-150">Represents the destination folder for a copied or moved item or folder.</span></span> <br/> <br/>  <span data-ttu-id="06dd1-151">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="06dd1-151">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/MoveFolder/ToFolderId` <br/> <br/> `/CopyFolder/ToFolderId` <br/> <br/> `/MoveItem/ToFolderId`<br/> <br/>  `/CopyItem/ToFolderId` <br/> |
|[<span data-ttu-id="06dd1-152">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="06dd1-152">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> | <span data-ttu-id="06dd1-153">Exchange ストア内のアイテムを更新、送信、および作成する操作のターゲットフォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-153">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/><br/>  <span data-ttu-id="06dd1-154">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="06dd1-154">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/CreateItem/SavedItemFolderId` <br/><br/>  `/UpdateItem/SavedItemFolderId` <br/><br/>  `/SendItem/SavedItemFolderId` <br/> |
|[<span data-ttu-id="06dd1-155">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="06dd1-155">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="06dd1-156">同期するアイテムを含むフォルダを表します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-156">Represents the folder that contains the items to synchronize.</span></span>  <br/> |
|[<span data-ttu-id="06dd1-157">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="06dd1-157">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="06dd1-158">ユーザー構成オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-158">Represents the name of a user configuration object.</span></span> <span data-ttu-id="06dd1-159">ユーザー構成オブジェクトの名前は、ユーザー構成オブジェクトの識別子です。</span><span class="sxs-lookup"><span data-stu-id="06dd1-159">The user configuration object name is the identifier for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="06dd1-160">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="06dd1-160">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="06dd1-161">電子メールアイテムがコピーされるフォルダーの ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-161">Identifies the ID of the folder that e-mail items will be copied to.</span></span>  <br/> |
|[<span data-ttu-id="06dd1-162">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="06dd1-162">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="06dd1-163">電子メールアイテムの移動先フォルダーの ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="06dd1-163">Identifies the ID of the folder that e-mail items will be moved to.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="06dd1-164">テキスト値</span><span class="sxs-lookup"><span data-stu-id="06dd1-164">Text value</span></span>

<span data-ttu-id="06dd1-165">なし。</span><span class="sxs-lookup"><span data-stu-id="06dd1-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="06dd1-166">注釈</span><span class="sxs-lookup"><span data-stu-id="06dd1-166">Remarks</span></span>

<span data-ttu-id="06dd1-167">すべての**FolderId**要素は、 **folderidtype**型です。</span><span class="sxs-lookup"><span data-stu-id="06dd1-167">All **FolderId** elements are of the **FolderIdType** type.</span></span> <span data-ttu-id="06dd1-168">**FolderId**要素は、すべての場合に必要です。ただし、Type が**basefoldertype**を拡張する要素、または**FolderId**要素が選択範囲の一部である場合を除きます。</span><span class="sxs-lookup"><span data-stu-id="06dd1-168">The **FolderId** element is required in every case except in elements whose type extends the **BaseFolderType** or where the **FolderId** element is a part of a choice.</span></span> <span data-ttu-id="06dd1-169">詳細については、「スキーマ」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06dd1-169">Review the schema for more information.</span></span> 
  
<span data-ttu-id="06dd1-170">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="06dd1-170">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06dd1-171">要素の情報</span><span class="sxs-lookup"><span data-stu-id="06dd1-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06dd1-172">Namespace</span><span class="sxs-lookup"><span data-stu-id="06dd1-172">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="06dd1-173">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="06dd1-173">Schema Name</span></span>  <br/> |<span data-ttu-id="06dd1-174">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="06dd1-174">Types schema</span></span>  <br/> |
|<span data-ttu-id="06dd1-175">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="06dd1-175">Validation File</span></span>  <br/> |<span data-ttu-id="06dd1-176">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="06dd1-176">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="06dd1-177">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="06dd1-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="06dd1-178">正しくない</span><span class="sxs-lookup"><span data-stu-id="06dd1-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06dd1-179">関連項目</span><span class="sxs-lookup"><span data-stu-id="06dd1-179">See also</span></span>

- [<span data-ttu-id="06dd1-180">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="06dd1-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="06dd1-181">フォルダーの作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="06dd1-181">Creating Folders (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)


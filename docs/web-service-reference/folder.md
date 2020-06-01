---
title: フォルダー
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folder
api_type:
- schema
ms.assetid: 812948d8-c7db-45ce-bb3a-77233a53a974
description: Folder 要素は、作成、取得、検索、同期、更新を行うフォルダーを定義します。
ms.openlocfilehash: 156813b3f7ecc6a2e1437f473ae1daa76b138e6e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457250"
---
# <a name="folder"></a><span data-ttu-id="1cd72-103">フォルダー</span><span class="sxs-lookup"><span data-stu-id="1cd72-103">Folder</span></span>

<span data-ttu-id="1cd72-104">**Folder**要素は、作成、取得、検索、同期、更新を行うフォルダーを定義します。</span><span class="sxs-lookup"><span data-stu-id="1cd72-104">The **Folder** element defines a folder to create, get, find, synchronize, or update.</span></span> 
  
```xml
<Folder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <UnreadCount/>
   <PermissionSet/>
   <EffectiveRights/>
</Folder>
```

 <span data-ttu-id="1cd72-105">**FolderType**</span><span class="sxs-lookup"><span data-stu-id="1cd72-105">**FolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1cd72-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1cd72-106">Attributes and elements</span></span>

<span data-ttu-id="1cd72-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1cd72-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1cd72-108">属性</span><span class="sxs-lookup"><span data-stu-id="1cd72-108">Attributes</span></span>

<span data-ttu-id="1cd72-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1cd72-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1cd72-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1cd72-110">Child elements</span></span>

|<span data-ttu-id="1cd72-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="1cd72-111">**Element**</span></span>|<span data-ttu-id="1cd72-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1cd72-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1cd72-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="1cd72-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="1cd72-114">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1cd72-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="1cd72-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="1cd72-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="1cd72-116">フォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="1cd72-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="1cd72-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="1cd72-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="1cd72-118">指定したフォルダーのフォルダークラスを表します。</span><span class="sxs-lookup"><span data-stu-id="1cd72-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="1cd72-119">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="1cd72-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="1cd72-120">フォルダーの表示名を含みます。</span><span class="sxs-lookup"><span data-stu-id="1cd72-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="1cd72-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="1cd72-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="1cd72-122">指定したフォルダー内のアイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="1cd72-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="1cd72-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="1cd72-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="1cd72-124">フォルダー内に含まれる子フォルダーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="1cd72-124">Represents the number of child folders that are contained within a folder.</span></span> <span data-ttu-id="1cd72-125">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="1cd72-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="1cd72-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="1cd72-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="1cd72-127">フォルダーの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="1cd72-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="1cd72-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="1cd72-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="1cd72-129">管理フォルダーに関する情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="1cd72-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="1cd72-130">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="1cd72-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="1cd72-131">指定したフォルダー内の未読アイテムの数を表します。</span><span class="sxs-lookup"><span data-stu-id="1cd72-131">Represents the count of unread items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="1cd72-132">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="1cd72-132">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="1cd72-133">フォルダーに対して構成されているすべてのアクセス許可が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1cd72-133">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="1cd72-134">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1cd72-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="1cd72-135">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="1cd72-135">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="1cd72-136">アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1cd72-136">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="1cd72-137">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1cd72-137">This element is read-only.</span></span> <span data-ttu-id="1cd72-138">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1cd72-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1cd72-139">親要素</span><span class="sxs-lookup"><span data-stu-id="1cd72-139">Parent elements</span></span>

|<span data-ttu-id="1cd72-140">**要素**</span><span class="sxs-lookup"><span data-stu-id="1cd72-140">**Element**</span></span>|<span data-ttu-id="1cd72-141">**説明**</span><span class="sxs-lookup"><span data-stu-id="1cd72-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1cd72-142">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="1cd72-142">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="1cd72-143">[Updatefolder 操作](updatefolder-operation.md)中に folder プロパティに追加するデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="1cd72-143">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="1cd72-144">Create (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="1cd72-144">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="1cd72-145">ローカルクライアントストアに作成する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="1cd72-145">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="1cd72-146">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="1cd72-146">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="1cd72-147">[Updatefolder 操作](updatefolder-operation.md)のフォルダーの1つのプロパティに対する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="1cd72-147">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="1cd72-148">Update (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="1cd72-148">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="1cd72-149">ローカルクライアントストアで更新する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="1cd72-149">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="1cd72-150">フォルダー</span><span class="sxs-lookup"><span data-stu-id="1cd72-150">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1cd72-151">Folder 操作で使用されるフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1cd72-151">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1cd72-152">注釈</span><span class="sxs-lookup"><span data-stu-id="1cd72-152">Remarks</span></span>

<span data-ttu-id="1cd72-153">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1cd72-153">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1cd72-154">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1cd72-154">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1cd72-155">Namespace</span><span class="sxs-lookup"><span data-stu-id="1cd72-155">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1cd72-156">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1cd72-156">Schema Name</span></span>  <br/> |<span data-ttu-id="1cd72-157">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="1cd72-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="1cd72-158">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1cd72-158">Validation File</span></span>  <br/> |<span data-ttu-id="1cd72-159">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1cd72-159">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1cd72-160">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1cd72-160">Can be Empty</span></span>  <br/> |<span data-ttu-id="1cd72-161">正しくない</span><span class="sxs-lookup"><span data-stu-id="1cd72-161">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1cd72-162">関連項目</span><span class="sxs-lookup"><span data-stu-id="1cd72-162">See also</span></span>



[<span data-ttu-id="1cd72-163">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="1cd72-163">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="1cd72-164">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1cd72-164">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: Folder
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
description: Folder 要素は、作成、取得、検索、同期、または更新するフォルダーを定義します。
ms.openlocfilehash: ecfea52d2105599372a22b78778ac0d0d066bc60
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760564"
---
# <a name="folder"></a><span data-ttu-id="6e6ba-103">Folder</span><span class="sxs-lookup"><span data-stu-id="6e6ba-103">Folder</span></span>

<span data-ttu-id="6e6ba-104">**Folder**要素は、作成、取得、検索、同期、または更新するフォルダーを定義します。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-104">The **Folder** element defines a folder to create, get, find, synchronize, or update.</span></span> 
  
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

 <span data-ttu-id="6e6ba-105">**FolderType**</span><span class="sxs-lookup"><span data-stu-id="6e6ba-105">**FolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e6ba-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6e6ba-106">Attributes and elements</span></span>

<span data-ttu-id="6e6ba-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e6ba-108">属性</span><span class="sxs-lookup"><span data-stu-id="6e6ba-108">Attributes</span></span>

<span data-ttu-id="6e6ba-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e6ba-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6e6ba-110">Child elements</span></span>

|<span data-ttu-id="6e6ba-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="6e6ba-111">**Element**</span></span>|<span data-ttu-id="6e6ba-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6e6ba-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e6ba-113">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="6e6ba-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="6e6ba-114">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="6e6ba-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="6e6ba-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="6e6ba-116">フォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="6e6ba-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="6e6ba-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="6e6ba-118">指定されたフォルダーのフォルダー クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="6e6ba-119">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="6e6ba-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="6e6ba-120">フォルダーの表示名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="6e6ba-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="6e6ba-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="6e6ba-122">指定したフォルダー内のアイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="6e6ba-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="6e6ba-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="6e6ba-124">フォルダー内に含まれる子フォルダーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-124">Represents the number of child folders that are contained within a folder.</span></span> <span data-ttu-id="6e6ba-125">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="6e6ba-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="6e6ba-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="6e6ba-127">フォルダーの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="6e6ba-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="6e6ba-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="6e6ba-129">管理フォルダーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="6e6ba-130">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="6e6ba-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="6e6ba-131">指定したフォルダー内の未読アイテムの数を表します。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-131">Represents the count of unread items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="6e6ba-132">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="6e6ba-132">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="6e6ba-133">フォルダーに対して構成されているすべてのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-133">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="6e6ba-134">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="6e6ba-135">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="6e6ba-135">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="6e6ba-136">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-136">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="6e6ba-137">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-137">This element is read-only.</span></span> <span data-ttu-id="6e6ba-138">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6e6ba-139">親要素</span><span class="sxs-lookup"><span data-stu-id="6e6ba-139">Parent elements</span></span>

|<span data-ttu-id="6e6ba-140">**要素**</span><span class="sxs-lookup"><span data-stu-id="6e6ba-140">**Element**</span></span>|<span data-ttu-id="6e6ba-141">**説明**</span><span class="sxs-lookup"><span data-stu-id="6e6ba-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e6ba-142">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="6e6ba-142">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="6e6ba-143">[UpdateFolder 操作](updatefolder-operation.md)中にフォルダーのプロパティを追加するデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-143">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="6e6ba-144">(集合的) を作成します。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-144">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="6e6ba-145">ローカル クライアント ストアに作成する 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-145">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="6e6ba-146">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="6e6ba-146">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="6e6ba-147">[UpdateFolder 操作](updatefolder-operation.md)でフォルダーの 1 つのプロパティには、更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-147">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="6e6ba-148">更新 (集合的)</span><span class="sxs-lookup"><span data-stu-id="6e6ba-148">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="6e6ba-149">ローカル クライアント ストアで更新する 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-149">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="6e6ba-150">フォルダー</span><span class="sxs-lookup"><span data-stu-id="6e6ba-150">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6e6ba-151">フォルダーの操作で使用されているフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-151">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6e6ba-152">備考</span><span class="sxs-lookup"><span data-stu-id="6e6ba-152">Remarks</span></span>

<span data-ttu-id="6e6ba-153">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割を持つ Exchange 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6e6ba-153">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e6ba-154">要素情報</span><span class="sxs-lookup"><span data-stu-id="6e6ba-154">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e6ba-155">名前空間</span><span class="sxs-lookup"><span data-stu-id="6e6ba-155">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6e6ba-156">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6e6ba-156">Schema Name</span></span>  <br/> |<span data-ttu-id="6e6ba-157">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6e6ba-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="6e6ba-158">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6e6ba-158">Validation File</span></span>  <br/> |<span data-ttu-id="6e6ba-159">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6e6ba-159">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6e6ba-160">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6e6ba-160">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e6ba-161">False</span><span class="sxs-lookup"><span data-stu-id="6e6ba-161">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e6ba-162">関連項目</span><span class="sxs-lookup"><span data-stu-id="6e6ba-162">See also</span></span>



[<span data-ttu-id="6e6ba-163">SyncFolderItems の操作</span><span class="sxs-lookup"><span data-stu-id="6e6ba-163">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="6e6ba-164">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6e6ba-164">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: TasksFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TasksFolder
api_type:
- schema
ms.assetid: 5a9a4612-8064-4986-b467-c44f268c64df
description: 仕事フォルダー要素は、メールボックスに含まれる Tasks フォルダーを表します。
ms.openlocfilehash: 522fe485482bd8159927f9925b7a5582ba2e1c22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465339"
---
# <a name="tasksfolder"></a><span data-ttu-id="7d45d-103">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="7d45d-103">TasksFolder</span></span>

<span data-ttu-id="7d45d-104">仕事**フォルダー要素は、メール**ボックスに含まれる Tasks フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="7d45d-104">The **TasksFolder** element represents a Tasks folder that is contained in a mailbox.</span></span> 
  
```xml
<TasksFolder>
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
</TasksFolder>
```

<span data-ttu-id="7d45d-105">**TasksFolderType**</span><span class="sxs-lookup"><span data-stu-id="7d45d-105">**TasksFolderType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7d45d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7d45d-106">Attributes and elements</span></span>

<span data-ttu-id="7d45d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7d45d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d45d-108">属性</span><span class="sxs-lookup"><span data-stu-id="7d45d-108">Attributes</span></span>

<span data-ttu-id="7d45d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7d45d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d45d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7d45d-110">Child elements</span></span>

|<span data-ttu-id="7d45d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="7d45d-111">**Element**</span></span>|<span data-ttu-id="7d45d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7d45d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d45d-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="7d45d-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="7d45d-114">Tasks フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7d45d-114">Contains the identifier and change key of a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="7d45d-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="7d45d-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="7d45d-116">タスクフォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="7d45d-116">Represents the identifier of the parent folder that contains the Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="7d45d-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="7d45d-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="7d45d-118">Tasks フォルダーの folder クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="7d45d-118">Represents the folder class for a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="7d45d-119">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="7d45d-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="7d45d-120">タスクフォルダーの表示名を含みます。</span><span class="sxs-lookup"><span data-stu-id="7d45d-120">Contains the display name of a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="7d45d-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="7d45d-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="7d45d-122">タスクフォルダー内のアイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="7d45d-122">Represents the total count of items within a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="7d45d-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="7d45d-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="7d45d-124">Tasks フォルダー内に含まれる子フォルダーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="7d45d-124">Represents the number of child folders that are contained within a Tasks folder.</span></span> <span data-ttu-id="7d45d-125">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="7d45d-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="7d45d-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="7d45d-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="7d45d-127">タスクフォルダーの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="7d45d-127">Identifies extended properties on a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="7d45d-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="7d45d-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="7d45d-129">管理フォルダーに関する情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="7d45d-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="7d45d-130">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="7d45d-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="7d45d-131">仕事フォルダー内の未読アイテムの数を表します。</span><span class="sxs-lookup"><span data-stu-id="7d45d-131">Represents the count of unread items within a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="7d45d-132">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="7d45d-132">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="7d45d-133">フォルダーに対して構成されているすべてのアクセス許可が含まれます。</span><span class="sxs-lookup"><span data-stu-id="7d45d-133">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="7d45d-134">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7d45d-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="7d45d-135">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="7d45d-135">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="7d45d-136">アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7d45d-136">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="7d45d-137">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="7d45d-137">This element is read-only.</span></span> <span data-ttu-id="7d45d-138">この要素は、Microsoft Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7d45d-138">This element was introduced in Microsoft Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7d45d-139">親要素</span><span class="sxs-lookup"><span data-stu-id="7d45d-139">Parent elements</span></span>

|<span data-ttu-id="7d45d-140">**要素**</span><span class="sxs-lookup"><span data-stu-id="7d45d-140">**Element**</span></span>|<span data-ttu-id="7d45d-141">**説明**</span><span class="sxs-lookup"><span data-stu-id="7d45d-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d45d-142">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="7d45d-142">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="7d45d-143">[Updatefolder 操作](updatefolder-operation.md)中に folder プロパティに追加するデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="7d45d-143">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="7d45d-144">Create (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="7d45d-144">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="7d45d-145">ローカルクライアントストアに作成する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="7d45d-145">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="7d45d-146">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="7d45d-146">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="7d45d-147">[Updatefolder 操作](updatefolder-operation.md)のフォルダーの1つのプロパティに対する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="7d45d-147">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="7d45d-148">Update (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="7d45d-148">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="7d45d-149">ローカルクライアントストアで更新する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="7d45d-149">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="7d45d-150">フォルダー</span><span class="sxs-lookup"><span data-stu-id="7d45d-150">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7d45d-151">Folder 操作で使用されるフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7d45d-151">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7d45d-152">注釈</span><span class="sxs-lookup"><span data-stu-id="7d45d-152">Remarks</span></span>

<span data-ttu-id="7d45d-153">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7d45d-153">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d45d-154">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7d45d-154">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d45d-155">Namespace</span><span class="sxs-lookup"><span data-stu-id="7d45d-155">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7d45d-156">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7d45d-156">Schema Name</span></span>  <br/> |<span data-ttu-id="7d45d-157">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7d45d-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="7d45d-158">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7d45d-158">Validation File</span></span>  <br/> |<span data-ttu-id="7d45d-159">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7d45d-159">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7d45d-160">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7d45d-160">Can be Empty</span></span>  <br/> |<span data-ttu-id="7d45d-161">正しくない</span><span class="sxs-lookup"><span data-stu-id="7d45d-161">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d45d-162">関連項目</span><span class="sxs-lookup"><span data-stu-id="7d45d-162">See also</span></span>

- [<span data-ttu-id="7d45d-163">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7d45d-163">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


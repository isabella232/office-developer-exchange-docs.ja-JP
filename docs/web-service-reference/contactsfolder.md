---
title: ContactsFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactsFolder
api_type:
- schema
ms.assetid: 6c299de8-2087-4aeb-8e66-2bc7586509a6
description: ContactsFolder 要素は、メールボックスに格納されている連絡先フォルダーを表します。
ms.openlocfilehash: 997b4f603198e6d05a011c4ef6bac7fe4dfbfe52
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529435"
---
# <a name="contactsfolder"></a><span data-ttu-id="d211e-103">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="d211e-103">ContactsFolder</span></span>

<span data-ttu-id="d211e-104">**ContactsFolder**要素は、メールボックスに格納されている連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="d211e-104">The **ContactsFolder** element represents a contacts folder that is contained in a mailbox.</span></span> 
  
```xml
<ContactsFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <EffectiveRights/>
   <SharingEffectiveRights/>
   <PermissionSet/>
</ContactsFolder>
```

 <span data-ttu-id="d211e-105">**ContactsFolderType**</span><span class="sxs-lookup"><span data-stu-id="d211e-105">**ContactsFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d211e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d211e-106">Attributes and elements</span></span>

<span data-ttu-id="d211e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d211e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d211e-108">属性</span><span class="sxs-lookup"><span data-stu-id="d211e-108">Attributes</span></span>

<span data-ttu-id="d211e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d211e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d211e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d211e-110">Child elements</span></span>

|<span data-ttu-id="d211e-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d211e-111">**Element**</span></span>|<span data-ttu-id="d211e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d211e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d211e-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="d211e-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="d211e-114">連絡先フォルダーの識別子と変更キーが保存されています。</span><span class="sxs-lookup"><span data-stu-id="d211e-114">Contains the identifier and change key of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="d211e-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="d211e-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="d211e-116">連絡先フォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="d211e-116">Represents the identifier of the parent folder that contains the contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="d211e-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="d211e-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="d211e-118">連絡先フォルダーのフォルダークラスを表します。</span><span class="sxs-lookup"><span data-stu-id="d211e-118">Represents the folder class for a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="d211e-119">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="d211e-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="d211e-120">連絡先フォルダーの表示名を含みます。</span><span class="sxs-lookup"><span data-stu-id="d211e-120">Contains the display name of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="d211e-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="d211e-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="d211e-122">連絡先フォルダー内のアイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="d211e-122">Represents the total count of items within a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="d211e-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="d211e-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="d211e-124">連絡先フォルダー内に含まれる子フォルダーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="d211e-124">Represents the number of child folders that are contained within a contacts folder.</span></span> <span data-ttu-id="d211e-125">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="d211e-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="d211e-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="d211e-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="d211e-127">連絡先フォルダーの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="d211e-127">Identifies extended properties on contacts folders.</span></span>  <br/> |
|[<span data-ttu-id="d211e-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="d211e-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="d211e-129">管理フォルダーに関する情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="d211e-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="d211e-130">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="d211e-130">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="d211e-131">アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d211e-131">Contains the client's rights based on the permission settings for the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="d211e-132">SharingEffectiveRights (PermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="d211e-132">SharingEffectiveRights (PermissionReadAccessType)</span></span>](sharingeffectiverights-permissionreadaccesstype.md) <br/> |<span data-ttu-id="d211e-133">共有されている連絡先データに対してユーザーが持っているアクセス許可を示します。</span><span class="sxs-lookup"><span data-stu-id="d211e-133">Indicates the permissions that the user has for the contact data that is being shared.</span></span>  <br/> |
|[<span data-ttu-id="d211e-134">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="d211e-134">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="d211e-135">フォルダーに対して構成されているすべてのアクセス許可が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d211e-135">Contains all the configured permissions for a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d211e-136">親要素</span><span class="sxs-lookup"><span data-stu-id="d211e-136">Parent elements</span></span>

|<span data-ttu-id="d211e-137">**要素**</span><span class="sxs-lookup"><span data-stu-id="d211e-137">**Element**</span></span>|<span data-ttu-id="d211e-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="d211e-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d211e-139">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="d211e-139">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="d211e-140">[Updatefolder 操作](updatefolder-operation.md)中に folder プロパティに追加するデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="d211e-140">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="d211e-141">Create (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="d211e-141">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="d211e-142">ローカルクライアントストアに作成する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="d211e-142">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="d211e-143">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="d211e-143">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="d211e-144">[Updatefolder 操作](updatefolder-operation.md)のフォルダーの1つのプロパティに対する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="d211e-144">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="d211e-145">Update (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="d211e-145">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="d211e-146">ローカルクライアントストアで更新する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="d211e-146">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="d211e-147">フォルダー</span><span class="sxs-lookup"><span data-stu-id="d211e-147">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d211e-148">Folder 操作で使用されるフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d211e-148">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d211e-149">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d211e-149">Text value</span></span>

<span data-ttu-id="d211e-150">なし。</span><span class="sxs-lookup"><span data-stu-id="d211e-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d211e-151">注釈</span><span class="sxs-lookup"><span data-stu-id="d211e-151">Remarks</span></span>

<span data-ttu-id="d211e-152">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d211e-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d211e-153">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d211e-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d211e-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="d211e-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d211e-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d211e-155">Schema Name</span></span>  <br/> |<span data-ttu-id="d211e-156">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d211e-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="d211e-157">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d211e-157">Validation File</span></span>  <br/> |<span data-ttu-id="d211e-158">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d211e-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d211e-159">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d211e-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="d211e-160">正しくない</span><span class="sxs-lookup"><span data-stu-id="d211e-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d211e-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="d211e-161">See also</span></span>



- [<span data-ttu-id="d211e-162">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d211e-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


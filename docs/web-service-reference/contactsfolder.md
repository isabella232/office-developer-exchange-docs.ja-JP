---
title: メッセージ
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
description: メッセージ要素は、メールボックスに格納されている連絡先フォルダーを表します。
ms.openlocfilehash: 01302f00d84cfff9713e3b188b7799c537fc0629
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759681"
---
# <a name="contactsfolder"></a><span data-ttu-id="e1b45-103">メッセージ</span><span class="sxs-lookup"><span data-stu-id="e1b45-103">ContactsFolder</span></span>

<span data-ttu-id="e1b45-104">**メッセージ**要素は、メールボックスに格納されている連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="e1b45-104">The **ContactsFolder** element represents a contacts folder that is contained in a mailbox.</span></span> 
  
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

 <span data-ttu-id="e1b45-105">**ContactsFolderType**</span><span class="sxs-lookup"><span data-stu-id="e1b45-105">**ContactsFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1b45-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e1b45-106">Attributes and elements</span></span>

<span data-ttu-id="e1b45-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e1b45-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1b45-108">属性</span><span class="sxs-lookup"><span data-stu-id="e1b45-108">Attributes</span></span>

<span data-ttu-id="e1b45-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e1b45-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1b45-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e1b45-110">Child elements</span></span>

|<span data-ttu-id="e1b45-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="e1b45-111">**Element**</span></span>|<span data-ttu-id="e1b45-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e1b45-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1b45-113">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="e1b45-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="e1b45-114">連絡先フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e1b45-114">Contains the identifier and change key of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="e1b45-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="e1b45-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="e1b45-116">連絡先フォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="e1b45-116">Represents the identifier of the parent folder that contains the contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="e1b45-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="e1b45-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="e1b45-118">連絡先フォルダーのフォルダー クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="e1b45-118">Represents the folder class for a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="e1b45-119">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="e1b45-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="e1b45-120">連絡先フォルダーの表示名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e1b45-120">Contains the display name of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="e1b45-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="e1b45-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="e1b45-122">連絡先フォルダー内のアイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="e1b45-122">Represents the total count of items within a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="e1b45-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="e1b45-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="e1b45-124">連絡先フォルダー内に含まれる子フォルダーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="e1b45-124">Represents the number of child folders that are contained within a contacts folder.</span></span> <span data-ttu-id="e1b45-125">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e1b45-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="e1b45-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="e1b45-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="e1b45-127">連絡先フォルダーの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="e1b45-127">Identifies extended properties on contacts folders.</span></span>  <br/> |
|[<span data-ttu-id="e1b45-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="e1b45-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="e1b45-129">管理フォルダーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e1b45-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="e1b45-130">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="e1b45-130">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="e1b45-131">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e1b45-131">Contains the client's rights based on the permission settings for the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="e1b45-132">SharingEffectiveRights (PermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="e1b45-132">SharingEffectiveRights (PermissionReadAccessType)</span></span>](sharingeffectiverights-permissionreadaccesstype.md) <br/> |<span data-ttu-id="e1b45-133">ユーザーが共有されている連絡先のデータを持っているアクセス許可を示します。</span><span class="sxs-lookup"><span data-stu-id="e1b45-133">Indicates the permissions that the user has for the contact data that is being shared.</span></span>  <br/> |
|[<span data-ttu-id="e1b45-134">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="e1b45-134">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="e1b45-135">フォルダーに対して構成されているすべてのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e1b45-135">Contains all the configured permissions for a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e1b45-136">親要素</span><span class="sxs-lookup"><span data-stu-id="e1b45-136">Parent elements</span></span>

|<span data-ttu-id="e1b45-137">**要素**</span><span class="sxs-lookup"><span data-stu-id="e1b45-137">**Element**</span></span>|<span data-ttu-id="e1b45-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="e1b45-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1b45-139">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="e1b45-139">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="e1b45-140">[UpdateFolder 操作](updatefolder-operation.md)中にフォルダーのプロパティを追加するデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="e1b45-140">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="e1b45-141">(集合的) を作成します。</span><span class="sxs-lookup"><span data-stu-id="e1b45-141">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="e1b45-142">ローカル クライアント ストアに作成する 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="e1b45-142">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="e1b45-143">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="e1b45-143">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="e1b45-144">[UpdateFolder 操作](updatefolder-operation.md)でフォルダーの 1 つのプロパティには、更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="e1b45-144">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="e1b45-145">更新 (集合的)</span><span class="sxs-lookup"><span data-stu-id="e1b45-145">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="e1b45-146">ローカル クライアント ストアで更新する 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="e1b45-146">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="e1b45-147">フォルダー</span><span class="sxs-lookup"><span data-stu-id="e1b45-147">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e1b45-148">フォルダーの操作で使用されているフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e1b45-148">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e1b45-149">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e1b45-149">Text value</span></span>

<span data-ttu-id="e1b45-150">なし。</span><span class="sxs-lookup"><span data-stu-id="e1b45-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e1b45-151">備考</span><span class="sxs-lookup"><span data-stu-id="e1b45-151">Remarks</span></span>

<span data-ttu-id="e1b45-152">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e1b45-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1b45-153">要素情報</span><span class="sxs-lookup"><span data-stu-id="e1b45-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1b45-154">名前空間</span><span class="sxs-lookup"><span data-stu-id="e1b45-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e1b45-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e1b45-155">Schema Name</span></span>  <br/> |<span data-ttu-id="e1b45-156">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e1b45-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="e1b45-157">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e1b45-157">Validation File</span></span>  <br/> |<span data-ttu-id="e1b45-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e1b45-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e1b45-159">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e1b45-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="e1b45-160">False</span><span class="sxs-lookup"><span data-stu-id="e1b45-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e1b45-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="e1b45-161">See also</span></span>



- [<span data-ttu-id="e1b45-162">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e1b45-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


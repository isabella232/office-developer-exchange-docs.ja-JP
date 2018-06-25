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
description: TasksFolder 要素は、メールボックスに含まれるタスク フォルダーを表します。
ms.openlocfilehash: b2151c68519a6ff15fbc74b48fc93a7e06af9e76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839650"
---
# <a name="tasksfolder"></a><span data-ttu-id="aebb1-103">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="aebb1-103">TasksFolder</span></span>

<span data-ttu-id="aebb1-104">**TasksFolder**要素は、メールボックスに含まれるタスク フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="aebb1-104">The **TasksFolder** element represents a Tasks folder that is contained in a mailbox.</span></span> 
  
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

<span data-ttu-id="aebb1-105">**TasksFolderType**</span><span class="sxs-lookup"><span data-stu-id="aebb1-105">**TasksFolderType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="aebb1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="aebb1-106">Attributes and elements</span></span>

<span data-ttu-id="aebb1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="aebb1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aebb1-108">属性</span><span class="sxs-lookup"><span data-stu-id="aebb1-108">Attributes</span></span>

<span data-ttu-id="aebb1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="aebb1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aebb1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="aebb1-110">Child elements</span></span>

|<span data-ttu-id="aebb1-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="aebb1-111">**Element**</span></span>|<span data-ttu-id="aebb1-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="aebb1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aebb1-113">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="aebb1-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="aebb1-114">タスク フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="aebb1-114">Contains the identifier and change key of a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="aebb1-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="aebb1-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="aebb1-116">[仕事] フォルダーを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="aebb1-116">Represents the identifier of the parent folder that contains the Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="aebb1-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="aebb1-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="aebb1-118">タスク フォルダーのフォルダー クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="aebb1-118">Represents the folder class for a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="aebb1-119">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="aebb1-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="aebb1-120">タスク フォルダーの表示名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="aebb1-120">Contains the display name of a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="aebb1-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="aebb1-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="aebb1-122">タスク フォルダー内のアイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="aebb1-122">Represents the total count of items within a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="aebb1-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="aebb1-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="aebb1-124">タスク フォルダー内に含まれる子フォルダーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="aebb1-124">Represents the number of child folders that are contained within a Tasks folder.</span></span> <span data-ttu-id="aebb1-125">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="aebb1-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="aebb1-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="aebb1-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="aebb1-127">タスク フォルダーの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="aebb1-127">Identifies extended properties on a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="aebb1-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="aebb1-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="aebb1-129">管理フォルダーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="aebb1-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="aebb1-130">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="aebb1-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="aebb1-131">タスク フォルダー内の未読アイテムの数を表します。</span><span class="sxs-lookup"><span data-stu-id="aebb1-131">Represents the count of unread items within a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="aebb1-132">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="aebb1-132">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="aebb1-133">フォルダーに対して構成されているすべてのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="aebb1-133">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="aebb1-134">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="aebb1-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="aebb1-135">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="aebb1-135">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="aebb1-136">アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。</span><span class="sxs-lookup"><span data-stu-id="aebb1-136">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="aebb1-137">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="aebb1-137">This element is read-only.</span></span> <span data-ttu-id="aebb1-138">この要素は、Microsoft Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="aebb1-138">This element was introduced in Microsoft Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aebb1-139">親要素</span><span class="sxs-lookup"><span data-stu-id="aebb1-139">Parent elements</span></span>

|<span data-ttu-id="aebb1-140">**要素**</span><span class="sxs-lookup"><span data-stu-id="aebb1-140">**Element**</span></span>|<span data-ttu-id="aebb1-141">**説明**</span><span class="sxs-lookup"><span data-stu-id="aebb1-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aebb1-142">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="aebb1-142">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="aebb1-143">[UpdateFolder 操作](updatefolder-operation.md)中にフォルダーのプロパティを追加するデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="aebb1-143">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="aebb1-144">(集合的) を作成します。</span><span class="sxs-lookup"><span data-stu-id="aebb1-144">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="aebb1-145">ローカル クライアント ストアに作成する 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="aebb1-145">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="aebb1-146">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="aebb1-146">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="aebb1-147">[UpdateFolder 操作](updatefolder-operation.md)でフォルダーの 1 つのプロパティには、更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="aebb1-147">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="aebb1-148">更新 (集合的)</span><span class="sxs-lookup"><span data-stu-id="aebb1-148">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="aebb1-149">ローカル クライアント ストアで更新する 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="aebb1-149">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="aebb1-150">フォルダー</span><span class="sxs-lookup"><span data-stu-id="aebb1-150">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="aebb1-151">フォルダーの操作で使用されているフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="aebb1-151">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aebb1-152">備考</span><span class="sxs-lookup"><span data-stu-id="aebb1-152">Remarks</span></span>

<span data-ttu-id="aebb1-153">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="aebb1-153">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aebb1-154">要素情報</span><span class="sxs-lookup"><span data-stu-id="aebb1-154">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aebb1-155">名前空間</span><span class="sxs-lookup"><span data-stu-id="aebb1-155">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aebb1-156">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="aebb1-156">Schema Name</span></span>  <br/> |<span data-ttu-id="aebb1-157">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="aebb1-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="aebb1-158">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="aebb1-158">Validation File</span></span>  <br/> |<span data-ttu-id="aebb1-159">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aebb1-159">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aebb1-160">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="aebb1-160">Can be Empty</span></span>  <br/> |<span data-ttu-id="aebb1-161">False</span><span class="sxs-lookup"><span data-stu-id="aebb1-161">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aebb1-162">関連項目</span><span class="sxs-lookup"><span data-stu-id="aebb1-162">See also</span></span>

- [<span data-ttu-id="aebb1-163">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="aebb1-163">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


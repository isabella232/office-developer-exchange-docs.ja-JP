---
title: ManagedFolderInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ManagedFolderInformation
api_type:
- schema
ms.assetid: dea980eb-8303-47fe-a380-20a8efc9ead6
description: ManagedFolderInformation 要素には、管理されたカスタムフォルダーに関する情報が含まれています。
ms.openlocfilehash: ce15dcb15cccdce253494beefd2f4a2a7a0c0ad8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44450950"
---
# <a name="managedfolderinformation"></a><span data-ttu-id="b0919-103">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="b0919-103">ManagedFolderInformation</span></span>

<span data-ttu-id="b0919-104">**Managedfolderinformation**要素には、管理されたカスタムフォルダーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0919-104">The **ManagedFolderInformation** element contains information about a managed custom folder.</span></span> 
  
```xml
<ManagedFolderInformation>
   <CanDelete/>
   <CanRenameOrMove/>
   <MustDisplayComment/>
   <HasQuota/>
   <IsManagedFoldersRoot/>
   <ManagedFolderId/>
   <Comment/>
   <StorageQuota/>
   <FolderSize/>
   <HomePage/>
</ManagedFolderInformation>
```

 <span data-ttu-id="b0919-105">**ManagedFolderInformationType**</span><span class="sxs-lookup"><span data-stu-id="b0919-105">**ManagedFolderInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0919-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b0919-106">Attributes and elements</span></span>

<span data-ttu-id="b0919-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b0919-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0919-108">属性</span><span class="sxs-lookup"><span data-stu-id="b0919-108">Attributes</span></span>

<span data-ttu-id="b0919-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b0919-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0919-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b0919-110">Child elements</span></span>

|<span data-ttu-id="b0919-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="b0919-111">**Element**</span></span>|<span data-ttu-id="b0919-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0919-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0919-113">CanDelete</span><span class="sxs-lookup"><span data-stu-id="b0919-113">CanDelete</span></span>](candelete.md) <br/> |<span data-ttu-id="b0919-114">管理フォルダーを顧客が削除できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b0919-114">Indicates whether a managed folder can be deleted by a customer.</span></span>  <br/> |
|[<span data-ttu-id="b0919-115">CanRenameOrMove</span><span class="sxs-lookup"><span data-stu-id="b0919-115">CanRenameOrMove</span></span>](canrenameormove.md) <br/> |<span data-ttu-id="b0919-116">ユーザーが、特定の管理フォルダーの名前を変更するか、移動できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b0919-116">Indicates whether a given managed folder can be renamed or moved by the customer.</span></span>  <br/> |
|[<span data-ttu-id="b0919-117">On Displaycomment</span><span class="sxs-lookup"><span data-stu-id="b0919-117">MustDisplayComment</span></span>](mustdisplaycomment.md) <br/> |<span data-ttu-id="b0919-118">管理フォルダーのコメントを表示する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b0919-118">Indicates whether the managed folder comment must be displayed.</span></span>  <br/> |
|[<span data-ttu-id="b0919-119">HasQuota</span><span class="sxs-lookup"><span data-stu-id="b0919-119">HasQuota</span></span>](hasquota.md) <br/> |<span data-ttu-id="b0919-120">管理フォルダーにクォータがあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b0919-120">Indicates whether the managed folder has a quota.</span></span>  <br/> |
|[<span data-ttu-id="b0919-121">Ismanagedフォルダーのルート</span><span class="sxs-lookup"><span data-stu-id="b0919-121">IsManagedFoldersRoot</span></span>](ismanagedfoldersroot.md) <br/> |<span data-ttu-id="b0919-122">管理フォルダーがすべての管理フォルダーのルートであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b0919-122">Indicates whether the managed folder is the root for all managed folders.</span></span>  <br/> |
|[<span data-ttu-id="b0919-123">ManagedFolderId</span><span class="sxs-lookup"><span data-stu-id="b0919-123">ManagedFolderId</span></span>](managedfolderid.md) <br/> |<span data-ttu-id="b0919-124">管理フォルダーのフォルダー ID を格納します。</span><span class="sxs-lookup"><span data-stu-id="b0919-124">Contains the folder ID of the managed folder.</span></span>  <br/> |
|[<span data-ttu-id="b0919-125">Comment</span><span class="sxs-lookup"><span data-stu-id="b0919-125">Comment</span></span>](comment.md) <br/> |<span data-ttu-id="b0919-126">管理フォルダーに関連付けられているコメントが保存されています。</span><span class="sxs-lookup"><span data-stu-id="b0919-126">Contains the comment that is associated with a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="b0919-127">StorageQuota</span><span class="sxs-lookup"><span data-stu-id="b0919-127">StorageQuota</span></span>](storagequota.md) <br/> |<span data-ttu-id="b0919-128">管理フォルダーの記憶域のクォータを示します。</span><span class="sxs-lookup"><span data-stu-id="b0919-128">Describes the storage quota for the managed folder.</span></span>  <br/> |
|[<span data-ttu-id="b0919-129">FolderSize</span><span class="sxs-lookup"><span data-stu-id="b0919-129">FolderSize</span></span>](foldersize.md) <br/> |<span data-ttu-id="b0919-130">管理フォルダーのすべてのコンテンツの合計サイズを示します。</span><span class="sxs-lookup"><span data-stu-id="b0919-130">Describes the total size of all the contents of a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="b0919-131">HomePage</span><span class="sxs-lookup"><span data-stu-id="b0919-131">HomePage</span></span>](homepage.md) <br/> |<span data-ttu-id="b0919-132">管理フォルダーの既定のホームページとなる URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="b0919-132">Specifies the URL that will be the default home page for the managed folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0919-133">親要素</span><span class="sxs-lookup"><span data-stu-id="b0919-133">Parent elements</span></span>

|<span data-ttu-id="b0919-134">**要素**</span><span class="sxs-lookup"><span data-stu-id="b0919-134">**Element**</span></span>|<span data-ttu-id="b0919-135">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0919-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0919-136">Folder</span><span class="sxs-lookup"><span data-stu-id="b0919-136">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="b0919-137">Exchange ストア内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="b0919-137">Represents a folder in the Exchange store.</span></span> <span data-ttu-id="b0919-138">管理されたカスタムフォルダーは、**管理フォルダー**という名前のフォルダーのサブフォルダーにのみ設定できます。</span><span class="sxs-lookup"><span data-stu-id="b0919-138">Managed custom folders can only be subfolders of the folder named **Managed Folders**.</span></span>  <br/> |
|[<span data-ttu-id="b0919-139">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="b0919-139">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="b0919-140">該当なし。</span><span class="sxs-lookup"><span data-stu-id="b0919-140">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="b0919-141">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="b0919-141">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="b0919-142">該当なし。</span><span class="sxs-lookup"><span data-stu-id="b0919-142">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="b0919-143">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="b0919-143">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="b0919-144">該当なし。</span><span class="sxs-lookup"><span data-stu-id="b0919-144">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="b0919-145">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="b0919-145">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="b0919-146">なし。</span><span class="sxs-lookup"><span data-stu-id="b0919-146">Not applicable.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b0919-147">注釈</span><span class="sxs-lookup"><span data-stu-id="b0919-147">Remarks</span></span>

<span data-ttu-id="b0919-148">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b0919-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0919-149">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b0919-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0919-150">Namespace</span><span class="sxs-lookup"><span data-stu-id="b0919-150">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b0919-151">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b0919-151">Schema name</span></span>  <br/> |<span data-ttu-id="b0919-152">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b0919-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="b0919-153">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b0919-153">Validation file</span></span>  <br/> |<span data-ttu-id="b0919-154">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b0919-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b0919-155">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b0919-155">Can be empty</span></span>  <br/> |<span data-ttu-id="b0919-156">正しくない</span><span class="sxs-lookup"><span data-stu-id="b0919-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0919-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="b0919-157">See also</span></span>



[<span data-ttu-id="b0919-158">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="b0919-158">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="b0919-159">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b0919-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="b0919-160">管理フォルダーの追加</span><span class="sxs-lookup"><span data-stu-id="b0919-160">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)


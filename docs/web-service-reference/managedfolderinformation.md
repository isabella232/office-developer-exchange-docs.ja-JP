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
description: ManagedFolderInformation 要素には、管理されたカスタム フォルダーに関する情報が含まれています。
ms.openlocfilehash: ef46e2e0db440de2a8acae8316ce98d11bd6710e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832341"
---
# <a name="managedfolderinformation"></a><span data-ttu-id="0afff-103">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="0afff-103">ManagedFolderInformation</span></span>

<span data-ttu-id="0afff-104">**ManagedFolderInformation**要素には、管理されたカスタム フォルダーに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0afff-104">The **ManagedFolderInformation** element contains information about a managed custom folder.</span></span> 
  
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

 <span data-ttu-id="0afff-105">**ManagedFolderInformationType**</span><span class="sxs-lookup"><span data-stu-id="0afff-105">**ManagedFolderInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0afff-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0afff-106">Attributes and elements</span></span>

<span data-ttu-id="0afff-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0afff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0afff-108">属性</span><span class="sxs-lookup"><span data-stu-id="0afff-108">Attributes</span></span>

<span data-ttu-id="0afff-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0afff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0afff-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0afff-110">Child elements</span></span>

|<span data-ttu-id="0afff-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="0afff-111">**Element**</span></span>|<span data-ttu-id="0afff-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0afff-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0afff-113">CanDelete</span><span class="sxs-lookup"><span data-stu-id="0afff-113">CanDelete</span></span>](candelete.md) <br/> |<span data-ttu-id="0afff-114">顧客が管理対象のフォルダーを削除できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0afff-114">Indicates whether a managed folder can be deleted by a customer.</span></span>  <br/> |
|[<span data-ttu-id="0afff-115">CanRenameOrMove</span><span class="sxs-lookup"><span data-stu-id="0afff-115">CanRenameOrMove</span></span>](canrenameormove.md) <br/> |<span data-ttu-id="0afff-116">指定された管理フォルダーの名前の変更やお客様が移動するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0afff-116">Indicates whether a given managed folder can be renamed or moved by the customer.</span></span>  <br/> |
|[<span data-ttu-id="0afff-117">MustDisplayComment</span><span class="sxs-lookup"><span data-stu-id="0afff-117">MustDisplayComment</span></span>](mustdisplaycomment.md) <br/> |<span data-ttu-id="0afff-118">管理フォルダーのコメントを表示する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0afff-118">Indicates whether the managed folder comment must be displayed.</span></span>  <br/> |
|[<span data-ttu-id="0afff-119">HasQuota</span><span class="sxs-lookup"><span data-stu-id="0afff-119">HasQuota</span></span>](hasquota.md) <br/> |<span data-ttu-id="0afff-120">管理フォルダーがクォータを持つかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0afff-120">Indicates whether the managed folder has a quota.</span></span>  <br/> |
|[<span data-ttu-id="0afff-121">IsManagedFoldersRoot</span><span class="sxs-lookup"><span data-stu-id="0afff-121">IsManagedFoldersRoot</span></span>](ismanagedfoldersroot.md) <br/> |<span data-ttu-id="0afff-122">管理フォルダーがすべての管理フォルダーのルートであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0afff-122">Indicates whether the managed folder is the root for all managed folders.</span></span>  <br/> |
|[<span data-ttu-id="0afff-123">ManagedFolderId</span><span class="sxs-lookup"><span data-stu-id="0afff-123">ManagedFolderId</span></span>](managedfolderid.md) <br/> |<span data-ttu-id="0afff-124">管理フォルダーのフォルダー ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0afff-124">Contains the folder ID of the managed folder.</span></span>  <br/> |
|[<span data-ttu-id="0afff-125">Comment</span><span class="sxs-lookup"><span data-stu-id="0afff-125">Comment</span></span>](comment.md) <br/> |<span data-ttu-id="0afff-126">管理フォルダーに関連付けられているコメントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0afff-126">Contains the comment that is associated with a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="0afff-127">StorageQuota</span><span class="sxs-lookup"><span data-stu-id="0afff-127">StorageQuota</span></span>](storagequota.md) <br/> |<span data-ttu-id="0afff-128">管理フォルダーの記憶域のクォータについて説明します。</span><span class="sxs-lookup"><span data-stu-id="0afff-128">Describes the storage quota for the managed folder.</span></span>  <br/> |
|[<span data-ttu-id="0afff-129">FolderSize</span><span class="sxs-lookup"><span data-stu-id="0afff-129">FolderSize</span></span>](foldersize.md) <br/> |<span data-ttu-id="0afff-130">管理フォルダーのすべての内容の合計サイズを示します。</span><span class="sxs-lookup"><span data-stu-id="0afff-130">Describes the total size of all the contents of a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="0afff-131">ホームページ</span><span class="sxs-lookup"><span data-stu-id="0afff-131">HomePage</span></span>](homepage.md) <br/> |<span data-ttu-id="0afff-132">管理フォルダーの既定のホーム ページとなる URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="0afff-132">Specifies the URL that will be the default home page for the managed folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0afff-133">親要素</span><span class="sxs-lookup"><span data-stu-id="0afff-133">Parent elements</span></span>

|<span data-ttu-id="0afff-134">**要素**</span><span class="sxs-lookup"><span data-stu-id="0afff-134">**Element**</span></span>|<span data-ttu-id="0afff-135">**説明**</span><span class="sxs-lookup"><span data-stu-id="0afff-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0afff-136">Folder</span><span class="sxs-lookup"><span data-stu-id="0afff-136">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="0afff-137">Exchange ストア内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="0afff-137">Represents a folder in the Exchange store.</span></span> <span data-ttu-id="0afff-138">管理されたカスタム フォルダーは、**管理対象フォルダー**をという名前のフォルダーのサブフォルダーのみできます。</span><span class="sxs-lookup"><span data-stu-id="0afff-138">Managed custom folders can only be subfolders of the folder named **Managed Folders**.</span></span>  <br/> |
|[<span data-ttu-id="0afff-139">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="0afff-139">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="0afff-140">該当なし。</span><span class="sxs-lookup"><span data-stu-id="0afff-140">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="0afff-141">メッセージ</span><span class="sxs-lookup"><span data-stu-id="0afff-141">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="0afff-142">該当なし。</span><span class="sxs-lookup"><span data-stu-id="0afff-142">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="0afff-143">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="0afff-143">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="0afff-144">該当なし。</span><span class="sxs-lookup"><span data-stu-id="0afff-144">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="0afff-145">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="0afff-145">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="0afff-146">該当なし。</span><span class="sxs-lookup"><span data-stu-id="0afff-146">Not applicable.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0afff-147">注釈</span><span class="sxs-lookup"><span data-stu-id="0afff-147">Remarks</span></span>

<span data-ttu-id="0afff-148">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="0afff-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0afff-149">要素情報</span><span class="sxs-lookup"><span data-stu-id="0afff-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0afff-150">名前空間</span><span class="sxs-lookup"><span data-stu-id="0afff-150">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0afff-151">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0afff-151">Schema name</span></span>  <br/> |<span data-ttu-id="0afff-152">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="0afff-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="0afff-153">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0afff-153">Validation file</span></span>  <br/> |<span data-ttu-id="0afff-154">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0afff-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0afff-155">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0afff-155">Can be empty</span></span>  <br/> |<span data-ttu-id="0afff-156">False</span><span class="sxs-lookup"><span data-stu-id="0afff-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0afff-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="0afff-157">See also</span></span>



[<span data-ttu-id="0afff-158">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="0afff-158">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="0afff-159">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0afff-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="0afff-160">管理フォルダーを追加します。</span><span class="sxs-lookup"><span data-stu-id="0afff-160">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)


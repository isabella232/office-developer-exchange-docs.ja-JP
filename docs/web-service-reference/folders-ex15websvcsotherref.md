---
title: フォルダー
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folders
api_type:
- schema
ms.assetid: 8e71cb44-1df6-444a-add7-0c1363863f65
description: フォルダーの要素には、フォルダーの操作で使用されているフォルダーの配列が含まれています。
ms.openlocfilehash: e1b9e337f633dbf6fda159c28725d3fb8dcd55a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760570"
---
# <a name="folders"></a><span data-ttu-id="ec0fe-103">フォルダー</span><span class="sxs-lookup"><span data-stu-id="ec0fe-103">Folders</span></span>

<span data-ttu-id="ec0fe-104">**フォルダー**の要素には、フォルダーの操作で使用されているフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-104">The **Folders** element contains an array of folders that are used in folder operations.</span></span> 
  
```xml
<Folders>
   <Folder/>
</Folders>
```

 <span data-ttu-id="ec0fe-105">**ArrayOfFoldersType**または**NonEmptyArrayOfFoldersType**</span><span class="sxs-lookup"><span data-stu-id="ec0fe-105">**ArrayOfFoldersType** or **NonEmptyArrayOfFoldersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ec0fe-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ec0fe-106">Attributes and elements</span></span>

<span data-ttu-id="ec0fe-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec0fe-108">属性</span><span class="sxs-lookup"><span data-stu-id="ec0fe-108">Attributes</span></span>

<span data-ttu-id="ec0fe-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ec0fe-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ec0fe-110">Child elements</span></span>

|<span data-ttu-id="ec0fe-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="ec0fe-111">**Element**</span></span>|<span data-ttu-id="ec0fe-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ec0fe-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec0fe-113">Folder</span><span class="sxs-lookup"><span data-stu-id="ec0fe-113">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="ec0fe-114">作成、取得、検索、同期、または更新するフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-114">Identifies a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="ec0fe-115">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="ec0fe-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="ec0fe-116">主に予定表のアイテムを含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-116">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="ec0fe-117">メッセージ</span><span class="sxs-lookup"><span data-stu-id="ec0fe-117">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="ec0fe-118">メールボックスの連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-118">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ec0fe-119">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="ec0fe-119">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="ec0fe-120">メールボックスに含まれている検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-120">Represents a Search folder contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ec0fe-121">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="ec0fe-121">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="ec0fe-122">メールボックス内のタスク フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-122">Represents a Tasks folder in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ec0fe-123">親要素</span><span class="sxs-lookup"><span data-stu-id="ec0fe-123">Parent elements</span></span>

|<span data-ttu-id="ec0fe-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="ec0fe-124">**Element**</span></span>|<span data-ttu-id="ec0fe-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="ec0fe-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec0fe-126">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ec0fe-126">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md) <br/> |<span data-ttu-id="ec0fe-127">状態および 1 つの結果が含まれています[CopyFolder 操作](copyfolder-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-127">Contains the status and result of a single [CopyFolder operation](copyfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="ec0fe-128">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="ec0fe-128">CreateFolder</span></span>](createfolder.md) <br/> |<span data-ttu-id="ec0fe-129">Exchange ストア内のフォルダーを作成する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-129">Defines a request to create a folder in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ec0fe-130">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ec0fe-130">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md) <br/> |<span data-ttu-id="ec0fe-131">状態および 1 つの結果が含まれています[CreateFolder 操作](createfolder-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-131">Contains the status and result of a single [CreateFolder operation](createfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="ec0fe-132">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ec0fe-132">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md) <br/> |<span data-ttu-id="ec0fe-133">状態および 1 つの結果が含まれています[CreateManagedFolder 操作](createmanagedfolder-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-133">Contains the status and result of a single [CreateManagedFolder operation](createmanagedfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="ec0fe-134">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ec0fe-134">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md) <br/> |<span data-ttu-id="ec0fe-135">[GetFolder 操作](getfolder-operation.md)要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-135">Contains the status and result of a [GetFolder operation](getfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="ec0fe-136">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ec0fe-136">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md) <br/> |<span data-ttu-id="ec0fe-137">[MoveFolder 操作](movefolder-operation.md)要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-137">Contains the status and result of a [MoveFolder operation](movefolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="ec0fe-138">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="ec0fe-138">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="ec0fe-139">新しいフォルダーの作成先フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-139">Identifies the folder where a new folder is created.</span></span>  <br/> |
|[<span data-ttu-id="ec0fe-140">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="ec0fe-140">RootFolder (FindFolderResponseMessage)</span></span>](rootfolder-findfolderresponsemessage.md) <br/> |<span data-ttu-id="ec0fe-141">[FindFolder 操作](findfolder-operation.md)中に単一のルート フォルダーの検索結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-141">Contains the results from searching a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ec0fe-142">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ec0fe-142">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md) <br/> |<span data-ttu-id="ec0fe-143">状態および 1 つの結果が含まれています[UpdateFolder 操作](updatefolder-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-143">Contains the status and result of a single [UpdateFolder operation](updatefolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ec0fe-144">備考</span><span class="sxs-lookup"><span data-stu-id="ec0fe-144">Remarks</span></span>

<span data-ttu-id="ec0fe-145">この要素は、 [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素の必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-145">This element is a required child element of the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span> 
  
<span data-ttu-id="ec0fe-146">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="ec0fe-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec0fe-147">要素情報</span><span class="sxs-lookup"><span data-stu-id="ec0fe-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec0fe-148">名前空間</span><span class="sxs-lookup"><span data-stu-id="ec0fe-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ec0fe-149">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ec0fe-149">Schema Name</span></span>  <br/> |<span data-ttu-id="ec0fe-150">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ec0fe-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="ec0fe-151">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ec0fe-151">Validation File</span></span>  <br/> |<span data-ttu-id="ec0fe-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ec0fe-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ec0fe-153">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ec0fe-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="ec0fe-154">False</span><span class="sxs-lookup"><span data-stu-id="ec0fe-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ec0fe-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="ec0fe-155">See also</span></span>



[<span data-ttu-id="ec0fe-156">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="ec0fe-156">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)


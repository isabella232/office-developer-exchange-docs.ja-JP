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
description: Folders 要素には、フォルダー操作で使用されるフォルダーの配列が含まれています。
ms.openlocfilehash: b087be0501f04390b80458458e7e7ccc24bf27bd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530980"
---
# <a name="folders"></a><span data-ttu-id="9f96e-103">フォルダー</span><span class="sxs-lookup"><span data-stu-id="9f96e-103">Folders</span></span>

<span data-ttu-id="9f96e-104">**Folders**要素には、フォルダー操作で使用されるフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9f96e-104">The **Folders** element contains an array of folders that are used in folder operations.</span></span> 
  
```xml
<Folders>
   <Folder/>
</Folders>
```

```xml
<Folders>
   <ContactsFolder/> 
</Folders>
```

```xml
<Folders>
   <TasksFolder/>
</Folders>
```

```xml
<Folders>
   <CalendarFolder/>
</Folders>
```

```xml
<Folders>
   <SearchFolder/> 
</Folders>
```

<span data-ttu-id="9f96e-105">**Arrayoffolderstype**または**Nonemptyarrayoffolderstype**</span><span class="sxs-lookup"><span data-stu-id="9f96e-105">**ArrayOfFoldersType** or **NonEmptyArrayOfFoldersType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9f96e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9f96e-106">Attributes and elements</span></span>

<span data-ttu-id="9f96e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9f96e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f96e-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f96e-108">Attributes</span></span>

<span data-ttu-id="9f96e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9f96e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f96e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9f96e-110">Child elements</span></span>

|<span data-ttu-id="9f96e-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="9f96e-111">**Element**</span></span>|<span data-ttu-id="9f96e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9f96e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f96e-113">Folder</span><span class="sxs-lookup"><span data-stu-id="9f96e-113">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="9f96e-114">作成、取得、検索、同期、更新を行うフォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="9f96e-114">Identifies a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="9f96e-115">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="9f96e-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="9f96e-116">主に予定表アイテムを含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="9f96e-116">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="9f96e-117">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="9f96e-117">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="9f96e-118">メールボックス内の連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="9f96e-118">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9f96e-119">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="9f96e-119">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="9f96e-120">メールボックスに含まれている検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="9f96e-120">Represents a Search folder contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9f96e-121">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="9f96e-121">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="9f96e-122">メールボックス内のタスクフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="9f96e-122">Represents a Tasks folder in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f96e-123">親要素</span><span class="sxs-lookup"><span data-stu-id="9f96e-123">Parent elements</span></span>

|<span data-ttu-id="9f96e-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="9f96e-124">**Element**</span></span>|<span data-ttu-id="9f96e-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="9f96e-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f96e-126">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9f96e-126">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md) <br/> |<span data-ttu-id="9f96e-127">1つの[Copyfolder 操作](copyfolder-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="9f96e-127">Contains the status and result of a single [CopyFolder operation](copyfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="9f96e-128">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="9f96e-128">CreateFolder</span></span>](createfolder.md) <br/> |<span data-ttu-id="9f96e-129">Exchange ストア内にフォルダーを作成するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="9f96e-129">Defines a request to create a folder in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9f96e-130">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9f96e-130">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md) <br/> |<span data-ttu-id="9f96e-131">単一の[CreateFolder 操作](createfolder-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="9f96e-131">Contains the status and result of a single [CreateFolder operation](createfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="9f96e-132">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9f96e-132">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md) <br/> |<span data-ttu-id="9f96e-133">単一の[CreateManagedFolder 操作](createmanagedfolder-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="9f96e-133">Contains the status and result of a single [CreateManagedFolder operation](createmanagedfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="9f96e-134">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9f96e-134">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md) <br/> |<span data-ttu-id="9f96e-135">[Getfolder 操作](getfolder-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="9f96e-135">Contains the status and result of a [GetFolder operation](getfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="9f96e-136">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9f96e-136">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md) <br/> |<span data-ttu-id="9f96e-137">[Movefolder 操作](movefolder-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="9f96e-137">Contains the status and result of a [MoveFolder operation](movefolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="9f96e-138">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="9f96e-138">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="9f96e-139">新しいフォルダーを作成するフォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="9f96e-139">Identifies the folder where a new folder is created.</span></span>  <br/> |
|[<span data-ttu-id="9f96e-140">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="9f96e-140">RootFolder (FindFolderResponseMessage)</span></span>](rootfolder-findfolderresponsemessage.md) <br/> |<span data-ttu-id="9f96e-141">[Findfolder 操作](findfolder-operation.md)中に1つのルートフォルダーを検索した結果が格納されます。</span><span class="sxs-lookup"><span data-stu-id="9f96e-141">Contains the results from searching a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="9f96e-142">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9f96e-142">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md) <br/> |<span data-ttu-id="9f96e-143">1つの[Updatefolder 操作](updatefolder-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="9f96e-143">Contains the status and result of a single [UpdateFolder operation](updatefolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9f96e-144">注釈</span><span class="sxs-lookup"><span data-stu-id="9f96e-144">Remarks</span></span>

<span data-ttu-id="9f96e-145">この要素は、 [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素の必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="9f96e-145">This element is a required child element of the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span> 
  
<span data-ttu-id="9f96e-146">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="9f96e-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f96e-147">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9f96e-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f96e-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="9f96e-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9f96e-149">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9f96e-149">Schema Name</span></span>  <br/> |<span data-ttu-id="9f96e-150">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9f96e-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="9f96e-151">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9f96e-151">Validation File</span></span>  <br/> |<span data-ttu-id="9f96e-152">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9f96e-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9f96e-153">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9f96e-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="9f96e-154">正しくない</span><span class="sxs-lookup"><span data-stu-id="9f96e-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f96e-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="9f96e-155">See also</span></span>

- [<span data-ttu-id="9f96e-156">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="9f96e-156">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)


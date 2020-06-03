---
title: Update (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Update
api_type:
- schema
ms.assetid: 47ed8edb-2a94-471b-b965-93f91456252e
description: Update 要素は、ローカルクライアントストアで更新する1つのフォルダーを識別します。
ms.openlocfilehash: 5c1b5b1fd87e4651125293eac431c56f732c6c02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467138"
---
# <a name="update-foldersync"></a><span data-ttu-id="e1389-103">Update (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="e1389-103">Update (FolderSync)</span></span>

<span data-ttu-id="e1389-104">**Update**要素は、ローカルクライアントストアで更新する1つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="e1389-104">The **Update** element identifies a single folder to update in the local client store.</span></span> 
  
- [<span data-ttu-id="e1389-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="e1389-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md) 
- [<span data-ttu-id="e1389-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e1389-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="e1389-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e1389-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)  
- [<span data-ttu-id="e1389-108">変更 (階層)</span><span class="sxs-lookup"><span data-stu-id="e1389-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md) 
- [<span data-ttu-id="e1389-109">Update (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="e1389-109">Update (FolderSync)</span></span>](update-foldersync.md)
  
```xml
<Update>
   <Folder/>
</Update>
```

```xml
<Update>
   <CalendarFolder/>
</Update>
```

```xml
<Update>
   <ContactsFolder/>
</Update>
```

```xml
<Update>
   <TasksFolder/>
</Update>
```

```xml
<Update>
   <SearchFolder/>
</Update>
```

<span data-ttu-id="e1389-110">**SyncFolderHierarchyCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="e1389-110">**SyncFolderHierarchyCreateOrUpdateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e1389-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e1389-111">Attributes and elements</span></span>

<span data-ttu-id="e1389-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e1389-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1389-113">属性</span><span class="sxs-lookup"><span data-stu-id="e1389-113">Attributes</span></span>

<span data-ttu-id="e1389-114">なし。</span><span class="sxs-lookup"><span data-stu-id="e1389-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1389-115">子要素</span><span class="sxs-lookup"><span data-stu-id="e1389-115">Child elements</span></span>

|<span data-ttu-id="e1389-116">**Element**</span><span class="sxs-lookup"><span data-stu-id="e1389-116">**Element**</span></span>|<span data-ttu-id="e1389-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="e1389-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1389-118">Folder</span><span class="sxs-lookup"><span data-stu-id="e1389-118">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="e1389-119">作成、取得、検索、同期、または更新するフォルダーを定義します。</span><span class="sxs-lookup"><span data-stu-id="e1389-119">Defines the folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="e1389-120">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="e1389-120">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="e1389-121">主に予定表アイテムを含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="e1389-121">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="e1389-122">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="e1389-122">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="e1389-123">メールボックス内の連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="e1389-123">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e1389-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="e1389-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="e1389-125">メールボックスに含まれている検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="e1389-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e1389-126">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="e1389-126">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="e1389-127">メールボックスに含まれているタスクフォルダー t を表します。</span><span class="sxs-lookup"><span data-stu-id="e1389-127">Represents a task folder t is thcontained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e1389-128">親要素</span><span class="sxs-lookup"><span data-stu-id="e1389-128">Parent elements</span></span>

|<span data-ttu-id="e1389-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="e1389-129">**Element**</span></span>|<span data-ttu-id="e1389-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="e1389-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1389-131">変更 (階層)</span><span class="sxs-lookup"><span data-stu-id="e1389-131">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="e1389-132">クライアント上のフォルダーと Exchange サーバー上のフォルダーとの相違点の種類を表す、変更の種類のシーケンス配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="e1389-132">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e1389-133">注釈</span><span class="sxs-lookup"><span data-stu-id="e1389-133">Remarks</span></span>

<span data-ttu-id="e1389-134">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e1389-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1389-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e1389-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1389-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="e1389-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e1389-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e1389-137">Schema name</span></span>  <br/> |<span data-ttu-id="e1389-138">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e1389-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="e1389-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e1389-139">Validation file</span></span>  <br/> |<span data-ttu-id="e1389-140">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e1389-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e1389-141">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e1389-141">Can be empty</span></span>  <br/> |<span data-ttu-id="e1389-142">正しくない</span><span class="sxs-lookup"><span data-stu-id="e1389-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e1389-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="e1389-143">See also</span></span>

- [<span data-ttu-id="e1389-144">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="e1389-144">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="e1389-145">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e1389-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


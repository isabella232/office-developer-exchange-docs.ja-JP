---
title: 更新 (集合的)
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
description: 更新プログラム要素は、ローカル クライアント ストアで更新する 1 つのフォルダーを識別します。
ms.openlocfilehash: 6d4a6233df41ea95e1fd9b394502bfb2728bddb6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839825"
---
# <a name="update-foldersync"></a><span data-ttu-id="40bed-103">更新 (集合的)</span><span class="sxs-lookup"><span data-stu-id="40bed-103">Update (FolderSync)</span></span>

<span data-ttu-id="40bed-104">**Update**要素は、ローカル クライアント ストアで更新する 1 つのフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="40bed-104">The **Update** element identifies a single folder to update in the local client store.</span></span> 
  
[<span data-ttu-id="40bed-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="40bed-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="40bed-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="40bed-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="40bed-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="40bed-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="40bed-108">(階層) の変更</span><span class="sxs-lookup"><span data-stu-id="40bed-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
  
[<span data-ttu-id="40bed-109">更新 (集合的)</span><span class="sxs-lookup"><span data-stu-id="40bed-109">Update (FolderSync)</span></span>](update-foldersync.md)
  
```xml
<Update>
   <Folder/>
</Update>
```

 <span data-ttu-id="40bed-110">**SyncFolderHierarchyCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="40bed-110">**SyncFolderHierarchyCreateOrUpdateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="40bed-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="40bed-111">Attributes and elements</span></span>

<span data-ttu-id="40bed-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="40bed-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40bed-113">属性</span><span class="sxs-lookup"><span data-stu-id="40bed-113">Attributes</span></span>

<span data-ttu-id="40bed-114">なし。</span><span class="sxs-lookup"><span data-stu-id="40bed-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="40bed-115">子要素</span><span class="sxs-lookup"><span data-stu-id="40bed-115">Child elements</span></span>

|<span data-ttu-id="40bed-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="40bed-116">**Element**</span></span>|<span data-ttu-id="40bed-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="40bed-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40bed-118">Folder</span><span class="sxs-lookup"><span data-stu-id="40bed-118">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="40bed-119">作成、取得、検索、同期、または更新するフォルダーを定義します。</span><span class="sxs-lookup"><span data-stu-id="40bed-119">Defines the folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="40bed-120">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="40bed-120">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="40bed-121">主に予定表のアイテムを含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="40bed-121">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="40bed-122">メッセージ</span><span class="sxs-lookup"><span data-stu-id="40bed-122">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="40bed-123">メールボックスの連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="40bed-123">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="40bed-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="40bed-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="40bed-125">メールボックスに格納されている検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="40bed-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="40bed-126">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="40bed-126">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="40bed-127">タスクを表す t] フォルダーは、メールボックス内の thcontained です。</span><span class="sxs-lookup"><span data-stu-id="40bed-127">Represents a task folder t is thcontained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="40bed-128">親要素</span><span class="sxs-lookup"><span data-stu-id="40bed-128">Parent elements</span></span>

|<span data-ttu-id="40bed-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="40bed-129">**Element**</span></span>|<span data-ttu-id="40bed-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="40bed-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40bed-131">(階層) の変更</span><span class="sxs-lookup"><span data-stu-id="40bed-131">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="40bed-132">クライアント上のフォルダーと Exchange サーバー上のフォルダーの相違点の種類を表すの種類の変更の順序付けされた配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="40bed-132">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="40bed-133">備考</span><span class="sxs-lookup"><span data-stu-id="40bed-133">Remarks</span></span>

<span data-ttu-id="40bed-134">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="40bed-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="40bed-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="40bed-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="40bed-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="40bed-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="40bed-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="40bed-137">Schema name</span></span>  <br/> |<span data-ttu-id="40bed-138">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="40bed-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="40bed-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="40bed-139">Validation file</span></span>  <br/> |<span data-ttu-id="40bed-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="40bed-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="40bed-141">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="40bed-141">Can be empty</span></span>  <br/> |<span data-ttu-id="40bed-142">False</span><span class="sxs-lookup"><span data-stu-id="40bed-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="40bed-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="40bed-143">See also</span></span>



[<span data-ttu-id="40bed-144">SyncFolderItems の操作</span><span class="sxs-lookup"><span data-stu-id="40bed-144">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="40bed-145">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="40bed-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


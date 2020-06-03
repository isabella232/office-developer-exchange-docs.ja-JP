---
title: DeleteFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: e37963f4-af9e-4481-b389-16175711e66d
description: DeleteFolder 要素は、Exchange ストア内のメールボックスからフォルダーを削除するための要求を定義します。
ms.openlocfilehash: eb705a47b78b19c79b2e87561ba3696ed40e09cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458769"
---
# <a name="deletefolder"></a><span data-ttu-id="3e064-103">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="3e064-103">DeleteFolder</span></span>

<span data-ttu-id="3e064-104">**Deletefolder**要素は、Exchange ストア内のメールボックスからフォルダーを削除するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="3e064-104">The **DeleteFolder** element defines a request to delete folders from a mailbox in the Exchange store.</span></span> 
  
```XML
<DeleteFolder DeleteType="">
   <FolderIds/>
</DeleteFolder>
```

 <span data-ttu-id="3e064-105">**DeleteFolderType**</span><span class="sxs-lookup"><span data-stu-id="3e064-105">**DeleteFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3e064-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3e064-106">Attributes and elements</span></span>

<span data-ttu-id="3e064-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3e064-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3e064-108">属性</span><span class="sxs-lookup"><span data-stu-id="3e064-108">Attributes</span></span>

|<span data-ttu-id="3e064-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="3e064-109">**Attribute**</span></span>|<span data-ttu-id="3e064-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="3e064-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3e064-111">**DeleteType**</span><span class="sxs-lookup"><span data-stu-id="3e064-111">**DeleteType**</span></span> <br/> |<span data-ttu-id="3e064-112">フォルダーが削除される方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="3e064-112">Describes how a folder is deleted.</span></span> <span data-ttu-id="3e064-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="3e064-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="3e064-114">DeleteType 属性</span><span class="sxs-lookup"><span data-stu-id="3e064-114">DeleteType attribute</span></span>

|<span data-ttu-id="3e064-115">**値**</span><span class="sxs-lookup"><span data-stu-id="3e064-115">**Value**</span></span>|<span data-ttu-id="3e064-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="3e064-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3e064-117">HardDelete</span><span class="sxs-lookup"><span data-stu-id="3e064-117">HardDelete</span></span>  <br/> |<span data-ttu-id="3e064-118">フォルダーがストアから完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="3e064-118">A folder is permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="3e064-119">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="3e064-119">SoftDelete</span></span>  <br/> |<span data-ttu-id="3e064-120">収集が有効になっている場合、フォルダーは収集に移動されます。</span><span class="sxs-lookup"><span data-stu-id="3e064-120">A folder is moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="3e064-121">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="3e064-121">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="3e064-122">フォルダーが [削除済みアイテム] フォルダーに移動されます。</span><span class="sxs-lookup"><span data-stu-id="3e064-122">A folder is moved to the Deleted Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3e064-123">子要素</span><span class="sxs-lookup"><span data-stu-id="3e064-123">Child elements</span></span>

|<span data-ttu-id="3e064-124">**Element**</span><span class="sxs-lookup"><span data-stu-id="3e064-124">**Element**</span></span>|<span data-ttu-id="3e064-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="3e064-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e064-126">FolderIds</span><span class="sxs-lookup"><span data-stu-id="3e064-126">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="3e064-127">削除するフォルダーを識別するために使用されるフォルダー識別子の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="3e064-127">Contains an array of folder identifiers that are used to identify folders to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3e064-128">親要素</span><span class="sxs-lookup"><span data-stu-id="3e064-128">Parent elements</span></span>

<span data-ttu-id="3e064-129">なし。</span><span class="sxs-lookup"><span data-stu-id="3e064-129">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3e064-130">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3e064-130">Text value</span></span>

<span data-ttu-id="3e064-131">なし。</span><span class="sxs-lookup"><span data-stu-id="3e064-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3e064-132">注釈</span><span class="sxs-lookup"><span data-stu-id="3e064-132">Remarks</span></span>

<span data-ttu-id="3e064-133">**MoveToDeletedItems**および**ハード削除**オプションは、トランザクションであり、Web サービスの呼び出しが完了すると、データベースがアイテムを削除済みアイテムフォルダーに移動したか、または Exchange データベースからアイテムを完全に削除したことを意味します。</span><span class="sxs-lookup"><span data-stu-id="3e064-133">The **MoveToDeletedItems** and **HardDelete** options are transactional, which means that by the time a Web service call completes, the database has moved the item to the Deleted Items folder or permanently removed the item from the Exchange database.</span></span> <span data-ttu-id="3e064-134">この動作は、Microsoft Exchange Server 2007 および Exchange Server 2010 の場合と同じです。</span><span class="sxs-lookup"><span data-stu-id="3e064-134">This behavior is the same for MicrosoftExchange Server 2007 and Exchange Server 2010.</span></span> 
  
<span data-ttu-id="3e064-135">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3e064-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3e064-136">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3e064-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3e064-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="3e064-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3e064-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3e064-138">Schema Name</span></span>  <br/> |<span data-ttu-id="3e064-139">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="3e064-139">Message schema</span></span>  <br/> |
|<span data-ttu-id="3e064-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3e064-140">Validation File</span></span>  <br/> |<span data-ttu-id="3e064-141">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3e064-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3e064-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3e064-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="3e064-143">正しくない</span><span class="sxs-lookup"><span data-stu-id="3e064-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3e064-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="3e064-144">See also</span></span>

- [<span data-ttu-id="3e064-145">DeleteFolder 操作 </span><span class="sxs-lookup"><span data-stu-id="3e064-145">DeleteFolder operation</span></span>](deletefolder-operation.md)


---
title: EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 502b2841-103d-4340-97d5-51a1db813fb2
description: EmptyFolder 要素は、Exchange ストア内のメールボックス内のフォルダーを空にする要求を定義します。 必要に応じて、フォルダーを空にしたときにサブフォルダーを削除することもできます。
ms.openlocfilehash: a42e4e3f25741a96ee65fe6f87fc3236b68f4dc9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457278"
---
# <a name="emptyfolder"></a><span data-ttu-id="69516-104">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="69516-104">EmptyFolder</span></span>

<span data-ttu-id="69516-105">**Emptyfolder**要素は、Exchange ストア内のメールボックス内のフォルダーを空にする要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="69516-105">The **EmptyFolder** element defines a request to empty a folder in a mailbox in the Exchange store.</span></span> <span data-ttu-id="69516-106">必要に応じて、フォルダーを空にしたときにサブフォルダーを削除することもできます。</span><span class="sxs-lookup"><span data-stu-id="69516-106">Optionally, subfolders can also be deleted when the folder is emptied.</span></span> 
  
```XML
<EmptyFolder>
   <FolderIds/>
</EmptyFolder>
```

 <span data-ttu-id="69516-107">**EmptyFolderType**</span><span class="sxs-lookup"><span data-stu-id="69516-107">**EmptyFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="69516-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="69516-108">Attributes and elements</span></span>

<span data-ttu-id="69516-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="69516-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69516-110">属性</span><span class="sxs-lookup"><span data-stu-id="69516-110">Attributes</span></span>

|<span data-ttu-id="69516-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="69516-111">**Attribute**</span></span>|<span data-ttu-id="69516-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="69516-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="69516-113">**DeleteType**</span><span class="sxs-lookup"><span data-stu-id="69516-113">**DeleteType**</span></span> <br/> |<span data-ttu-id="69516-114">フォルダーを空にする方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="69516-114">Specifies how a folder is emptied.</span></span> <span data-ttu-id="69516-115">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="69516-115">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="69516-116">**DeleteSubFolders**</span><span class="sxs-lookup"><span data-stu-id="69516-116">**DeleteSubFolders**</span></span> <br/> |<span data-ttu-id="69516-117">サブフォルダーを削除するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="69516-117">Specifies whether subfolders are to be deleted.</span></span> <span data-ttu-id="69516-118">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="69516-118">This attribute is required.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="69516-119">DeleteType 属性</span><span class="sxs-lookup"><span data-stu-id="69516-119">DeleteType Attribute</span></span>

|<span data-ttu-id="69516-120">**値**</span><span class="sxs-lookup"><span data-stu-id="69516-120">**Value**</span></span>|<span data-ttu-id="69516-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="69516-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="69516-122">HardDelete</span><span class="sxs-lookup"><span data-stu-id="69516-122">HardDelete</span></span>  <br/> |<span data-ttu-id="69516-123">メッセージとフォルダーがストアから完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="69516-123">A messages and folders are permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="69516-124">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="69516-124">SoftDelete</span></span>  <br/> |<span data-ttu-id="69516-125">収集が有効になっている場合、メッセージとフォルダーは収集に移動されます。</span><span class="sxs-lookup"><span data-stu-id="69516-125">A messages and folders are moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="69516-126">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="69516-126">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="69516-127">メッセージとフォルダーが [削除済みアイテム] フォルダーに移動されます。</span><span class="sxs-lookup"><span data-stu-id="69516-127">A messages and folders are moved to the Deleted Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="69516-128">子要素</span><span class="sxs-lookup"><span data-stu-id="69516-128">Child elements</span></span>

|<span data-ttu-id="69516-129">**Element**</span><span class="sxs-lookup"><span data-stu-id="69516-129">**Element**</span></span>|<span data-ttu-id="69516-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="69516-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69516-131">FolderIds</span><span class="sxs-lookup"><span data-stu-id="69516-131">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="69516-132">削除するフォルダーを識別するために使用されるフォルダー識別子の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="69516-132">Contains an array of folder identifiers that are used to identify folders to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="69516-133">親要素</span><span class="sxs-lookup"><span data-stu-id="69516-133">Parent elements</span></span>

<span data-ttu-id="69516-134">なし。</span><span class="sxs-lookup"><span data-stu-id="69516-134">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="69516-135">テキスト値</span><span class="sxs-lookup"><span data-stu-id="69516-135">Text value</span></span>

<span data-ttu-id="69516-136">なし。</span><span class="sxs-lookup"><span data-stu-id="69516-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="69516-137">注釈</span><span class="sxs-lookup"><span data-stu-id="69516-137">Remarks</span></span>

<span data-ttu-id="69516-138">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="69516-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69516-139">要素の情報</span><span class="sxs-lookup"><span data-stu-id="69516-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69516-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="69516-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="69516-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="69516-141">Schema Name</span></span>  <br/> |<span data-ttu-id="69516-142">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="69516-142">Message schema</span></span>  <br/> |
|<span data-ttu-id="69516-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="69516-143">Validation File</span></span>  <br/> |<span data-ttu-id="69516-144">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="69516-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="69516-145">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="69516-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="69516-146">正しくない</span><span class="sxs-lookup"><span data-stu-id="69516-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69516-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="69516-147">See also</span></span>



[<span data-ttu-id="69516-148">EmptyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="69516-148">EmptyFolder operation</span></span>](emptyfolder-operation.md)


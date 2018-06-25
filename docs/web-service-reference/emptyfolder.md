---
title: EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 502b2841-103d-4340-97d5-51a1db813fb2
description: EmptyFolder 要素は、Exchange ストア内のメールボックス内のフォルダーを空にする要求を定義します。 オプションでは、サブフォルダーは、フォルダーを空にしたときにも削除できます。
ms.openlocfilehash: c72e11cea29e2e55c9c29754eec60e73bd1e4d9c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760269"
---
# <a name="emptyfolder"></a><span data-ttu-id="49a63-104">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="49a63-104">EmptyFolder</span></span>

<span data-ttu-id="49a63-105">**EmptyFolder**要素は、Exchange ストア内のメールボックス内のフォルダーを空にする要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="49a63-105">The **EmptyFolder** element defines a request to empty a folder in a mailbox in the Exchange store.</span></span> <span data-ttu-id="49a63-106">オプションでは、サブフォルダーは、フォルダーを空にしたときにも削除できます。</span><span class="sxs-lookup"><span data-stu-id="49a63-106">Optionally, subfolders can also be deleted when the folder is emptied.</span></span> 
  
```XML
<EmptyFolder>
   <FolderIds/>
</EmptyFolder>
```

 <span data-ttu-id="49a63-107">**EmptyFolderType**</span><span class="sxs-lookup"><span data-stu-id="49a63-107">**EmptyFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="49a63-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="49a63-108">Attributes and elements</span></span>

<span data-ttu-id="49a63-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="49a63-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49a63-110">属性</span><span class="sxs-lookup"><span data-stu-id="49a63-110">Attributes</span></span>

|<span data-ttu-id="49a63-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="49a63-111">**Attribute**</span></span>|<span data-ttu-id="49a63-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="49a63-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="49a63-113">**削除の種類**</span><span class="sxs-lookup"><span data-stu-id="49a63-113">**DeleteType**</span></span> <br/> |<span data-ttu-id="49a63-114">フォルダーを空にする方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="49a63-114">Specifies how a folder is emptied.</span></span> <span data-ttu-id="49a63-115">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="49a63-115">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="49a63-116">**DeleteSubFolders**</span><span class="sxs-lookup"><span data-stu-id="49a63-116">**DeleteSubFolders**</span></span> <br/> |<span data-ttu-id="49a63-117">サブフォルダーを削除するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="49a63-117">Specifies whether subfolders are to be deleted.</span></span> <span data-ttu-id="49a63-118">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="49a63-118">This attribute is required.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="49a63-119">削除の種類の属性</span><span class="sxs-lookup"><span data-stu-id="49a63-119">DeleteType Attribute</span></span>

|<span data-ttu-id="49a63-120">**値**</span><span class="sxs-lookup"><span data-stu-id="49a63-120">**Value**</span></span>|<span data-ttu-id="49a63-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="49a63-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="49a63-122">HardDelete</span><span class="sxs-lookup"><span data-stu-id="49a63-122">HardDelete</span></span>  <br/> |<span data-ttu-id="49a63-123">A メッセージおよびフォルダーがストアから完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="49a63-123">A messages and folders are permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="49a63-124">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="49a63-124">SoftDelete</span></span>  <br/> |<span data-ttu-id="49a63-125">A メッセージおよびフォルダーを移動する、ごみ箱をあさる場合、収集を有効にします。</span><span class="sxs-lookup"><span data-stu-id="49a63-125">A messages and folders are moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="49a63-126">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="49a63-126">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="49a63-127">A のメッセージとフォルダーは削除済みアイテム フォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="49a63-127">A messages and folders are moved to the Deleted Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="49a63-128">子要素</span><span class="sxs-lookup"><span data-stu-id="49a63-128">Child elements</span></span>

|<span data-ttu-id="49a63-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="49a63-129">**Element**</span></span>|<span data-ttu-id="49a63-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="49a63-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49a63-131">FolderIds</span><span class="sxs-lookup"><span data-stu-id="49a63-131">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="49a63-132">削除するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="49a63-132">Contains an array of folder identifiers that are used to identify folders to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="49a63-133">親要素</span><span class="sxs-lookup"><span data-stu-id="49a63-133">Parent elements</span></span>

<span data-ttu-id="49a63-134">なし。</span><span class="sxs-lookup"><span data-stu-id="49a63-134">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="49a63-135">テキスト値</span><span class="sxs-lookup"><span data-stu-id="49a63-135">Text value</span></span>

<span data-ttu-id="49a63-136">なし。</span><span class="sxs-lookup"><span data-stu-id="49a63-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="49a63-137">備考</span><span class="sxs-lookup"><span data-stu-id="49a63-137">Remarks</span></span>

<span data-ttu-id="49a63-138">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="49a63-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49a63-139">要素情報</span><span class="sxs-lookup"><span data-stu-id="49a63-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49a63-140">名前空間</span><span class="sxs-lookup"><span data-stu-id="49a63-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="49a63-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="49a63-141">Schema Name</span></span>  <br/> |<span data-ttu-id="49a63-142">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="49a63-142">Message schema</span></span>  <br/> |
|<span data-ttu-id="49a63-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="49a63-143">Validation File</span></span>  <br/> |<span data-ttu-id="49a63-144">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="49a63-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="49a63-145">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="49a63-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="49a63-146">False</span><span class="sxs-lookup"><span data-stu-id="49a63-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="49a63-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="49a63-147">See also</span></span>



[<span data-ttu-id="49a63-148">EmptyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="49a63-148">EmptyFolder operation</span></span>](emptyfolder-operation.md)


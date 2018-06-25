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
description: DeleteFolder 要素は、Exchange ストア内のメールボックスからフォルダーを削除する要求を定義します。
ms.openlocfilehash: d31f98f26f537104e40b303de4199f45c65f49c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759978"
---
# <a name="deletefolder"></a><span data-ttu-id="45f9b-103">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="45f9b-103">DeleteFolder</span></span>

<span data-ttu-id="45f9b-104">**DeleteFolder**要素は、Exchange ストア内のメールボックスからフォルダーを削除する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="45f9b-104">The **DeleteFolder** element defines a request to delete folders from a mailbox in the Exchange store.</span></span> 
  
```XML
<DeleteFolder DeleteType="">
   <FolderIds/>
</DeleteFolder>
```

 <span data-ttu-id="45f9b-105">**DeleteFolderType**</span><span class="sxs-lookup"><span data-stu-id="45f9b-105">**DeleteFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="45f9b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="45f9b-106">Attributes and elements</span></span>

<span data-ttu-id="45f9b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="45f9b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="45f9b-108">属性</span><span class="sxs-lookup"><span data-stu-id="45f9b-108">Attributes</span></span>

|<span data-ttu-id="45f9b-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="45f9b-109">**Attribute**</span></span>|<span data-ttu-id="45f9b-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="45f9b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="45f9b-111">**削除の種類**</span><span class="sxs-lookup"><span data-stu-id="45f9b-111">**DeleteType**</span></span> <br/> |<span data-ttu-id="45f9b-112">フォルダーを削除する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="45f9b-112">Describes how a folder is deleted.</span></span> <span data-ttu-id="45f9b-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="45f9b-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="45f9b-114">削除の種類の属性</span><span class="sxs-lookup"><span data-stu-id="45f9b-114">DeleteType attribute</span></span>

|<span data-ttu-id="45f9b-115">**値**</span><span class="sxs-lookup"><span data-stu-id="45f9b-115">**Value**</span></span>|<span data-ttu-id="45f9b-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="45f9b-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="45f9b-117">HardDelete</span><span class="sxs-lookup"><span data-stu-id="45f9b-117">HardDelete</span></span>  <br/> |<span data-ttu-id="45f9b-118">フォルダーはストアから完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="45f9b-118">A folder is permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="45f9b-119">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="45f9b-119">SoftDelete</span></span>  <br/> |<span data-ttu-id="45f9b-120">フォルダーを移動、ごみ箱をあさる場合、収集を有効にします。</span><span class="sxs-lookup"><span data-stu-id="45f9b-120">A folder is moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="45f9b-121">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="45f9b-121">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="45f9b-122">フォルダーは、削除済みアイテム フォルダーに移動されます。</span><span class="sxs-lookup"><span data-stu-id="45f9b-122">A folder is moved to the Deleted Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="45f9b-123">子要素</span><span class="sxs-lookup"><span data-stu-id="45f9b-123">Child elements</span></span>

|<span data-ttu-id="45f9b-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="45f9b-124">**Element**</span></span>|<span data-ttu-id="45f9b-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="45f9b-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45f9b-126">FolderIds</span><span class="sxs-lookup"><span data-stu-id="45f9b-126">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="45f9b-127">削除するフォルダーを識別するために使用されるフォルダー識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="45f9b-127">Contains an array of folder identifiers that are used to identify folders to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="45f9b-128">親要素</span><span class="sxs-lookup"><span data-stu-id="45f9b-128">Parent elements</span></span>

<span data-ttu-id="45f9b-129">なし。</span><span class="sxs-lookup"><span data-stu-id="45f9b-129">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="45f9b-130">テキスト値</span><span class="sxs-lookup"><span data-stu-id="45f9b-130">Text value</span></span>

<span data-ttu-id="45f9b-131">なし。</span><span class="sxs-lookup"><span data-stu-id="45f9b-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="45f9b-132">備考</span><span class="sxs-lookup"><span data-stu-id="45f9b-132">Remarks</span></span>

<span data-ttu-id="45f9b-133">**MoveToDeletedItems**および**HardDelete**オプションは、時間によって、Web サービスの呼び出しが完了していることを意味する、トランザクション、データベースは削除済みアイテム フォルダーにアイテムを移動または Exchange データベースから項目を完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="45f9b-133">The **MoveToDeletedItems** and **HardDelete** options are transactional, which means that by the time a Web service call completes, the database has moved the item to the Deleted Items folder or permanently removed the item from the Exchange database.</span></span> <span data-ttu-id="45f9b-134">この現象は、MicrosoftExchange Server 2007 および Exchange Server 2010 と同じです。</span><span class="sxs-lookup"><span data-stu-id="45f9b-134">This behavior is the same for MicrosoftExchange Server 2007 and Exchange Server 2010.</span></span> 
  
<span data-ttu-id="45f9b-135">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="45f9b-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="45f9b-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="45f9b-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="45f9b-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="45f9b-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="45f9b-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="45f9b-138">Schema Name</span></span>  <br/> |<span data-ttu-id="45f9b-139">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="45f9b-139">Message schema</span></span>  <br/> |
|<span data-ttu-id="45f9b-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="45f9b-140">Validation File</span></span>  <br/> |<span data-ttu-id="45f9b-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="45f9b-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="45f9b-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="45f9b-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="45f9b-143">False</span><span class="sxs-lookup"><span data-stu-id="45f9b-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="45f9b-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="45f9b-144">See also</span></span>

- [<span data-ttu-id="45f9b-145">DeleteFolder 操作</span><span class="sxs-lookup"><span data-stu-id="45f9b-145">DeleteFolder operation</span></span>](deletefolder-operation.md)


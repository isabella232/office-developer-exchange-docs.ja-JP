---
title: Item (UploadItemType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7058f2-615f-4393-a0d4-af76727f37e9
description: Item 要素は、メールボックスにアップロードする単一のアイテムを表します。
ms.openlocfilehash: 82c0fdf89c06ddfb812c2b2f1899b589eedeb7d8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467551"
---
# <a name="item-uploaditemtype"></a><span data-ttu-id="e9056-103">Item (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="e9056-103">Item (UploadItemType)</span></span>

<span data-ttu-id="e9056-104">**Item**要素は、メールボックスにアップロードする単一のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="e9056-104">The **Item** element represents a single item to upload into a mailbox.</span></span> 
  
[<span data-ttu-id="e9056-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="e9056-105">UploadItems</span></span>](uploaditems.md)
  
[<span data-ttu-id="e9056-106">アイテム (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="e9056-106">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md)
  
[<span data-ttu-id="e9056-107">Item (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="e9056-107">Item (UploadItemType)</span></span>](item-uploaditemtype.md)
  
```XML
<Item CreateAction="" IsAssociated="">
   <ParentFolderId/>
   <ItemId/>
   <Data/>
</Item>
```

 <span data-ttu-id="e9056-108">**UploadItemType**</span><span class="sxs-lookup"><span data-stu-id="e9056-108">**UploadItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9056-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e9056-109">Attributes and elements</span></span>

<span data-ttu-id="e9056-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e9056-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9056-111">属性</span><span class="sxs-lookup"><span data-stu-id="e9056-111">Attributes</span></span>

|<span data-ttu-id="e9056-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="e9056-112">**Attribute**</span></span>|<span data-ttu-id="e9056-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9056-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e9056-114">**CreateAction**</span><span class="sxs-lookup"><span data-stu-id="e9056-114">**CreateAction**</span></span> <br/> |<span data-ttu-id="e9056-115">メールボックスにアイテムをアップロードするアクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="e9056-115">Specifies the action for uploading an item into a mailbox.</span></span> <span data-ttu-id="e9056-116">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="e9056-116">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="e9056-117">**IsAssociated**</span><span class="sxs-lookup"><span data-stu-id="e9056-117">**IsAssociated**</span></span> <br/> |<span data-ttu-id="e9056-118">アップロードされたアイテムがフォルダーに関連付けられたアイテムであるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e9056-118">Specifies whether the uploaded item is a folder associated item.</span></span> <span data-ttu-id="e9056-119">この属性はブール値です。</span><span class="sxs-lookup"><span data-stu-id="e9056-119">This attribute is a Boolean value.</span></span> <span data-ttu-id="e9056-120">値が**true の場合**は、アイテムがフォルダーに関連付けられたアイテムであることを示します。</span><span class="sxs-lookup"><span data-stu-id="e9056-120">A value of **true** indicates that the item is a folder associated item.</span></span> <span data-ttu-id="e9056-121">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="e9056-121">This attribute is optional.</span></span>  <br/> |
   
#### <a name="createaction-attribute"></a><span data-ttu-id="e9056-122">CreateAction 属性</span><span class="sxs-lookup"><span data-stu-id="e9056-122">CreateAction Attribute</span></span>

|<span data-ttu-id="e9056-123">**値**</span><span class="sxs-lookup"><span data-stu-id="e9056-123">**Value**</span></span>|<span data-ttu-id="e9056-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9056-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e9056-125">**CreateNew**</span><span class="sxs-lookup"><span data-stu-id="e9056-125">**CreateNew**</span></span> <br/> |<span data-ttu-id="e9056-126">元のアイテムの新しいコピーがメールボックスにアップロードされることを示します。</span><span class="sxs-lookup"><span data-stu-id="e9056-126">Indicates that a new copy of the original item is uploaded to the mailbox.</span></span> <span data-ttu-id="e9056-127">CreateNew 値が使用されている場合、 [ItemId](itemid.md)要素を指定することはできません。</span><span class="sxs-lookup"><span data-stu-id="e9056-127">The [ItemId](itemid.md) element must not be present if the CreateNew value is used.</span></span> <span data-ttu-id="e9056-128">新しいアイテム識別子が応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="e9056-128">The new item identifier is returned in the response.</span></span>  <br/> |
|<span data-ttu-id="e9056-129">**Update**</span><span class="sxs-lookup"><span data-stu-id="e9056-129">**Update**</span></span> <br/> |<span data-ttu-id="e9056-130">**ItemId**要素によって指定されたアイテムが更新されるように指定します。</span><span class="sxs-lookup"><span data-stu-id="e9056-130">Specifies that the item indicated by the **ItemId** element will be updated.</span></span> <span data-ttu-id="e9056-131">**ItemId**要素が存在しない場合、またはアイテムが[ParentFolderId](parentfolderid.md)要素によって識別されるフォルダー内に存在しない場合は、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="e9056-131">An error is returned if the **ItemId** element is not present or if the item does not exist in the folder identified by the [ParentFolderId](parentfolderid.md) element.</span></span>  <br/> |
|<span data-ttu-id="e9056-132">**UpdateOrCreate**</span><span class="sxs-lookup"><span data-stu-id="e9056-132">**UpdateOrCreate**</span></span> <br/> |<span data-ttu-id="e9056-133">アイテムを更新するために最初に試行が行われたことを示します。</span><span class="sxs-lookup"><span data-stu-id="e9056-133">Indicates that an attempt is first made to update the item.</span></span> <span data-ttu-id="e9056-134">**ParentFolderId**要素によって指定されたフォルダーにアイテムが存在しない場合は、新しいアイテムが作成されます。</span><span class="sxs-lookup"><span data-stu-id="e9056-134">If the item does not exist in the folder specified by the **ParentFolderId** element, a new item is created.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e9056-135">子要素</span><span class="sxs-lookup"><span data-stu-id="e9056-135">Child elements</span></span>

|<span data-ttu-id="e9056-136">**Element**</span><span class="sxs-lookup"><span data-stu-id="e9056-136">**Element**</span></span>|<span data-ttu-id="e9056-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9056-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9056-138">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="e9056-138">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="e9056-139">新しいアイテムが作成された、または更新するアイテムを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="e9056-139">Represents the identifier of the parent folder where a new item is created or that contains the item to update.</span></span>  <br/> |
|[<span data-ttu-id="e9056-140">ItemId</span><span class="sxs-lookup"><span data-stu-id="e9056-140">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="e9056-141">Exchange ストアで作成または更新するアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9056-141">Contains the unique identifier and change key of an item to create or update in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e9056-142">Data (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="e9056-142">Data (base64Binary)</span></span>](data-base64binary.md) <br/> |<span data-ttu-id="e9056-143">メールボックスにアップロードする1つのアイテムのデータを格納します。</span><span class="sxs-lookup"><span data-stu-id="e9056-143">Contains the data of a single item to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e9056-144">親要素</span><span class="sxs-lookup"><span data-stu-id="e9056-144">Parent elements</span></span>

|<span data-ttu-id="e9056-145">**要素**</span><span class="sxs-lookup"><span data-stu-id="e9056-145">**Element**</span></span>|<span data-ttu-id="e9056-146">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9056-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9056-147">アイテム (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="e9056-147">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md) <br/> |<span data-ttu-id="e9056-148">メールボックスにアップロードするアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9056-148">Contains an array of item to upload into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e9056-149">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e9056-149">Text value</span></span>

<span data-ttu-id="e9056-150">なし。</span><span class="sxs-lookup"><span data-stu-id="e9056-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e9056-151">注釈</span><span class="sxs-lookup"><span data-stu-id="e9056-151">Remarks</span></span>

<span data-ttu-id="e9056-152">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e9056-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9056-153">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e9056-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9056-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="e9056-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9056-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e9056-155">Schema Name</span></span>  <br/> |<span data-ttu-id="e9056-156">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e9056-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="e9056-157">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e9056-157">Validation File</span></span>  <br/> |<span data-ttu-id="e9056-158">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e9056-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9056-159">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e9056-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9056-160">正しくない</span><span class="sxs-lookup"><span data-stu-id="e9056-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9056-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="e9056-161">See also</span></span>



[<span data-ttu-id="e9056-162">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="e9056-162">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="e9056-163">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="e9056-163">UploadItems operation</span></span>](uploaditems-operation.md)


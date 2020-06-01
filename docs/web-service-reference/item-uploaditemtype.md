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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467551"
---
# <a name="item-uploaditemtype"></a><span data-ttu-id="a866f-103">Item (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="a866f-103">Item (UploadItemType)</span></span>

<span data-ttu-id="a866f-104">**Item**要素は、メールボックスにアップロードする単一のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="a866f-104">The **Item** element represents a single item to upload into a mailbox.</span></span> 
  
[<span data-ttu-id="a866f-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="a866f-105">UploadItems</span></span>](uploaditems.md)
  
[<span data-ttu-id="a866f-106">アイテム (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="a866f-106">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md)
  
[<span data-ttu-id="a866f-107">Item (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="a866f-107">Item (UploadItemType)</span></span>](item-uploaditemtype.md)
  
```XML
<Item CreateAction="" IsAssociated="">
   <ParentFolderId/>
   <ItemId/>
   <Data/>
</Item>
```

 <span data-ttu-id="a866f-108">**UploadItemType**</span><span class="sxs-lookup"><span data-stu-id="a866f-108">**UploadItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a866f-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a866f-109">Attributes and elements</span></span>

<span data-ttu-id="a866f-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a866f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a866f-111">属性</span><span class="sxs-lookup"><span data-stu-id="a866f-111">Attributes</span></span>

|<span data-ttu-id="a866f-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="a866f-112">**Attribute**</span></span>|<span data-ttu-id="a866f-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="a866f-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a866f-114">**CreateAction**</span><span class="sxs-lookup"><span data-stu-id="a866f-114">**CreateAction**</span></span> <br/> |<span data-ttu-id="a866f-115">メールボックスにアイテムをアップロードするアクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="a866f-115">Specifies the action for uploading an item into a mailbox.</span></span> <span data-ttu-id="a866f-116">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="a866f-116">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="a866f-117">**IsAssociated**</span><span class="sxs-lookup"><span data-stu-id="a866f-117">**IsAssociated**</span></span> <br/> |<span data-ttu-id="a866f-118">アップロードされたアイテムがフォルダーに関連付けられたアイテムであるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a866f-118">Specifies whether the uploaded item is a folder associated item.</span></span> <span data-ttu-id="a866f-119">この属性はブール値です。</span><span class="sxs-lookup"><span data-stu-id="a866f-119">This attribute is a Boolean value.</span></span> <span data-ttu-id="a866f-120">値が**true の場合**は、アイテムがフォルダーに関連付けられたアイテムであることを示します。</span><span class="sxs-lookup"><span data-stu-id="a866f-120">A value of **true** indicates that the item is a folder associated item.</span></span> <span data-ttu-id="a866f-121">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="a866f-121">This attribute is optional.</span></span>  <br/> |
   
#### <a name="createaction-attribute"></a><span data-ttu-id="a866f-122">CreateAction 属性</span><span class="sxs-lookup"><span data-stu-id="a866f-122">CreateAction Attribute</span></span>

|<span data-ttu-id="a866f-123">**値**</span><span class="sxs-lookup"><span data-stu-id="a866f-123">**Value**</span></span>|<span data-ttu-id="a866f-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="a866f-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a866f-125">**CreateNew**</span><span class="sxs-lookup"><span data-stu-id="a866f-125">**CreateNew**</span></span> <br/> |<span data-ttu-id="a866f-126">元のアイテムの新しいコピーがメールボックスにアップロードされることを示します。</span><span class="sxs-lookup"><span data-stu-id="a866f-126">Indicates that a new copy of the original item is uploaded to the mailbox.</span></span> <span data-ttu-id="a866f-127">CreateNew 値が使用されている場合、 [ItemId](itemid.md)要素を指定することはできません。</span><span class="sxs-lookup"><span data-stu-id="a866f-127">The [ItemId](itemid.md) element must not be present if the CreateNew value is used.</span></span> <span data-ttu-id="a866f-128">新しいアイテム識別子が応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="a866f-128">The new item identifier is returned in the response.</span></span>  <br/> |
|<span data-ttu-id="a866f-129">**Update**</span><span class="sxs-lookup"><span data-stu-id="a866f-129">**Update**</span></span> <br/> |<span data-ttu-id="a866f-130">**ItemId**要素によって指定されたアイテムが更新されるように指定します。</span><span class="sxs-lookup"><span data-stu-id="a866f-130">Specifies that the item indicated by the **ItemId** element will be updated.</span></span> <span data-ttu-id="a866f-131">**ItemId**要素が存在しない場合、またはアイテムが[ParentFolderId](parentfolderid.md)要素によって識別されるフォルダー内に存在しない場合は、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="a866f-131">An error is returned if the **ItemId** element is not present or if the item does not exist in the folder identified by the [ParentFolderId](parentfolderid.md) element.</span></span>  <br/> |
|<span data-ttu-id="a866f-132">**UpdateOrCreate**</span><span class="sxs-lookup"><span data-stu-id="a866f-132">**UpdateOrCreate**</span></span> <br/> |<span data-ttu-id="a866f-133">アイテムを更新するために最初に試行が行われたことを示します。</span><span class="sxs-lookup"><span data-stu-id="a866f-133">Indicates that an attempt is first made to update the item.</span></span> <span data-ttu-id="a866f-134">**ParentFolderId**要素によって指定されたフォルダーにアイテムが存在しない場合は、新しいアイテムが作成されます。</span><span class="sxs-lookup"><span data-stu-id="a866f-134">If the item does not exist in the folder specified by the **ParentFolderId** element, a new item is created.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a866f-135">子要素</span><span class="sxs-lookup"><span data-stu-id="a866f-135">Child elements</span></span>

|<span data-ttu-id="a866f-136">**Element**</span><span class="sxs-lookup"><span data-stu-id="a866f-136">**Element**</span></span>|<span data-ttu-id="a866f-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="a866f-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a866f-138">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="a866f-138">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="a866f-139">新しいアイテムが作成された、または更新するアイテムを含む親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="a866f-139">Represents the identifier of the parent folder where a new item is created or that contains the item to update.</span></span>  <br/> |
|[<span data-ttu-id="a866f-140">ItemId</span><span class="sxs-lookup"><span data-stu-id="a866f-140">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="a866f-141">Exchange ストアで作成または更新するアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a866f-141">Contains the unique identifier and change key of an item to create or update in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a866f-142">Data (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="a866f-142">Data (base64Binary)</span></span>](data-base64binary.md) <br/> |<span data-ttu-id="a866f-143">メールボックスにアップロードする1つのアイテムのデータを格納します。</span><span class="sxs-lookup"><span data-stu-id="a866f-143">Contains the data of a single item to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a866f-144">親要素</span><span class="sxs-lookup"><span data-stu-id="a866f-144">Parent elements</span></span>

|<span data-ttu-id="a866f-145">**要素**</span><span class="sxs-lookup"><span data-stu-id="a866f-145">**Element**</span></span>|<span data-ttu-id="a866f-146">**説明**</span><span class="sxs-lookup"><span data-stu-id="a866f-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a866f-147">アイテム (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="a866f-147">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md) <br/> |<span data-ttu-id="a866f-148">メールボックスにアップロードするアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a866f-148">Contains an array of item to upload into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a866f-149">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a866f-149">Text value</span></span>

<span data-ttu-id="a866f-150">なし。</span><span class="sxs-lookup"><span data-stu-id="a866f-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a866f-151">注釈</span><span class="sxs-lookup"><span data-stu-id="a866f-151">Remarks</span></span>

<span data-ttu-id="a866f-152">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a866f-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a866f-153">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a866f-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a866f-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="a866f-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a866f-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a866f-155">Schema Name</span></span>  <br/> |<span data-ttu-id="a866f-156">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a866f-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="a866f-157">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a866f-157">Validation File</span></span>  <br/> |<span data-ttu-id="a866f-158">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a866f-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a866f-159">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a866f-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="a866f-160">正しくない</span><span class="sxs-lookup"><span data-stu-id="a866f-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a866f-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="a866f-161">See also</span></span>



[<span data-ttu-id="a866f-162">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="a866f-162">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="a866f-163">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="a866f-163">UploadItems operation</span></span>](uploaditems-operation.md)


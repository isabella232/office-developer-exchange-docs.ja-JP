---
title: 項目 (UploadItemType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7058f2-615f-4393-a0d4-af76727f37e9
description: Item 要素は、メールボックスにアップロードする 1 つの項目を表します。
ms.openlocfilehash: 8fecef9a2368a44e38633eb9fddaa8197620f6a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832138"
---
# <a name="item-uploaditemtype"></a><span data-ttu-id="32d85-103">項目 (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="32d85-103">Item (UploadItemType)</span></span>

<span data-ttu-id="32d85-104">**Item**要素は、メールボックスにアップロードする 1 つの項目を表します。</span><span class="sxs-lookup"><span data-stu-id="32d85-104">The **Item** element represents a single item to upload into a mailbox.</span></span> 
  
[<span data-ttu-id="32d85-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="32d85-105">UploadItems</span></span>](uploaditems.md)
  
[<span data-ttu-id="32d85-106">アイテム (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="32d85-106">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md)
  
[<span data-ttu-id="32d85-107">項目 (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="32d85-107">Item (UploadItemType)</span></span>](item-uploaditemtype.md)
  
```XML
<Item CreateAction="" IsAssociated="">
   <ParentFolderId/>
   <ItemId/>
   <Data/>
</Item>
```

 <span data-ttu-id="32d85-108">**UploadItemType**</span><span class="sxs-lookup"><span data-stu-id="32d85-108">**UploadItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32d85-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="32d85-109">Attributes and elements</span></span>

<span data-ttu-id="32d85-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="32d85-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32d85-111">属性</span><span class="sxs-lookup"><span data-stu-id="32d85-111">Attributes</span></span>

|<span data-ttu-id="32d85-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="32d85-112">**Attribute**</span></span>|<span data-ttu-id="32d85-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="32d85-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="32d85-114">**CreateAction**</span><span class="sxs-lookup"><span data-stu-id="32d85-114">**CreateAction**</span></span> <br/> |<span data-ttu-id="32d85-115">メールボックスにアイテムをアップロードするアクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="32d85-115">Specifies the action for uploading an item into a mailbox.</span></span> <span data-ttu-id="32d85-116">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="32d85-116">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="32d85-117">**IsAssociated**</span><span class="sxs-lookup"><span data-stu-id="32d85-117">**IsAssociated**</span></span> <br/> |<span data-ttu-id="32d85-118">アップロードしたアイテムがフォルダーに関連付けられている項目であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="32d85-118">Specifies whether the uploaded item is a folder associated item.</span></span> <span data-ttu-id="32d85-119">この属性は、ブール値です。</span><span class="sxs-lookup"><span data-stu-id="32d85-119">This attribute is a Boolean value.</span></span> <span data-ttu-id="32d85-120">**True**の場合、項目が項目に関連付けられているフォルダーであることを示します。</span><span class="sxs-lookup"><span data-stu-id="32d85-120">A value of **true** indicates that the item is a folder associated item.</span></span> <span data-ttu-id="32d85-121">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="32d85-121">This attribute is optional.</span></span>  <br/> |
   
#### <a name="createaction-attribute"></a><span data-ttu-id="32d85-122">CreateAction 属性</span><span class="sxs-lookup"><span data-stu-id="32d85-122">CreateAction Attribute</span></span>

|<span data-ttu-id="32d85-123">**値**</span><span class="sxs-lookup"><span data-stu-id="32d85-123">**Value**</span></span>|<span data-ttu-id="32d85-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="32d85-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="32d85-125">**CreateNew**</span><span class="sxs-lookup"><span data-stu-id="32d85-125">**CreateNew**</span></span> <br/> |<span data-ttu-id="32d85-126">メールボックスを元のアイテムの新しいコピーがアップロードされたことを示します。</span><span class="sxs-lookup"><span data-stu-id="32d85-126">Indicates that a new copy of the original item is uploaded to the mailbox.</span></span> <span data-ttu-id="32d85-127">[ItemId](itemid.md)の要素に新しい値を使用する場合に存在できません。</span><span class="sxs-lookup"><span data-stu-id="32d85-127">The [ItemId](itemid.md) element must not be present if the CreateNew value is used.</span></span> <span data-ttu-id="32d85-128">新しい項目の識別子は、応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="32d85-128">The new item identifier is returned in the response.</span></span>  <br/> |
|<span data-ttu-id="32d85-129">**Update**</span><span class="sxs-lookup"><span data-stu-id="32d85-129">**Update**</span></span> <br/> |<span data-ttu-id="32d85-130">**ItemId**要素で指定された項目を更新することを指定します。</span><span class="sxs-lookup"><span data-stu-id="32d85-130">Specifies that the item indicated by the **ItemId** element will be updated.</span></span> <span data-ttu-id="32d85-131">**ItemId**の要素が存在しない場合、または[ParentFolderId](parentfolderid.md)要素で指定されたフォルダーにアイテムが存在しない場合は、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="32d85-131">An error is returned if the **ItemId** element is not present or if the item does not exist in the folder identified by the [ParentFolderId](parentfolderid.md) element.</span></span>  <br/> |
|<span data-ttu-id="32d85-132">**UpdateOrCreate**</span><span class="sxs-lookup"><span data-stu-id="32d85-132">**UpdateOrCreate**</span></span> <br/> |<span data-ttu-id="32d85-133">しようとしましたが最初の項目を更新することを示します。</span><span class="sxs-lookup"><span data-stu-id="32d85-133">Indicates that an attempt is first made to update the item.</span></span> <span data-ttu-id="32d85-134">**ParentFolderId**要素によって指定されたフォルダーにアイテムがない場合は、新しいアイテムが作成されます。</span><span class="sxs-lookup"><span data-stu-id="32d85-134">If the item does not exist in the folder specified by the **ParentFolderId** element, a new item is created.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="32d85-135">子要素</span><span class="sxs-lookup"><span data-stu-id="32d85-135">Child elements</span></span>

|<span data-ttu-id="32d85-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="32d85-136">**Element**</span></span>|<span data-ttu-id="32d85-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="32d85-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32d85-138">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="32d85-138">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="32d85-139">新しい項目を作成または更新する項目を含む位置の親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="32d85-139">Represents the identifier of the parent folder where a new item is created or that contains the item to update.</span></span>  <br/> |
|[<span data-ttu-id="32d85-140">ItemId</span><span class="sxs-lookup"><span data-stu-id="32d85-140">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="32d85-141">作成または Exchange ストア内で更新する項目の一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="32d85-141">Contains the unique identifier and change key of an item to create or update in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="32d85-142">データ (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="32d85-142">Data (base64Binary)</span></span>](data-base64binary.md) <br/> |<span data-ttu-id="32d85-143">メールボックスにアップロードする 1 つの項目のデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="32d85-143">Contains the data of a single item to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="32d85-144">親要素</span><span class="sxs-lookup"><span data-stu-id="32d85-144">Parent elements</span></span>

|<span data-ttu-id="32d85-145">**要素**</span><span class="sxs-lookup"><span data-stu-id="32d85-145">**Element**</span></span>|<span data-ttu-id="32d85-146">**説明**</span><span class="sxs-lookup"><span data-stu-id="32d85-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32d85-147">アイテム (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="32d85-147">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md) <br/> |<span data-ttu-id="32d85-148">メールボックスにアップロードするには項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="32d85-148">Contains an array of item to upload into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="32d85-149">テキスト値</span><span class="sxs-lookup"><span data-stu-id="32d85-149">Text value</span></span>

<span data-ttu-id="32d85-150">なし。</span><span class="sxs-lookup"><span data-stu-id="32d85-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="32d85-151">備考</span><span class="sxs-lookup"><span data-stu-id="32d85-151">Remarks</span></span>

<span data-ttu-id="32d85-152">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="32d85-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="32d85-153">要素情報</span><span class="sxs-lookup"><span data-stu-id="32d85-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32d85-154">名前空間</span><span class="sxs-lookup"><span data-stu-id="32d85-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="32d85-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="32d85-155">Schema Name</span></span>  <br/> |<span data-ttu-id="32d85-156">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="32d85-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="32d85-157">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="32d85-157">Validation File</span></span>  <br/> |<span data-ttu-id="32d85-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="32d85-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="32d85-159">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="32d85-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="32d85-160">False</span><span class="sxs-lookup"><span data-stu-id="32d85-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32d85-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="32d85-161">See also</span></span>



[<span data-ttu-id="32d85-162">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="32d85-162">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="32d85-163">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="32d85-163">UploadItems operation</span></span>](uploaditems-operation.md)


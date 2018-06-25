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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832138"
---
# <a name="item-uploaditemtype"></a><span data-ttu-id="ed2cf-103">項目 (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="ed2cf-103">Item (UploadItemType)</span></span>

<span data-ttu-id="ed2cf-104">**Item**要素は、メールボックスにアップロードする 1 つの項目を表します。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-104">The **Item** element represents a single item to upload into a mailbox.</span></span> 
  
[<span data-ttu-id="ed2cf-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="ed2cf-105">UploadItems</span></span>](uploaditems.md)
  
[<span data-ttu-id="ed2cf-106">アイテム (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="ed2cf-106">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md)
  
[<span data-ttu-id="ed2cf-107">項目 (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="ed2cf-107">Item (UploadItemType)</span></span>](item-uploaditemtype.md)
  
```XML
<Item CreateAction="" IsAssociated="">
   <ParentFolderId/>
   <ItemId/>
   <Data/>
</Item>
```

 <span data-ttu-id="ed2cf-108">**UploadItemType**</span><span class="sxs-lookup"><span data-stu-id="ed2cf-108">**UploadItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ed2cf-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ed2cf-109">Attributes and elements</span></span>

<span data-ttu-id="ed2cf-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed2cf-111">属性</span><span class="sxs-lookup"><span data-stu-id="ed2cf-111">Attributes</span></span>

|<span data-ttu-id="ed2cf-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="ed2cf-112">**Attribute**</span></span>|<span data-ttu-id="ed2cf-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="ed2cf-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ed2cf-114">**CreateAction**</span><span class="sxs-lookup"><span data-stu-id="ed2cf-114">**CreateAction**</span></span> <br/> |<span data-ttu-id="ed2cf-115">メールボックスにアイテムをアップロードするアクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-115">Specifies the action for uploading an item into a mailbox.</span></span> <span data-ttu-id="ed2cf-116">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-116">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="ed2cf-117">**IsAssociated**</span><span class="sxs-lookup"><span data-stu-id="ed2cf-117">**IsAssociated**</span></span> <br/> |<span data-ttu-id="ed2cf-118">アップロードしたアイテムがフォルダーに関連付けられている項目であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-118">Specifies whether the uploaded item is a folder associated item.</span></span> <span data-ttu-id="ed2cf-119">この属性は、ブール値です。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-119">This attribute is a Boolean value.</span></span> <span data-ttu-id="ed2cf-120">**True**の場合、項目が項目に関連付けられているフォルダーであることを示します。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-120">A value of **true** indicates that the item is a folder associated item.</span></span> <span data-ttu-id="ed2cf-121">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-121">This attribute is optional.</span></span>  <br/> |
   
#### <a name="createaction-attribute"></a><span data-ttu-id="ed2cf-122">CreateAction 属性</span><span class="sxs-lookup"><span data-stu-id="ed2cf-122">CreateAction Attribute</span></span>

|<span data-ttu-id="ed2cf-123">**値**</span><span class="sxs-lookup"><span data-stu-id="ed2cf-123">**Value**</span></span>|<span data-ttu-id="ed2cf-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="ed2cf-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ed2cf-125">**CreateNew**</span><span class="sxs-lookup"><span data-stu-id="ed2cf-125">**CreateNew**</span></span> <br/> |<span data-ttu-id="ed2cf-126">メールボックスを元のアイテムの新しいコピーがアップロードされたことを示します。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-126">Indicates that a new copy of the original item is uploaded to the mailbox.</span></span> <span data-ttu-id="ed2cf-127">[ItemId](itemid.md)の要素に新しい値を使用する場合に存在できません。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-127">The [ItemId](itemid.md) element must not be present if the CreateNew value is used.</span></span> <span data-ttu-id="ed2cf-128">新しい項目の識別子は、応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-128">The new item identifier is returned in the response.</span></span>  <br/> |
|<span data-ttu-id="ed2cf-129">**Update**</span><span class="sxs-lookup"><span data-stu-id="ed2cf-129">**Update**</span></span> <br/> |<span data-ttu-id="ed2cf-130">**ItemId**要素で指定された項目を更新することを指定します。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-130">Specifies that the item indicated by the **ItemId** element will be updated.</span></span> <span data-ttu-id="ed2cf-131">**ItemId**の要素が存在しない場合、または[ParentFolderId](parentfolderid.md)要素で指定されたフォルダーにアイテムが存在しない場合は、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-131">An error is returned if the **ItemId** element is not present or if the item does not exist in the folder identified by the [ParentFolderId](parentfolderid.md) element.</span></span>  <br/> |
|<span data-ttu-id="ed2cf-132">**UpdateOrCreate**</span><span class="sxs-lookup"><span data-stu-id="ed2cf-132">**UpdateOrCreate**</span></span> <br/> |<span data-ttu-id="ed2cf-133">しようとしましたが最初の項目を更新することを示します。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-133">Indicates that an attempt is first made to update the item.</span></span> <span data-ttu-id="ed2cf-134">**ParentFolderId**要素によって指定されたフォルダーにアイテムがない場合は、新しいアイテムが作成されます。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-134">If the item does not exist in the folder specified by the **ParentFolderId** element, a new item is created.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ed2cf-135">子要素</span><span class="sxs-lookup"><span data-stu-id="ed2cf-135">Child elements</span></span>

|<span data-ttu-id="ed2cf-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="ed2cf-136">**Element**</span></span>|<span data-ttu-id="ed2cf-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="ed2cf-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed2cf-138">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="ed2cf-138">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="ed2cf-139">新しい項目を作成または更新する項目を含む位置の親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-139">Represents the identifier of the parent folder where a new item is created or that contains the item to update.</span></span>  <br/> |
|[<span data-ttu-id="ed2cf-140">ItemId</span><span class="sxs-lookup"><span data-stu-id="ed2cf-140">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ed2cf-141">作成または Exchange ストア内で更新する項目の一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-141">Contains the unique identifier and change key of an item to create or update in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ed2cf-142">データ (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="ed2cf-142">Data (base64Binary)</span></span>](data-base64binary.md) <br/> |<span data-ttu-id="ed2cf-143">メールボックスにアップロードする 1 つの項目のデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-143">Contains the data of a single item to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ed2cf-144">親要素</span><span class="sxs-lookup"><span data-stu-id="ed2cf-144">Parent elements</span></span>

|<span data-ttu-id="ed2cf-145">**要素**</span><span class="sxs-lookup"><span data-stu-id="ed2cf-145">**Element**</span></span>|<span data-ttu-id="ed2cf-146">**説明**</span><span class="sxs-lookup"><span data-stu-id="ed2cf-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed2cf-147">アイテム (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="ed2cf-147">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md) <br/> |<span data-ttu-id="ed2cf-148">メールボックスにアップロードするには項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-148">Contains an array of item to upload into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ed2cf-149">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ed2cf-149">Text value</span></span>

<span data-ttu-id="ed2cf-150">なし。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ed2cf-151">備考</span><span class="sxs-lookup"><span data-stu-id="ed2cf-151">Remarks</span></span>

<span data-ttu-id="ed2cf-152">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="ed2cf-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed2cf-153">要素情報</span><span class="sxs-lookup"><span data-stu-id="ed2cf-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed2cf-154">名前空間</span><span class="sxs-lookup"><span data-stu-id="ed2cf-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ed2cf-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ed2cf-155">Schema Name</span></span>  <br/> |<span data-ttu-id="ed2cf-156">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ed2cf-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="ed2cf-157">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ed2cf-157">Validation File</span></span>  <br/> |<span data-ttu-id="ed2cf-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ed2cf-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ed2cf-159">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ed2cf-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="ed2cf-160">False</span><span class="sxs-lookup"><span data-stu-id="ed2cf-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed2cf-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="ed2cf-161">See also</span></span>



[<span data-ttu-id="ed2cf-162">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="ed2cf-162">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="ed2cf-163">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="ed2cf-163">UploadItems operation</span></span>](uploaditems-operation.md)


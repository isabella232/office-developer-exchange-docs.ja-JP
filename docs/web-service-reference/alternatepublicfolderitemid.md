---
title: AlternatePublicFolderItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternatePublicFolderItemId
api_type:
- schema
ms.assetid: a67df9b9-8fdb-42de-b9c5-8377b71fa3d9
description: AlternatePublicFolderItemId 要素は、別の識別子の形式に変換する、パブリック フォルダー アイテムの識別子について説明します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 2240f3ff80c2c5b705611c3cf9286faa62d204cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759318"
---
# <a name="alternatepublicfolderitemid"></a><span data-ttu-id="fb13c-104">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="fb13c-104">AlternatePublicFolderItemId</span></span>

<span data-ttu-id="fb13c-105">**AlternatePublicFolderItemId**要素は、別の識別子の形式に変換する、パブリック フォルダー アイテムの識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="fb13c-105">The **AlternatePublicFolderItemId** element describes a public folder item identifier to convert to another identifier format.</span></span> <span data-ttu-id="fb13c-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fb13c-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
- [<span data-ttu-id="fb13c-107">ConvertId</span><span class="sxs-lookup"><span data-stu-id="fb13c-107">ConvertId</span></span>](convertid.md)
  
- [<span data-ttu-id="fb13c-108">SourceIds</span><span class="sxs-lookup"><span data-stu-id="fb13c-108">SourceIds</span></span>](sourceids.md)
  
- [<span data-ttu-id="fb13c-109">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="fb13c-109">AlternatePublicFolderItemId</span></span>](alternatepublicfolderitemid.md)
  
```xml
<AlternatePublicFolderItemId FolderId="" Format="" ItemId=""/>
```

 <span data-ttu-id="fb13c-110">**AlternatePublicFolderItemIdType**</span><span class="sxs-lookup"><span data-stu-id="fb13c-110">**AlternatePublicFolderItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb13c-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fb13c-111">Attributes and elements</span></span>

<span data-ttu-id="fb13c-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fb13c-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb13c-113">属性</span><span class="sxs-lookup"><span data-stu-id="fb13c-113">Attributes</span></span>

|<span data-ttu-id="fb13c-114">**属性**</span><span class="sxs-lookup"><span data-stu-id="fb13c-114">**Attribute**</span></span>|<span data-ttu-id="fb13c-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb13c-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fb13c-116">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="fb13c-116">FolderId</span></span>  <br/> |<span data-ttu-id="fb13c-117">パブリック フォルダーのアイテムを含むパブリック フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="fb13c-117">Identifies the public folder that contains the public folder item.</span></span> <span data-ttu-id="fb13c-118">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="fb13c-118">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="fb13c-119">Format</span><span class="sxs-lookup"><span data-stu-id="fb13c-119">Format</span></span>  <br/> |<span data-ttu-id="fb13c-120">変換するパブリック フォルダーの項目の識別子を記述する形式を識別します。</span><span class="sxs-lookup"><span data-stu-id="fb13c-120">Identifies the format that describes the public folder item identifier to convert.</span></span> <span data-ttu-id="fb13c-121">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="fb13c-121">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="fb13c-122">ItemId</span><span class="sxs-lookup"><span data-stu-id="fb13c-122">ItemId</span></span>  <br/> |<span data-ttu-id="fb13c-123">変換するパブリック フォルダーのアイテムの識別子です。</span><span class="sxs-lookup"><span data-stu-id="fb13c-123">Identifier the public folder item to convert.</span></span> <span data-ttu-id="fb13c-124">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="fb13c-124">This attribute is required.</span></span>  <br/> |
   
#### <a name="format-attribute-values"></a><span data-ttu-id="fb13c-125">属性の値を書式設定</span><span class="sxs-lookup"><span data-stu-id="fb13c-125">Format attribute values</span></span>

|<span data-ttu-id="fb13c-126">**値**</span><span class="sxs-lookup"><span data-stu-id="fb13c-126">**Value**</span></span>|<span data-ttu-id="fb13c-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb13c-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fb13c-128">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="fb13c-128">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="fb13c-129">Exchange 2007 の最初のリリース版の Exchange Web サービスによって生成される識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="fb13c-129">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="fb13c-130">EwsId</span><span class="sxs-lookup"><span data-stu-id="fb13c-130">EwsId</span></span>  <br/> |<span data-ttu-id="fb13c-131">Exchange 2007 SP1 以降の Exchange Web サービスによって生成される識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="fb13c-131">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="fb13c-132">EntryId</span><span class="sxs-lookup"><span data-stu-id="fb13c-132">EntryId</span></span>  <br/> |<span data-ttu-id="fb13c-133">PR_ENTRYID プロパティと同様に、MAPI 識別子をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="fb13c-133">Describes MAPI identifiers, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="fb13c-134">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="fb13c-134">HexEntryId</span></span>  <br/> |<span data-ttu-id="fb13c-135">PR_ENTRYID プロパティの 16 進数でエンコードされた表現を説明します。</span><span class="sxs-lookup"><span data-stu-id="fb13c-135">Describes a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span> <span data-ttu-id="fb13c-136">これは、可用性の予定表のイベント識別子の形式です。</span><span class="sxs-lookup"><span data-stu-id="fb13c-136">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="fb13c-137">StoreId</span><span class="sxs-lookup"><span data-stu-id="fb13c-137">StoreId</span></span>  <br/> |<span data-ttu-id="fb13c-138">Exchange ストア識別子をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="fb13c-138">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="fb13c-139">OwaId</span><span class="sxs-lookup"><span data-stu-id="fb13c-139">OwaId</span></span>  <br/> |<span data-ttu-id="fb13c-140">Outlook Web Access 識別子をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="fb13c-140">Describes an Outlook Web Access identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fb13c-141">子要素</span><span class="sxs-lookup"><span data-stu-id="fb13c-141">Child elements</span></span>

<span data-ttu-id="fb13c-142">なし。</span><span class="sxs-lookup"><span data-stu-id="fb13c-142">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fb13c-143">親要素</span><span class="sxs-lookup"><span data-stu-id="fb13c-143">Parent elements</span></span>

|<span data-ttu-id="fb13c-144">**要素**</span><span class="sxs-lookup"><span data-stu-id="fb13c-144">**Element**</span></span>|<span data-ttu-id="fb13c-145">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb13c-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb13c-146">SourceIds</span><span class="sxs-lookup"><span data-stu-id="fb13c-146">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="fb13c-147">変換するソース識別子が含まれます。</span><span class="sxs-lookup"><span data-stu-id="fb13c-147">Contains the source identifiers to convert.</span></span> <span data-ttu-id="fb13c-148">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fb13c-148">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fb13c-149">備考</span><span class="sxs-lookup"><span data-stu-id="fb13c-149">Remarks</span></span>

<span data-ttu-id="fb13c-150">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="fb13c-150">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb13c-151">要素情報</span><span class="sxs-lookup"><span data-stu-id="fb13c-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb13c-152">名前空間</span><span class="sxs-lookup"><span data-stu-id="fb13c-152">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fb13c-153">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fb13c-153">Schema Name</span></span>  <br/> |<span data-ttu-id="fb13c-154">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="fb13c-154">Types schema</span></span>  <br/> |
|<span data-ttu-id="fb13c-155">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fb13c-155">Validation File</span></span>  <br/> |<span data-ttu-id="fb13c-156">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fb13c-156">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fb13c-157">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fb13c-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="fb13c-158">True</span><span class="sxs-lookup"><span data-stu-id="fb13c-158">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb13c-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="fb13c-159">See also</span></span>

- [<span data-ttu-id="fb13c-160">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="fb13c-160">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="fb13c-161">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="fb13c-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="fb13c-162">識別子に変換します。</span><span class="sxs-lookup"><span data-stu-id="fb13c-162">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)


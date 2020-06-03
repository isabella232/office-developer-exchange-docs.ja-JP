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
description: AlternatePublicFolderItemId 要素は、別の識別子形式に変換するためのパブリックフォルダーアイテム識別子を表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 11a9fafec78a9bd14e4d98982fd38954d45e4d1a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464771"
---
# <a name="alternatepublicfolderitemid"></a><span data-ttu-id="d6e5c-104">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="d6e5c-104">AlternatePublicFolderItemId</span></span>

<span data-ttu-id="d6e5c-105">**Alternatepublicfolderitemid**要素は、別の識別子形式に変換するためのパブリックフォルダーアイテム識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-105">The **AlternatePublicFolderItemId** element describes a public folder item identifier to convert to another identifier format.</span></span> <span data-ttu-id="d6e5c-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
- [<span data-ttu-id="d6e5c-107">ConvertId</span><span class="sxs-lookup"><span data-stu-id="d6e5c-107">ConvertId</span></span>](convertid.md)
  
- [<span data-ttu-id="d6e5c-108">SourceIds</span><span class="sxs-lookup"><span data-stu-id="d6e5c-108">SourceIds</span></span>](sourceids.md)
  
- [<span data-ttu-id="d6e5c-109">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="d6e5c-109">AlternatePublicFolderItemId</span></span>](alternatepublicfolderitemid.md)
  
```xml
<AlternatePublicFolderItemId FolderId="" Format="" ItemId=""/>
```

 <span data-ttu-id="d6e5c-110">**AlternatePublicFolderItemIdType**</span><span class="sxs-lookup"><span data-stu-id="d6e5c-110">**AlternatePublicFolderItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d6e5c-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d6e5c-111">Attributes and elements</span></span>

<span data-ttu-id="d6e5c-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6e5c-113">属性</span><span class="sxs-lookup"><span data-stu-id="d6e5c-113">Attributes</span></span>

|<span data-ttu-id="d6e5c-114">**属性**</span><span class="sxs-lookup"><span data-stu-id="d6e5c-114">**Attribute**</span></span>|<span data-ttu-id="d6e5c-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="d6e5c-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d6e5c-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="d6e5c-116">FolderId</span></span>  <br/> |<span data-ttu-id="d6e5c-117">パブリックフォルダーアイテムを含むパブリックフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-117">Identifies the public folder that contains the public folder item.</span></span> <span data-ttu-id="d6e5c-118">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-118">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="d6e5c-119">Format</span><span class="sxs-lookup"><span data-stu-id="d6e5c-119">Format</span></span>  <br/> |<span data-ttu-id="d6e5c-120">変換するパブリックフォルダーアイテム識別子を説明する形式を識別します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-120">Identifies the format that describes the public folder item identifier to convert.</span></span> <span data-ttu-id="d6e5c-121">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-121">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="d6e5c-122">ItemId</span><span class="sxs-lookup"><span data-stu-id="d6e5c-122">ItemId</span></span>  <br/> |<span data-ttu-id="d6e5c-123">識別子変換するパブリックフォルダーアイテム。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-123">Identifier the public folder item to convert.</span></span> <span data-ttu-id="d6e5c-124">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-124">This attribute is required.</span></span>  <br/> |
   
#### <a name="format-attribute-values"></a><span data-ttu-id="d6e5c-125">書式属性値</span><span class="sxs-lookup"><span data-stu-id="d6e5c-125">Format attribute values</span></span>

|<span data-ttu-id="d6e5c-126">**値**</span><span class="sxs-lookup"><span data-stu-id="d6e5c-126">**Value**</span></span>|<span data-ttu-id="d6e5c-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="d6e5c-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d6e5c-128">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="d6e5c-128">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="d6e5c-129">Exchange 2007 の最初のリリースバージョンで Exchange Web サービスによって生成された識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-129">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="d6e5c-130">EwsId</span><span class="sxs-lookup"><span data-stu-id="d6e5c-130">EwsId</span></span>  <br/> |<span data-ttu-id="d6e5c-131">Exchange 2007 SP1 以降の Exchange Web サービスによって生成される識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-131">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="d6e5c-132">EntryId</span><span class="sxs-lookup"><span data-stu-id="d6e5c-132">EntryId</span></span>  <br/> |<span data-ttu-id="d6e5c-133">PR_ENTRYID プロパティのように、MAPI 識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-133">Describes MAPI identifiers, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="d6e5c-134">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="d6e5c-134">HexEntryId</span></span>  <br/> |<span data-ttu-id="d6e5c-135">PR_ENTRYID プロパティの16進数でエンコードされた表現を記述します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-135">Describes a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span> <span data-ttu-id="d6e5c-136">これは、可用性カレンダーイベント識別子の形式です。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-136">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="d6e5c-137">StoreId</span><span class="sxs-lookup"><span data-stu-id="d6e5c-137">StoreId</span></span>  <br/> |<span data-ttu-id="d6e5c-138">Exchange ストア識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-138">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="d6e5c-139">OwaId</span><span class="sxs-lookup"><span data-stu-id="d6e5c-139">OwaId</span></span>  <br/> |<span data-ttu-id="d6e5c-140">Outlook Web Access 識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-140">Describes an Outlook Web Access identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d6e5c-141">子要素</span><span class="sxs-lookup"><span data-stu-id="d6e5c-141">Child elements</span></span>

<span data-ttu-id="d6e5c-142">なし。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-142">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d6e5c-143">親要素</span><span class="sxs-lookup"><span data-stu-id="d6e5c-143">Parent elements</span></span>

|<span data-ttu-id="d6e5c-144">**要素**</span><span class="sxs-lookup"><span data-stu-id="d6e5c-144">**Element**</span></span>|<span data-ttu-id="d6e5c-145">**説明**</span><span class="sxs-lookup"><span data-stu-id="d6e5c-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6e5c-146">SourceIds</span><span class="sxs-lookup"><span data-stu-id="d6e5c-146">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="d6e5c-147">変換するソース識別子を含みます。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-147">Contains the source identifiers to convert.</span></span> <span data-ttu-id="d6e5c-148">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-148">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d6e5c-149">注釈</span><span class="sxs-lookup"><span data-stu-id="d6e5c-149">Remarks</span></span>

<span data-ttu-id="d6e5c-150">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="d6e5c-150">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d6e5c-151">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d6e5c-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6e5c-152">Namespace</span><span class="sxs-lookup"><span data-stu-id="d6e5c-152">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d6e5c-153">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d6e5c-153">Schema Name</span></span>  <br/> |<span data-ttu-id="d6e5c-154">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d6e5c-154">Types schema</span></span>  <br/> |
|<span data-ttu-id="d6e5c-155">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d6e5c-155">Validation File</span></span>  <br/> |<span data-ttu-id="d6e5c-156">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d6e5c-156">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d6e5c-157">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d6e5c-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="d6e5c-158">正しい</span><span class="sxs-lookup"><span data-stu-id="d6e5c-158">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d6e5c-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="d6e5c-159">See also</span></span>

- [<span data-ttu-id="d6e5c-160">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="d6e5c-160">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="d6e5c-161">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d6e5c-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="d6e5c-162">識別子の変換</span><span class="sxs-lookup"><span data-stu-id="d6e5c-162">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)


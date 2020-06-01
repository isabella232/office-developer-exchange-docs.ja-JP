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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464771"
---
# <a name="alternatepublicfolderitemid"></a><span data-ttu-id="72098-104">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="72098-104">AlternatePublicFolderItemId</span></span>

<span data-ttu-id="72098-105">**Alternatepublicfolderitemid**要素は、別の識別子形式に変換するためのパブリックフォルダーアイテム識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="72098-105">The **AlternatePublicFolderItemId** element describes a public folder item identifier to convert to another identifier format.</span></span> <span data-ttu-id="72098-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="72098-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
- [<span data-ttu-id="72098-107">ConvertId</span><span class="sxs-lookup"><span data-stu-id="72098-107">ConvertId</span></span>](convertid.md)
  
- [<span data-ttu-id="72098-108">SourceIds</span><span class="sxs-lookup"><span data-stu-id="72098-108">SourceIds</span></span>](sourceids.md)
  
- [<span data-ttu-id="72098-109">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="72098-109">AlternatePublicFolderItemId</span></span>](alternatepublicfolderitemid.md)
  
```xml
<AlternatePublicFolderItemId FolderId="" Format="" ItemId=""/>
```

 <span data-ttu-id="72098-110">**AlternatePublicFolderItemIdType**</span><span class="sxs-lookup"><span data-stu-id="72098-110">**AlternatePublicFolderItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="72098-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="72098-111">Attributes and elements</span></span>

<span data-ttu-id="72098-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="72098-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72098-113">属性</span><span class="sxs-lookup"><span data-stu-id="72098-113">Attributes</span></span>

|<span data-ttu-id="72098-114">**属性**</span><span class="sxs-lookup"><span data-stu-id="72098-114">**Attribute**</span></span>|<span data-ttu-id="72098-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="72098-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="72098-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="72098-116">FolderId</span></span>  <br/> |<span data-ttu-id="72098-117">パブリックフォルダーアイテムを含むパブリックフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="72098-117">Identifies the public folder that contains the public folder item.</span></span> <span data-ttu-id="72098-118">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="72098-118">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="72098-119">Format</span><span class="sxs-lookup"><span data-stu-id="72098-119">Format</span></span>  <br/> |<span data-ttu-id="72098-120">変換するパブリックフォルダーアイテム識別子を説明する形式を識別します。</span><span class="sxs-lookup"><span data-stu-id="72098-120">Identifies the format that describes the public folder item identifier to convert.</span></span> <span data-ttu-id="72098-121">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="72098-121">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="72098-122">ItemId</span><span class="sxs-lookup"><span data-stu-id="72098-122">ItemId</span></span>  <br/> |<span data-ttu-id="72098-123">識別子変換するパブリックフォルダーアイテム。</span><span class="sxs-lookup"><span data-stu-id="72098-123">Identifier the public folder item to convert.</span></span> <span data-ttu-id="72098-124">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="72098-124">This attribute is required.</span></span>  <br/> |
   
#### <a name="format-attribute-values"></a><span data-ttu-id="72098-125">書式属性値</span><span class="sxs-lookup"><span data-stu-id="72098-125">Format attribute values</span></span>

|<span data-ttu-id="72098-126">**値**</span><span class="sxs-lookup"><span data-stu-id="72098-126">**Value**</span></span>|<span data-ttu-id="72098-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="72098-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="72098-128">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="72098-128">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="72098-129">Exchange 2007 の最初のリリースバージョンで Exchange Web サービスによって生成された識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="72098-129">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="72098-130">EwsId</span><span class="sxs-lookup"><span data-stu-id="72098-130">EwsId</span></span>  <br/> |<span data-ttu-id="72098-131">Exchange 2007 SP1 以降の Exchange Web サービスによって生成される識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="72098-131">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="72098-132">EntryId</span><span class="sxs-lookup"><span data-stu-id="72098-132">EntryId</span></span>  <br/> |<span data-ttu-id="72098-133">PR_ENTRYID プロパティのように、MAPI 識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="72098-133">Describes MAPI identifiers, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="72098-134">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="72098-134">HexEntryId</span></span>  <br/> |<span data-ttu-id="72098-135">PR_ENTRYID プロパティの16進数でエンコードされた表現を記述します。</span><span class="sxs-lookup"><span data-stu-id="72098-135">Describes a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span> <span data-ttu-id="72098-136">これは、可用性カレンダーイベント識別子の形式です。</span><span class="sxs-lookup"><span data-stu-id="72098-136">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="72098-137">StoreId</span><span class="sxs-lookup"><span data-stu-id="72098-137">StoreId</span></span>  <br/> |<span data-ttu-id="72098-138">Exchange ストア識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="72098-138">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="72098-139">OwaId</span><span class="sxs-lookup"><span data-stu-id="72098-139">OwaId</span></span>  <br/> |<span data-ttu-id="72098-140">Outlook Web Access 識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="72098-140">Describes an Outlook Web Access identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="72098-141">子要素</span><span class="sxs-lookup"><span data-stu-id="72098-141">Child elements</span></span>

<span data-ttu-id="72098-142">なし。</span><span class="sxs-lookup"><span data-stu-id="72098-142">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="72098-143">親要素</span><span class="sxs-lookup"><span data-stu-id="72098-143">Parent elements</span></span>

|<span data-ttu-id="72098-144">**要素**</span><span class="sxs-lookup"><span data-stu-id="72098-144">**Element**</span></span>|<span data-ttu-id="72098-145">**説明**</span><span class="sxs-lookup"><span data-stu-id="72098-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72098-146">SourceIds</span><span class="sxs-lookup"><span data-stu-id="72098-146">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="72098-147">変換するソース識別子を含みます。</span><span class="sxs-lookup"><span data-stu-id="72098-147">Contains the source identifiers to convert.</span></span> <span data-ttu-id="72098-148">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="72098-148">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="72098-149">注釈</span><span class="sxs-lookup"><span data-stu-id="72098-149">Remarks</span></span>

<span data-ttu-id="72098-150">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="72098-150">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="72098-151">要素の情報</span><span class="sxs-lookup"><span data-stu-id="72098-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72098-152">Namespace</span><span class="sxs-lookup"><span data-stu-id="72098-152">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="72098-153">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="72098-153">Schema Name</span></span>  <br/> |<span data-ttu-id="72098-154">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="72098-154">Types schema</span></span>  <br/> |
|<span data-ttu-id="72098-155">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="72098-155">Validation File</span></span>  <br/> |<span data-ttu-id="72098-156">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="72098-156">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="72098-157">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="72098-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="72098-158">正しい</span><span class="sxs-lookup"><span data-stu-id="72098-158">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="72098-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="72098-159">See also</span></span>

- [<span data-ttu-id="72098-160">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="72098-160">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="72098-161">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="72098-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="72098-162">識別子の変換</span><span class="sxs-lookup"><span data-stu-id="72098-162">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)


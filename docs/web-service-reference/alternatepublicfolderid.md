---
title: AlternatePublicFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternatePublicFolderId
api_type:
- schema
ms.assetid: 0a4dc1cc-959e-4b93-aa3a-3020ca8b8a02
description: AlternatePublicFolderId 要素は、別の識別子の形式に変換するのには、パブリック フォルダーの識別子について説明します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 32e6e75eb381e479baf5fdb5ad0a40b32c1b02a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759319"
---
# <a name="alternatepublicfolderid"></a><span data-ttu-id="4963c-104">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="4963c-104">AlternatePublicFolderId</span></span>

<span data-ttu-id="4963c-105">**AlternatePublicFolderId**要素は、別の識別子の形式に変換するのには、パブリック フォルダーの識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="4963c-105">The **AlternatePublicFolderId** element describes a public folder identifier to convert to another identifier format.</span></span> <span data-ttu-id="4963c-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4963c-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
- [<span data-ttu-id="4963c-107">ConvertId</span><span class="sxs-lookup"><span data-stu-id="4963c-107">ConvertId</span></span>](convertid.md)
  
- [<span data-ttu-id="4963c-108">SourceIds</span><span class="sxs-lookup"><span data-stu-id="4963c-108">SourceIds</span></span>](sourceids.md)
  
- [<span data-ttu-id="4963c-109">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="4963c-109">AlternatePublicFolderId</span></span>](alternatepublicfolderid.md)
  
```xml
<AlternatePublicFolderId FolderId="" Format="" />
```

 <span data-ttu-id="4963c-110">**AlternatePublicFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="4963c-110">**AlternatePublicFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4963c-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4963c-111">Attributes and elements</span></span>

<span data-ttu-id="4963c-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4963c-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4963c-113">属性</span><span class="sxs-lookup"><span data-stu-id="4963c-113">Attributes</span></span>

|<span data-ttu-id="4963c-114">**属性**</span><span class="sxs-lookup"><span data-stu-id="4963c-114">**Attribute**</span></span>|<span data-ttu-id="4963c-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="4963c-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4963c-116">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="4963c-116">FolderId</span></span>  <br/> |<span data-ttu-id="4963c-117">変換するパブリック フォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4963c-117">Contains the public folder identifier to convert.</span></span> <span data-ttu-id="4963c-118">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="4963c-118">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="4963c-119">Format</span><span class="sxs-lookup"><span data-stu-id="4963c-119">Format</span></span>  <br/> |<span data-ttu-id="4963c-120">変換するパブリック フォルダーの識別子を記述する形式を識別します。</span><span class="sxs-lookup"><span data-stu-id="4963c-120">Identifies the format that describes the public folder identifier to convert.</span></span> <span data-ttu-id="4963c-121">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="4963c-121">This attribute is required.</span></span>  <br/> |
   
#### <a name="format-attribute"></a><span data-ttu-id="4963c-122">形式の属性</span><span class="sxs-lookup"><span data-stu-id="4963c-122">Format attribute</span></span>

|<span data-ttu-id="4963c-123">**値**</span><span class="sxs-lookup"><span data-stu-id="4963c-123">**Value**</span></span>|<span data-ttu-id="4963c-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="4963c-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4963c-125">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="4963c-125">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="4963c-126">Exchange 2007 の最初のリリース版の Exchange Web サービスによって生成される識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="4963c-126">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="4963c-127">EwsId</span><span class="sxs-lookup"><span data-stu-id="4963c-127">EwsId</span></span>  <br/> |<span data-ttu-id="4963c-128">Exchange 2007 SP1 以降の Exchange Web サービスによって生成される識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="4963c-128">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="4963c-129">EntryId</span><span class="sxs-lookup"><span data-stu-id="4963c-129">EntryId</span></span>  <br/> |<span data-ttu-id="4963c-130">PR_ENTRYID プロパティと同様に、MAPI 識別子をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="4963c-130">Describes MAPI identifiers, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="4963c-131">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="4963c-131">HexEntryId</span></span>  <br/> |<span data-ttu-id="4963c-132">PR_ENTRYID プロパティの 16 進数でエンコードされた表現を説明します。</span><span class="sxs-lookup"><span data-stu-id="4963c-132">Describes a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span> <span data-ttu-id="4963c-133">これは、可用性の予定表のイベント識別子の形式です。</span><span class="sxs-lookup"><span data-stu-id="4963c-133">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="4963c-134">StoreId</span><span class="sxs-lookup"><span data-stu-id="4963c-134">StoreId</span></span>  <br/> |<span data-ttu-id="4963c-135">Exchange ストア識別子をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="4963c-135">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="4963c-136">OwaId</span><span class="sxs-lookup"><span data-stu-id="4963c-136">OwaId</span></span>  <br/> |<span data-ttu-id="4963c-137">Outlook Web Access 識別子をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="4963c-137">Describes an Outlook Web Access identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4963c-138">子要素</span><span class="sxs-lookup"><span data-stu-id="4963c-138">Child elements</span></span>

<span data-ttu-id="4963c-139">なし。</span><span class="sxs-lookup"><span data-stu-id="4963c-139">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4963c-140">親要素</span><span class="sxs-lookup"><span data-stu-id="4963c-140">Parent elements</span></span>

|<span data-ttu-id="4963c-141">**要素**</span><span class="sxs-lookup"><span data-stu-id="4963c-141">**Element**</span></span>|<span data-ttu-id="4963c-142">**説明**</span><span class="sxs-lookup"><span data-stu-id="4963c-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4963c-143">SourceIds</span><span class="sxs-lookup"><span data-stu-id="4963c-143">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="4963c-144">変換するソース識別子が含まれます。</span><span class="sxs-lookup"><span data-stu-id="4963c-144">Contains the source identifiers to convert.</span></span> <span data-ttu-id="4963c-145">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4963c-145">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="4963c-146">要素情報</span><span class="sxs-lookup"><span data-stu-id="4963c-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4963c-147">名前空間</span><span class="sxs-lookup"><span data-stu-id="4963c-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4963c-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4963c-148">Schema Name</span></span>  <br/> |<span data-ttu-id="4963c-149">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4963c-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="4963c-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4963c-150">Validation File</span></span>  <br/> |<span data-ttu-id="4963c-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4963c-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4963c-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4963c-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="4963c-153">True</span><span class="sxs-lookup"><span data-stu-id="4963c-153">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4963c-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="4963c-154">See also</span></span>

- [<span data-ttu-id="4963c-155">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="4963c-155">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="4963c-156">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4963c-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="4963c-157">識別子に変換します。</span><span class="sxs-lookup"><span data-stu-id="4963c-157">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)


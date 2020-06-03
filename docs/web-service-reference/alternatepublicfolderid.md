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
description: AlternatePublicFolderId 要素は、別の識別子形式に変換するためのパブリックフォルダー識別子を表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 54ad663117839222ea1174cd1c25600f31aa6b43
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464799"
---
# <a name="alternatepublicfolderid"></a><span data-ttu-id="cb19d-104">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="cb19d-104">AlternatePublicFolderId</span></span>

<span data-ttu-id="cb19d-105">**AlternatePublicFolderId**要素は、別の識別子形式に変換するためのパブリックフォルダー識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="cb19d-105">The **AlternatePublicFolderId** element describes a public folder identifier to convert to another identifier format.</span></span> <span data-ttu-id="cb19d-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="cb19d-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
- [<span data-ttu-id="cb19d-107">ConvertId</span><span class="sxs-lookup"><span data-stu-id="cb19d-107">ConvertId</span></span>](convertid.md)
  
- [<span data-ttu-id="cb19d-108">SourceIds</span><span class="sxs-lookup"><span data-stu-id="cb19d-108">SourceIds</span></span>](sourceids.md)
  
- [<span data-ttu-id="cb19d-109">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="cb19d-109">AlternatePublicFolderId</span></span>](alternatepublicfolderid.md)
  
```xml
<AlternatePublicFolderId FolderId="" Format="" />
```

 <span data-ttu-id="cb19d-110">**AlternatePublicFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="cb19d-110">**AlternatePublicFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cb19d-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cb19d-111">Attributes and elements</span></span>

<span data-ttu-id="cb19d-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cb19d-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cb19d-113">属性</span><span class="sxs-lookup"><span data-stu-id="cb19d-113">Attributes</span></span>

|<span data-ttu-id="cb19d-114">**属性**</span><span class="sxs-lookup"><span data-stu-id="cb19d-114">**Attribute**</span></span>|<span data-ttu-id="cb19d-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="cb19d-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cb19d-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="cb19d-116">FolderId</span></span>  <br/> |<span data-ttu-id="cb19d-117">変換するパブリックフォルダーの識別子を含みます。</span><span class="sxs-lookup"><span data-stu-id="cb19d-117">Contains the public folder identifier to convert.</span></span> <span data-ttu-id="cb19d-118">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="cb19d-118">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="cb19d-119">Format</span><span class="sxs-lookup"><span data-stu-id="cb19d-119">Format</span></span>  <br/> |<span data-ttu-id="cb19d-120">変換するパブリックフォルダー識別子を説明する形式を識別します。</span><span class="sxs-lookup"><span data-stu-id="cb19d-120">Identifies the format that describes the public folder identifier to convert.</span></span> <span data-ttu-id="cb19d-121">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="cb19d-121">This attribute is required.</span></span>  <br/> |
   
#### <a name="format-attribute"></a><span data-ttu-id="cb19d-122">Format 属性</span><span class="sxs-lookup"><span data-stu-id="cb19d-122">Format attribute</span></span>

|<span data-ttu-id="cb19d-123">**値**</span><span class="sxs-lookup"><span data-stu-id="cb19d-123">**Value**</span></span>|<span data-ttu-id="cb19d-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="cb19d-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cb19d-125">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="cb19d-125">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="cb19d-126">Exchange 2007 の最初のリリースバージョンで Exchange Web サービスによって生成された識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="cb19d-126">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="cb19d-127">EwsId</span><span class="sxs-lookup"><span data-stu-id="cb19d-127">EwsId</span></span>  <br/> |<span data-ttu-id="cb19d-128">Exchange 2007 SP1 以降の Exchange Web サービスによって生成される識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="cb19d-128">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="cb19d-129">EntryId</span><span class="sxs-lookup"><span data-stu-id="cb19d-129">EntryId</span></span>  <br/> |<span data-ttu-id="cb19d-130">PR_ENTRYID プロパティのように、MAPI 識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="cb19d-130">Describes MAPI identifiers, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="cb19d-131">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="cb19d-131">HexEntryId</span></span>  <br/> |<span data-ttu-id="cb19d-132">PR_ENTRYID プロパティの16進数でエンコードされた表現を記述します。</span><span class="sxs-lookup"><span data-stu-id="cb19d-132">Describes a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span> <span data-ttu-id="cb19d-133">これは、可用性カレンダーイベント識別子の形式です。</span><span class="sxs-lookup"><span data-stu-id="cb19d-133">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="cb19d-134">StoreId</span><span class="sxs-lookup"><span data-stu-id="cb19d-134">StoreId</span></span>  <br/> |<span data-ttu-id="cb19d-135">Exchange ストア識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="cb19d-135">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="cb19d-136">OwaId</span><span class="sxs-lookup"><span data-stu-id="cb19d-136">OwaId</span></span>  <br/> |<span data-ttu-id="cb19d-137">Outlook Web Access 識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="cb19d-137">Describes an Outlook Web Access identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="cb19d-138">子要素</span><span class="sxs-lookup"><span data-stu-id="cb19d-138">Child elements</span></span>

<span data-ttu-id="cb19d-139">なし。</span><span class="sxs-lookup"><span data-stu-id="cb19d-139">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cb19d-140">親要素</span><span class="sxs-lookup"><span data-stu-id="cb19d-140">Parent elements</span></span>

|<span data-ttu-id="cb19d-141">**要素**</span><span class="sxs-lookup"><span data-stu-id="cb19d-141">**Element**</span></span>|<span data-ttu-id="cb19d-142">**説明**</span><span class="sxs-lookup"><span data-stu-id="cb19d-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb19d-143">SourceIds</span><span class="sxs-lookup"><span data-stu-id="cb19d-143">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="cb19d-144">変換するソース識別子を含みます。</span><span class="sxs-lookup"><span data-stu-id="cb19d-144">Contains the source identifiers to convert.</span></span> <span data-ttu-id="cb19d-145">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="cb19d-145">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="cb19d-146">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cb19d-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cb19d-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="cb19d-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cb19d-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cb19d-148">Schema Name</span></span>  <br/> |<span data-ttu-id="cb19d-149">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="cb19d-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="cb19d-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cb19d-150">Validation File</span></span>  <br/> |<span data-ttu-id="cb19d-151">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="cb19d-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cb19d-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cb19d-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="cb19d-153">正しい</span><span class="sxs-lookup"><span data-stu-id="cb19d-153">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cb19d-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="cb19d-154">See also</span></span>

- [<span data-ttu-id="cb19d-155">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="cb19d-155">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="cb19d-156">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="cb19d-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="cb19d-157">識別子の変換</span><span class="sxs-lookup"><span data-stu-id="cb19d-157">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)


---
title: AlternateId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternateId
api_type:
- schema
ms.assetid: 9c01fdc3-4adf-4e23-bc33-45d2a45ea08b
description: AlternateId 要素は、要求で変換する識別子と、応答で変換された id の結果を示します。
ms.openlocfilehash: 26df68bd814c2d323630c6bb40b4c31745017c71
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527454"
---
# <a name="alternateid"></a><span data-ttu-id="390f7-103">AlternateId</span><span class="sxs-lookup"><span data-stu-id="390f7-103">AlternateId</span></span>

<span data-ttu-id="390f7-104">**Alternateid**要素は、要求で変換する識別子と、応答で変換された id の結果を示します。</span><span class="sxs-lookup"><span data-stu-id="390f7-104">The **AlternateId** element describes an identifier to convert in a request and the results of a converted identifier in the response.</span></span> 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 <span data-ttu-id="390f7-105">**AlternateIdType**</span><span class="sxs-lookup"><span data-stu-id="390f7-105">**AlternateIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="390f7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="390f7-106">Attributes and elements</span></span>

<span data-ttu-id="390f7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="390f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="390f7-108">属性</span><span class="sxs-lookup"><span data-stu-id="390f7-108">Attributes</span></span>

|<span data-ttu-id="390f7-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="390f7-109">**Attribute**</span></span>|<span data-ttu-id="390f7-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="390f7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="390f7-111">ID</span><span class="sxs-lookup"><span data-stu-id="390f7-111">Id</span></span>  <br/> |<span data-ttu-id="390f7-112">変換[tid 操作](convertid-operation.md)要求のソース識別子を記述し、変換[tid 操作](convertid-operation.md)応答で宛先識別子を記述します。</span><span class="sxs-lookup"><span data-stu-id="390f7-112">Describes the source identifier in a [ConvertId operation](convertid-operation.md) request and describes the destination identifier in a [ConvertId operation](convertid-operation.md) response.</span></span>  <br/> |
|<span data-ttu-id="390f7-113">Format</span><span class="sxs-lookup"><span data-stu-id="390f7-113">Format</span></span>  <br/> |<span data-ttu-id="390f7-114">変換[tid 操作](convertid-operation.md)要求のソース形式を記述し、変換[tid 操作](convertid-operation.md)の応答で宛先の形式を記述します。</span><span class="sxs-lookup"><span data-stu-id="390f7-114">Describes the source format in a [ConvertId operation](convertid-operation.md) request and describes the destination format in a [ConvertId operation](convertid-operation.md) response.</span></span> <span data-ttu-id="390f7-115">転送先の形式は、要求の変換[tid](convertid.md)要素の**destinationformat**属性によって記述されます。</span><span class="sxs-lookup"><span data-stu-id="390f7-115">The destination format is described by the **DestinationFormat** attribute of the [ConvertId](convertid.md) element in the request.</span></span> <span data-ttu-id="390f7-116">この属性の型は**IdFormatType**です。</span><span class="sxs-lookup"><span data-stu-id="390f7-116">This attribute is of type **IdFormatType**.</span></span>  <br/> |
|<span data-ttu-id="390f7-117">メールボックス</span><span class="sxs-lookup"><span data-stu-id="390f7-117">Mailbox</span></span>  <br/> |<span data-ttu-id="390f7-118">変換する識別子を含むメールボックスのプライマリ SMTP (Simple Mail Transfer Protocol) アドレスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="390f7-118">Describes the mailbox primary Simple Mail Transfer Protocol (SMTP) address that contains the identifiers to translate.</span></span>  <br/> |
|<span data-ttu-id="390f7-119">IsArchive</span><span class="sxs-lookup"><span data-stu-id="390f7-119">IsArchive</span></span>  <br/> |<span data-ttu-id="390f7-120">識別子がアーカイブされたアイテムまたはフォルダーを表しているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="390f7-120">Indicates whether the identifier represents an archived item or folder.</span></span> <span data-ttu-id="390f7-121">値が**true の場合**は、識別子がアーカイブされたアイテムまたはフォルダーを表していることを示します。</span><span class="sxs-lookup"><span data-stu-id="390f7-121">A value of **true** indicates that the identifier represents an archived item or folder.</span></span> <span data-ttu-id="390f7-122">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="390f7-122">This attribute is optional.</span></span>  <br/> |
   
#### <a name="format-attribute-values"></a><span data-ttu-id="390f7-123">書式属性値</span><span class="sxs-lookup"><span data-stu-id="390f7-123">Format attribute values</span></span>

|<span data-ttu-id="390f7-124">**値**</span><span class="sxs-lookup"><span data-stu-id="390f7-124">**Value**</span></span>|<span data-ttu-id="390f7-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="390f7-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="390f7-126">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="390f7-126">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="390f7-127">Exchange 2007 の最初のリリースバージョンで Exchange Web サービスによって生成された識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="390f7-127">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="390f7-128">EwsId</span><span class="sxs-lookup"><span data-stu-id="390f7-128">EwsId</span></span>  <br/> |<span data-ttu-id="390f7-129">Exchange 2007 SP1 以降の Exchange Web サービスによって生成される識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="390f7-129">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="390f7-130">EntryId</span><span class="sxs-lookup"><span data-stu-id="390f7-130">EntryId</span></span>  <br/> |<span data-ttu-id="390f7-131">**PR_ENTRYID**プロパティのように、MAPI 識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="390f7-131">Describes MAPI identifiers, as in the **PR_ENTRYID** property.</span></span>  <br/> |
|<span data-ttu-id="390f7-132">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="390f7-132">HexEntryId</span></span>  <br/> |<span data-ttu-id="390f7-133">**PR_ENTRYID**プロパティの16進数でエンコードされた表現を記述します。</span><span class="sxs-lookup"><span data-stu-id="390f7-133">Describes a hexadecimal-encoded representation of the **PR_ENTRYID** property.</span></span> <span data-ttu-id="390f7-134">これは、可用性カレンダーイベント識別子の形式です。</span><span class="sxs-lookup"><span data-stu-id="390f7-134">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="390f7-135">StoreId</span><span class="sxs-lookup"><span data-stu-id="390f7-135">StoreId</span></span>  <br/> |<span data-ttu-id="390f7-136">Exchange ストア識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="390f7-136">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="390f7-137">OwaId</span><span class="sxs-lookup"><span data-stu-id="390f7-137">OwaId</span></span>  <br/> |<span data-ttu-id="390f7-138">Outlook Web App 識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="390f7-138">Describes an Outlook Web App identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="390f7-139">子要素</span><span class="sxs-lookup"><span data-stu-id="390f7-139">Child elements</span></span>

<span data-ttu-id="390f7-140">なし。</span><span class="sxs-lookup"><span data-stu-id="390f7-140">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="390f7-141">親要素</span><span class="sxs-lookup"><span data-stu-id="390f7-141">Parent elements</span></span>

|<span data-ttu-id="390f7-142">**要素**</span><span class="sxs-lookup"><span data-stu-id="390f7-142">**Element**</span></span>|<span data-ttu-id="390f7-143">**説明**</span><span class="sxs-lookup"><span data-stu-id="390f7-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="390f7-144">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="390f7-144">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md) <br/> |<span data-ttu-id="390f7-145">[状態]-[バケット][操作](convertid-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="390f7-145">Contains the status and result of a [ConvertId operation](convertid-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="390f7-146">SourceIds</span><span class="sxs-lookup"><span data-stu-id="390f7-146">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="390f7-147">変換するソース識別子を含みます。</span><span class="sxs-lookup"><span data-stu-id="390f7-147">Contains the source identifiers to convert.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="390f7-148">テキスト値</span><span class="sxs-lookup"><span data-stu-id="390f7-148">Text value</span></span>

<span data-ttu-id="390f7-149">なし。</span><span class="sxs-lookup"><span data-stu-id="390f7-149">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="390f7-150">注釈</span><span class="sxs-lookup"><span data-stu-id="390f7-150">Remarks</span></span>

<span data-ttu-id="390f7-151">**Alternateid**要素[は、2](convertid-operation.md)つの識別子、変換される変換元識別子、および[ConvertIdResponse](convertidresponse.md)要素の変換された識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="390f7-151">The **AlternateId** element describes two identifiers, the source identifier that is to be converted in the [ConvertId operation](convertid-operation.md) request, and the converted identifier in the [ConvertIdResponse](convertidresponse.md) element.</span></span> 
  
<span data-ttu-id="390f7-152">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="390f7-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="390f7-153">要素の情報</span><span class="sxs-lookup"><span data-stu-id="390f7-153">Element information</span></span>

||||
|:-----|:-----|:-----|
|<span data-ttu-id="390f7-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="390f7-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="390f7-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="390f7-155">Schema Name</span></span>  <br/> |<span data-ttu-id="390f7-156">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="390f7-156">Messages schema</span></span>  <br/> |<span data-ttu-id="390f7-157">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="390f7-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="390f7-158">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="390f7-158">Validation File</span></span>  <br/> |<span data-ttu-id="390f7-159">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="390f7-159">Messages.xsd</span></span>  <br/> |<span data-ttu-id="390f7-160">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="390f7-160">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="390f7-161">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="390f7-161">Can be Empty</span></span>  <br/> |<span data-ttu-id="390f7-162">False</span><span class="sxs-lookup"><span data-stu-id="390f7-162">False</span></span>  <br/> |<span data-ttu-id="390f7-163">False</span><span class="sxs-lookup"><span data-stu-id="390f7-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="390f7-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="390f7-164">See also</span></span>

- [<span data-ttu-id="390f7-165">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="390f7-165">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="390f7-166">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="390f7-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="390f7-167">識別子の変換</span><span class="sxs-lookup"><span data-stu-id="390f7-167">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)


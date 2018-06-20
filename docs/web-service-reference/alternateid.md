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
description: AlternateId 要素は、要求と応答に変換された識別子の結果に変換するのには識別子について説明します。
ms.openlocfilehash: e4d29087b63b52638dd93e4e3b643cdee39a5b97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759312"
---
# <a name="alternateid"></a><span data-ttu-id="88500-103">AlternateId</span><span class="sxs-lookup"><span data-stu-id="88500-103">AlternateId</span></span>

<span data-ttu-id="88500-104">**AlternateId**要素は、要求と応答に変換された識別子の結果に変換するのには識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="88500-104">The **AlternateId** element describes an identifier to convert in a request and the results of a converted identifier in the response.</span></span> 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 <span data-ttu-id="88500-105">**AlternateIdType**</span><span class="sxs-lookup"><span data-stu-id="88500-105">**AlternateIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88500-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="88500-106">Attributes and elements</span></span>

<span data-ttu-id="88500-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="88500-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88500-108">属性</span><span class="sxs-lookup"><span data-stu-id="88500-108">Attributes</span></span>

|<span data-ttu-id="88500-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="88500-109">**Attribute**</span></span>|<span data-ttu-id="88500-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="88500-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="88500-111">ID</span><span class="sxs-lookup"><span data-stu-id="88500-111">Id</span></span>  <br/> |<span data-ttu-id="88500-112">[ConvertId 操作](convertid-operation.md)の要求の送信元識別子および[ConvertId 操作](convertid-operation.md)の応答の送信先識別子を説明します。</span><span class="sxs-lookup"><span data-stu-id="88500-112">Describes the source identifier in a [ConvertId operation](convertid-operation.md) request and describes the destination identifier in a [ConvertId operation](convertid-operation.md) response.</span></span>  <br/> |
|<span data-ttu-id="88500-113">Format</span><span class="sxs-lookup"><span data-stu-id="88500-113">Format</span></span>  <br/> |<span data-ttu-id="88500-114">[ConvertId 操作](convertid-operation.md)の要求のソース フォーマットおよび[ConvertId 操作](convertid-operation.md)の応答に変換先の形式を説明します。</span><span class="sxs-lookup"><span data-stu-id="88500-114">Describes the source format in a [ConvertId operation](convertid-operation.md) request and describes the destination format in a [ConvertId operation](convertid-operation.md) response.</span></span> <span data-ttu-id="88500-115">変換先の形式は、要求内の[ConvertId](convertid.md)要素の**DestinationFormat**属性で表されます。</span><span class="sxs-lookup"><span data-stu-id="88500-115">The destination format is described by the **DestinationFormat** attribute of the [ConvertId](convertid.md) element in the request.</span></span> <span data-ttu-id="88500-116">この属性は、型**IdFormatType**のです。</span><span class="sxs-lookup"><span data-stu-id="88500-116">This attribute is of type **IdFormatType**.</span></span>  <br/> |
|<span data-ttu-id="88500-117">メールボックス</span><span class="sxs-lookup"><span data-stu-id="88500-117">Mailbox</span></span>  <br/> |<span data-ttu-id="88500-118">変換するための識別子が含まれているメールボックス プライマリ簡易メール転送プロトコル (SMTP) アドレスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="88500-118">Describes the mailbox primary Simple Mail Transfer Protocol (SMTP) address that contains the identifiers to translate.</span></span>  <br/> |
|<span data-ttu-id="88500-119">IsArchive</span><span class="sxs-lookup"><span data-stu-id="88500-119">IsArchive</span></span>  <br/> |<span data-ttu-id="88500-120">アーカイブされたアイテムまたはフォルダーの識別子を表すかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="88500-120">Indicates whether the identifier represents an archived item or folder.</span></span> <span data-ttu-id="88500-121">**True**の場合は、識別子がアーカイブされたアイテムまたはフォルダーを表すことを示します。</span><span class="sxs-lookup"><span data-stu-id="88500-121">A value of **true** indicates that the identifier represents an archived item or folder.</span></span> <span data-ttu-id="88500-122">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="88500-122">This attribute is optional.</span></span>  <br/> |
   
#### <a name="format-attribute-values"></a><span data-ttu-id="88500-123">属性の値を書式設定</span><span class="sxs-lookup"><span data-stu-id="88500-123">Format attribute values</span></span>

|<span data-ttu-id="88500-124">**値**</span><span class="sxs-lookup"><span data-stu-id="88500-124">**Value**</span></span>|<span data-ttu-id="88500-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="88500-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="88500-126">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="88500-126">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="88500-127">Exchange 2007 の最初のリリース版の Exchange Web サービスによって生成される識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="88500-127">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="88500-128">EwsId</span><span class="sxs-lookup"><span data-stu-id="88500-128">EwsId</span></span>  <br/> |<span data-ttu-id="88500-129">Exchange 2007 SP1 以降の Exchange Web サービスによって生成される識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="88500-129">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="88500-130">EntryId</span><span class="sxs-lookup"><span data-stu-id="88500-130">EntryId</span></span>  <br/> |<span data-ttu-id="88500-131">**PR_ENTRYID**プロパティと同様に、MAPI 識別子をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="88500-131">Describes MAPI identifiers, as in the **PR_ENTRYID** property.</span></span>  <br/> |
|<span data-ttu-id="88500-132">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="88500-132">HexEntryId</span></span>  <br/> |<span data-ttu-id="88500-133">**PR_ENTRYID**プロパティの 16 進数でエンコードされた表現を説明します。</span><span class="sxs-lookup"><span data-stu-id="88500-133">Describes a hexadecimal-encoded representation of the **PR_ENTRYID** property.</span></span> <span data-ttu-id="88500-134">これは、可用性の予定表のイベント識別子の形式です。</span><span class="sxs-lookup"><span data-stu-id="88500-134">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="88500-135">StoreId</span><span class="sxs-lookup"><span data-stu-id="88500-135">StoreId</span></span>  <br/> |<span data-ttu-id="88500-136">Exchange ストア識別子をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="88500-136">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="88500-137">OwaId</span><span class="sxs-lookup"><span data-stu-id="88500-137">OwaId</span></span>  <br/> |<span data-ttu-id="88500-138">Outlook Web App の識別子をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="88500-138">Describes an Outlook Web App identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="88500-139">子要素</span><span class="sxs-lookup"><span data-stu-id="88500-139">Child elements</span></span>

<span data-ttu-id="88500-140">なし。</span><span class="sxs-lookup"><span data-stu-id="88500-140">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="88500-141">親要素</span><span class="sxs-lookup"><span data-stu-id="88500-141">Parent elements</span></span>

|<span data-ttu-id="88500-142">**要素**</span><span class="sxs-lookup"><span data-stu-id="88500-142">**Element**</span></span>|<span data-ttu-id="88500-143">**説明**</span><span class="sxs-lookup"><span data-stu-id="88500-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88500-144">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="88500-144">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md) <br/> |<span data-ttu-id="88500-145">状態と[ConvertId の操作](convertid-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="88500-145">Contains the status and result of a [ConvertId operation](convertid-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="88500-146">SourceIds</span><span class="sxs-lookup"><span data-stu-id="88500-146">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="88500-147">変換するソース識別子が含まれます。</span><span class="sxs-lookup"><span data-stu-id="88500-147">Contains the source identifiers to convert.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="88500-148">テキスト値</span><span class="sxs-lookup"><span data-stu-id="88500-148">Text value</span></span>

<span data-ttu-id="88500-149">なし。</span><span class="sxs-lookup"><span data-stu-id="88500-149">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="88500-150">備考</span><span class="sxs-lookup"><span data-stu-id="88500-150">Remarks</span></span>

<span data-ttu-id="88500-151">**AlternateId**要素は、2 つの識別子、 [ConvertId 操作](convertid-operation.md)の要求に変換するのには送信元識別子、および[ConvertIdResponse](convertidresponse.md)要素の変換後の識別子について説明します。</span><span class="sxs-lookup"><span data-stu-id="88500-151">The **AlternateId** element describes two identifiers, the source identifier that is to be converted in the [ConvertId operation](convertid-operation.md) request, and the converted identifier in the [ConvertIdResponse](convertidresponse.md) element.</span></span> 
  
<span data-ttu-id="88500-152">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="88500-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88500-153">要素情報</span><span class="sxs-lookup"><span data-stu-id="88500-153">Element information</span></span>

||||
|:-----|:-----|:-----|
|<span data-ttu-id="88500-154">名前空間</span><span class="sxs-lookup"><span data-stu-id="88500-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="88500-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="88500-155">Schema Name</span></span>  <br/> |<span data-ttu-id="88500-156">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="88500-156">Messages schema</span></span>  <br/> |<span data-ttu-id="88500-157">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="88500-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="88500-158">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="88500-158">Validation File</span></span>  <br/> |<span data-ttu-id="88500-159">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="88500-159">Messages.xsd</span></span>  <br/> |<span data-ttu-id="88500-160">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="88500-160">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="88500-161">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="88500-161">Can be Empty</span></span>  <br/> |<span data-ttu-id="88500-162">False</span><span class="sxs-lookup"><span data-stu-id="88500-162">False</span></span>  <br/> |<span data-ttu-id="88500-163">False</span><span class="sxs-lookup"><span data-stu-id="88500-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88500-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="88500-164">See also</span></span>

- [<span data-ttu-id="88500-165">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="88500-165">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="88500-166">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="88500-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="88500-167">識別子に変換します。</span><span class="sxs-lookup"><span data-stu-id="88500-167">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)


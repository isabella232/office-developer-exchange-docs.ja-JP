---
title: ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 9684c22c-29d4-4f7f-befc-8cd41da56d38
description: 変換 Tid 要素は、サポートされている Exchange 形式間でアイテムとフォルダーの識別子を変換する要求を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: d421baf1f29fb59a8c6eb2b09e1fa0e8a38ffaa4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452539"
---
# <a name="convertid"></a><span data-ttu-id="fb92c-104">ConvertId</span><span class="sxs-lookup"><span data-stu-id="fb92c-104">ConvertId</span></span>

<span data-ttu-id="fb92c-105">変換**tid**要素は、サポートされている Exchange 形式間でアイテムとフォルダーの識別子を変換する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="fb92c-105">The **ConvertId** element defines a request to convert item and folder identifiers between supported Exchange formats.</span></span> <span data-ttu-id="fb92c-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fb92c-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ConvertId DestinationFormat="">
   <SourceIds/>
</ConvertId>
```

 <span data-ttu-id="fb92c-107">**ConvertIdType**</span><span class="sxs-lookup"><span data-stu-id="fb92c-107">**ConvertIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb92c-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fb92c-108">Attributes and elements</span></span>

<span data-ttu-id="fb92c-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fb92c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb92c-110">属性</span><span class="sxs-lookup"><span data-stu-id="fb92c-110">Attributes</span></span>

|<span data-ttu-id="fb92c-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="fb92c-111">**Attribute**</span></span>|<span data-ttu-id="fb92c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb92c-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fb92c-113">**DestinationFormat**</span><span class="sxs-lookup"><span data-stu-id="fb92c-113">**DestinationFormat**</span></span> <br/> |<span data-ttu-id="fb92c-114">変換されたすべての識別子に対して返される識別子の形式を記述します。</span><span class="sxs-lookup"><span data-stu-id="fb92c-114">Describes the identifier format that will be returned for all the converted identifiers.</span></span> <span data-ttu-id="fb92c-115">DestinationFormat は、IdFormatType によって記述されます。</span><span class="sxs-lookup"><span data-stu-id="fb92c-115">The DestinationFormat is described by the IdFormatType.</span></span>  <br/> |
   
#### <a name="destinationformat-attribute"></a><span data-ttu-id="fb92c-116">DestinationFormat 属性</span><span class="sxs-lookup"><span data-stu-id="fb92c-116">DestinationFormat Attribute</span></span>

|<span data-ttu-id="fb92c-117">**値**</span><span class="sxs-lookup"><span data-stu-id="fb92c-117">**Value**</span></span>|<span data-ttu-id="fb92c-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb92c-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fb92c-119">**EwsLegacyId**</span><span class="sxs-lookup"><span data-stu-id="fb92c-119">**EwsLegacyId**</span></span> <br/> |<span data-ttu-id="fb92c-120">Exchange 2007 の最初のリリースバージョンで提供される Exchange Web サービス識別子に使用される識別子の形式を表します。</span><span class="sxs-lookup"><span data-stu-id="fb92c-120">Represents the identifier format that is used for Exchange Web Services identifiers that are provided in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="fb92c-121">**EwsId**</span><span class="sxs-lookup"><span data-stu-id="fb92c-121">**EwsId**</span></span> <br/> |<span data-ttu-id="fb92c-122">Exchange Server 2007 SP1 以降の Exchange Web サービス識別子に使用される識別子の形式を表します。</span><span class="sxs-lookup"><span data-stu-id="fb92c-122">Represents the identifier format that is used for Exchange Web Services identifiers starting with Exchange Server 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="fb92c-123">**EntryId**</span><span class="sxs-lookup"><span data-stu-id="fb92c-123">**EntryId**</span></span> <br/> |<span data-ttu-id="fb92c-124">PR_ENTRYID プロパティのように、MAPI 識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="fb92c-124">Represents the MAPI identifier, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="fb92c-125">**HexEntryId**</span><span class="sxs-lookup"><span data-stu-id="fb92c-125">**HexEntryId**</span></span> <br/> |<span data-ttu-id="fb92c-126">可用性カレンダーイベント識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="fb92c-126">Represents the availability calendar event identifier.</span></span> <span data-ttu-id="fb92c-127">これは、PR_ENTRYID プロパティを16進数でエンコードした表記です。</span><span class="sxs-lookup"><span data-stu-id="fb92c-127">This is a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="fb92c-128">**StoreId**</span><span class="sxs-lookup"><span data-stu-id="fb92c-128">**StoreId**</span></span> <br/> |<span data-ttu-id="fb92c-129">Exchange ストア識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="fb92c-129">Represents the Exchange store identifier.</span></span>  <br/> |
|<span data-ttu-id="fb92c-130">**OwaId**</span><span class="sxs-lookup"><span data-stu-id="fb92c-130">**OwaId**</span></span> <br/> |<span data-ttu-id="fb92c-131">Outlook Web Access 識別子の形式を表します。</span><span class="sxs-lookup"><span data-stu-id="fb92c-131">Represents the Outlook Web Access identifier format.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fb92c-132">子要素</span><span class="sxs-lookup"><span data-stu-id="fb92c-132">Child elements</span></span>

|<span data-ttu-id="fb92c-133">**Element**</span><span class="sxs-lookup"><span data-stu-id="fb92c-133">**Element**</span></span>|<span data-ttu-id="fb92c-134">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb92c-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb92c-135">SourceIds</span><span class="sxs-lookup"><span data-stu-id="fb92c-135">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="fb92c-136">変換するソース識別子を含みます。</span><span class="sxs-lookup"><span data-stu-id="fb92c-136">Contains the source identifiers to convert.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fb92c-137">親要素</span><span class="sxs-lookup"><span data-stu-id="fb92c-137">Parent elements</span></span>

<span data-ttu-id="fb92c-138">なし。</span><span class="sxs-lookup"><span data-stu-id="fb92c-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fb92c-139">注釈</span><span class="sxs-lookup"><span data-stu-id="fb92c-139">Remarks</span></span>

<span data-ttu-id="fb92c-140">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="fb92c-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb92c-141">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fb92c-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb92c-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="fb92c-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fb92c-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fb92c-143">Schema Name</span></span>  <br/> |<span data-ttu-id="fb92c-144">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="fb92c-144">messages schema</span></span>  <br/> |
|<span data-ttu-id="fb92c-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fb92c-145">Validation File</span></span>  <br/> |<span data-ttu-id="fb92c-146">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="fb92c-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fb92c-147">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fb92c-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="fb92c-148">正しくない</span><span class="sxs-lookup"><span data-stu-id="fb92c-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb92c-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="fb92c-149">See also</span></span>



[<span data-ttu-id="fb92c-150">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="fb92c-150">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="fb92c-151">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="fb92c-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="fb92c-152">識別子の変換</span><span class="sxs-lookup"><span data-stu-id="fb92c-152">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)


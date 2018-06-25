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
description: ConvertId 要素は、Exchange でサポートされる形式の間でのアイテムおよびフォルダーの識別子を変換するための要求を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 956f6464fd9013f9e72d2915f21c3b011d0add5b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759767"
---
# <a name="convertid"></a><span data-ttu-id="1f395-104">ConvertId</span><span class="sxs-lookup"><span data-stu-id="1f395-104">ConvertId</span></span>

<span data-ttu-id="1f395-105">**ConvertId**要素は、Exchange でサポートされる形式の間でのアイテムおよびフォルダーの識別子を変換するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="1f395-105">The **ConvertId** element defines a request to convert item and folder identifiers between supported Exchange formats.</span></span> <span data-ttu-id="1f395-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1f395-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ConvertId DestinationFormat="">
   <SourceIds/>
</ConvertId>
```

 <span data-ttu-id="1f395-107">**ConvertIdType**</span><span class="sxs-lookup"><span data-stu-id="1f395-107">**ConvertIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f395-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1f395-108">Attributes and elements</span></span>

<span data-ttu-id="1f395-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1f395-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f395-110">属性</span><span class="sxs-lookup"><span data-stu-id="1f395-110">Attributes</span></span>

|<span data-ttu-id="1f395-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="1f395-111">**Attribute**</span></span>|<span data-ttu-id="1f395-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f395-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1f395-113">**DestinationFormat**</span><span class="sxs-lookup"><span data-stu-id="1f395-113">**DestinationFormat**</span></span> <br/> |<span data-ttu-id="1f395-114">変換後のすべての識別子の返される識別子の形式を表します。</span><span class="sxs-lookup"><span data-stu-id="1f395-114">Describes the identifier format that will be returned for all the converted identifiers.</span></span> <span data-ttu-id="1f395-115">DestinationFormat は、IdFormatType で説明されています。</span><span class="sxs-lookup"><span data-stu-id="1f395-115">The DestinationFormat is described by the IdFormatType.</span></span>  <br/> |
   
#### <a name="destinationformat-attribute"></a><span data-ttu-id="1f395-116">DestinationFormat 属性</span><span class="sxs-lookup"><span data-stu-id="1f395-116">DestinationFormat Attribute</span></span>

|<span data-ttu-id="1f395-117">**値**</span><span class="sxs-lookup"><span data-stu-id="1f395-117">**Value**</span></span>|<span data-ttu-id="1f395-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f395-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1f395-119">**EwsLegacyId**</span><span class="sxs-lookup"><span data-stu-id="1f395-119">**EwsLegacyId**</span></span> <br/> |<span data-ttu-id="1f395-120">初期リリース版の Exchange 2007 で提供されている Exchange Web サービスの識別子に使用される識別子の形式を表します。</span><span class="sxs-lookup"><span data-stu-id="1f395-120">Represents the identifier format that is used for Exchange Web Services identifiers that are provided in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="1f395-121">**EwsId**</span><span class="sxs-lookup"><span data-stu-id="1f395-121">**EwsId**</span></span> <br/> |<span data-ttu-id="1f395-122">Exchange Web サービスの識別子が Exchange Server 2007 sp1 の起動に使用される識別子の形式を表します。</span><span class="sxs-lookup"><span data-stu-id="1f395-122">Represents the identifier format that is used for Exchange Web Services identifiers starting with Exchange Server 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="1f395-123">**エントリ Id**</span><span class="sxs-lookup"><span data-stu-id="1f395-123">**EntryId**</span></span> <br/> |<span data-ttu-id="1f395-124">PR_ENTRYID プロパティと同様に、MAPI id を表します。</span><span class="sxs-lookup"><span data-stu-id="1f395-124">Represents the MAPI identifier, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="1f395-125">**HexEntryId**</span><span class="sxs-lookup"><span data-stu-id="1f395-125">**HexEntryId**</span></span> <br/> |<span data-ttu-id="1f395-126">可用性の予定表のイベント識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="1f395-126">Represents the availability calendar event identifier.</span></span> <span data-ttu-id="1f395-127">これは、PR_ENTRYID プロパティの 16 進数でエンコードされた表現です。</span><span class="sxs-lookup"><span data-stu-id="1f395-127">This is a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="1f395-128">**StoreId**</span><span class="sxs-lookup"><span data-stu-id="1f395-128">**StoreId**</span></span> <br/> |<span data-ttu-id="1f395-129">Exchange ストアの id を表します。</span><span class="sxs-lookup"><span data-stu-id="1f395-129">Represents the Exchange store identifier.</span></span>  <br/> |
|<span data-ttu-id="1f395-130">**OwaId**</span><span class="sxs-lookup"><span data-stu-id="1f395-130">**OwaId**</span></span> <br/> |<span data-ttu-id="1f395-131">Outlook Web Access の識別子の形式を表します。</span><span class="sxs-lookup"><span data-stu-id="1f395-131">Represents the Outlook Web Access identifier format.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1f395-132">子要素</span><span class="sxs-lookup"><span data-stu-id="1f395-132">Child elements</span></span>

|<span data-ttu-id="1f395-133">**要素**</span><span class="sxs-lookup"><span data-stu-id="1f395-133">**Element**</span></span>|<span data-ttu-id="1f395-134">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f395-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f395-135">SourceIds</span><span class="sxs-lookup"><span data-stu-id="1f395-135">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="1f395-136">変換するソース識別子が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1f395-136">Contains the source identifiers to convert.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1f395-137">親要素</span><span class="sxs-lookup"><span data-stu-id="1f395-137">Parent elements</span></span>

<span data-ttu-id="1f395-138">なし。</span><span class="sxs-lookup"><span data-stu-id="1f395-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1f395-139">備考</span><span class="sxs-lookup"><span data-stu-id="1f395-139">Remarks</span></span>

<span data-ttu-id="1f395-140">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1f395-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f395-141">要素情報</span><span class="sxs-lookup"><span data-stu-id="1f395-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f395-142">名前空間</span><span class="sxs-lookup"><span data-stu-id="1f395-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1f395-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1f395-143">Schema Name</span></span>  <br/> |<span data-ttu-id="1f395-144">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="1f395-144">messages schema</span></span>  <br/> |
|<span data-ttu-id="1f395-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1f395-145">Validation File</span></span>  <br/> |<span data-ttu-id="1f395-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1f395-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1f395-147">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1f395-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="1f395-148">False</span><span class="sxs-lookup"><span data-stu-id="1f395-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f395-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="1f395-149">See also</span></span>



[<span data-ttu-id="1f395-150">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="1f395-150">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="1f395-151">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1f395-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="1f395-152">識別子に変換します。</span><span class="sxs-lookup"><span data-stu-id="1f395-152">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)


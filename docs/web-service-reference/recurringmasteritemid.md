---
title: RecurringMasterItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringMasterItemId
api_type:
- schema
ms.assetid: 5800b58c-f3d7-4d8f-acc0-d13e02f4e258
description: RecurringMasterItemId 要素は、関連するオカレンスアイテムの1つの識別子を識別することによって、定期的なアイテムのマスターアイテムを識別します。
ms.openlocfilehash: 896a9ce95d619e7bb44c8158288bc4f62ce417d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529883"
---
# <a name="recurringmasteritemid"></a><span data-ttu-id="78def-103">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="78def-103">RecurringMasterItemId</span></span>

<span data-ttu-id="78def-104">**RecurringMasterItemId**要素は、関連するオカレンスアイテムの1つの識別子を識別することによって、定期的なアイテムのマスターアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="78def-104">The **RecurringMasterItemId** element identifies a recurrence master item by identifying the identifiers of one of its related occurrence items.</span></span> 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 <span data-ttu-id="78def-105">**RecurringMasterItemIdType**</span><span class="sxs-lookup"><span data-stu-id="78def-105">**RecurringMasterItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="78def-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="78def-106">Attributes and elements</span></span>

<span data-ttu-id="78def-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="78def-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78def-108">属性</span><span class="sxs-lookup"><span data-stu-id="78def-108">Attributes</span></span>

|<span data-ttu-id="78def-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="78def-109">**Attribute**</span></span>|<span data-ttu-id="78def-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="78def-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="78def-111">**OccurrenceId**</span><span class="sxs-lookup"><span data-stu-id="78def-111">**OccurrenceId**</span></span> <br/> |<span data-ttu-id="78def-112">定期的なアイテムのマスターアイテムの1つの発生を識別します。</span><span class="sxs-lookup"><span data-stu-id="78def-112">Identifies a single occurrence of a recurring master item.</span></span> <span data-ttu-id="78def-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="78def-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="78def-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="78def-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="78def-115">定期的なアイテムの1つのオカレンスの特定のバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="78def-115">Identifies a specific version of a single occurrence of a recurring master item.</span></span> <span data-ttu-id="78def-116">また、定期的なマスターアイテムと単一のオカレンスに同じ変更キーが含まれているため、これらも確認されます。</span><span class="sxs-lookup"><span data-stu-id="78def-116">Additionally, the recurring master item is also identified because it and the single occurrence will contain the same change key.</span></span> <span data-ttu-id="78def-117">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="78def-117">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="78def-118">子要素</span><span class="sxs-lookup"><span data-stu-id="78def-118">Child elements</span></span>

<span data-ttu-id="78def-119">なし。</span><span class="sxs-lookup"><span data-stu-id="78def-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="78def-120">親要素</span><span class="sxs-lookup"><span data-stu-id="78def-120">Parent elements</span></span>

|<span data-ttu-id="78def-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="78def-121">**Element**</span></span>|<span data-ttu-id="78def-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="78def-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78def-123">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="78def-123">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="78def-124">メールボックス内のすべての会話アイテムのアイテム識別子のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="78def-124">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="78def-125">ItemChange</span><span class="sxs-lookup"><span data-stu-id="78def-125">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="78def-126">アイテム識別子と、アイテムに適用する更新を含みます。</span><span class="sxs-lookup"><span data-stu-id="78def-126">Contains an item identifier and the updates to apply to the item.</span></span> <br/> <br/> <span data-ttu-id="78def-127">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="78def-127">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[<span data-ttu-id="78def-128">ItemIds</span><span class="sxs-lookup"><span data-stu-id="78def-128">ItemIds</span></span>](itemids.md) <br/> | <span data-ttu-id="78def-129">Exchange ストア内のアイテムの削除、送信、取得、移動、またはコピーに使用されるアイテム、オカレンスアイテム、定期的なマスターアイテムの一意の id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="78def-129">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span> <br/> <br/>  <span data-ttu-id="78def-130">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="78def-130">The following are the XPath expressions to this element:</span></span>  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="78def-131">テキスト値</span><span class="sxs-lookup"><span data-stu-id="78def-131">Text value</span></span>

<span data-ttu-id="78def-132">なし。</span><span class="sxs-lookup"><span data-stu-id="78def-132">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="78def-133">注釈</span><span class="sxs-lookup"><span data-stu-id="78def-133">Remarks</span></span>

<span data-ttu-id="78def-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="78def-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="78def-135">例</span><span class="sxs-lookup"><span data-stu-id="78def-135">Example</span></span>

<span data-ttu-id="78def-136">次の例では、56lkjh6 という識別子を持つオカレンスの1つを識別することによって、定期的なマスターアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="78def-136">The following example identifies the recurring master item by identifying one of its occurrences with the identifier 56lkjh6.</span></span>
  
```XML
<RecurringMasterItemId OccurrenceId="56lkjh6" />
```

## <a name="element-information"></a><span data-ttu-id="78def-137">要素の情報</span><span class="sxs-lookup"><span data-stu-id="78def-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78def-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="78def-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="78def-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="78def-139">Schema Name</span></span>  <br/> |<span data-ttu-id="78def-140">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="78def-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="78def-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="78def-141">Validation File</span></span>  <br/> |<span data-ttu-id="78def-142">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="78def-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="78def-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="78def-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="78def-144">正しくない</span><span class="sxs-lookup"><span data-stu-id="78def-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="78def-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="78def-145">See also</span></span>

- [<span data-ttu-id="78def-146">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="78def-146">OccurrenceItemId</span></span>](occurrenceitemid.md)
- [<span data-ttu-id="78def-147">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="78def-147">FindConversation operation</span></span>](findconversation-operation.md)


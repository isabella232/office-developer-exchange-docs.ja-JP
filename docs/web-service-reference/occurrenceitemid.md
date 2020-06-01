---
title: OccurrenceItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OccurrenceItemId
api_type:
- schema
ms.assetid: 4a15bbc3-5b93-4193-b9ec-da32f0a9a552
description: OccurrenceItemId 要素は、定期的なアイテムの単一のオカレンスを識別します。
ms.openlocfilehash: 37c3a2442afb3302bca88ef0301e98013ff0319b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468377"
---
# <a name="occurrenceitemid"></a><span data-ttu-id="b98e0-103">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="b98e0-103">OccurrenceItemId</span></span>

<span data-ttu-id="b98e0-104">**OccurrenceItemId**要素は、定期的なアイテムの単一のオカレンスを識別します。</span><span class="sxs-lookup"><span data-stu-id="b98e0-104">The **OccurrenceItemId** element identifies a single occurrence of a recurring item.</span></span> 
  
```XML
<OccurrenceItemId RecurringMasterId="" ChangeKey="" InstanceIndex=""/>
```

<span data-ttu-id="b98e0-105">**OccurrenceItemIdType**</span><span class="sxs-lookup"><span data-stu-id="b98e0-105">**OccurrenceItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b98e0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b98e0-106">Attributes and elements</span></span>

<span data-ttu-id="b98e0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b98e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b98e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="b98e0-108">Attributes</span></span>

|<span data-ttu-id="b98e0-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="b98e0-109">**Attribute**</span></span>|<span data-ttu-id="b98e0-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="b98e0-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b98e0-111">**RecurringMasterId**</span><span class="sxs-lookup"><span data-stu-id="b98e0-111">**RecurringMasterId**</span></span> <br/> |<span data-ttu-id="b98e0-112">定期的なアイテムの定期的なマスターを識別します。</span><span class="sxs-lookup"><span data-stu-id="b98e0-112">Identifies the recurring master of a recurring item.</span></span> <span data-ttu-id="b98e0-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="b98e0-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="b98e0-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="b98e0-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="b98e0-115">特定のバージョンの定期的なマスターまたはアイテムの発生を識別します。</span><span class="sxs-lookup"><span data-stu-id="b98e0-115">Identifies a specific version of the recurring master or an item occurrence.</span></span> <span data-ttu-id="b98e0-116">定期的マスターまたはそのいずれかのオカレンスが変更された場合は、 **Changekey**が変更されます。</span><span class="sxs-lookup"><span data-stu-id="b98e0-116">If either the recurring master or any of its occurrences change, the **ChangeKey** changes.</span></span> <span data-ttu-id="b98e0-117">**Changekey**は、定期的なマスターとすべてのオカレンスで同じです。</span><span class="sxs-lookup"><span data-stu-id="b98e0-117">The **ChangeKey** is the same for the recurring master and all occurrences.</span></span>  <br/> |
|<span data-ttu-id="b98e0-118">**InstanceIndex**</span><span class="sxs-lookup"><span data-stu-id="b98e0-118">**InstanceIndex**</span></span> <br/> |<span data-ttu-id="b98e0-119">アイテムのオカレンスのインデックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="b98e0-119">Identifies the index of the item occurrence.</span></span> <span data-ttu-id="b98e0-120">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="b98e0-120">This attribute is required.</span></span> <span data-ttu-id="b98e0-121">この値は、整数を表します。</span><span class="sxs-lookup"><span data-stu-id="b98e0-121">This value represents an integer.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b98e0-122">子要素</span><span class="sxs-lookup"><span data-stu-id="b98e0-122">Child elements</span></span>

<span data-ttu-id="b98e0-123">なし。</span><span class="sxs-lookup"><span data-stu-id="b98e0-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b98e0-124">親要素</span><span class="sxs-lookup"><span data-stu-id="b98e0-124">Parent elements</span></span>

|<span data-ttu-id="b98e0-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="b98e0-125">**Element**</span></span>|<span data-ttu-id="b98e0-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="b98e0-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b98e0-127">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="b98e0-127">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="b98e0-128">メールボックス内のすべての会話アイテムのアイテム識別子のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b98e0-128">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="b98e0-129">ItemIds</span><span class="sxs-lookup"><span data-stu-id="b98e0-129">ItemIds</span></span>](itemids.md) <br/> | <span data-ttu-id="b98e0-130">Exchange ストア内のアイテムの削除、送信、取得、移動、またはコピーに使用されるアイテム、オカレンスアイテム、定期的なマスターアイテムの一意の id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b98e0-130">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span> <br/><br/><span data-ttu-id="b98e0-131">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="b98e0-131">The following are the XPath expressions to this element:</span></span> <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/><span data-ttu-id="b98e0-132">**注**: [Moveitem](moveitem-operation.md)操作と[copyitem 操作](copyitem-operation.md)は、1つの予定表アイテムおよび定期的なマスターアイテムに対してのみ機能します。</span><span class="sxs-lookup"><span data-stu-id="b98e0-132">**NOTE**: [MoveItem operation](moveitem-operation.md) and [CopyItem operation](copyitem-operation.md) only work with single calendar items and recurring master items.</span></span> <span data-ttu-id="b98e0-133">アイテムの出現は、これらの操作では無効です。</span><span class="sxs-lookup"><span data-stu-id="b98e0-133">Item occurrences are invalid with these operations.</span></span>           |
|[<span data-ttu-id="b98e0-134">ItemChange</span><span class="sxs-lookup"><span data-stu-id="b98e0-134">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="b98e0-135">アイテム識別子と、アイテムに適用する更新を含みます。</span><span class="sxs-lookup"><span data-stu-id="b98e0-135">Contains an item identifier and the updates to apply to the item.</span></span><br/><br/> <span data-ttu-id="b98e0-136">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b98e0-136">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b98e0-137">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b98e0-137">Text value</span></span>

<span data-ttu-id="b98e0-138">なし。</span><span class="sxs-lookup"><span data-stu-id="b98e0-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b98e0-139">注釈</span><span class="sxs-lookup"><span data-stu-id="b98e0-139">Remarks</span></span>

<span data-ttu-id="b98e0-140">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b98e0-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="b98e0-141">例</span><span class="sxs-lookup"><span data-stu-id="b98e0-141">Example</span></span>

<span data-ttu-id="b98e0-142">次の例では、id が34vswe4 である定期的なアイテムの4番目の発生を識別します。</span><span class="sxs-lookup"><span data-stu-id="b98e0-142">The following example identifies the fourth occurrence of a recurring item that has the identity 34vswe4.</span></span>
  
```XML
<OccurrenceItemId RecurringMasterId="34vswe4" InstanceIndex="4" />
```

## <a name="element-information"></a><span data-ttu-id="b98e0-143">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b98e0-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b98e0-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="b98e0-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b98e0-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b98e0-145">Schema Name</span></span>  <br/> |<span data-ttu-id="b98e0-146">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b98e0-146">Types schema</span></span>  <br/> |
|<span data-ttu-id="b98e0-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b98e0-147">Validation File</span></span>  <br/> |<span data-ttu-id="b98e0-148">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b98e0-148">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b98e0-149">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b98e0-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="b98e0-150">正しくない</span><span class="sxs-lookup"><span data-stu-id="b98e0-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b98e0-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="b98e0-151">See also</span></span>

- [<span data-ttu-id="b98e0-152">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="b98e0-152">RecurringMasterItemId</span></span>](recurringmasteritemid.md)
- [<span data-ttu-id="b98e0-153">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="b98e0-153">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="b98e0-154">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b98e0-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


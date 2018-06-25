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
description: OccurrenceItemId 要素は、定期的なアイテムの 1 回の発生を識別します。
ms.openlocfilehash: e3d7b6efc49775f54219ce0dc0ec39a34a95f8fd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832639"
---
# <a name="occurrenceitemid"></a><span data-ttu-id="0fa83-103">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="0fa83-103">OccurrenceItemId</span></span>

<span data-ttu-id="0fa83-104">**OccurrenceItemId**要素は、定期的なアイテムの 1 回の発生を識別します。</span><span class="sxs-lookup"><span data-stu-id="0fa83-104">The **OccurrenceItemId** element identifies a single occurrence of a recurring item.</span></span> 
  
```XML
<OccurrenceItemId RecurringMasterId="" ChangeKey="" InstanceIndex=""/>
```

<span data-ttu-id="0fa83-105">**OccurrenceItemIdType**</span><span class="sxs-lookup"><span data-stu-id="0fa83-105">**OccurrenceItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0fa83-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0fa83-106">Attributes and elements</span></span>

<span data-ttu-id="0fa83-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0fa83-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0fa83-108">属性</span><span class="sxs-lookup"><span data-stu-id="0fa83-108">Attributes</span></span>

|<span data-ttu-id="0fa83-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="0fa83-109">**Attribute**</span></span>|<span data-ttu-id="0fa83-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="0fa83-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0fa83-111">**RecurringMasterId**</span><span class="sxs-lookup"><span data-stu-id="0fa83-111">**RecurringMasterId**</span></span> <br/> |<span data-ttu-id="0fa83-112">定期的なアイテムの定期的なマスターを識別します。</span><span class="sxs-lookup"><span data-stu-id="0fa83-112">Identifies the recurring master of a recurring item.</span></span> <span data-ttu-id="0fa83-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="0fa83-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="0fa83-114">**変更キー**</span><span class="sxs-lookup"><span data-stu-id="0fa83-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="0fa83-115">定期的なマスターか、アイテムの特定のバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="0fa83-115">Identifies a specific version of the recurring master or an item occurrence.</span></span> <span data-ttu-id="0fa83-116">定期的なマスターまたはその項目のいずれかのいずれかを変更する場合は、**変更キー**が変更されます。</span><span class="sxs-lookup"><span data-stu-id="0fa83-116">If either the recurring master or any of its occurrences change, the **ChangeKey** changes.</span></span> <span data-ttu-id="0fa83-117">**変更キー**は、定期的なマスターとすべて同じです。</span><span class="sxs-lookup"><span data-stu-id="0fa83-117">The **ChangeKey** is the same for the recurring master and all occurrences.</span></span>  <br/> |
|<span data-ttu-id="0fa83-118">**InstanceIndex**</span><span class="sxs-lookup"><span data-stu-id="0fa83-118">**InstanceIndex**</span></span> <br/> |<span data-ttu-id="0fa83-119">アイテムの出現するインデックス位置を識別します。</span><span class="sxs-lookup"><span data-stu-id="0fa83-119">Identifies the index of the item occurrence.</span></span> <span data-ttu-id="0fa83-120">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="0fa83-120">This attribute is required.</span></span> <span data-ttu-id="0fa83-121">この値は、整数を表します。</span><span class="sxs-lookup"><span data-stu-id="0fa83-121">This value represents an integer.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0fa83-122">子要素</span><span class="sxs-lookup"><span data-stu-id="0fa83-122">Child elements</span></span>

<span data-ttu-id="0fa83-123">なし。</span><span class="sxs-lookup"><span data-stu-id="0fa83-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0fa83-124">親要素</span><span class="sxs-lookup"><span data-stu-id="0fa83-124">Parent elements</span></span>

|<span data-ttu-id="0fa83-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="0fa83-125">**Element**</span></span>|<span data-ttu-id="0fa83-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="0fa83-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0fa83-127">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="0fa83-127">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="0fa83-128">メールボックス内のすべての会話項目の項目の識別子のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0fa83-128">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0fa83-129">Itemid</span><span class="sxs-lookup"><span data-stu-id="0fa83-129">ItemIds</span></span>](itemids.md) <br/> | <span data-ttu-id="0fa83-130">アイテム、出現アイテム、および削除、送信、取得、移動、または Exchange ストア内のアイテムのコピーに使用される、マスターの定期的なアイテムの一意の id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0fa83-130">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span> <br/><br/><span data-ttu-id="0fa83-131">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="0fa83-131">The following are the XPath expressions to this element:</span></span> <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/><span data-ttu-id="0fa83-132">**注**: [MoveItem 操作](moveitem-operation.md)および[CopyItem の操作](copyitem-operation.md)が 1 つの予定表アイテムと定期的なアイテムをマスターでのみ動作します。</span><span class="sxs-lookup"><span data-stu-id="0fa83-132">**Note**:  [MoveItem operation](moveitem-operation.md) and [CopyItem operation](copyitem-operation.md) only work with single calendar items and recurring master items.</span></span> <span data-ttu-id="0fa83-133">アイテムの出現回数は、これらの操作では無効です。</span><span class="sxs-lookup"><span data-stu-id="0fa83-133">Item occurrences are invalid with these operations.</span></span>           |
|[<span data-ttu-id="0fa83-134">ItemChange</span><span class="sxs-lookup"><span data-stu-id="0fa83-134">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="0fa83-135">アイテム識別子と、アイテムに適用する更新プログラムが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0fa83-135">Contains an item identifier and the updates to apply to the item.</span></span><br/><br/> <span data-ttu-id="0fa83-136">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="0fa83-136">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0fa83-137">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0fa83-137">Text value</span></span>

<span data-ttu-id="0fa83-138">なし。</span><span class="sxs-lookup"><span data-stu-id="0fa83-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0fa83-139">備考</span><span class="sxs-lookup"><span data-stu-id="0fa83-139">Remarks</span></span>

<span data-ttu-id="0fa83-140">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0fa83-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="0fa83-141">例</span><span class="sxs-lookup"><span data-stu-id="0fa83-141">Example</span></span>

<span data-ttu-id="0fa83-142">次の例では、4 番目の id 34vswe4 を持つ定期的なアイテムの発生を識別します。</span><span class="sxs-lookup"><span data-stu-id="0fa83-142">The following example identifies the fourth occurrence of a recurring item that has the identity 34vswe4.</span></span>
  
```XML
<OccurrenceItemId RecurringMasterId="34vswe4" InstanceIndex="4" />
```

## <a name="element-information"></a><span data-ttu-id="0fa83-143">要素情報</span><span class="sxs-lookup"><span data-stu-id="0fa83-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0fa83-144">名前空間</span><span class="sxs-lookup"><span data-stu-id="0fa83-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0fa83-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0fa83-145">Schema Name</span></span>  <br/> |<span data-ttu-id="0fa83-146">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="0fa83-146">Types schema</span></span>  <br/> |
|<span data-ttu-id="0fa83-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0fa83-147">Validation File</span></span>  <br/> |<span data-ttu-id="0fa83-148">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0fa83-148">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0fa83-149">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0fa83-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="0fa83-150">False</span><span class="sxs-lookup"><span data-stu-id="0fa83-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0fa83-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="0fa83-151">See also</span></span>

- [<span data-ttu-id="0fa83-152">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="0fa83-152">RecurringMasterItemId</span></span>](recurringmasteritemid.md)
- <span data-ttu-id="0fa83-153">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="0fa83-153">[FindConversation operation](findconversation-operation.md)</span></span>
- [<span data-ttu-id="0fa83-154">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0fa83-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


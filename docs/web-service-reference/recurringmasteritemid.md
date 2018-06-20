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
description: RecurringMasterItemId 要素は、その出現の関連する項目の 1 つの識別子を識別することによって、定期的な予定のマスター アイテムを識別します。
ms.openlocfilehash: ae59e33ece55d85435ece4c9030ccda32eb62eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833015"
---
# <a name="recurringmasteritemid"></a><span data-ttu-id="5e3e7-103">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="5e3e7-103">RecurringMasterItemId</span></span>

<span data-ttu-id="5e3e7-104">**RecurringMasterItemId**要素は、その出現の関連する項目の 1 つの識別子を識別することによって、定期的な予定のマスター アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="5e3e7-104">The **RecurringMasterItemId** element identifies a recurrence master item by identifying the identifiers of one of its related occurrence items.</span></span> 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 <span data-ttu-id="5e3e7-105">**RecurringMasterItemIdType**</span><span class="sxs-lookup"><span data-stu-id="5e3e7-105">**RecurringMasterItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5e3e7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5e3e7-106">Attributes and elements</span></span>

<span data-ttu-id="5e3e7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5e3e7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5e3e7-108">属性</span><span class="sxs-lookup"><span data-stu-id="5e3e7-108">Attributes</span></span>

|<span data-ttu-id="5e3e7-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="5e3e7-109">**Attribute**</span></span>|<span data-ttu-id="5e3e7-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="5e3e7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5e3e7-111">**OccurrenceId**</span><span class="sxs-lookup"><span data-stu-id="5e3e7-111">**OccurrenceId**</span></span> <br/> |<span data-ttu-id="5e3e7-112">マスターの定期的なアイテムの 1 回の発生を識別します。</span><span class="sxs-lookup"><span data-stu-id="5e3e7-112">Identifies a single occurrence of a recurring master item.</span></span> <span data-ttu-id="5e3e7-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e3e7-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="5e3e7-114">**変更キー**</span><span class="sxs-lookup"><span data-stu-id="5e3e7-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="5e3e7-115">マスターの定期的なアイテムの 1 回の特定のバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="5e3e7-115">Identifies a specific version of a single occurrence of a recurring master item.</span></span> <span data-ttu-id="5e3e7-116">さらに、定期的なマスター アイテムは、1 回の会議と同じキーの変更が格納されるためにも識別されます。</span><span class="sxs-lookup"><span data-stu-id="5e3e7-116">Additionally, the recurring master item is also identified because it and the single occurrence will contain the same change key.</span></span> <span data-ttu-id="5e3e7-117">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="5e3e7-117">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5e3e7-118">子要素</span><span class="sxs-lookup"><span data-stu-id="5e3e7-118">Child elements</span></span>

<span data-ttu-id="5e3e7-119">なし。</span><span class="sxs-lookup"><span data-stu-id="5e3e7-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5e3e7-120">親要素</span><span class="sxs-lookup"><span data-stu-id="5e3e7-120">Parent elements</span></span>

|<span data-ttu-id="5e3e7-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="5e3e7-121">**Element**</span></span>|<span data-ttu-id="5e3e7-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="5e3e7-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e3e7-123">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="5e3e7-123">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="5e3e7-124">メールボックス内のすべての会話項目の項目の識別子のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5e3e7-124">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5e3e7-125">ItemChange</span><span class="sxs-lookup"><span data-stu-id="5e3e7-125">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="5e3e7-126">アイテム識別子と、アイテムに適用する更新プログラムが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5e3e7-126">Contains an item identifier and the updates to apply to the item.</span></span> <br/> <br/> <span data-ttu-id="5e3e7-127">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="5e3e7-127">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[<span data-ttu-id="5e3e7-128">Itemid</span><span class="sxs-lookup"><span data-stu-id="5e3e7-128">ItemIds</span></span>](itemids.md) <br/> | <span data-ttu-id="5e3e7-129">アイテム、出現アイテム、および削除、送信、取得、移動、または Exchange ストア内のアイテムのコピーに使用される、マスターの定期的なアイテムの一意の id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5e3e7-129">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span> <br/> <br/>  <span data-ttu-id="5e3e7-130">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="5e3e7-130">The following are the XPath expressions to this element:</span></span>  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5e3e7-131">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5e3e7-131">Text value</span></span>

<span data-ttu-id="5e3e7-132">なし。</span><span class="sxs-lookup"><span data-stu-id="5e3e7-132">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5e3e7-133">備考</span><span class="sxs-lookup"><span data-stu-id="5e3e7-133">Remarks</span></span>

<span data-ttu-id="5e3e7-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5e3e7-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="5e3e7-135">例</span><span class="sxs-lookup"><span data-stu-id="5e3e7-135">Example</span></span>

<span data-ttu-id="5e3e7-136">次の例では、その識別子の 56lkjh6 とのいずれかを識別することによって定期的なマスター アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="5e3e7-136">The following example identifies the recurring master item by identifying one of its occurrences with the identifier 56lkjh6.</span></span>
  
```XML
<RecurringMasterItemId OccurrenceId="56lkjh6" />
```

## <a name="element-information"></a><span data-ttu-id="5e3e7-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="5e3e7-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5e3e7-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="5e3e7-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5e3e7-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5e3e7-139">Schema Name</span></span>  <br/> |<span data-ttu-id="5e3e7-140">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5e3e7-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="5e3e7-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5e3e7-141">Validation File</span></span>  <br/> |<span data-ttu-id="5e3e7-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5e3e7-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5e3e7-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5e3e7-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="5e3e7-144">False</span><span class="sxs-lookup"><span data-stu-id="5e3e7-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5e3e7-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="5e3e7-145">See also</span></span>

- [<span data-ttu-id="5e3e7-146">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="5e3e7-146">OccurrenceItemId</span></span>](occurrenceitemid.md)
- <span data-ttu-id="5e3e7-147">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="5e3e7-147">[FindConversation operation](findconversation-operation.md)</span></span>


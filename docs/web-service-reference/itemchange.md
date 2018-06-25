---
title: ItemChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemChange
api_type:
- schema
ms.assetid: 5cb43b02-d444-4d9c-9075-cdc5a4427daf
description: ItemChange 要素には、項目 id と、アイテムに適用する更新プログラムが含まれています。
ms.openlocfilehash: d10ce96cacb0be7411c4e8230ebc9b2803b7a5b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832145"
---
# <a name="itemchange"></a><span data-ttu-id="13055-103">ItemChange</span><span class="sxs-lookup"><span data-stu-id="13055-103">ItemChange</span></span>

<span data-ttu-id="13055-104">**ItemChange**要素には、項目 id と、アイテムに適用する更新プログラムが含まれています。</span><span class="sxs-lookup"><span data-stu-id="13055-104">The **ItemChange** element contains an item identifier and the updates to apply to the item.</span></span> 
  
[<span data-ttu-id="13055-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="13055-105">UpdateItem</span></span>](updateitem.md)
  
[<span data-ttu-id="13055-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="13055-106">ItemChanges</span></span>](itemchanges.md)
  
[<span data-ttu-id="13055-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="13055-107">ItemChange</span></span>](itemchange.md)
  
```xml
<ItemChange>
   <ItemId/>
   <Updates>...</Updates>
</ItemChange>
```

 <span data-ttu-id="13055-108">**ItemChangeType**</span><span class="sxs-lookup"><span data-stu-id="13055-108">**ItemChangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="13055-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="13055-109">Attributes and elements</span></span>

<span data-ttu-id="13055-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="13055-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="13055-111">属性</span><span class="sxs-lookup"><span data-stu-id="13055-111">Attributes</span></span>

<span data-ttu-id="13055-112">なし。</span><span class="sxs-lookup"><span data-stu-id="13055-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="13055-113">子要素</span><span class="sxs-lookup"><span data-stu-id="13055-113">Child elements</span></span>

|<span data-ttu-id="13055-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="13055-114">**Element**</span></span>|<span data-ttu-id="13055-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="13055-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13055-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="13055-116">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="13055-117">Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="13055-117">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="13055-118">[OccurrenceItemId](occurrenceitemid.md)または[RecurringMasterItemId](recurringmasteritemid.md)要素を使用しない場合、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="13055-118">This element is required if the [OccurrenceItemId](occurrenceitemid.md) or [RecurringMasterItemId](recurringmasteritemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="13055-119">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="13055-119">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="13055-120">定期的なアイテムの 1 回の発生を識別します。</span><span class="sxs-lookup"><span data-stu-id="13055-120">Identifies a single occurrence of a recurring item.</span></span> <span data-ttu-id="13055-121">使用する場合、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="13055-121">This element is required if used.</span></span> <span data-ttu-id="13055-122">[RecurringMasterItemId](recurringmasteritemid.md)または[アイテム Id](itemid.md)要素を使用しない場合、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="13055-122">This element is required if the [RecurringMasterItemId](recurringmasteritemid.md) or [ItemId](itemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="13055-123">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="13055-123">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="13055-124">関連の出現アイテムの id のいずれかを識別することによって、定期的な予定のマスター アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="13055-124">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span> <span data-ttu-id="13055-125">使用する場合、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="13055-125">This element is required if used.</span></span> <span data-ttu-id="13055-126">[OccurrenceItemId](occurrenceitemid.md)または[アイテム Id](itemid.md)要素を使用しない場合、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="13055-126">This element is required if the [OccurrenceItemId](occurrenceitemid.md) or [ItemId](itemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="13055-127">更新 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="13055-127">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="13055-128">定義する配列が含まれていて、このオプションを設定すると、アイテムのプロパティの変更を削除します。</span><span class="sxs-lookup"><span data-stu-id="13055-128">Contains an array that defines append, set, and delete changes to item properties.</span></span> <span data-ttu-id="13055-129">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="13055-129">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="13055-130">親要素</span><span class="sxs-lookup"><span data-stu-id="13055-130">Parent elements</span></span>

|<span data-ttu-id="13055-131">**要素**</span><span class="sxs-lookup"><span data-stu-id="13055-131">**Element**</span></span>|<span data-ttu-id="13055-132">**説明**</span><span class="sxs-lookup"><span data-stu-id="13055-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13055-133">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="13055-133">ItemChanges</span></span>](itemchanges.md) <br/> |<span data-ttu-id="13055-134">アイテムと、アイテムに適用する更新プログラムを識別する[ItemChange](itemchange.md)要素の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="13055-134">Contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span>  <br/> <span data-ttu-id="13055-135">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="13055-135">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem/ItemChanges` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="13055-136">備考</span><span class="sxs-lookup"><span data-stu-id="13055-136">Remarks</span></span>

<span data-ttu-id="13055-137">**ItemChange**要素では、唯一の[アイテム Id](itemid.md)、 [OccurrenceItemId](occurrenceitemid.md)、または[RecurringMasterItemId](recurringmasteritemid.md)要素を使用できます。</span><span class="sxs-lookup"><span data-stu-id="13055-137">Only a single [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md), or [RecurringMasterItemId](recurringmasteritemid.md) element can be used in an **ItemChange** element.</span></span> 
  
<span data-ttu-id="13055-138">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="13055-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="13055-139">要素情報</span><span class="sxs-lookup"><span data-stu-id="13055-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="13055-140">名前空間</span><span class="sxs-lookup"><span data-stu-id="13055-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="13055-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="13055-141">Schema Name</span></span>  <br/> |<span data-ttu-id="13055-142">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="13055-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="13055-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="13055-143">Validation File</span></span>  <br/> |<span data-ttu-id="13055-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="13055-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="13055-145">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="13055-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="13055-146">False</span><span class="sxs-lookup"><span data-stu-id="13055-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="13055-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="13055-147">See also</span></span>



<span data-ttu-id="13055-148">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="13055-148">[UpdateItem operation](updateitem-operation.md)</span></span>


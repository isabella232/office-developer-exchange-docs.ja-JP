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
description: ItemChange 要素には、アイテムの識別子と、アイテムに適用する更新が含まれています。
ms.openlocfilehash: 916ef1ba2c7a709ec1fd80ababd72999506773c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459918"
---
# <a name="itemchange"></a><span data-ttu-id="b4332-103">ItemChange</span><span class="sxs-lookup"><span data-stu-id="b4332-103">ItemChange</span></span>

<span data-ttu-id="b4332-104">**Itemchange**要素には、アイテムの識別子と、アイテムに適用する更新が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b4332-104">The **ItemChange** element contains an item identifier and the updates to apply to the item.</span></span> 
  
- [<span data-ttu-id="b4332-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="b4332-105">UpdateItem</span></span>](updateitem.md) 
- [<span data-ttu-id="b4332-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="b4332-106">ItemChanges</span></span>](itemchanges.md)
- [<span data-ttu-id="b4332-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="b4332-107">ItemChange</span></span>](itemchange.md)
  
```xml
<ItemChange>
   <ItemId/>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <OccurrenceItemId>...</OccurrenceItemId>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <RecurringMasterItemId>...</RecurringMasterItemId>
   <Updates>...</Updates>
</ItemChange>
```

<span data-ttu-id="b4332-108">**ItemChangeType**</span><span class="sxs-lookup"><span data-stu-id="b4332-108">**ItemChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b4332-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b4332-109">Attributes and elements</span></span>

<span data-ttu-id="b4332-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b4332-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b4332-111">属性</span><span class="sxs-lookup"><span data-stu-id="b4332-111">Attributes</span></span>

<span data-ttu-id="b4332-112">なし。</span><span class="sxs-lookup"><span data-stu-id="b4332-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b4332-113">子要素</span><span class="sxs-lookup"><span data-stu-id="b4332-113">Child elements</span></span>

|<span data-ttu-id="b4332-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="b4332-114">**Element**</span></span>|<span data-ttu-id="b4332-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="b4332-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4332-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="b4332-116">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="b4332-117">Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b4332-117">Contains the unique identifier and change key of an item in the Exchange store.</span></span> <span data-ttu-id="b4332-118">この要素は、 [OccurrenceItemId](occurrenceitemid.md)または[RecurringMasterItemId](recurringmasteritemid.md)要素が使用されていない場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="b4332-118">This element is required if the [OccurrenceItemId](occurrenceitemid.md) or [RecurringMasterItemId](recurringmasteritemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="b4332-119">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="b4332-119">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="b4332-120">定期的なアイテムの1回の出現を識別します。</span><span class="sxs-lookup"><span data-stu-id="b4332-120">Identifies a single occurrence of a recurring item.</span></span> <span data-ttu-id="b4332-121">この要素は、使用する場合は必須です。</span><span class="sxs-lookup"><span data-stu-id="b4332-121">This element is required if used.</span></span> <span data-ttu-id="b4332-122">この要素は、 [RecurringMasterItemId](recurringmasteritemid.md)または[ItemId](itemid.md)要素が使用されていない場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="b4332-122">This element is required if the [RecurringMasterItemId](recurringmasteritemid.md) or [ItemId](itemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="b4332-123">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="b4332-123">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="b4332-124">関連するオカレンスアイテムの識別子の1つを識別することによって、定期的なアイテムのマスターアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="b4332-124">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span> <span data-ttu-id="b4332-125">この要素は、使用する場合は必須です。</span><span class="sxs-lookup"><span data-stu-id="b4332-125">This element is required if used.</span></span> <span data-ttu-id="b4332-126">この要素は、 [OccurrenceItemId](occurrenceitemid.md)または[ItemId](itemid.md)要素が使用されていない場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="b4332-126">This element is required if the [OccurrenceItemId](occurrenceitemid.md) or [ItemId](itemid.md) element is not used.</span></span>  <br/> |
|[<span data-ttu-id="b4332-127">Updates (Item)</span><span class="sxs-lookup"><span data-stu-id="b4332-127">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="b4332-128">アイテムのプロパティに対する追加、設定、および削除の変更を定義する配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="b4332-128">Contains an array that defines append, set, and delete changes to item properties.</span></span> <span data-ttu-id="b4332-129">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="b4332-129">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b4332-130">親要素</span><span class="sxs-lookup"><span data-stu-id="b4332-130">Parent elements</span></span>

|<span data-ttu-id="b4332-131">**要素**</span><span class="sxs-lookup"><span data-stu-id="b4332-131">**Element**</span></span>|<span data-ttu-id="b4332-132">**説明**</span><span class="sxs-lookup"><span data-stu-id="b4332-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4332-133">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="b4332-133">ItemChanges</span></span>](itemchanges.md) <br/> |<span data-ttu-id="b4332-134">アイテムとアイテムに適用する更新を識別する[Itemchange](itemchange.md)要素の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b4332-134">Contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span>  <br/> <span data-ttu-id="b4332-135">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b4332-135">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem/ItemChanges` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b4332-136">注釈</span><span class="sxs-lookup"><span data-stu-id="b4332-136">Remarks</span></span>

<span data-ttu-id="b4332-137">**Itemchange**要素に使用できる[ItemId](itemid.md)、 [OccurrenceItemId](occurrenceitemid.md)、または[RecurringMasterItemId](recurringmasteritemid.md)要素は1つだけです。</span><span class="sxs-lookup"><span data-stu-id="b4332-137">Only a single [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md), or [RecurringMasterItemId](recurringmasteritemid.md) element can be used in an **ItemChange** element.</span></span> 
  
<span data-ttu-id="b4332-138">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b4332-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b4332-139">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b4332-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b4332-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="b4332-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b4332-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b4332-141">Schema Name</span></span>  <br/> |<span data-ttu-id="b4332-142">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b4332-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="b4332-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b4332-143">Validation File</span></span>  <br/> |<span data-ttu-id="b4332-144">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b4332-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b4332-145">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b4332-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="b4332-146">正しくない</span><span class="sxs-lookup"><span data-stu-id="b4332-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b4332-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="b4332-147">See also</span></span>

- <span data-ttu-id="b4332-148">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="b4332-148">[UpdateItem operation](updateitem-operation.md)</span></span>


---
title: ItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemIds
api_type:
- schema
ms.assetid: 6b82122b-5544-4adf-91b7-ef2db7d5046f
description: ItemIds 要素には、アイテム、発生アイテム、および定期的なマスターアイテムの一意の id が含まれており、Exchange ストア内のアイテムの削除、送信、取得、移動、またはコピーに使用できます。
ms.openlocfilehash: bbd594ce2610bd625b0e16a0383fda552ee9eb19
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460604"
---
# <a name="itemids"></a><span data-ttu-id="dc3ae-103">ItemIds</span><span class="sxs-lookup"><span data-stu-id="dc3ae-103">ItemIds</span></span>
  
<span data-ttu-id="dc3ae-104">**Itemids**要素には、アイテム、発生アイテム、および定期的なマスターアイテムの一意の id が含まれており、Exchange ストア内のアイテムの削除、送信、取得、移動、またはコピーに使用できます。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-104">The **ItemIds** element contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span>
  
```xml
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

<span data-ttu-id="dc3ae-105">**非 Emptyarrayofbaseitemidstype**</span><span class="sxs-lookup"><span data-stu-id="dc3ae-105">**NonEmptyArrayOfBaseItemIdsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="dc3ae-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="dc3ae-106">Attributes and elements</span></span>

<span data-ttu-id="dc3ae-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-107">The following sections describe attributes, child elements, and parent elements.</span></span> 
  
### <a name="attributes"></a><span data-ttu-id="dc3ae-108">属性</span><span class="sxs-lookup"><span data-stu-id="dc3ae-108">Attributes</span></span>

<span data-ttu-id="dc3ae-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc3ae-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dc3ae-110">Child elements</span></span>

|<span data-ttu-id="dc3ae-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="dc3ae-111">**Element**</span></span>|<span data-ttu-id="dc3ae-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="dc3ae-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc3ae-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="dc3ae-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="dc3ae-114">Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-114">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="dc3ae-115">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="dc3ae-115">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="dc3ae-116">定期的なアイテムの1回の出現を識別します。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-116">Identifies a single occurrence of a recurring item.</span></span>  <br/> |
|[<span data-ttu-id="dc3ae-117">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="dc3ae-117">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="dc3ae-118">関連するオカレンスアイテムの識別子の1つを識別することによって、定期的なアイテムのマスターアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-118">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dc3ae-119">親要素</span><span class="sxs-lookup"><span data-stu-id="dc3ae-119">Parent elements</span></span>

|<span data-ttu-id="dc3ae-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="dc3ae-120">**Element**</span></span>|<span data-ttu-id="dc3ae-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="dc3ae-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc3ae-122">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="dc3ae-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="dc3ae-123">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-123">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="dc3ae-124">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="dc3ae-124">DeleteItem</span></span>](deleteitem.md) <br/> |<span data-ttu-id="dc3ae-125">Exchange ストア内のアイテムを削除するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-125">Defines a request to delete items in the Exchange store.</span></span>  <br/> <span data-ttu-id="dc3ae-126">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-126">The following is the XPath expression to this element:</span></span>  <br/>  `/DeleteItem` <br/> |
|[<span data-ttu-id="dc3ae-127">SendItem</span><span class="sxs-lookup"><span data-stu-id="dc3ae-127">SendItem</span></span>](senditem.md) <br/> |<span data-ttu-id="dc3ae-128">Exchange ストア内のアイテムを送信するための要求を定義するルート要素です。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-128">The root element that defines a request to send items in the Exchange store.</span></span>  <br/> <span data-ttu-id="dc3ae-129">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-129">The following is the XPath expression to this element:</span></span>  <br/>  `/SendItem` <br/> |
|[<span data-ttu-id="dc3ae-130">GetItem</span><span class="sxs-lookup"><span data-stu-id="dc3ae-130">GetItem</span></span>](getitem.md) <br/> |<span data-ttu-id="dc3ae-131">Exchange ストアからアイテムを取得するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-131">Defines a request to get items from the Exchange store.</span></span>  <br/> <span data-ttu-id="dc3ae-132">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetItem` <br/> |
|[<span data-ttu-id="dc3ae-133">MoveItem</span><span class="sxs-lookup"><span data-stu-id="dc3ae-133">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="dc3ae-134">Exchange ストア内のアイテムを移動する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-134">Defines a request to move items in the Exchange store.</span></span>  <br/> <span data-ttu-id="dc3ae-135">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-135">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="dc3ae-136">CopyItem</span><span class="sxs-lookup"><span data-stu-id="dc3ae-136">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="dc3ae-137">Exchange ストア内のアイテムをコピーするための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-137">Defines a request to copy items in the Exchange store.</span></span>  <br/> <span data-ttu-id="dc3ae-138">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-138">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dc3ae-139">注釈</span><span class="sxs-lookup"><span data-stu-id="dc3ae-139">Remarks</span></span>

<span data-ttu-id="dc3ae-140">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="dc3ae-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc3ae-141">要素の情報</span><span class="sxs-lookup"><span data-stu-id="dc3ae-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc3ae-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="dc3ae-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dc3ae-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dc3ae-143">Schema Name</span></span>  <br/> |<span data-ttu-id="dc3ae-144">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="dc3ae-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dc3ae-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dc3ae-145">Validation File</span></span>  <br/> |<span data-ttu-id="dc3ae-146">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="dc3ae-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dc3ae-147">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dc3ae-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="dc3ae-148">正しくない</span><span class="sxs-lookup"><span data-stu-id="dc3ae-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc3ae-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="dc3ae-149">See also</span></span>

- [<span data-ttu-id="dc3ae-150">DeleteItem 操作</span><span class="sxs-lookup"><span data-stu-id="dc3ae-150">DeleteItem operation</span></span>](deleteitem-operation.md)
- [<span data-ttu-id="dc3ae-151">SendItem 操作</span><span class="sxs-lookup"><span data-stu-id="dc3ae-151">SendItem operation</span></span>](senditem-operation.md) 
- <span data-ttu-id="dc3ae-152">
  [GetItem 操作](getitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="dc3ae-152">[GetItem operation](getitem-operation.md)</span></span>
- <span data-ttu-id="dc3ae-153">
  [MoveItem 操作](moveitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="dc3ae-153">[MoveItem operation](moveitem-operation.md)</span></span>
- <span data-ttu-id="dc3ae-154">
  [CopyItem 操作](copyitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="dc3ae-154">[CopyItem operation](copyitem-operation.md)</span></span>
- [<span data-ttu-id="dc3ae-155">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="dc3ae-155">FindConversation operation</span></span>](findconversation-operation.md)


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
description: Itemid の要素には、アイテム、出現アイテム、および削除、送信、取得、移動、または Exchange ストア内のアイテムのコピーに使用される、マスターの定期的なアイテムの一意の id が含まれています。
ms.openlocfilehash: 1bd4d6f4593a7c3b418561269d8b29707cc6030c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832155"
---
# <a name="itemids"></a><span data-ttu-id="bc622-103">ItemIds</span><span class="sxs-lookup"><span data-stu-id="bc622-103">ItemIds</span></span>
  
<span data-ttu-id="bc622-104">**Itemid**の要素には、アイテム、出現アイテム、および削除、送信、取得、移動、または Exchange ストア内のアイテムのコピーに使用される、マスターの定期的なアイテムの一意の id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bc622-104">The **ItemIds** element contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span>
  
```xml
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

<span data-ttu-id="bc622-105">**NonEmptyArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="bc622-105">**NonEmptyArrayOfBaseItemIdsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bc622-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bc622-106">Attributes and elements</span></span>

<span data-ttu-id="bc622-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bc622-107">The following sections describe attributes, child elements, and parent elements.</span></span> 
  
### <a name="attributes"></a><span data-ttu-id="bc622-108">属性</span><span class="sxs-lookup"><span data-stu-id="bc622-108">Attributes</span></span>

<span data-ttu-id="bc622-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bc622-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc622-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bc622-110">Child elements</span></span>

|<span data-ttu-id="bc622-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="bc622-111">**Element**</span></span>|<span data-ttu-id="bc622-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="bc622-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc622-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="bc622-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="bc622-114">Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bc622-114">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="bc622-115">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="bc622-115">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="bc622-116">定期的なアイテムの 1 回の発生を識別します。</span><span class="sxs-lookup"><span data-stu-id="bc622-116">Identifies a single occurrence of a recurring item.</span></span>  <br/> |
|[<span data-ttu-id="bc622-117">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="bc622-117">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="bc622-118">関連の出現アイテムの id のいずれかを識別することによって、定期的な予定のマスター アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="bc622-118">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bc622-119">親要素</span><span class="sxs-lookup"><span data-stu-id="bc622-119">Parent elements</span></span>

|<span data-ttu-id="bc622-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="bc622-120">**Element**</span></span>|<span data-ttu-id="bc622-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="bc622-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc622-122">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="bc622-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="bc622-123">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="bc622-123">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="bc622-124">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="bc622-124">DeleteItem</span></span>](deleteitem.md) <br/> |<span data-ttu-id="bc622-125">Exchange ストア内の項目を削除する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="bc622-125">Defines a request to delete items in the Exchange store.</span></span>  <br/> <span data-ttu-id="bc622-126">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="bc622-126">The following is the XPath expression to this element:</span></span>  <br/>  `/DeleteItem` <br/> |
|[<span data-ttu-id="bc622-127">SendItem</span><span class="sxs-lookup"><span data-stu-id="bc622-127">SendItem</span></span>](senditem.md) <br/> |<span data-ttu-id="bc622-128">Exchange ストア内のアイテムを送信する要求を定義するルート要素です。</span><span class="sxs-lookup"><span data-stu-id="bc622-128">The root element that defines a request to send items in the Exchange store.</span></span>  <br/> <span data-ttu-id="bc622-129">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="bc622-129">The following is the XPath expression to this element:</span></span>  <br/>  `/SendItem` <br/> |
|[<span data-ttu-id="bc622-130">GetItem</span><span class="sxs-lookup"><span data-stu-id="bc622-130">GetItem</span></span>](getitem.md) <br/> |<span data-ttu-id="bc622-131">Exchange ストアから項目を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="bc622-131">Defines a request to get items from the Exchange store.</span></span>  <br/> <span data-ttu-id="bc622-132">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="bc622-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetItem` <br/> |
|[<span data-ttu-id="bc622-133">MoveItem</span><span class="sxs-lookup"><span data-stu-id="bc622-133">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="bc622-134">Exchange ストア内のアイテムを移動するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="bc622-134">Defines a request to move items in the Exchange store.</span></span>  <br/> <span data-ttu-id="bc622-135">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="bc622-135">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="bc622-136">CopyItem</span><span class="sxs-lookup"><span data-stu-id="bc622-136">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="bc622-137">Exchange ストア内のアイテムをコピーするための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="bc622-137">Defines a request to copy items in the Exchange store.</span></span>  <br/> <span data-ttu-id="bc622-138">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="bc622-138">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bc622-139">備考</span><span class="sxs-lookup"><span data-stu-id="bc622-139">Remarks</span></span>

<span data-ttu-id="bc622-140">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="bc622-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc622-141">要素情報</span><span class="sxs-lookup"><span data-stu-id="bc622-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc622-142">名前空間</span><span class="sxs-lookup"><span data-stu-id="bc622-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bc622-143">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bc622-143">Schema Name</span></span>  <br/> |<span data-ttu-id="bc622-144">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="bc622-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bc622-145">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bc622-145">Validation File</span></span>  <br/> |<span data-ttu-id="bc622-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bc622-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bc622-147">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bc622-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc622-148">False</span><span class="sxs-lookup"><span data-stu-id="bc622-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc622-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="bc622-149">See also</span></span>

- [<span data-ttu-id="bc622-150">DeleteItem の操作</span><span class="sxs-lookup"><span data-stu-id="bc622-150">DeleteItem operation</span></span>](deleteitem-operation.md)
- <span data-ttu-id="bc622-151">
  [SendItem 操作](senditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="bc622-151">[SendItem operation](senditem-operation.md)</span></span> 
- <span data-ttu-id="bc622-152">
  [GetItem 操作](getitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="bc622-152">[GetItem operation](getitem-operation.md)</span></span>
- <span data-ttu-id="bc622-153">
  [MoveItem 操作](moveitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="bc622-153">[MoveItem operation](moveitem-operation.md)</span></span>
- <span data-ttu-id="bc622-154">
  [CopyItem 操作](copyitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="bc622-154">[CopyItem operation](copyitem-operation.md)</span></span>
- <span data-ttu-id="bc622-155">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="bc622-155">[FindConversation operation](findconversation-operation.md)</span></span>


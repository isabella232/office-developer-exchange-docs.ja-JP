---
title: GroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupBy
api_type:
- schema
ms.assetid: 9728619b-4674-4b9d-9f6c-e75c6165966c
description: GroupBy 要素は、FindItem クエリの任意のグループ化を指定します。
ms.openlocfilehash: 0d681e5376e4dd71921cc97f270211e49179db85
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530100"
---
# <a name="groupby"></a><span data-ttu-id="49941-103">GroupBy</span><span class="sxs-lookup"><span data-stu-id="49941-103">GroupBy</span></span>

<span data-ttu-id="49941-104">**GroupBy**要素は、FindItem クエリの任意のグループ化を指定します。</span><span class="sxs-lookup"><span data-stu-id="49941-104">The **GroupBy** element specifies an arbitrary grouping for FindItem queries.</span></span> 
  
- [<span data-ttu-id="49941-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="49941-105">FindItem</span></span>](finditem.md)
- [<span data-ttu-id="49941-106">GroupBy</span><span class="sxs-lookup"><span data-stu-id="49941-106">GroupBy</span></span>](groupby.md)
  
```xml
<GroupBy Order="">
   <FieldURI/>
   <AggregateOn/>
</GroupBy>
```

```xml
<GroupBy Order="">
   <ExtendededFieldURI/>
   <AggregateOn/>
</GroupBy>
```

```xml
<GroupBy Order="">
   <IndexedFieldURI/>
   <AggregateOn/>
</GroupBy>
```

<span data-ttu-id="49941-107">**GroupByType**</span><span class="sxs-lookup"><span data-stu-id="49941-107">**GroupByType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="49941-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="49941-108">Attributes and elements</span></span>

<span data-ttu-id="49941-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="49941-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49941-110">属性</span><span class="sxs-lookup"><span data-stu-id="49941-110">Attributes</span></span>

|<span data-ttu-id="49941-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="49941-111">**Attribute**</span></span>|<span data-ttu-id="49941-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="49941-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="49941-113">**Order**</span><span class="sxs-lookup"><span data-stu-id="49941-113">**Order**</span></span> <br/> | <span data-ttu-id="49941-114">応答で返されるグループ化されたアイテムの配列内のグループの順序を指定します。</span><span class="sxs-lookup"><span data-stu-id="49941-114">Determines the order of the groups in the grouped item array that is returned in the response.</span></span> <span data-ttu-id="49941-115">この属性の型は Sortdirection 型です。</span><span class="sxs-lookup"><span data-stu-id="49941-115">This attribute is of type SortDirectionType.</span></span>  <br/> |
   
#### <a name="order-attribute-values"></a><span data-ttu-id="49941-116">Order 属性の値</span><span class="sxs-lookup"><span data-stu-id="49941-116">Order attribute values</span></span>

|<span data-ttu-id="49941-117">**値**</span><span class="sxs-lookup"><span data-stu-id="49941-117">**Value**</span></span>|<span data-ttu-id="49941-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="49941-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="49941-119">Ascending/昇順</span><span class="sxs-lookup"><span data-stu-id="49941-119">Ascending</span></span>  <br/> |<span data-ttu-id="49941-120">グループは昇順で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="49941-120">The groups are ordered in ascending order.</span></span>  <br/> |
|<span data-ttu-id="49941-121">Descending/降順</span><span class="sxs-lookup"><span data-stu-id="49941-121">Descending</span></span>  <br/> |<span data-ttu-id="49941-122">グループは、降順で順序付けられます。</span><span class="sxs-lookup"><span data-stu-id="49941-122">The groups are ordered in descending order.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="49941-123">子要素</span><span class="sxs-lookup"><span data-stu-id="49941-123">Child elements</span></span>

|<span data-ttu-id="49941-124">**Element**</span><span class="sxs-lookup"><span data-stu-id="49941-124">**Element**</span></span>|<span data-ttu-id="49941-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="49941-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49941-126">FieldURI</span><span class="sxs-lookup"><span data-stu-id="49941-126">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="49941-127">URI で頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="49941-127">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="49941-128">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="49941-128">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="49941-129">辞書の個々のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="49941-129">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="49941-130">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="49941-130">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="49941-131">取得、設定、または作成する拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="49941-131">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="49941-132">AggregateOn</span><span class="sxs-lookup"><span data-stu-id="49941-132">AggregateOn</span></span>](aggregateon.md) <br/> |<span data-ttu-id="49941-133">応答内のグループの順序を決定するために使用されるフィールドを表します。</span><span class="sxs-lookup"><span data-stu-id="49941-133">Represents the field that is used to determine the order of groups in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="49941-134">親要素</span><span class="sxs-lookup"><span data-stu-id="49941-134">Parent elements</span></span>

|<span data-ttu-id="49941-135">**要素**</span><span class="sxs-lookup"><span data-stu-id="49941-135">**Element**</span></span>|<span data-ttu-id="49941-136">**説明**</span><span class="sxs-lookup"><span data-stu-id="49941-136">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49941-137">FindItem</span><span class="sxs-lookup"><span data-stu-id="49941-137">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="49941-138">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="49941-138">Defines a request to find items in a mailbox.</span></span>  <br/><br/> <span data-ttu-id="49941-139">この要素の XPath 式を次に示します。`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="49941-139">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="49941-140">注釈</span><span class="sxs-lookup"><span data-stu-id="49941-140">Remarks</span></span>

<span data-ttu-id="49941-141">FindItem 応答には、グループのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="49941-141">The FindItem response will contain a collection of groups.</span></span> <span data-ttu-id="49941-142">各グループには、 **GroupBy**プロパティに一致する値を持つすべてのアイテムが含まれます。</span><span class="sxs-lookup"><span data-stu-id="49941-142">Each group will contain all items that had matching values for the **GroupBy** property.</span></span> <span data-ttu-id="49941-143">グループ化を決定するプロパティは、 [FieldURI](fielduri.md)、 [IndexedFieldURI](indexedfielduri.md)、または[ExtendedFieldURI](extendedfielduri.md)要素で識別されます。</span><span class="sxs-lookup"><span data-stu-id="49941-143">The property that determines the grouping is identified in the [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md), or [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
  
<span data-ttu-id="49941-144">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="49941-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49941-145">要素の情報</span><span class="sxs-lookup"><span data-stu-id="49941-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49941-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="49941-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="49941-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="49941-147">Schema Name</span></span>  <br/> |<span data-ttu-id="49941-148">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="49941-148">Messages schema</span></span>  <br/> |
|<span data-ttu-id="49941-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="49941-149">Validation File</span></span>  <br/> |<span data-ttu-id="49941-150">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="49941-150">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="49941-151">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="49941-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="49941-152">正しくない</span><span class="sxs-lookup"><span data-stu-id="49941-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="49941-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="49941-153">See also</span></span>

- [<span data-ttu-id="49941-154">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="49941-154">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="49941-155">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="49941-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="49941-156">アイテムの検索</span><span class="sxs-lookup"><span data-stu-id="49941-156">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)


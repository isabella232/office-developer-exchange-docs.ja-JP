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
ms.openlocfilehash: d85c0fddec244c99dfbea1f85da331fc5319536d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831753"
---
# <a name="groupby"></a><span data-ttu-id="9905d-103">GroupBy</span><span class="sxs-lookup"><span data-stu-id="9905d-103">GroupBy</span></span>

<span data-ttu-id="9905d-104">**GroupBy**要素は、FindItem クエリの任意のグループ化を指定します。</span><span class="sxs-lookup"><span data-stu-id="9905d-104">The **GroupBy** element specifies an arbitrary grouping for FindItem queries.</span></span> 
  
- [<span data-ttu-id="9905d-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="9905d-105">FindItem</span></span>](finditem.md)
- [<span data-ttu-id="9905d-106">GroupBy</span><span class="sxs-lookup"><span data-stu-id="9905d-106">GroupBy</span></span>](groupby.md)
  
```xml
<GroupBy Order="">
   <FieldURI/>
   <AggregateOn/>
</GroupBy>
```

 <span data-ttu-id="9905d-107">**GroupByType**</span><span class="sxs-lookup"><span data-stu-id="9905d-107">**GroupByType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9905d-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9905d-108">Attributes and elements</span></span>

<span data-ttu-id="9905d-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9905d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9905d-110">属性</span><span class="sxs-lookup"><span data-stu-id="9905d-110">Attributes</span></span>

|<span data-ttu-id="9905d-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="9905d-111">**Attribute**</span></span>|<span data-ttu-id="9905d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9905d-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9905d-113">**Order**</span><span class="sxs-lookup"><span data-stu-id="9905d-113">**Order**</span></span> <br/> | <span data-ttu-id="9905d-114">応答で返されるグループ化されたアイテムの配列内のグループの順序を決定します。</span><span class="sxs-lookup"><span data-stu-id="9905d-114">Determines the order of the groups in the grouped item array that is returned in the response.</span></span> <span data-ttu-id="9905d-115">この属性は、型 SortDirectionType のです。</span><span class="sxs-lookup"><span data-stu-id="9905d-115">This attribute is of type SortDirectionType.</span></span>  <br/> |
   
#### <a name="order-attribute-values"></a><span data-ttu-id="9905d-116">順序属性の値</span><span class="sxs-lookup"><span data-stu-id="9905d-116">Order attribute values</span></span>

|<span data-ttu-id="9905d-117">**値**</span><span class="sxs-lookup"><span data-stu-id="9905d-117">**Value**</span></span>|<span data-ttu-id="9905d-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="9905d-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9905d-119">Ascending/昇順</span><span class="sxs-lookup"><span data-stu-id="9905d-119">Ascending</span></span>  <br/> |<span data-ttu-id="9905d-120">グループは昇順で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="9905d-120">The groups are ordered in ascending order.</span></span>  <br/> |
|<span data-ttu-id="9905d-121">降順</span><span class="sxs-lookup"><span data-stu-id="9905d-121">Descending</span></span>  <br/> |<span data-ttu-id="9905d-122">グループは降順で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="9905d-122">The groups are ordered in descending order.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9905d-123">子要素</span><span class="sxs-lookup"><span data-stu-id="9905d-123">Child elements</span></span>

|<span data-ttu-id="9905d-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="9905d-124">**Element**</span></span>|<span data-ttu-id="9905d-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="9905d-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9905d-126">FieldURI</span><span class="sxs-lookup"><span data-stu-id="9905d-126">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="9905d-127">URI によって頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="9905d-127">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="9905d-128">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="9905d-128">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="9905d-129">辞書の個々 のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="9905d-129">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="9905d-130">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="9905d-130">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="9905d-131">取得、設定、または作成する拡張の MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="9905d-131">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="9905d-132">AggregateOn</span><span class="sxs-lookup"><span data-stu-id="9905d-132">AggregateOn</span></span>](aggregateon.md) <br/> |<span data-ttu-id="9905d-133">応答内のグループの順序を決定するために使用されるフィールドを表します。</span><span class="sxs-lookup"><span data-stu-id="9905d-133">Represents the field that is used to determine the order of groups in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9905d-134">親要素</span><span class="sxs-lookup"><span data-stu-id="9905d-134">Parent elements</span></span>

|<span data-ttu-id="9905d-135">**要素**</span><span class="sxs-lookup"><span data-stu-id="9905d-135">**Element**</span></span>|<span data-ttu-id="9905d-136">**説明**</span><span class="sxs-lookup"><span data-stu-id="9905d-136">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9905d-137">FindItem</span><span class="sxs-lookup"><span data-stu-id="9905d-137">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="9905d-138">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="9905d-138">Defines a request to find items in a mailbox.</span></span>  <br/><br/> <span data-ttu-id="9905d-139">この要素への XPath 式は、次のようにします。`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="9905d-139">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9905d-140">備考</span><span class="sxs-lookup"><span data-stu-id="9905d-140">Remarks</span></span>

<span data-ttu-id="9905d-141">FindItem 応答グループのコレクションが含まれます。</span><span class="sxs-lookup"><span data-stu-id="9905d-141">The FindItem response will contain a collection of groups.</span></span> <span data-ttu-id="9905d-142">**GroupBy**プロパティの値が一致するすべての項目は、各グループが含まれます。</span><span class="sxs-lookup"><span data-stu-id="9905d-142">Each group will contain all items that had matching values for the **GroupBy** property.</span></span> <span data-ttu-id="9905d-143">[FieldURI](fielduri.md)、 [IndexedFieldURI](indexedfielduri.md)、または[ExtendedFieldURI](extendedfielduri.md)要素のグループ化を決定するプロパティが識別されます。</span><span class="sxs-lookup"><span data-stu-id="9905d-143">The property that determines the grouping is identified in the [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md), or [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
  
<span data-ttu-id="9905d-144">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9905d-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9905d-145">要素情報</span><span class="sxs-lookup"><span data-stu-id="9905d-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9905d-146">名前空間</span><span class="sxs-lookup"><span data-stu-id="9905d-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9905d-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9905d-147">Schema Name</span></span>  <br/> |<span data-ttu-id="9905d-148">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9905d-148">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9905d-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9905d-149">Validation File</span></span>  <br/> |<span data-ttu-id="9905d-150">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9905d-150">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9905d-151">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9905d-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="9905d-152">False</span><span class="sxs-lookup"><span data-stu-id="9905d-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9905d-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="9905d-153">See also</span></span>

- <span data-ttu-id="9905d-154">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="9905d-154">[FindItem operation](finditem-operation.md)</span></span>
- [<span data-ttu-id="9905d-155">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9905d-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="9905d-156">項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="9905d-156">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

